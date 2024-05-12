# Comparing `tmp/portfolio_tracker-0.1.2.tar.gz` & `tmp/portfolio_tracker-0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_tracker-0.1.2.tar", last modified: Sun May 12 11:19:03 2024, max compression
+gzip compressed data, was "portfolio_tracker-0.1.2.1.tar", last modified: Sun May 12 11:23:35 2024, max compression
```

## Comparing `portfolio_tracker-0.1.2.tar` & `portfolio_tracker-0.1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 11:19:03.255773 portfolio_tracker-0.1.2/
--rw-rw-rw-   0        0        0     3351 2024-05-12 11:19:03.254744 portfolio_tracker-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2888 2024-05-12 11:17:53.000000 portfolio_tracker-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 11:19:03.247999 portfolio_tracker-0.1.2/portfolio_tracker/
--rw-rw-rw-   0        0        0      154 2024-05-12 10:43:36.000000 portfolio_tracker-0.1.2/portfolio_tracker/__init__.py
--rw-rw-rw-   0        0        0    17652 2024-05-12 09:30:40.000000 portfolio_tracker-0.1.2/portfolio_tracker/manager.py
--rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.1.2/portfolio_tracker/price_repo.py
--rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.1.2/portfolio_tracker/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 11:19:03.253744 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/
--rw-rw-rw-   0        0        0     3351 2024-05-12 11:19:03.000000 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2024-05-12 11:19:03.000000 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 11:19:03.000000 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-12 11:19:03.000000 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-12 11:19:03.000000 portfolio_tracker-0.1.2/portfolio_tracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 11:19:03.255773 portfolio_tracker-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      896 2024-05-12 11:18:58.000000 portfolio_tracker-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:23:35.240400 portfolio_tracker-0.1.2.1/
+-rw-rw-rw-   0        0        0     3359 2024-05-12 11:23:35.238361 portfolio_tracker-0.1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2894 2024-05-12 11:23:27.000000 portfolio_tracker-0.1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 11:23:35.222361 portfolio_tracker-0.1.2.1/portfolio_tracker/
+-rw-rw-rw-   0        0        0      154 2024-05-12 10:43:36.000000 portfolio_tracker-0.1.2.1/portfolio_tracker/__init__.py
+-rw-rw-rw-   0        0        0    17652 2024-05-12 09:30:40.000000 portfolio_tracker-0.1.2.1/portfolio_tracker/manager.py
+-rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.1.2.1/portfolio_tracker/price_repo.py
+-rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.1.2.1/portfolio_tracker/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:23:35.237362 portfolio_tracker-0.1.2.1/portfolio_tracker.egg-info/
+-rw-rw-rw-   0        0        0     3359 2024-05-12 11:23:35.000000 portfolio_tracker-0.1.2.1/portfolio_tracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2024-05-12 11:23:35.000000 portfolio_tracker-0.1.2.1/portfolio_tracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 11:23:35.000000 portfolio_tracker-0.1.2.1/portfolio_tracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-12 11:23:35.000000 portfolio_tracker-0.1.2.1/portfolio_tracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-12 11:23:35.000000 portfolio_tracker-0.1.2.1/portfolio_tracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 11:23:35.240400 portfolio_tracker-0.1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      898 2024-05-12 11:20:52.000000 portfolio_tracker-0.1.2.1/setup.py
```

### Comparing `portfolio_tracker-0.1.2/PKG-INFO` & `portfolio_tracker-0.1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio_tracker
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: A portfolio tracker library, that allows to track a portfolio of stocks and their performance.
 Author: Poli Luca
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: yfinance
 Requires-Dist: numpy
@@ -20,15 +20,15 @@
 
 The project includes the following modules:
 
 - `price_repo.py`: Manages the stock prices repository, which is a csv file containing the prices of the stocks. This is used to avoid downloading the prices every time the program is executed.
 - `manager.py`: Contains the portfolio class and the functions to manage it. It allows for portfolio rebalancing, rolling forward, and other operations.
 - `utils.py`: Includes utility functions used in the project, such as functions for computing returns and rolling dates to business days.
 
-For a more detailed description of the modules, check the docstrings in the source code, or the documentation in the `docs` folder.
+For a more detailed documentation check the `docs` folder on GitHub: `https://github.com/LucaPoli59/PortfolioTrackerLib/tree/master/docs`
 
 ## Installation
 
 To install the library, run the following command:
 
 ```bash 
 pip install portfolio_tracker
@@ -75,10 +75,10 @@
 ```
 
 For more examples, check the `example.ipynb` notebook.
 
 
 ## Development
 
