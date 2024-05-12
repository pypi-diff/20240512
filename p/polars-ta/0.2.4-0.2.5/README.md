# Comparing `tmp/polars_ta-0.2.4.tar.gz` & `tmp/polars_ta-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polars_ta-0.2.4.tar", last modified: Thu Apr 18 02:56:55 2024, max compression
+gzip compressed data, was "polars_ta-0.2.5.tar", last modified: Sun May 12 11:49:37 2024, max compression
```

## Comparing `polars_ta-0.2.4.tar` & `polars_ta-0.2.5.tar`

### file list

```diff
@@ -1,77 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.252782 polars_ta-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-18 02:56:51.000000 polars_ta-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-04-18 02:56:55.252782 polars_ta-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-18 02:56:51.000000 polars_ta-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.244782 polars_ta-0.2.4/polars_ta/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.244782 polars_ta-0.2.4/polars_ta/candles/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/candles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/candles/cdl1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/candles/cdl1_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/candles/cdl2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/noise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.244782 polars_ta-0.2.4/polars_ta/performance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/performance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/performance/drawdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/performance/returns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.248782 polars_ta-0.2.4/polars_ta/prefix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/cdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/ta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/talib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/tdx.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/prefix/wq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.248782 polars_ta-0.2.4/polars_ta/ta/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/momentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/price.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/statistic.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/volatility.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/ta/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.248782 polars_ta-0.2.4/polars_ta/talib/
--rw-r--r--   0 runner    (1001) docker     (127)    34381 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/talib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.252782 polars_ta-0.2.4/polars_ta/tdx/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/choice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/moving_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/over_bought_over_sold.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/pressure_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/statistic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/trend.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/tdx/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.252782 polars_ta-0.2.4/polars_ta/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/numba_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/pandas_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/pit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/utils/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.252782 polars_ta-0.2.4/polars_ta/wq/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/cross_sectional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/time_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-18 02:56:51.000000 polars_ta-0.2.4/polars_ta/wq/transformational.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:56:55.252782 polars_ta-0.2.4/polars_ta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-04-18 02:56:55.000000 polars_ta-0.2.4/polars_ta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-18 02:56:55.000000 polars_ta-0.2.4/polars_ta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:56:55.000000 polars_ta-0.2.4/polars_ta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 02:56:55.000000 polars_ta-0.2.4/polars_ta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 02:56:55.000000 polars_ta-0.2.4/polars_ta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-18 02:56:51.000000 polars_ta-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:56:55.252782 polars_ta-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:56:51.000000 polars_ta-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.911649 polars_ta-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-12 11:49:33.000000 polars_ta-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-12 11:49:37.911649 polars_ta-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-12 11:49:33.000000 polars_ta-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.899649 polars_ta-0.2.5/polars_ta/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.903649 polars_ta-0.2.5/polars_ta/candles/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/candles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/candles/cdl1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/candles/cdl1_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/candles/cdl2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/noise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.903649 polars_ta-0.2.5/polars_ta/performance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/performance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/performance/drawdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/performance/returns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.903649 polars_ta-0.2.5/polars_ta/prefix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/prefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/prefix/cdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/prefix/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/prefix/ta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/prefix/talib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/prefix/tdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/prefix/wq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.903649 polars_ta-0.2.5/polars_ta/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/reports/cicc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.903649 polars_ta-0.2.5/polars_ta/ta/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/ta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/ta/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/ta/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/ta/overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/ta/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/ta/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/ta/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/ta/volatility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/ta/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.907649 polars_ta-0.2.5/polars_ta/talib/
+-rw-r--r--   0 runner    (1001) docker     (127)    34381 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/talib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.907649 polars_ta-0.2.5/polars_ta/tdx/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/over_bought_over_sold.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/pressure_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/statistic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/tdx/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.907649 polars_ta-0.2.5/polars_ta/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/utils/numba_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/utils/pandas_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/utils/pit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/utils/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.911649 polars_ta-0.2.5/polars_ta/wq/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/wq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/wq/_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/wq/_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/wq/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/wq/cross_sectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/wq/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/wq/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/wq/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/wq/transformational.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-12 11:49:33.000000 polars_ta-0.2.5/polars_ta/wq/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:49:37.911649 polars_ta-0.2.5/polars_ta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10651 2024-05-12 11:49:37.000000 polars_ta-0.2.5/polars_ta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-12 11:49:37.000000 polars_ta-0.2.5/polars_ta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 11:49:37.000000 polars_ta-0.2.5/polars_ta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 11:49:37.000000 polars_ta-0.2.5/polars_ta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 11:49:37.000000 polars_ta-0.2.5/polars_ta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-12 11:49:33.000000 polars_ta-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 11:49:37.911649 polars_ta-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 11:49:33.000000 polars_ta-0.2.5/setup.py
```

### Comparing `polars_ta-0.2.4/LICENSE` & `polars_ta-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/PKG-INFO` & `polars_ta-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_ta
-Version: 0.2.4
+Version: 0.2.5
 Summary: polars expressions
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2023 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polars_ta-0.2.4/README.md` & `polars_ta-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/candles/cdl1.py` & `polars_ta-0.2.5/polars_ta/candles/cdl1.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/candles/cdl1_limit.py` & `polars_ta-0.2.5/polars_ta/candles/cdl1_limit.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/candles/cdl2.py` & `polars_ta-0.2.5/polars_ta/candles/cdl2.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/noise.py` & `polars_ta-0.2.5/polars_ta/noise.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/performance/returns.py` & `polars_ta-0.2.5/polars_ta/performance/returns.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/prefix/ta.py` & `polars_ta-0.2.5/polars_ta/prefix/ta.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/prefix/talib.py` & `polars_ta-0.2.5/polars_ta/prefix/talib.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/prefix/tdx.py` & `polars_ta-0.2.5/polars_ta/prefix/tdx.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/ta/momentum.py` & `polars_ta-0.2.5/polars_ta/ta/momentum.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/ta/operators.py` & `polars_ta-0.2.5/polars_ta/ta/operators.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/ta/overlap.py` & `polars_ta-0.2.5/polars_ta/ta/overlap.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/ta/statistic.py` & `polars_ta-0.2.5/polars_ta/ta/statistic.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/ta/transform.py` & `polars_ta-0.2.5/polars_ta/ta/transform.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/ta/volatility.py` & `polars_ta-0.2.5/polars_ta/ta/volatility.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/ta/volume.py` & `polars_ta-0.2.5/polars_ta/ta/volume.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/talib/__init__.py` & `polars_ta-0.2.5/polars_ta/talib/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/__init__.py` & `polars_ta-0.2.5/polars_ta/tdx/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/_nb.py` & `polars_ta-0.2.5/polars_ta/tdx/_nb.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/arithmetic.py` & `polars_ta-0.2.5/polars_ta/tdx/arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/choice.py` & `polars_ta-0.2.5/polars_ta/tdx/choice.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/energy.py` & `polars_ta-0.2.5/polars_ta/tdx/energy.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/logical.py` & `polars_ta-0.2.5/polars_ta/tdx/logical.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/over_bought_over_sold.py` & `polars_ta-0.2.5/polars_ta/tdx/over_bought_over_sold.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/pressure_support.py` & `polars_ta-0.2.5/polars_ta/tdx/pressure_support.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/reference.py` & `polars_ta-0.2.5/polars_ta/tdx/reference.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/statistic.py` & `polars_ta-0.2.5/polars_ta/tdx/statistic.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/trend.py` & `polars_ta-0.2.5/polars_ta/tdx/trend.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/tdx/volume.py` & `polars_ta-0.2.5/polars_ta/tdx/volume.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/utils/helper.py` & `polars_ta-0.2.5/polars_ta/utils/helper.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/utils/pandas_.py` & `polars_ta-0.2.5/polars_ta/utils/pandas_.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/utils/pit.py` & `polars_ta-0.2.5/polars_ta/utils/pit.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/utils/wrapper.py` & `polars_ta-0.2.5/polars_ta/utils/wrapper.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/wq/_nb.py` & `polars_ta-0.2.5/polars_ta/wq/_nb.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/wq/_slow.py` & `polars_ta-0.2.5/polars_ta/wq/_slow.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/wq/arithmetic.py` & `polars_ta-0.2.5/polars_ta/wq/arithmetic.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,16 +181,16 @@
     return x.sin()
 
 
 def sinh(x: Expr) -> Expr:
     return x.sinh()
 
 
