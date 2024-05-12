# Comparing `tmp/pkscreener-0.44.20240512.361.tar.gz` & `tmp/pkscreener-0.44.20240512.362.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240512.361.tar", last modified: Sun May 12 14:27:58 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240512.362.tar", last modified: Sun May 12 14:41:45 2024, max compression
```

## Comparing `pkscreener-0.44.20240512.361.tar` & `pkscreener-0.44.20240512.362.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 14:27:58.551696 pkscreener-0.44.20240512.361/
--rw-rw-rw-   0        0        0     1086 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-12 14:27:58.551696 pkscreener-0.44.20240512.361/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 14:27:58.536077 pkscreener-0.44.20240512.361/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:27:58.551696 pkscreener-0.44.20240512.361/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    27458 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11236 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    30922 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11667 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18597 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   128044 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    55796 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83233 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-12 14:27:50.000000 pkscreener-0.44.20240512.361/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   131494 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/globals.py
--rw-rw-rw-   0        0        0      929 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    51608 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    30222 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:27:58.536077 pkscreener-0.44.20240512.361/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-12 14:27:58.551696 pkscreener-0.44.20240512.361/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:41:45.668179 pkscreener-0.44.20240512.362/
+-rw-rw-rw-   0        0        0     1086 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-12 14:41:45.668179 pkscreener-0.44.20240512.362/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 14:41:45.652561 pkscreener-0.44.20240512.362/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:41:45.668179 pkscreener-0.44.20240512.362/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    28414 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11236 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30922 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11667 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18597 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   128056 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    55925 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83233 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-12 14:41:40.000000 pkscreener-0.44.20240512.362/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   131494 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      929 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    51608 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    30222 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:41:45.652561 pkscreener-0.44.20240512.362/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-12 14:41:45.668179 pkscreener-0.44.20240512.362/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/setup.py
```

### Comparing `pkscreener-0.44.20240512.361/LICENSE` & `pkscreener-0.44.20240512.362/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/LICENSE-Others` & `pkscreener-0.44.20240512.362/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/PKG-INFO` & `pkscreener-0.44.20240512.362/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240512.361
+Version: 0.44.20240512.362
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240512.361.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240512.362.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240512.361/README.md` & `pkscreener-0.44.20240512.362/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240512.361/pkscreener/__init__.py` & `pkscreener-0.44.20240512.362/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/ConfigManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,16 @@
         self.backtestPeriod = 120
         self.maxBacktestWindow = 30
         self.minVolume = 10000
         self.morninganalysiscandlenumber = 25 # 9:40am IST, since market opens at 9:15am IST
         self.morninganalysiscandleduration = '1m'
         self.logger = None
         self.showPastStrategyData = False
+        self.atrTrailingStopSensitivity = 1
+        self.atrTrailingStopPeriod = 10
         # This determines how many days apart the backtest calculations are run.
         # For example, for weekly backtest calculations, set this to 5 (5 days = 1 week)
         # For fortnightly, set this to 10 and so on (10 trading sessions = 2 weeks)
         self.backtestPeriodFactor = 1
         self.maxDashboardWidgetsPerRow = 3
         self.maxNumResultRowsInMonitor = 2
         self.calculatersiintraday = False
@@ -137,14 +139,16 @@
                 parser.remove_section("config")
                 parser.remove_section("filters")
             except Exception as e:  # pragma: no cover
                 self.default_logger.debug(e, exc_info=True)
                 pass
             parser.add_section("config")
             parser.add_section("filters")
+            parser.set("config", "atrtrailingstopperiod", str(self.atrTrailingStopPeriod))
+            parser.set("config", "atrtrailingstopsensitivity", str(self.atrTrailingStopSensitivity))
             parser.set("config", "backtestPeriod", str(self.backtestPeriod))
             parser.set("config", "backtestPeriodFactor", str(self.backtestPeriodFactor))
             parser.set("config", "cacheStockData", "y" if self.cacheEnabled else "n")
             parser.set("config", "calculatersiintraday", "y" if self.calculatersiintraday else "n")
             parser.set("config", "daysToLookback", str(self.daysToLookback))
             parser.set("config", "defaultIndex", str(self.defaultIndex))
             parser.set("config", "defaultMonitorOptions", str(self.defaultMonitorOptions))
@@ -302,14 +306,22 @@
             )
             self.backtestPeriodFactor = input(
                 "[+] Factor for backtest periods. If you choose 5, 1-Pd would mean 5-Pd returns. (number)(Optimal = 1): "
             )
             self.minimumChangePercentage = input(
                 "[+] Minimun change in stock price (in percentage). (number)(Optimal = 0): "
             )
+            self.atrTrailingStopPeriod = input(
+                "[+] ATR Trailing Stop Periods. (number)(Optimal = 10): "
+            )
+            self.atrTrailingStopSensitivity = input(
+                "[+] ATR Trailing Stop Sensitivity. (number)(Optimal = 1): "
+            )
+            parser.set("config", "atrtrailingstopperiod", self.atrTrailingStopPeriod)
+            parser.set("config", "atrtrailingstopsensitivity", self.atrTrailingStopSensitivity)
             parser.set("config", "backtestPeriod", self.backtestPeriod)
             parser.set("config", "backtestPeriodFactor", self.backtestPeriodFactor)
             parser.set("config", "cacheStockData", self.cacheStockData)
             parser.set("config", "calculatersiintraday", self.calculatersiintraday)
             parser.set("config", "daysToLookback", self.daysToLookback)
             parser.set("config", "defaultIndex", self.defaultIndex)
             parser.set("config", "defaultMonitorOptions", self.defaultMonitorOptions)
