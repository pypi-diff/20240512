# Comparing `tmp/portfolio_tracker-0.1.1.3.tar.gz` & `tmp/portfolio_tracker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_tracker-0.1.1.3.tar", last modified: Sun May 12 11:18:03 2024, max compression
+gzip compressed data, was "portfolio_tracker-0.1.2.tar", last modified: Sun May 12 11:19:03 2024, max compression
```

## Comparing `portfolio_tracker-0.1.1.3.tar` & `portfolio_tracker-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 11:18:03.691139 portfolio_tracker-0.1.1.3/
--rw-rw-rw-   0        0        0     3355 2024-05-12 11:18:03.690129 portfolio_tracker-0.1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2888 2024-05-12 11:17:53.000000 portfolio_tracker-0.1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 11:18:03.675128 portfolio_tracker-0.1.1.3/portfolio_tracker/
--rw-rw-rw-   0        0        0      154 2024-05-12 10:43:36.000000 portfolio_tracker-0.1.1.3/portfolio_tracker/__init__.py
--rw-rw-rw-   0        0        0    17652 2024-05-12 09:30:40.000000 portfolio_tracker-0.1.1.3/portfolio_tracker/manager.py
--rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.1.1.3/portfolio_tracker/price_repo.py
--rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.1.1.3/portfolio_tracker/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:18:03.689157 portfolio_tracker-0.1.1.3/portfolio_tracker.egg-info/
--rw-rw-rw-   0        0        0     3355 2024-05-12 11:18:03.000000 portfolio_tracker-0.1.1.3/portfolio_tracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2024-05-12 11:18:03.000000 portfolio_tracker-0.1.1.3/portfolio_tracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 11:18:03.000000 portfolio_tracker-0.1.1.3/portfolio_tracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-12 11:18:03.000000 portfolio_tracker-0.1.1.3/portfolio_tracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-12 11:18:03.000000 portfolio_tracker-0.1.1.3/portfolio_tracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 11:18:03.691139 portfolio_tracker-0.1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      906 2024-05-12 11:17:53.000000 portfolio_tracker-0.1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:19:03.255773 portfolio_tracker-0.1.2/
+-rw-rw-rw-   0        0        0     3351 2024-05-12 11:19:03.254744 portfolio_tracker-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2888 2024-05-12 11:17:53.000000 portfolio_tracker-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 11:19:03.247999 portfolio_tracker-0.1.2/portfolio_tracker/
+-rw-rw-rw-   0        0        0      154 2024-05-12 10:43:36.000000 portfolio_tracker-0.1.2/portfolio_tracker/__init__.py
+-rw-rw-rw-   0        0        0    17652 2024-05-12 09:30:40.000000 portfolio_tracker-0.1.2/portfolio_tracker/manager.py
+-rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.1.2/portfolio_tracker/price_repo.py
+-rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.1.2/portfolio_tracker/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:19:03.253744 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/
+-rw-rw-rw-   0        0        0     3351 2024-05-12 11:19:03.000000 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2024-05-12 11:19:03.000000 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 11:19:03.000000 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-12 11:19:03.000000 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-12 11:19:03.000000 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 11:19:03.255773 portfolio_tracker-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      896 2024-05-12 11:18:58.000000 portfolio_tracker-0.1.2/setup.py
```

### Comparing `portfolio_tracker-0.1.1.3/PKG-INFO` & `portfolio_tracker-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: portfolio_tracker
-Version: 0.1.1.3
+Version: 0.1.2
 Summary: A portfolio tracker library, that allows to track a portfolio of stocks and their performance.
 Author: Poli Luca
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: yfinance
 Requires-Dist: numpy
 Requires-Dist: pandas_market_calendars
 Requires-Dist: openpyxl
 
-\n
+
 # Stock Portfolio Tracker
 
 This library provides a set of Python modules for managing and tracking a stock portfolio.
 
 ## Description
 
 The project includes the following modules:
```

### Comparing `portfolio_tracker-0.1.1.3/README.md` & `portfolio_tracker-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.1.3/portfolio_tracker/manager.py` & `portfolio_tracker-0.1.2/portfolio_tracker/manager.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.1.3/portfolio_tracker/price_repo.py` & `portfolio_tracker-0.1.2/portfolio_tracker/price_repo.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.1.3/portfolio_tracker/utils.py` & `portfolio_tracker-0.1.2/portfolio_tracker/utils.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.1.3/portfolio_tracker.egg-info/PKG-INFO` & `portfolio_tracker-0.1.2/portfolio_tracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: portfolio-tracker
-Version: 0.1.1.3
+Version: 0.1.2
 Summary: A portfolio tracker library, that allows to track a portfolio of stocks and their performance.
 Author: Poli Luca
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: yfinance
 Requires-Dist: numpy
 Requires-Dist: pandas_market_calendars
 Requires-Dist: openpyxl
 
-\n
+
 # Stock Portfolio Tracker
 
 This library provides a set of Python modules for managing and tracking a stock portfolio.
 
 ## Description
 
 The project includes the following modules:
```

### Comparing `portfolio_tracker-0.1.1.3/setup.py` & `portfolio_tracker-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 import os
 import codecs
 
 # version = '{{VERSION_PLACEHOLDER}}'
-version = '0.1.1.3'
+version = '0.1.2'
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\\n" + fh.read()
+    long_description = fh.read()
 
 setup(
     name='portfolio_tracker',
     python_requires='>=3.10',
     packages=find_packages(include=['portfolio_tracker']),
     version=version,
     description='A portfolio tracker library, that allows to track a portfolio of stocks and their performance.',
```

