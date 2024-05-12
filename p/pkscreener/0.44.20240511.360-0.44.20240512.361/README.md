# Comparing `tmp/pkscreener-0.44.20240511.360.tar.gz` & `tmp/pkscreener-0.44.20240512.361.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240511.360.tar", last modified: Sat May 11 09:32:20 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240512.361.tar", last modified: Sun May 12 14:27:58 2024, max compression
```

## Comparing `pkscreener-0.44.20240511.360.tar` & `pkscreener-0.44.20240512.361.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 09:32:20.990268 pkscreener-0.44.20240511.360/
--rw-rw-rw-   0        0        0     1086 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-11 09:32:20.990268 pkscreener-0.44.20240511.360/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 09:32:20.974645 pkscreener-0.44.20240511.360/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:32:20.990268 pkscreener-0.44.20240511.360/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    27458 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11236 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    30554 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11667 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    21948 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18597 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   120047 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    55336 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83173 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-11 09:32:11.000000 pkscreener-0.44.20240511.360/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   130149 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/globals.py
--rw-rw-rw-   0        0        0      929 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    51603 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    30211 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:32:20.974645 pkscreener-0.44.20240511.360/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-11 09:32:20.000000 pkscreener-0.44.20240511.360/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-11 09:32:20.000000 pkscreener-0.44.20240511.360/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 09:32:20.000000 pkscreener-0.44.20240511.360/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-11 09:32:20.000000 pkscreener-0.44.20240511.360/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-11 09:32:20.000000 pkscreener-0.44.20240511.360/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-11 09:32:20.000000 pkscreener-0.44.20240511.360/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-11 09:32:20.990268 pkscreener-0.44.20240511.360/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-11 09:27:27.000000 pkscreener-0.44.20240511.360/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:27:58.551696 pkscreener-0.44.20240512.361/
+-rw-rw-rw-   0        0        0     1086 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-12 14:27:58.551696 pkscreener-0.44.20240512.361/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 14:27:58.536077 pkscreener-0.44.20240512.361/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:27:58.551696 pkscreener-0.44.20240512.361/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    27458 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11236 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30922 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11667 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18597 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   128044 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    55796 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83233 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-12 14:27:50.000000 pkscreener-0.44.20240512.361/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   131494 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      929 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    51608 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    30222 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:27:58.536077 pkscreener-0.44.20240512.361/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-12 14:27:58.000000 pkscreener-0.44.20240512.361/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-12 14:27:58.551696 pkscreener-0.44.20240512.361/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-12 14:23:18.000000 pkscreener-0.44.20240512.361/setup.py
```

### Comparing `pkscreener-0.44.20240511.360/LICENSE` & `pkscreener-0.44.20240512.361/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/LICENSE-Others` & `pkscreener-0.44.20240512.361/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/PKG-INFO` & `pkscreener-0.44.20240512.361/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240511.360
+Version: 0.44.20240512.361
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240511.360.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240512.361.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240510.358/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240510.358/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240510.358/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240511.360/README.md` & `pkscreener-0.44.20240512.361/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240510.358/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240510.358/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240510.358/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240511.360/pkscreener/__init__.py` & `pkscreener-0.44.20240512.361/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/MenuOptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     "23": "Breaking out now               ",
     "24": "Higher Highs,Lows & Close (SuperTrend)",
     "25": "Lower Highs,Lows (Watch for Rev.)",
     "26": "Stocks with stock-split/bonus/dividends",
     "27": "ATR Cross                      ",
     "28": "Bullish Higher Opens           ",
     "29": "Intraday Bid/Ask Build-up      ",
+    "30": "ATR Trailing Stops(Swing Paper Trading)",
     # "28": "Extremely bullish daily close      ",
     # "29": "Rising RSI                      ",
     # "30": "RSI entering bullish territory",
     "42": "Show Last Screened Results",
     "M": "Back to the Top/Main menu",
     "Z": "Exit (Ctrl + C)",
 }
@@ -424,14 +425,21 @@
                 elif selectedMenu.menuKey == "22":
                     return self.renderLevel3_X_StockPerformance_Menus(
                         skip=skip,
                         asList=asList,
                         renderStyle=renderStyle,
                         parent=selectedMenu,
                     )
