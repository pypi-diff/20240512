# Comparing `tmp/PKNSETools-0.1.20240510.103.tar.gz` & `tmp/PKNSETools-0.1.20240512.104.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240510.103.tar", last modified: Fri May 10 18:56:05 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240512.104.tar", last modified: Sun May 12 13:51:43 2024, max compression
```

## Comparing `PKNSETools-0.1.20240510.103.tar` & `PKNSETools-0.1.20240512.104.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 18:56:05.535558 PKNSETools-0.1.20240510.103/
--rw-rw-rw-   0        0        0     2663 2024-05-10 18:56:05.535558 PKNSETools-0.1.20240510.103/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-10 18:56:05.519926 PKNSETools-0.1.20240510.103/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-05-10 18:56:05.535558 PKNSETools-0.1.20240510.103/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 18:56:05.535558 PKNSETools-0.1.20240510.103/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3386 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10770 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2635 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0    10376 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0    13763 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       31 2024-05-10 18:56:01.000000 PKNSETools-0.1.20240510.103/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 18:56:05.535558 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61961 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29916 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 18:56:05.535558 PKNSETools-0.1.20240510.103/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2663 2024-05-10 18:56:05.000000 PKNSETools-0.1.20240510.103/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-10 18:56:05.000000 PKNSETools-0.1.20240510.103/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 18:56:05.000000 PKNSETools-0.1.20240510.103/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-10 18:55:59.000000 PKNSETools-0.1.20240510.103/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-05-10 18:56:05.000000 PKNSETools-0.1.20240510.103/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-10 18:56:05.000000 PKNSETools-0.1.20240510.103/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/README.md
--rw-rw-rw-   0        0        0       86 2024-05-10 18:56:05.535558 PKNSETools-0.1.20240510.103/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-05-10 18:54:12.000000 PKNSETools-0.1.20240510.103/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:51:43.050501 PKNSETools-0.1.20240512.104/
+-rw-rw-rw-   0        0        0     2663 2024-05-12 13:51:43.050501 PKNSETools-0.1.20240512.104/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-12 13:51:43.050501 PKNSETools-0.1.20240512.104/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-12 13:51:43.050501 PKNSETools-0.1.20240512.104/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:51:43.050501 PKNSETools-0.1.20240512.104/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10770 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2635 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0    10388 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0    13763 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       31 2024-05-12 13:51:37.000000 PKNSETools-0.1.20240512.104/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:51:43.050501 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 13:51:43.050501 PKNSETools-0.1.20240512.104/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2663 2024-05-12 13:51:43.000000 PKNSETools-0.1.20240512.104/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-12 13:51:43.000000 PKNSETools-0.1.20240512.104/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 13:51:43.000000 PKNSETools-0.1.20240512.104/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-12 13:51:35.000000 PKNSETools-0.1.20240512.104/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-12 13:51:43.000000 PKNSETools-0.1.20240512.104/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-12 13:51:43.000000 PKNSETools-0.1.20240512.104/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-12 13:51:43.050501 PKNSETools-0.1.20240512.104/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-12 13:50:33.000000 PKNSETools-0.1.20240512.104/setup.py
```

### Comparing `PKNSETools-0.1.20240510.103/PKG-INFO` & `PKNSETools-0.1.20240512.104/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240510.103
+Version: 0.1.20240512.104
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240510.103.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240512.104.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240512.104/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240512.104/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240512.104/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240512.104/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240512.104/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240512.104/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240512.104/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240512.104/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240512.104/PKNSETools/PKIntraDay.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     def __init__(self, ticker:str):
         self.baseNumber = 0
         self.session = requests.session()
         self.ticker = ticker if ticker.upper().endswith("EQN") else f"{ticker}EQN"
         self.symbol = self.ticker[0:-3]
         # self.session.get(f'{_base_domain}', headers=_head)
         if len(self.session.cookies.keys()) == 0:
-            self.session.get(f'{_base_domain}{_quote_url_path_html}'.format(ticker), headers=_head)
+            self.session.get(f'{_base_domain}{_quote_url_path_html}'.format(ticker), headers=_head, timeout=10)
 
     def _secondsTotime(self, seconds):
         seconds = seconds % (24 * 3600)
         hour = seconds // 3600
         seconds %= 3600
         minutes = seconds // 60
         seconds %= 60
```

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240512.104/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240512.104/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240512.104/PKNSETools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240510.103
+Version: 0.1.20240512.104
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240510.103.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240512.104.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240510.103/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240512.104/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/README.md` & `PKNSETools-0.1.20240512.104/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240510.103/setup.py` & `PKNSETools-0.1.20240512.104/setup.py`

 * *Files identical despite different names*

