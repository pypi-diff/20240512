# Comparing `tmp/portfolio_tracker-0.1.0.tar.gz` & `tmp/portfolio_tracker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_tracker-0.1.0.tar", last modified: Sun May 12 10:03:57 2024, max compression
+gzip compressed data, was "portfolio_tracker-0.1.1.tar", last modified: Sun May 12 10:04:36 2024, max compression
```

## Comparing `portfolio_tracker-0.1.0.tar` & `portfolio_tracker-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 10:03:57.819791 portfolio_tracker-0.1.0/
--rw-rw-rw-   0        0        0      323 2024-05-12 10:03:57.818791 portfolio_tracker-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-12 10:03:57.806698 portfolio_tracker-0.1.0/portfolio_tracker/
--rw-rw-rw-   0        0        0      127 2024-05-12 10:02:34.000000 portfolio_tracker-0.1.0/portfolio_tracker/__init__.py
--rw-rw-rw-   0        0        0    17652 2024-05-12 09:30:40.000000 portfolio_tracker-0.1.0/portfolio_tracker/manager.py
--rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.1.0/portfolio_tracker/price_repo.py
--rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.1.0/portfolio_tracker/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:03:57.817792 portfolio_tracker-0.1.0/portfolio_tracker.egg-info/
--rw-rw-rw-   0        0        0      323 2024-05-12 10:03:57.000000 portfolio_tracker-0.1.0/portfolio_tracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2024-05-12 10:03:57.000000 portfolio_tracker-0.1.0/portfolio_tracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 10:03:57.000000 portfolio_tracker-0.1.0/portfolio_tracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-12 10:03:57.000000 portfolio_tracker-0.1.0/portfolio_tracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-12 10:03:57.000000 portfolio_tracker-0.1.0/portfolio_tracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 10:03:57.819791 portfolio_tracker-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      541 2024-05-12 09:47:06.000000 portfolio_tracker-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:04:36.169967 portfolio_tracker-0.1.1/
+-rw-rw-rw-   0        0        0      323 2024-05-12 10:04:36.168966 portfolio_tracker-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-12 10:04:36.162972 portfolio_tracker-0.1.1/portfolio_tracker/
+-rw-rw-rw-   0        0        0      127 2024-05-12 10:04:33.000000 portfolio_tracker-0.1.1/portfolio_tracker/__init__.py
+-rw-rw-rw-   0        0        0    17652 2024-05-12 09:30:40.000000 portfolio_tracker-0.1.1/portfolio_tracker/manager.py
+-rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.1.1/portfolio_tracker/price_repo.py
+-rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.1.1/portfolio_tracker/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 10:04:36.167967 portfolio_tracker-0.1.1/portfolio_tracker.egg-info/
+-rw-rw-rw-   0        0        0      323 2024-05-12 10:04:36.000000 portfolio_tracker-0.1.1/portfolio_tracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2024-05-12 10:04:36.000000 portfolio_tracker-0.1.1/portfolio_tracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 10:04:36.000000 portfolio_tracker-0.1.1/portfolio_tracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-12 10:04:36.000000 portfolio_tracker-0.1.1/portfolio_tracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-12 10:04:36.000000 portfolio_tracker-0.1.1/portfolio_tracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 10:04:36.169967 portfolio_tracker-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      541 2024-05-12 10:04:33.000000 portfolio_tracker-0.1.1/setup.py
```

### Comparing `portfolio_tracker-0.1.0/portfolio_tracker/manager.py` & `portfolio_tracker-0.1.1/portfolio_tracker/manager.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.0/portfolio_tracker/price_repo.py` & `portfolio_tracker-0.1.1/portfolio_tracker/price_repo.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.0/portfolio_tracker/utils.py` & `portfolio_tracker-0.1.1/portfolio_tracker/utils.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.0/setup.py` & `portfolio_tracker-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='portfolio_tracker',
     python_requires='>=3.10',
     packages=find_packages(include=['portfolio_tracker']),
-    version='0.1.0',
+    version='0.1.1',
     description='A portfolio tracker library, that allows to track a portfolio of stocks and their performance.',
     author='Poli Luca',
     install_requires=['pandas', 'yfinance', 'numpy', 'pandas_market_calendars'],
     package_data={'docs': ['manager.html', 'price_repo.html', 'utils.html', 'xlsx_example.xlsx', 'example.ipynb']},
 )
```

