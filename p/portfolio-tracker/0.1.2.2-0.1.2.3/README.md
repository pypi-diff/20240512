# Comparing `tmp/portfolio_tracker-0.1.2.2.tar.gz` & `tmp/portfolio_tracker-0.1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_tracker-0.1.2.2.tar", last modified: Sun May 12 11:24:49 2024, max compression
+gzip compressed data, was "portfolio_tracker-0.1.2.3.tar", last modified: Sun May 12 11:34:13 2024, max compression
```

## Comparing `portfolio_tracker-0.1.2.2.tar` & `portfolio_tracker-0.1.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 11:24:49.338956 portfolio_tracker-0.1.2.2/
--rw-rw-rw-   0        0        0     3357 2024-05-12 11:24:49.337956 portfolio_tracker-0.1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2892 2024-05-12 11:24:33.000000 portfolio_tracker-0.1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 11:24:49.331928 portfolio_tracker-0.1.2.2/portfolio_tracker/
--rw-rw-rw-   0        0        0      154 2024-05-12 10:43:36.000000 portfolio_tracker-0.1.2.2/portfolio_tracker/__init__.py
--rw-rw-rw-   0        0        0    17652 2024-05-12 09:30:40.000000 portfolio_tracker-0.1.2.2/portfolio_tracker/manager.py
--rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.1.2.2/portfolio_tracker/price_repo.py
--rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.1.2.2/portfolio_tracker/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:24:49.336953 portfolio_tracker-0.1.2.2/portfolio_tracker.egg-info/
--rw-rw-rw-   0        0        0     3357 2024-05-12 11:24:49.000000 portfolio_tracker-0.1.2.2/portfolio_tracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2024-05-12 11:24:49.000000 portfolio_tracker-0.1.2.2/portfolio_tracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 11:24:49.000000 portfolio_tracker-0.1.2.2/portfolio_tracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-12 11:24:49.000000 portfolio_tracker-0.1.2.2/portfolio_tracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-12 11:24:49.000000 portfolio_tracker-0.1.2.2/portfolio_tracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 11:24:49.339955 portfolio_tracker-0.1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      898 2024-05-12 11:24:45.000000 portfolio_tracker-0.1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:34:13.847457 portfolio_tracker-0.1.2.3/
+-rw-rw-rw-   0        0        0     3357 2024-05-12 11:34:13.846457 portfolio_tracker-0.1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2892 2024-05-12 11:24:33.000000 portfolio_tracker-0.1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 11:34:13.840458 portfolio_tracker-0.1.2.3/portfolio_tracker/
+-rw-rw-rw-   0        0        0      131 2024-05-12 11:34:01.000000 portfolio_tracker-0.1.2.3/portfolio_tracker/__init__.py
+-rw-rw-rw-   0        0        0    17652 2024-05-12 09:30:40.000000 portfolio_tracker-0.1.2.3/portfolio_tracker/manager.py
+-rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.1.2.3/portfolio_tracker/price_repo.py
+-rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.1.2.3/portfolio_tracker/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:34:13.845457 portfolio_tracker-0.1.2.3/portfolio_tracker.egg-info/
+-rw-rw-rw-   0        0        0     3357 2024-05-12 11:34:13.000000 portfolio_tracker-0.1.2.3/portfolio_tracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2024-05-12 11:34:13.000000 portfolio_tracker-0.1.2.3/portfolio_tracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 11:34:13.000000 portfolio_tracker-0.1.2.3/portfolio_tracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-12 11:34:13.000000 portfolio_tracker-0.1.2.3/portfolio_tracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-12 11:34:13.000000 portfolio_tracker-0.1.2.3/portfolio_tracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 11:34:13.847457 portfolio_tracker-0.1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      898 2024-05-12 11:34:01.000000 portfolio_tracker-0.1.2.3/setup.py
```

### Comparing `portfolio_tracker-0.1.2.2/PKG-INFO` & `portfolio_tracker-0.1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio_tracker
-Version: 0.1.2.2
+Version: 0.1.2.3
 Summary: A portfolio tracker library, that allows to track a portfolio of stocks and their performance.
 Author: Poli Luca
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: yfinance
 Requires-Dist: numpy
```

### Comparing `portfolio_tracker-0.1.2.2/README.md` & `portfolio_tracker-0.1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.2.2/portfolio_tracker/manager.py` & `portfolio_tracker-0.1.2.3/portfolio_tracker/manager.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.2.2/portfolio_tracker/price_repo.py` & `portfolio_tracker-0.1.2.3/portfolio_tracker/price_repo.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.2.2/portfolio_tracker/utils.py` & `portfolio_tracker-0.1.2.3/portfolio_tracker/utils.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.2.2/portfolio_tracker.egg-info/PKG-INFO` & `portfolio_tracker-0.1.2.3/portfolio_tracker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio-tracker
-Version: 0.1.2.2
+Version: 0.1.2.3
 Summary: A portfolio tracker library, that allows to track a portfolio of stocks and their performance.
 Author: Poli Luca
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: yfinance
 Requires-Dist: numpy
```

### Comparing `portfolio_tracker-0.1.2.2/setup.py` & `portfolio_tracker-0.1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 import codecs
 
 # version = '{{VERSION_PLACEHOLDER}}'
-version = '0.1.2.2'
+version = '0.1.2.3'
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='portfolio_tracker',
```