+                elif selectedMenu.menuKey in ["30"]:
+                    return self.renderLevel4_X_Lorenzian_Menus(
+                        skip=skip,
+                        asList=asList,
+                        renderStyle=renderStyle,
+                        parent=selectedMenu,
+                    )
             elif selectedMenu.level == 3:
                 self.level = 4
                 # next levelsub-menu of the selected sub-menu
                 if selectedMenu.parent.menuKey == "6" and selectedMenu.menuKey in ["7","10"]:
                     return self.renderLevel4_X_Lorenzian_Menus(
                         skip=skip,
                         asList=asList,
```

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/PKScanRunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.PKGitFolderDownloader import downloadFolder
 from PKDevTools.classes.PKMultiProcessorClient import PKMultiProcessorClient
 from PKDevTools.classes.multiprocessing_logging import LogQueueReader
 from PKDevTools.classes.SuppressOutput import SuppressOutput
-# from PKDevTools.classes.FunctionTimeouts import exit_after
+from PKDevTools.classes.FunctionTimeouts import exit_after
 
 from pkscreener.classes.StockScreener import StockScreener
 from pkscreener.classes.CandlePatterns import CandlePatterns
 from pkscreener.classes.ConfigManager import parser, tools
 from PKDevTools.classes.OutputControls import OutputControls
 from PKNSETools.PKIntraDay import Intra_Day
 import pkscreener.classes.Fetcher as Fetcher
@@ -289,14 +289,15 @@
         if userPassedArgs is not None and (userPassedArgs.monitor is None and "|" not in userPassedArgs.options) and not userPassedArgs.options.upper().startswith("C"):
             # Don't terminate the multiprocessing clients if we're 
             # going to pipe the results from an earlier run
             # or we're running in monitoring mode
             PKScanRunner.terminateAllWorkers(userPassedArgs,consumers, tasks_queue, testing)
         return screenResults, saveResults,backtest_df,tasks_queue, results_queue, consumers, logging_queue
 
+    @exit_after(180) # Should not remain stuck starting the multiprocessing clients beyond this time
     def prepareToRunScan(menuOption,keyboardInterruptEvent, screenCounter, screenResultsCounter, stockDictPrimary,stockDictSecondary, items, executeOption):
         tasks_queue, results_queue, totalConsumers, logging_queue = PKScanRunner.initQueues(len(items))
         scr = ScreeningStatistics.ScreeningStatistics(PKScanRunner.configManager, default_logger())
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=PKScanRunner.configManager.isIntradayConfig())
         sec_cache_file = cache_file if "intraday_" in cache_file else f"intraday_{cache_file}"
         consumers = [
                     PKMultiProcessorClient(
@@ -327,14 +328,15 @@
         # if executeOption == 29: # Intraday Bid/Ask, for which we need to fetch data from NSE instead of yahoo
         intradayFetcher = Intra_Day("SBINEQN") # This will initialise the cookies etc.
         for consumer in consumers:
             consumer.intradayNSEFetcher = intradayFetcher
         PKScanRunner.startWorkers(consumers)
         return tasks_queue,results_queue,consumers,logging_queue
 
+    @exit_after(180) # Should not remain stuck starting the multiprocessing clients beyond this time
     def startWorkers(consumers):
         try:
             from pytest_cov.embed import cleanup_on_signal, cleanup_on_sigterm
         except ImportError:
             pass
         else:
             if sys.platform.startswith("win"):
@@ -352,15 +354,15 @@
         start_time = time.time()
         for worker in consumers:
             sys.stdout.write(f"{round(time.time() - start_time)}.")
             worker.daemon = True
             worker.start()
         OutputControls().printOutput(f"Started all workers in {round(time.time() - start_time,4)}s")
         if OutputControls().enableMultipleLineOutput:
-            sys.stdout.write("\x1b[1A")
+            sys.stdout.write("\x1b[1A") # Move cursor up to hide the starting times we printed above
 
     def terminateAllWorkers(userPassedArgs,consumers, tasks_queue, testing=False):
         shouldSuppress = (userPassedArgs is None) or (userPassedArgs is not None and not userPassedArgs.log)
         with SuppressOutput(suppress_stderr=shouldSuppress, suppress_stdout=shouldSuppress):
             # Exit all processes. Without this, it threw error in next screening session
             for worker in consumers:
                 try:
@@ -439,8 +441,9 @@
             # stock or if we've already tried screening through 5% of the list.
             if (not shouldContinue) or (testing and counter >= int(numStocksPerIteration * 0.05)):
                 break
             # Add to the queue when we're through 75% of the previously added items already
             if counter >= numStocksPerIteration: #int(numStocksPerIteration * 0.75):
                 queueCounter += 1
                 counter = 0
+        
         return backtest_df, lastNonNoneResult
```

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/ScreeningStatistics.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,55 +233,223 @@
         bullishRSI = recent["RSI"].iloc[0] >= 55 or recent["RSIi"].iloc[0] >= 55
         smav7 = pktalib.SMA(data["Volume"],timeperiod=7).tail(1).iloc[0]
         atrCrossCondition = atrCross and bullishRSI and (smav7 < recent["Volume"].iloc[0])
         saveDict["ATR"] = round(atr.tail(1).iloc[0],1)
         screenDict["ATR"] = saveDict["ATR"] #(colorText.GREEN if atrCrossCondition else colorText.FAIL) + str(atr.tail(1).iloc[0]) + colorText.END
         return atrCrossCondition
 
-# study(title="UT Bot Alerts", overlay = true)
-
-# // Inputs
-# a = input(1,     title = "Key Vaule. 'This changes the sensitivity'")
-# c = input(10,    title = "ATR Period")
-# h = input(false, title = "Signals from Heikin Ashi Candles")
-
-# xATR  = atr(c)
-# nLoss = a * xATR
-
-# src = h ? security(heikinashi(syminfo.tickerid), timeframe.period, close, lookahead = false) : close
-
-# xATRTrailingStop = 0.0
-# xATRTrailingStop := iff(src > nz(xATRTrailingStop[1], 0) and src[1] > nz(xATRTrailingStop[1], 0), max(nz(xATRTrailingStop[1]), src - nLoss),
-#    iff(src < nz(xATRTrailingStop[1], 0) and src[1] < nz(xATRTrailingStop[1], 0), min(nz(xATRTrailingStop[1]), src + nLoss), 
-#    iff(src > nz(xATRTrailingStop[1], 0), src - nLoss, src + nLoss)))
- 
-# pos = 0   
-# pos :=	iff(src[1] < nz(xATRTrailingStop[1], 0) and src > nz(xATRTrailingStop[1], 0), 1,
-#    iff(src[1] > nz(xATRTrailingStop[1], 0) and src < nz(xATRTrailingStop[1], 0), -1, nz(pos[1], 0))) 
-   
-# xcolor = pos == -1 ? color.red: pos == 1 ? color.green : color.blue 
-
-# ema   = ema(src,1)
-# above = crossover(ema, xATRTrailingStop)
-# below = crossover(xATRTrailingStop, ema)
-
-# buy  = src > xATRTrailingStop and above 
-# sell = src < xATRTrailingStop and below
-
-# barbuy  = src > xATRTrailingStop 
-# barsell = src < xATRTrailingStop 
-
-# plotshape(buy,  title = "Buy",  text = 'Buy',  style = shape.labelup,   location = location.belowbar, color= color.green, textcolor = color.white, transp = 0, size = size.tiny)
-# plotshape(sell, title = "Sell", text = 'Sell', style = shape.labeldown, location = location.abovebar, color= color.red,   textcolor = color.white, transp = 0, size = size.tiny)
-
-# barcolor(barbuy  ? color.green : na)
-# barcolor(barsell ? color.red   : na)
+    # Function to compute ATRTrailingStop
+    def xATRTrailingStop_func(self,close, prev_close, prev_atr, nloss):
+        if close > prev_atr and prev_close > prev_atr:
+            return max(prev_atr, close - nloss)
+        elif close < prev_atr and prev_close < prev_atr:
+            return min(prev_atr, close + nloss)
+        elif close > prev_atr:
+            return close - nloss
+        else:
+            return close + nloss
+    
+    def findATRTrailingStops(self,df,key_value=1, atr_period=10, ema_period=200,buySellAll=1,saveDict=None,screenDict=None):
+        if df is None or len(df) == 0:
+            return False
+        data = df.copy()
+        data = data.fillna(0)
+        data = data.replace([np.inf, -np.inf], 0)
+        data = data[::-1]  # Reverse the dataframe so that its the oldest date first
+
+        SENSITIVITY = 1
+        # Compute ATR And nLoss variable
+        data["xATR"] = pktalib.ATR(data["High"], data["Low"], data["Close"], timeperiod=atr_period)
+        data["nLoss"] = SENSITIVITY * data["xATR"]
+        
+        #Drop all rows that have nan, X first depending on the ATR preiod for the moving average
+        data = data.dropna()
+        data = data.reset_index()
+        # Filling ATRTrailingStop Variable
+        data["ATRTrailingStop"] = [0.0] + [np.nan for i in range(len(data) - 1)]
+        
+        for i in range(1, len(data)):
+            data.loc[i, "ATRTrailingStop"] = self.xATRTrailingStop_func(
+                data.loc[i, "Close"],
+                data.loc[i - 1, "Close"],
+                data.loc[i - 1, "ATRTrailingStop"],
+                data.loc[i, "nLoss"],
+            )
+        data = self.computeBuySellSignals(data,ema_period=ema_period)
+        recent = data.tail(1)
+        print(recent)
+        buy = recent["Buy"].iloc[0]
+        sell = recent["Sell"].iloc[0]
+        saveDict["B/S"] = "Buy" if buy else ("Sell" if sell else "NA")
+        screenDict["B/S"] = ((colorText.GREEN + "Buy") if buy else ((colorText.FAIL+ "Sell") if sell else (colorText.WARN + "NA"))) + colorText.END
+        return buy if buySellAll==1 else (sell if buySellAll == 2 else (True if buySellAll == 3 else False))
+
+    #Calculating signals
+    def computeBuySellSignals(self,df,ema_period=200):
+        ema = pktalib.EMA(df["Close"], ema_period) #short_name='EMA', ewm=True)
+        
+        df["Above"] = ema > df["ATRTrailingStop"]
+        df["Below"] = ema < df["ATRTrailingStop"]
+        
+        df["Buy"] = (df["Close"] > df["ATRTrailingStop"]) & (df["Above"]==True)
+        df["Sell"] = (df["Close"] < df["ATRTrailingStop"]) & (df["Below"]==True)
+        return df
 
-# alertcondition(buy,  "UT Long",  "UT Long")
-# alertcondition(sell, "UT Short", "UT Short")
+    def findBuySellSignalsFromATRTrailing(self,df, key_value=1, atr_period=10, ema_period=200,buySellAll=1,saveDict=None,screenDict=None):
+        if df is None or len(df) == 0:
+            return False
+        data = df.copy()
+        data = data.fillna(0)
+        data = data.replace([np.inf, -np.inf], 0)
+        data = data[::-1]  # Reverse the dataframe so that its the oldest date first
+
+        # Calculate ATR and xATRTrailingStop
+        xATR = np.array(pktalib.ATR(data['High'], data['Low'], data['Close'], timeperiod=atr_period))
+        nLoss = key_value * xATR
+        src = data['Close']
+        # Initialize arrays
+        xATRTrailingStop = np.zeros(len(data))
+        xATRTrailingStop[0] = src[0] - nLoss[0]
+
+        # Calculate xATRTrailingStop using vectorized operations
+        mask_1 = (src > np.roll(xATRTrailingStop, 1)) & (np.roll(src, 1) > np.roll(xATRTrailingStop, 1))
+        mask_2 = (src < np.roll(xATRTrailingStop, 1)) & (np.roll(src, 1) < np.roll(xATRTrailingStop, 1))
+        mask_3 = src > np.roll(xATRTrailingStop, 1)
+
+        xATRTrailingStop = np.where(mask_1, np.maximum(np.roll(xATRTrailingStop, 1), src - nLoss), xATRTrailingStop)
+        xATRTrailingStop = np.where(mask_2, np.minimum(np.roll(xATRTrailingStop, 1), src + nLoss), xATRTrailingStop)
+        xATRTrailingStop = np.where(mask_3, src - nLoss, xATRTrailingStop)
+
+        mask_buy = (np.roll(src, 1) < xATRTrailingStop) & (src > np.roll(xATRTrailingStop, 1))
+        mask_sell = (np.roll(src, 1) > xATRTrailingStop) & (src < np.roll(xATRTrailingStop, 1))
+
+        pos = np.zeros(len(data))
+        pos = np.where(mask_buy, 1, pos)
+        pos = np.where(mask_sell, -1, pos)
+        pos[~((pos == 1) | (pos == -1))] = 0
+
+        ema = np.array(pktalib.EMA(data['Close'], timeperiod=ema_period))
+
+        buy_condition_utbot = (xATRTrailingStop > ema) & (pos > 0) & (src > ema)
+        sell_condition_utbot = (xATRTrailingStop < ema) & (pos < 0) & (src < ema)
+
+        # The resulting trend array holds values of 1 (buy), -1 (sell), or 0 (neutral).
+        trend = np.where(buy_condition_utbot, 1, np.where(sell_condition_utbot, -1, 0))
+        trend_arr = np.array(trend)
+        data.insert(len(data.columns), "trend", trend_arr)
+        trend = trend[0]
+        saveDict["B/S"] = "Buy" if trend == 1 else ("Sell" if trend == -1 else "NA")
+        screenDict["B/S"] = (colorText.GREEN + "Buy") if trend == 1 else ((colorText.FAIL+ "Sell") if trend == -1 else (colorText.WARN + "NA")) + colorText.END
+        return buySellAll == trend
+
+    # Example of combining UTBot Alerts with RSI and ADX
+    def custom_strategy(self,dataframe):
+        dataframe = self.findBuySellSignalsFromATRTrailing(dataframe, key_value=2, atr_period=7, ema_period=100)
+        
+        # Calculate RSI and ADX
+        rsi = pktalib.RSI(dataframe['Close'])
+        adx = pktalib.ADX(dataframe['High'], dataframe['Low'], dataframe['Close'])
+        
+        # Define conditions based on UTBot Alerts and additional indicators
+        # ... (your custom conditions here)
+        
+        return dataframe
+    
+    def populate_indicators(self, dataframe: pd.DataFrame, metadata: dict) -> pd.DataFrame:
+        if not self.dp:
+            # Don't do anything if DataProvider is not available.
+            return dataframe
+        L_optimize_trend_alert  = self.findBuySellSignalsFromATRTrailing(dataframe=dataframe, key_value= self.key_value_l.value, atr_period= self.atr_period_l.value, ema_period=self.ema_period_l.value)
+        # Long position?
+        dataframe['trend_l'] = L_optimize_trend_alert['trend']
+        S_optimize_trend_alert  = self.findBuySellSignalsFromATRTrailing(dataframe=dataframe, key_value= self.key_value_s.value, atr_period= self.atr_period_s.value, ema_period=self.ema_period_s.value)
+        # Short position?
+        dataframe['trend_s'] = S_optimize_trend_alert['trend']
+
+        # ADX
+        dataframe['adx'] = pktalib.ADX(dataframe)
+        
+        # RSI
+        # dataframe['rsi'] = ta.RSI(dataframe)
+
+        # EMA
+        dataframe['ema_l'] = pktalib.EMA(dataframe['close'], timeperiod=self.ema_period_l_exit.value)
+        dataframe['ema_s'] = pktalib.EMA(dataframe['close'], timeperiod=self.ema_period_s_exit.value)
+
+
+        # Volume Weighted
+        dataframe['volume_mean'] = dataframe['volume'].rolling(self.volume_check.value).mean().shift(1)
+        dataframe['volume_mean_exit'] = dataframe['volume'].rolling(self.volume_check_exit.value).mean().shift(1)
+
+        dataframe['volume_mean_s'] = dataframe['volume'].rolling(self.volume_check_s.value).mean().shift(1)
+        dataframe['volume_mean_exit_s'] = dataframe['volume'].rolling(self.volume_check_exit_s.value).mean().shift(1)
+        return dataframe
+    
+    def populate_entry_trend(self, dataframe: pd.DataFrame, metadata: dict) -> pd.DataFrame:
+
+        dataframe.loc[
+            (
+                        (dataframe['adx'] > self.adx_long_min.value) & # trend strength confirmation
+                        (dataframe['adx'] < self.adx_long_max.value) & # trend strength confirmation
+                        (dataframe['trend_l'] > 0) &
+                        (dataframe['volume'] > dataframe['volume_mean']) &
+                        (dataframe['volume'] > 0)
+
+            ),
+            'enter_long'] = 1
+
+        dataframe.loc[
+            (
+                        (dataframe['adx'] > self.adx_short_min.value) & # trend strength confirmation
+                        (dataframe['adx'] < self.adx_short_max.value) & # trend strength confirmation
+                        (dataframe['trend_s'] < 0) &
+                        (dataframe['volume'] > dataframe['volume_mean_s']) # volume weighted indicator
+            ),
+            'enter_short'] = 1
+        
+        return dataframe
+    
+    def populate_exit_trend(self, dataframe: pd.DataFrame, metadata: dict) -> pd.DataFrame:
+
+        conditions_long = []
+        conditions_short = []
+        dataframe.loc[:, 'exit_tag'] = ''
+
+        exit_long = (
+                # (dataframe['close'] < dataframe['low'].shift(self.sell_shift.value)) &
+                (dataframe['close'] < dataframe['ema_l']) &
+                (dataframe['volume'] > dataframe['volume_mean_exit'])
+        )
+
+        exit_short = (
+                # (dataframe['close'] > dataframe['high'].shift(self.sell_shift_short.value)) &
+                (dataframe['close'] > dataframe['ema_s']) &
+                (dataframe['volume'] > dataframe['volume_mean_exit_s'])
+        )
+
+
+        conditions_short.append(exit_short)
+        dataframe.loc[exit_short, 'exit_tag'] += 'exit_short'
+
+
+        conditions_long.append(exit_long)
+        dataframe.loc[exit_long, 'exit_tag'] += 'exit_long'
+
+
+        if conditions_long:
+            dataframe.loc[
+                pd.reduce(lambda x, y: x | y, conditions_long),
+                'exit_long'] = 1
+
+        if conditions_short:
+            dataframe.loc[
+                pd.reduce(lambda x, y: x | y, conditions_short),
+                'exit_short'] = 1
+            
+        return dataframe
 
     # Find accurate breakout value
     def findBreakingoutNow(self, df, fullData, saveDict, screenDict):
         if df is None or len(df) == 0:
             return False
         data = df.copy()
         reversedData = fullData[::-1].copy()
```

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/StockScreener.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,24 +184,24 @@
                     fullData = fullData.head(len(intraday_fullData))
                     intraday_fullData = intraday_fullData.head(len(fullData))
                     processedData = processedData.head(len(intraday_processedData))
                     intraday_processedData = intraday_processedData.head(len(processedData))
                     data = data.tail(len(intraday_data))
                     intraday_data = intraday_data.tail(len(data))
                     # Indexes won't match. Hence, we'd need to fallback on tolist
-                    processedData.loc[:,"RSIi"] = intraday_processedData["RSI"].tolist()
-                    fullData.loc[:,"RSIi"] = intraday_fullData["RSI"].tolist()
+                    processedData.insert(len(processedData.columns), "RSIi", intraday_processedData["RSI"].tolist())
+                    fullData.insert(len(fullData.columns), "RSIi", intraday_processedData["RSI"].tolist())
                 else:
                     with SuppressOutput(suppress_stderr=(logLevel==logging.NOTSET), suppress_stdout=(not (printCounter or testbuild))):
-                        processedData.loc[:,"RSIi"] = np.nan
-                        fullData.loc[:,"RSIi"] = np.nan
+                        processedData.insert(len(processedData.columns), "RSIi", np.array(np.nan))
+                        fullData.insert(len(fullData.columns), "RSIi", np.array(np.nan))
             else:
                     with SuppressOutput(suppress_stderr=(logLevel==logging.NOTSET), suppress_stdout=(not (printCounter or testbuild))):
-                        processedData.loc[:,"RSIi"] = np.nan
-                        fullData.loc[:,"RSIi"] = np.nan
+                        processedData.insert(len(processedData.columns), "RSIi", np.array(np.nan))
+                        fullData.insert(len(fullData.columns), "RSIi", np.array(np.nan))
 
             def returnLegibleData(exceptionMessage=None):
                 if backtestDuration == 0 or menuOption not in ["B"]:
                     raise ScreeningStatistics.EligibilityConditionNotMet(exceptionMessage)
                 elif (backtestDuration > 0 and backtestDuration <= configManager.maxBacktestWindow):
                     screener.validateMovingAverages(
                         processedData, screeningDictionary, saveDictionary, maRange=1.25
@@ -259,15 +259,15 @@
                 isBreaking = False
                 isValidCci = False
                 isVSA = False
                 isCandlePattern = False
                 isLowestVolume = False
                 hasBbandsSqz = False
 
-                isValidityCheckMet = self.performValidityCheckForExecuteOptions(executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData)
+                isValidityCheckMet = self.performValidityCheckForExecuteOptions(executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData,maLength)
                 if not isValidityCheckMet:
                     return returnLegibleData("Validity Check not met!")
                 isShortTermBullish = (executeOption == 11 and isValidityCheckMet)
                 if newlyListedOnly:
                     isIpoBase = screener.validateIpoBase(
                         stock, fullData, screeningDictionary, saveDictionary
                     )
@@ -542,15 +542,15 @@
                                                                   or (isBuyingTrendline))
                                                                   or (respChartPattern == 6 and hasBbandsSqz)
                                                                   or (respChartPattern == 7 and isCandlePattern))
                         or (executeOption == 8 and isValidCci)
                         or (executeOption == 9 and hasMinVolumeRatio)
                         or (executeOption == 10 and isPriceRisingByAtLeast2Percent)
                         or (executeOption == 11 and isShortTermBullish)
-                        or (executeOption in [12,13,14,15,16,17,18,19,20,23,24,25,27,28] and isValidityCheckMet)
+                        or (executeOption in [12,13,14,15,16,17,18,19,20,23,24,25,27,28,30] and isValidityCheckMet)
                         or (executeOption == 21 and (mfiStake > 0 and reversalOption in [3,5]))
                         or (executeOption == 21 and (mfiStake < 0 and reversalOption in [6,7]))
                         or (executeOption == 21 and (fairValueDiff > 0 and reversalOption in [8]))
                         or (executeOption == 21 and (fairValueDiff < 0 and reversalOption in [9]))
                         or (executeOption == 26)
                         or (executeOption == 29) and bidGreaterThanAsk
                     ):
@@ -675,17 +675,17 @@
                         "\n[+] Exception Occured while Screening %s! Skipping this stock.."
                         % stock
                     )
                     + colorText.END
                 )
         return None
 
-    def performValidityCheckForExecuteOptions(self,executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData):
+    def performValidityCheckForExecuteOptions(self,executeOption,screener,fullData,screeningDictionary,saveDictionary,processedData,buySellAll=3):
         isValid = True
-        if executeOption not in [11,12,13,14,15,16,17,18,19,20,23,24,25,27,28]:
+        if executeOption not in [11,12,13,14,15,16,17,18,19,20,23,24,25,27,28,30]:
             return True
         if executeOption == 11:
             isValid = screener.validateShortTermBullish(
                 fullData, screeningDictionary, saveDictionary
             )
         elif executeOption == 12:
             isValid = (
@@ -717,14 +717,16 @@
             )
         elif executeOption == 25:
             isValid = screener.validateLowerHighsLowerLows(processedData)
         elif executeOption == 27:
             isValid = screener.findATRCross(processedData,saveDictionary, screeningDictionary)
         elif executeOption == 28:
             isValid = screener.findHigherBullishOpens(processedData)
+        elif executeOption == 30: # findBuySellSignalsFromATRTrailing # findATRTrailingStops
+            isValid = screener.findATRTrailingStops(fullData,buySellAll=buySellAll,saveDict=saveDictionary,screenDict=screeningDictionary)
         
         return isValid        
                     
     def performBasicVolumeChecks(self, executeOption, volumeRatio, screeningDictionary, saveDictionary, processedData, configManager, screener):
         minVolume = configManager.minVolume / (
                     100 if configManager.isIntradayConfig() else 1
                 )
```

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 import pandas as pd
 from alive_progress import alive_bar
 from PIL import Image, ImageDraw, ImageFont
 from PKDevTools.classes import Archiver
 from PKDevTools.classes.PKDateUtilities import PKDateUtilities
 from PKDevTools.classes.Committer import Committer
 from PKDevTools.classes.SuppressOutput import SuppressOutput
+from PKDevTools.classes.FunctionTimeouts import exit_after
 from tabulate import tabulate
 
 import pkscreener.classes.ConfigManager as ConfigManager
 import pkscreener.classes.Fetcher as Fetcher
 from pkscreener.classes import VERSION, Changelog
 from pkscreener.classes.MenuOptions import menus
 from PKNSETools.PKNSEStockDataFetcher import nseStockDataFetcher
```

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/classes/keys.py` & `pkscreener-0.44.20240512.361/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/courbd.ttf` & `pkscreener-0.44.20240512.361/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/globals.py` & `pkscreener-0.44.20240512.361/pkscreener/globals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1084,22 +1084,37 @@
         ca_dfs = [dividend_df, bonus_df, stockSplit_df]
         listStockCodes = []
         for df in ca_dfs:
             df = df[
                 df["Stock"].astype(str).str.contains("BSE:") == False
             ]
             listStockCodes.extend(list(df["Stock"]))
+    if executeOption == 30:
+        selectedMenu = m2.find(str(executeOption))
+        if len(options) >= 4:
+            if str(options[3]).isnumeric():
+                maLength = int(options[3])
+            elif str(options[3]).upper() == "D":
+                maLength = 1
+        elif len(options) >= 3:
+            maLength = 1 # By default buy option
+        else:
+            maLength = Utility.tools.promptSubMenuOptions(selectedMenu)
+        if maLength == 0:
+            return None, None
+        else:
+            selectedChoice["3"] = str(maLength)
     if executeOption == 42:
         Utility.tools.getLastScreenedResults(defaultAnswer)
         return None, None
-    if executeOption >= 30 and executeOption <= 41:
+    if executeOption >= 31 and executeOption <= 41:
         OutputControls().printOutput(
             colorText.BOLD
             + colorText.FAIL
-            + "\n[+] Error: Option 30 to 41 Not implemented yet! Press <Enter> to continue."
+            + "\n[+] Error: Option 31 to 41 Not implemented yet! Press <Enter> to continue."
             + colorText.END
         )
         input("Press <Enter> to continue...")
         return None, None
     if (
         not str(indexOption).isnumeric() and indexOption in ["W", "E", "M", "N", "Z"]
     ) or (
@@ -1573,14 +1588,18 @@
         sorting = False
     return sorting
 
 def resetConfigToDefault():
     isIntraday = userPassedArgs is not None and userPassedArgs.intraday is not None
     if configManager.isIntradayConfig() or isIntraday:
         configManager.toggleConfig(candleDuration="1d", clearCache=False)
+    if "PKDevTools_Default_Log_Level" in os.environ.keys():
+        del os.environ['PKDevTools_Default_Log_Level']
+    configManager.logsEnabled = False
+    configManager.setConfig(ConfigManager.parser,default=True,showFileCreatedText=False)
 
 def prepareStocksForScreening(testing, downloadOnly, listStockCodes, indexOption):
     if not downloadOnly:
         updateMenuChoiceHierarchy()
     indexOption = int(indexOption)
     if listStockCodes is None or len(listStockCodes) == 0:
         if indexOption >= 0 and indexOption <= 14:
@@ -1730,14 +1749,20 @@
             + f'>{level3_X_Reversal_MenuDict[selectedChoice["3"]].strip()}'
         )
         if len(selectedChoice) >= 5 and selectedChoice["3"] in ["7","10"]:
             menuChoiceHierarchy = (
             menuChoiceHierarchy
             + f'>{level4_X_Lorenzian_MenuDict[selectedChoice["4"]].strip()}'
         )
+    elif selectedChoice["2"] in ["30"]:
+        if len(selectedChoice) >= 3:
+            menuChoiceHierarchy = (
+            menuChoiceHierarchy
+            + f'>{level4_X_Lorenzian_MenuDict[selectedChoice["3"]].strip()}'
+        )
     elif selectedChoice["2"] == "7":
         menuChoiceHierarchy = (
             menuChoiceHierarchy
             + f'>{level3_X_ChartPattern_MenuDict[selectedChoice["3"]].strip()}'
         )
         if len(selectedChoice) >= 5 and selectedChoice["3"] == "3":
             menuChoiceHierarchy = (
@@ -2257,22 +2282,25 @@
                                 headers="keys",
                                 showindex=False,
                                 tablefmt=colorText.No_Pad_GridFormat,
                                 maxcolwidths=Utility.tools.getMaxColumnWidths(scr_df)
                             )
                         tableLength = 2*len(lstscreen)+5
                         OutputControls().printOutput('\n'+tabulated_results)
+                        # Move the cursor up, back to the top because we want the progress bar to keep showing at the top
                         sys.stdout.write(f"\x1b[{tableLength}A")  # cursor up one line
                 if keyboardInterruptEventFired:
                     return False, backtest_df
                 return not ((testing and len(lstscreen) >= 1) or len(lstscreen) >= max_allowed), backtest_df
             otherArgs = (menuOption, backtestPeriod, result, lstscreen, lstsave)
             backtest_df, result =PKScanRunner.runScan(userPassedArgs,testing,numStocks,iterations,items,numStocksPerIteration,tasks_queue,results_queue,originalNumberOfStocks,backtest_df,*otherArgs,resultsReceivedCb=processResultsCallback)
 
         OutputControls().printOutput(f"\x1b[{3 if OutputControls().enableMultipleLineOutput else 1}A")
+        if len(lstscreen) == 0 and userPassedArgs is not None and userPassedArgs.monitor is None:
+            OutputControls().printOutput("\x1b[2K") # Delete the progress bar line
         elapsed_time = time.time() - start_time
         if menuOption in ["X", "G", "C"]:
             # create extension
             screenResults = pd.DataFrame(lstscreen)
             saveResults = pd.DataFrame(lstsave)
 
     except KeyboardInterrupt:
@@ -2641,15 +2669,14 @@
     )
     indexOption, executeOption = initPostLevel1Execution(
         indexOption=indexOption,
         executeOption=executeOption,
         skip=[
             "0",
             "29",
-            "30",
             "42",
         ],
     )
     return indexOption, executeOption, backtestPeriod
 
 def toggleUserConfig():
     configManager.toggleConfig(
```

### Comparing `pkscreener-0.44.20240511.360/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240512.361/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240512.361/pkscreener/pkscreenerbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,22 +110,22 @@
 TOP_LEVEL_SCANNER_MENUS = ["X", "B", "MI","DV"]
 TOP_LEVEL_SCANNER_SKIP_MENUS = ["M", "S", "G", "C", "T", "D", "I", "E", "U", "L", "Z"]
 INDEX_SKIP_MENUS = ["W","E","M","Z","0","2","3","4","6","7","9","10","13"]
 SCANNER_SKIP_MENUS_1_TO_6 = ["0","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_7_TO_12 = ["0","1","2","3","4","5","6","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_13_TO_18 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","19","20","21","22","23","24","25","26","27","28","29","30","42","M","Z"]
 SCANNER_SKIP_MENUS_19_TO_25 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","22","26","27","28","29","30","42","M","Z"]
-SCANNER_SKIP_MENUS_26_TO_31 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","30","42","M","Z"]
-SCANNER_MENUS_WITH_NO_SUBMENUS = ["1","2","3","10","11","12","13","14","15","16","17","18","19","20","21","23","24","25","26","27","28"]
+SCANNER_SKIP_MENUS_26_TO_31 = ["0","1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","42","M","Z"]
+SCANNER_MENUS_WITH_NO_SUBMENUS = ["1","2","3","10","11","12","13","14","15","16","17","18","19","20","21","23","24","25","26","27","28","29","30"]
 SCANNER_MENUS_WITH_SUBMENU_SUPPORT = ["6", "7", "21"]
 
 INDEX_COMMANDS_SKIP_MENUS_SCANNER = ["W", "E", "M", "Z"]
 INDEX_COMMANDS_SKIP_MENUS_BACKTEST = ["W", "E", "M", "Z", "N", "0", "15"]
-UNSUPPORTED_COMMAND_MENUS =["22","30","42","M","Z"]
-SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29"]
+UNSUPPORTED_COMMAND_MENUS =["22","42","M","Z"]
+SUPPORTED_COMMAND_MENUS = ["1","2","3","4","5","6","7","8","9","10","11","12","13","14","15","16","17","18","19","20","21","22","23","24","25","26","27","28","29","30"]
 
 async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, updatedResults=None, monitorIndex=0,chosenBotMenuOption="") -> int:
     """Send message on `/start`."""
     updateCarrier = None
     if update is None:
         return
     else:
```

### Comparing `pkscreener-0.44.20240511.360/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240512.361/pkscreener/pkscreenercli.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 start_time = None
 dbTimestamp = None
 elapsed_time = None
 configManager = ConfigManager.tools()
 
 def removeMonitorFile():
     from PKDevTools.classes import Archiver
-    from globals import resetConfigToDefault
+    from pkscreener.globals import resetConfigToDefault
     filePath = os.path.join(Archiver.get_user_outputs_dir(), "monitor_outputs")
     index = 0
     while index < configManager.maxDashboardWidgetsPerRow*configManager.maxNumResultRowsInMonitor:
         try:
             os.remove(f"{filePath}_{index}.txt")
         except:
             pass
```

### Comparing `pkscreener-0.44.20240511.360/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240512.361/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240511.360
+Version: 0.44.20240512.361
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240511.360.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240512.361.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240510.358/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240510.358/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240510.358/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240511.360/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240511.360/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240512.361/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240511.360/setup.py` & `pkscreener-0.44.20240512.361/setup.py`

 * *Files identical despite different names*