-def softsign(a: Expr) -> Expr:
-    return a / (1 + a.abs())
+def softsign(x: Expr) -> Expr:
+    return x / (1 + x.abs())
 
 
 def sqrt(x: Expr) -> Expr:
     return x.sqrt()
 
 
 def subtract(a: Expr, b: Expr, *args, filter_: bool = False) -> Expr:
```

### Comparing `polars_ta-0.2.4/polars_ta/wq/cross_sectional.py` & `polars_ta-0.2.5/polars_ta/wq/cross_sectional.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/wq/logical.py` & `polars_ta-0.2.5/polars_ta/wq/logical.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/wq/preprocess.py` & `polars_ta-0.2.5/polars_ta/wq/preprocess.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta/wq/time_series.py` & `polars_ta-0.2.5/polars_ta/wq/time_series.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import polars_ols as pls
 from polars import Expr, Int32, UInt16, map_batches
 from polars import arange, repeat
 from polars import rolling_corr, rolling_cov
 from polars_ols import RollingKwargs
 
 from polars_ta import TA_EPSILON
-from polars_ta.utils.numba_ import batches_i1_o1, batches_i2_o1
+from polars_ta.utils.numba_ import batches_i1_o1, batches_i2_o1, roll_split_i2_o1
 from polars_ta.utils.pandas_ import roll_kurt, roll_rank
 from polars_ta.wq._nb import roll_argmax, roll_argmin, roll_prod, roll_co_kurtosis, roll_co_skewness, roll_moment, roll_partial_corr, roll_triple_corr, _zip_prod, _zip_sum
 
 
 def ts_arg_max(x: Expr, d: int = 5, reverse: bool = True) -> Expr:
     return x.map_batches(lambda x1: batches_i1_o1(x1.to_numpy(), roll_argmax, d, reverse, dtype=UInt16))
 