@@ -425,14 +437,16 @@
                     else True
                 )
                 self.calculatersiintraday = (
                     False
                     if "y" not in str(parser.get("config", "calculatersiintraday")).lower()
                     else True
                 )
+                self.atrTrailingStopPeriod = int(parser.get("config", "atrtrailingstopperiod"))
+                self.atrTrailingStopSensitivity = float(parser.get("config", "atrtrailingstopsensitivity"))
                 self.generalTimeout = float(parser.get("config", "generalTimeout"))
                 self.defaultIndex = int(parser.get("config", "defaultIndex"))
                 self.longTimeout = float(parser.get("config", "longTimeout"))
                 self.maxNetworkRetryCount = int(
                     parser.get("config", "maxNetworkRetryCount")
                 )
                 self.backtestPeriod = int(parser.get("config", "backtestPeriod"))
```

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/ScreeningStatistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,23 +244,23 @@
         elif close < prev_atr and prev_close < prev_atr:
             return min(prev_atr, close + nloss)
         elif close > prev_atr:
             return close - nloss
         else:
             return close + nloss
     
-    def findATRTrailingStops(self,df,key_value=1, atr_period=10, ema_period=200,buySellAll=1,saveDict=None,screenDict=None):
+    def findATRTrailingStops(self,df,sensitivity=1, atr_period=10, ema_period=200,buySellAll=1,saveDict=None,screenDict=None):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         data = data.fillna(0)
         data = data.replace([np.inf, -np.inf], 0)
         data = data[::-1]  # Reverse the dataframe so that its the oldest date first
 
-        SENSITIVITY = 1
+        SENSITIVITY = sensitivity
         # Compute ATR And nLoss variable
         data["xATR"] = pktalib.ATR(data["High"], data["Low"], data["Close"], timeperiod=atr_period)
         data["nLoss"] = SENSITIVITY * data["xATR"]
         
         #Drop all rows that have nan, X first depending on the ATR preiod for the moving average
         data = data.dropna()
         data = data.reset_index()
```

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/StockScreener.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
                 isBreaking = False
                 isValidCci = False
                 isVSA = False
                 isCandlePattern = False
                 isLowestVolume = False
                 hasBbandsSqz = False
 
-                isValidityCheckMet = self.performValidityCheckForExecuteOptions(executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData,maLength)
+                isValidityCheckMet = self.performValidityCheckForExecuteOptions(executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData,configManager,maLength)
                 if not isValidityCheckMet:
                     return returnLegibleData("Validity Check not met!")
                 isShortTermBullish = (executeOption == 11 and isValidityCheckMet)
                 if newlyListedOnly:
                     isIpoBase = screener.validateIpoBase(
                         stock, fullData, screeningDictionary, saveDictionary
                     )
@@ -675,15 +675,15 @@
                         "\n[+] Exception Occured while Screening %s! Skipping this stock.."
                         % stock
                     )
                     + colorText.END
                 )
         return None
 
-    def performValidityCheckForExecuteOptions(self,executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData,buySellAll=3):
+    def performValidityCheckForExecuteOptions(self,executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData,configManager,buySellAll=3):
         isValid = True
         if executeOption not in [11,12,13,14,15,16,17,18,19,20,23,24,25,27,28,30]:
             return True
         if executeOption == 11:
             isValid = screener.validateShortTermBullish(
                 fullData, screeningDictionary, saveDictionary
             )
@@ -718,15 +718,15 @@
         elif executeOption == 25:
             isValid = screener.validateLowerHighsLowerLows(processedData)
         elif executeOption == 27:
             isValid = screener.findATRCross(processedData,saveDictionary, screeningDictionary)
         elif executeOption == 28:
             isValid = screener.findHigherBullishOpens(processedData)
         elif executeOption == 30: # findBuySellSignalsFromATRTrailing # findATRTrailingStops
-            isValid = screener.findATRTrailingStops(fullData,buySellAll=buySellAll,saveDict=saveDictionary,screenDict=screeningDictionary)
+            isValid = screener.findATRTrailingStops(fullData,sensitivity=configManager.atrTrailingStopSensitivity, atr_period=configManager.atrTrailingStopPeriod,buySellAll=buySellAll,saveDict=saveDictionary,screenDict=screeningDictionary)
         
         return isValid        
                     
     def performBasicVolumeChecks(self, executeOption, volumeRatio, screeningDictionary, saveDictionary, processedData, configManager, screener):
         minVolume = configManager.minVolume / (
                     100 if configManager.isIntradayConfig() else 1
                 )
```

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/classes/keys.py` & `pkscreener-0.44.20240512.362/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/courbd.ttf` & `pkscreener-0.44.20240512.362/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/globals.py` & `pkscreener-0.44.20240512.362/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240512.362/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240512.362/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240512.362/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240512.362/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240512.361
+Version: 0.44.20240512.362
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240512.361.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240512.362.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240512.361/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240512.362/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.361/setup.py` & `pkscreener-0.44.20240512.362/setup.py`

 * *Files identical despite different names*