-This project is meant to be a simple tool for tracking a stock portfolio, it has been developed by Luca Poli from the quant team of the MIURA group, for the group itself.
+This library is meant to be a simple tool for tracking a stock portfolio, it has been developed by Luca Poli from the quant team of the MIURA group, for the group itself.
 
 For any bug or suggestion, please contact me through discord at https://discordapp.com/users/326499540540588032
```

### Comparing `portfolio_tracker-0.1.2/README.md` & `portfolio_tracker-0.1.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 The project includes the following modules:
 
 - `price_repo.py`: Manages the stock prices repository, which is a csv file containing the prices of the stocks. This is used to avoid downloading the prices every time the program is executed.
 - `manager.py`: Contains the portfolio class and the functions to manage it. It allows for portfolio rebalancing, rolling forward, and other operations.
 - `utils.py`: Includes utility functions used in the project, such as functions for computing returns and rolling dates to business days.
 
-For a more detailed description of the modules, check the docstrings in the source code, or the documentation in the `docs` folder.
+For a more detailed documentation check the `docs` folder on GitHub: `https://github.com/LucaPoli59/PortfolioTrackerLib/tree/master/docs`
 
 ## Installation
 
 To install the library, run the following command:
 
 ```bash 
 pip install portfolio_tracker
@@ -62,10 +62,10 @@
 ```
 
 For more examples, check the `example.ipynb` notebook.
 
 
 ## Development
 
-This project is meant to be a simple tool for tracking a stock portfolio, it has been developed by Luca Poli from the quant team of the MIURA group, for the group itself.
+This library is meant to be a simple tool for tracking a stock portfolio, it has been developed by Luca Poli from the quant team of the MIURA group, for the group itself.
 
 For any bug or suggestion, please contact me through discord at https://discordapp.com/users/326499540540588032
```

### Comparing `portfolio_tracker-0.1.2/portfolio_tracker/manager.py` & `portfolio_tracker-0.1.2.1/portfolio_tracker/manager.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.2/portfolio_tracker/price_repo.py` & `portfolio_tracker-0.1.2.1/portfolio_tracker/price_repo.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.2/portfolio_tracker/utils.py` & `portfolio_tracker-0.1.2.1/portfolio_tracker/utils.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.2/portfolio_tracker.egg-info/PKG-INFO` & `portfolio_tracker-0.1.2.1/portfolio_tracker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio-tracker
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: A portfolio tracker library, that allows to track a portfolio of stocks and their performance.
 Author: Poli Luca
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: yfinance
 Requires-Dist: numpy
@@ -20,15 +20,15 @@
 
 The project includes the following modules:
 
 - `price_repo.py`: Manages the stock prices repository, which is a csv file containing the prices of the stocks. This is used to avoid downloading the prices every time the program is executed.
 - `manager.py`: Contains the portfolio class and the functions to manage it. It allows for portfolio rebalancing, rolling forward, and other operations.
 - `utils.py`: Includes utility functions used in the project, such as functions for computing returns and rolling dates to business days.
 
-For a more detailed description of the modules, check the docstrings in the source code, or the documentation in the `docs` folder.
+For a more detailed documentation check the `docs` folder on GitHub: `https://github.com/LucaPoli59/PortfolioTrackerLib/tree/master/docs`
 
 ## Installation
 
 To install the library, run the following command:
 
 ```bash 
 pip install portfolio_tracker
@@ -75,10 +75,10 @@
 ```
 
 For more examples, check the `example.ipynb` notebook.
 
 
 ## Development
 
-This project is meant to be a simple tool for tracking a stock portfolio, it has been developed by Luca Poli from the quant team of the MIURA group, for the group itself.
+This library is meant to be a simple tool for tracking a stock portfolio, it has been developed by Luca Poli from the quant team of the MIURA group, for the group itself.
 
 For any bug or suggestion, please contact me through discord at https://discordapp.com/users/326499540540588032
```

### Comparing `portfolio_tracker-0.1.2/setup.py` & `portfolio_tracker-0.1.2.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 import codecs
 
 # version = '{{VERSION_PLACEHOLDER}}'
-version = '0.1.2'
+version = '0.1.2.1'
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='portfolio_tracker',
```