@@ -66,15 +66,15 @@
 
 
 def ts_delta(x: Expr, d: int = 1) -> Expr:
     return x.diff(d)
 
 
 def ts_ir(x: Expr, d: int = 1) -> Expr:
-    return ts_mean(x, d) / ts_std_dev(x, d)
+    return ts_mean(x, d) / ts_std_dev(x, d, 0)
 
 
 def ts_kurtosis(x: Expr, d: int = 5) -> Expr:
     # TODO 等待polars官方出rolling_kurt
     return x.map_batches(lambda a: roll_kurt(a, d))
 
 
@@ -91,14 +91,18 @@
     return x - ts_max(x, d)
 
 
 def ts_mean(x: Expr, d: int = 5) -> Expr:
     return x.rolling_mean(d)
 
 
+def ts_gmean(x: Expr, d: int = 5) -> Expr:
+    return x.pow(2).rolling_sum(d).sqrt()
+
+
 def ts_median(x: Expr, d: int = 5) -> Expr:
     return x.rolling_median(d)
 
 
 def ts_min(x: Expr, d: int = 30) -> Expr:
     return x.rolling_min(d)
 
@@ -187,20 +191,48 @@
 
 def ts_zip_sum(x: Expr, y: Expr) -> Expr:
     """z字形累加"""
     return map_batches([x, y], lambda xx: batches_i2_o1([x1.to_numpy().astype(float) for x1 in xx], _zip_sum))
 
 
 def ts_regression_resid(y: Expr, x: Expr, d: int) -> Expr:
-    return pls.compute_rolling_least_squares(y, x, mode='residuals', add_intercept=True, rolling_kwargs=RollingKwargs(window_size=d))
+    return pls.compute_rolling_least_squares(y, x, mode='residuals', add_intercept=True, rolling_kwargs=RollingKwargs(window_size=d, min_periods=d))
 
 
 def ts_regression_pred(y: Expr, x: Expr, d: int) -> Expr:
-    return pls.compute_rolling_least_squares(y, x, mode='predictions', add_intercept=True, rolling_kwargs=RollingKwargs(window_size=d))
+    return pls.compute_rolling_least_squares(y, x, mode='predictions', add_intercept=True, rolling_kwargs=RollingKwargs(window_size=d, min_periods=d))
 
 
 def ts_regression_intercept(y: Expr, x: Expr, d: int) -> Expr:
-    return pls.compute_rolling_least_squares(y, x, mode='coefficients', add_intercept=True, rolling_kwargs=RollingKwargs(window_size=d)).struct[1]
+    return pls.compute_rolling_least_squares(y, x, mode='coefficients', add_intercept=True, rolling_kwargs=RollingKwargs(window_size=d, min_periods=d)).struct[1]
 
 
 def ts_regression_slope(y: Expr, x: Expr, d: int) -> Expr:
-    return pls.compute_rolling_least_squares(y, x, mode='coefficients', add_intercept=True, rolling_kwargs=RollingKwargs(window_size=d)).struct[0]
+    return pls.compute_rolling_least_squares(y, x, mode='coefficients', add_intercept=True, rolling_kwargs=RollingKwargs(window_size=d, min_periods=d)).struct[0]
+
+
+def ts_resid(y: Expr, *more_x: Expr, d: int) -> Expr:
+    """多元时序滚动回归取残差"""
+    return pls.compute_rolling_least_squares(y, *more_x, mode='residuals', rolling_kwargs=RollingKwargs(window_size=d, min_periods=d))
+
+
+def ts_pred(y: Expr, *more_x: Expr, d: int) -> Expr:
+    """多元时序滚动回归预测"""
+    return pls.compute_rolling_least_squares(y, *more_x, mode='predictions', rolling_kwargs=RollingKwargs(window_size=d, min_periods=d))
+
+
+def ts_weighted_mean(x: Expr, w: Expr, d: int) -> Expr:
+    """时序加权平均"""
+    return (x * w).rolling_sum(d) / w.rolling_sum(d)
+
+
+def ts_weighted_sum(x: Expr, w: Expr, d: int) -> Expr:
+    """时序加权求和"""
+    return (x * w).rolling_sum(d)
+
+
+def ts_split_sum(a: Expr, b: Expr, d: int, n: int) -> Expr:
+    """切割论求和，以b为依据，对a进行切割
+
+    在d窗口范围内以b为依据进行从小到大排序。最大的N个和-最小的N个和
+    """
+    return roll_split_i2_o1(a, b, d, n)
```

### Comparing `polars_ta-0.2.4/polars_ta/wq/transformational.py` & `polars_ta-0.2.5/polars_ta/wq/transformational.py`

 * *Files identical despite different names*

### Comparing `polars_ta-0.2.4/polars_ta.egg-info/PKG-INFO` & `polars_ta-0.2.5/polars_ta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars_ta
-Version: 0.2.4
+Version: 0.2.5
 Summary: polars expressions
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2023 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polars_ta-0.2.4/polars_ta.egg-info/SOURCES.txt` & `polars_ta-0.2.5/polars_ta.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,21 @@
 polars_ta/candles/cdl1_limit.py
 polars_ta/candles/cdl2.py
 polars_ta/performance/__init__.py
 polars_ta/performance/drawdown.py
 polars_ta/performance/returns.py
 polars_ta/prefix/__init__.py
 polars_ta/prefix/cdl.py
+polars_ta/prefix/reports.py
 polars_ta/prefix/ta.py
 polars_ta/prefix/talib.py
 polars_ta/prefix/tdx.py
 polars_ta/prefix/wq.py
+polars_ta/reports/__init__.py
+polars_ta/reports/cicc.py
 polars_ta/ta/__init__.py
 polars_ta/ta/momentum.py
 polars_ta/ta/operators.py
 polars_ta/ta/overlap.py
 polars_ta/ta/price.py
 polars_ta/ta/statistic.py
 polars_ta/ta/transform.py
@@ -57,8 +60,9 @@
 polars_ta/wq/_nb.py
 polars_ta/wq/_slow.py
 polars_ta/wq/arithmetic.py
 polars_ta/wq/cross_sectional.py
 polars_ta/wq/logical.py
 polars_ta/wq/preprocess.py
 polars_ta/wq/time_series.py
-polars_ta/wq/transformational.py
+polars_ta/wq/transformational.py
+polars_ta/wq/vector.py
```

### Comparing `polars_ta-0.2.4/pyproject.toml` & `polars_ta-0.2.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 [tool.setuptools]
 packages = [
     "polars_ta",
     "polars_ta.candles",
     "polars_ta.performance",
     "polars_ta.prefix",
+    "polars_ta.reports",
     "polars_ta.ta",
     "polars_ta.talib",
     "polars_ta.tdx",
     "polars_ta.utils",
     "polars_ta.wq",
 ]
```

