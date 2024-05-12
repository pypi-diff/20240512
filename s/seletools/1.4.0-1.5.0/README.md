# Comparing `tmp/seletools-1.4.0.tar.gz` & `tmp/seletools-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seletools-1.4.0.tar", last modified: Sun Apr  2 09:12:58 2023, max compression
+gzip compressed data, was "seletools-1.5.0.tar", last modified: Sun May 12 21:08:25 2024, max compression
```

## Comparing `seletools-1.4.0.tar` & `seletools-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 09:12:58.001074 seletools-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-02 09:12:38.000000 seletools-1.4.0/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-02 09:12:38.000000 seletools-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-02 09:12:38.000000 seletools-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-04-02 09:12:58.001074 seletools-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-04-02 09:12:38.000000 seletools-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-02 09:12:38.000000 seletools-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 09:12:58.001074 seletools-1.4.0/seletools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 09:12:38.000000 seletools-1.4.0/seletools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-02 09:12:38.000000 seletools-1.4.0/seletools/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-02 09:12:38.000000 seletools-1.4.0/seletools/drag_and_drop.js
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-02 09:12:38.000000 seletools-1.4.0/seletools/indexeddb.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-02 09:12:38.000000 seletools-1.4.0/seletools/localstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-02 09:12:38.000000 seletools-1.4.0/seletools/waits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 09:12:58.001074 seletools-1.4.0/seletools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-04-02 09:12:57.000000 seletools-1.4.0/seletools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-02 09:12:57.000000 seletools-1.4.0/seletools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 09:12:57.000000 seletools-1.4.0/seletools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-02 09:12:57.000000 seletools-1.4.0/seletools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 09:12:58.001074 seletools-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-02 09:12:38.000000 seletools-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:08:25.078578 seletools-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-12 21:08:16.000000 seletools-1.5.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-12 21:08:16.000000 seletools-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-12 21:08:16.000000 seletools-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-12 21:08:25.078578 seletools-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-12 21:08:16.000000 seletools-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-12 21:08:16.000000 seletools-1.5.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:08:25.078578 seletools-1.5.0/seletools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 21:08:16.000000 seletools-1.5.0/seletools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-12 21:08:16.000000 seletools-1.5.0/seletools/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-12 21:08:16.000000 seletools-1.5.0/seletools/drag_and_drop.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-12 21:08:16.000000 seletools-1.5.0/seletools/indexeddb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-12 21:08:16.000000 seletools-1.5.0/seletools/localstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-12 21:08:16.000000 seletools-1.5.0/seletools/waits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 21:08:25.078578 seletools-1.5.0/seletools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-12 21:08:25.000000 seletools-1.5.0/seletools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-12 21:08:25.000000 seletools-1.5.0/seletools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 21:08:25.000000 seletools-1.5.0/seletools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-12 21:08:25.000000 seletools-1.5.0/seletools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 21:08:25.078578 seletools-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-12 21:08:16.000000 seletools-1.5.0/setup.py
```

### Comparing `seletools-1.4.0/CHANGES` & `seletools-1.5.0/CHANGES`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Change Log
 ==========
 
+1.5.0
+----------
+- Added Quality Control workflow status badge to README
+- Updated Python version to 3.12.3 in GitHub Actions workflows
+- Updated package dependencies and minimum Python version
+- Updated IndexedDB setup in README
+- Updated license copyright year
+
 1.4.0
 ----------
 - Added remove item methods for IndexedDB & Local Storage
 - Added tests for remove item methods
 - Added monthly download stats
 - Added "black" as a code formatter
 - Updated package dependencies (selenium, pytest)
```

### Comparing `seletools-1.4.0/LICENSE` & `seletools-1.5.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Dmitrii Bormotov
+Copyright (c) 2024 Dmitrii Bormotov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `seletools-1.4.0/PKG-INFO` & `seletools-1.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: seletools
-Version: 1.4.0
+Version: 1.5.0
 Summary: Helpful tools for Selenium on Python
 Home-page: https://github.com/bormando/selenium-tools
 Author: Dmitrii Bormotov
 Author-email: squier7@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Selenium Tools
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/seletools)
+![Quality Control](https://github.com/bormando/selenium-tools/actions/workflows/qc.yml/badge.svg)
 
 ### About package
 Current package is called **Selenium Tools** for a reason - it contains useful helpers that are not included into Selenium natively. 
 
 Contributions are very welcome!
 
 ### Installation
@@ -79,22 +80,34 @@
 scripts = waits.scripts
 ```
 
 ### Interaction with IndexedDB
 It's possible to interact with IndexedDB database in browser via JavaScript. 
 This interface helps get/update/insert data in existing databases and tables.
 
-__Important: it's necessary to have logging enabled for your webdriver instance, since there's no other way for Selenium to get data from IndexedDB than gather it from the console. Here's how you can enable logging in your webdriver:__
+> [!WARNING]
+> It's necessary to have logging enabled for your webdriver instance, since there's no other way for Selenium to get data from IndexedDB than gather it from the console. The way to enable logs differs between versions of Selenium.
+
+#### Setup - Selenium 3
 ```
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 
+dc = DesiredCapabilities.CHROME
 dc["goog:loggingPrefs"] = {"browser": "ALL"}
 driver = webdriver.Chrome(desired_capabilities=dc)
 ```
 
+#### Setup - Selenium 4
+```
+from selenium import webdriver
+
+options = webdriver.ChromeOptions()
+options.set_capability("goog:loggingPrefs", {"browser": "ALL"})
+```
+
 Example:
 ```
 from seletools.indexeddb import IndexedDB
 
 idb = IndexedDB(driver, "mydb", 3)  # webdriver instance, db name, db version
 # GET value
 value = idb.get_value("keyvaluepairs", "foo")  # table name, key in table
```

### Comparing `seletools-1.4.0/README.md` & `seletools-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Selenium Tools
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/seletools)
+![Quality Control](https://github.com/bormando/selenium-tools/actions/workflows/qc.yml/badge.svg)
 
 ### About package
 Current package is called **Selenium Tools** for a reason - it contains useful helpers that are not included into Selenium natively. 
 
 Contributions are very welcome!
 
 ### Installation
@@ -64,22 +65,34 @@
 scripts = waits.scripts
 ```
 
 ### Interaction with IndexedDB
 It's possible to interact with IndexedDB database in browser via JavaScript. 
 This interface helps get/update/insert data in existing databases and tables.
 
-__Important: it's necessary to have logging enabled for your webdriver instance, since there's no other way for Selenium to get data from IndexedDB than gather it from the console. Here's how you can enable logging in your webdriver:__
+> [!WARNING]
+> It's necessary to have logging enabled for your webdriver instance, since there's no other way for Selenium to get data from IndexedDB than gather it from the console. The way to enable logs differs between versions of Selenium.
+
+#### Setup - Selenium 3
 ```
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 
+dc = DesiredCapabilities.CHROME
 dc["goog:loggingPrefs"] = {"browser": "ALL"}
 driver = webdriver.Chrome(desired_capabilities=dc)
 ```
 
+#### Setup - Selenium 4
+```
+from selenium import webdriver
+
+options = webdriver.ChromeOptions()
+options.set_capability("goog:loggingPrefs", {"browser": "ALL"})
+```
+
 Example:
 ```
 from seletools.indexeddb import IndexedDB
 
 idb = IndexedDB(driver, "mydb", 3)  # webdriver instance, db name, db version
 # GET value
 value = idb.get_value("keyvaluepairs", "foo")  # table name, key in table
```

### Comparing `seletools-1.4.0/seletools/actions.py` & `seletools-1.5.0/seletools/actions.py`

 * *Files identical despite different names*

### Comparing `seletools-1.4.0/seletools/drag_and_drop.js` & `seletools-1.5.0/seletools/drag_and_drop.js`

 * *Files identical despite different names*

### Comparing `seletools-1.4.0/seletools/indexeddb.py` & `seletools-1.5.0/seletools/indexeddb.py`

 * *Files identical despite different names*

### Comparing `seletools-1.4.0/seletools/waits.py` & `seletools-1.5.0/seletools/waits.py`

 * *Files identical despite different names*

### Comparing `seletools-1.4.0/seletools.egg-info/PKG-INFO` & `seletools-1.5.0/seletools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: seletools
-Version: 1.4.0
+Version: 1.5.0
 Summary: Helpful tools for Selenium on Python
 Home-page: https://github.com/bormando/selenium-tools
 Author: Dmitrii Bormotov
 Author-email: squier7@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Selenium Tools
 
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/seletools)
+![Quality Control](https://github.com/bormando/selenium-tools/actions/workflows/qc.yml/badge.svg)
 
 ### About package
 Current package is called **Selenium Tools** for a reason - it contains useful helpers that are not included into Selenium natively. 
 
 Contributions are very welcome!
 
 ### Installation
@@ -79,22 +80,34 @@
 scripts = waits.scripts
 ```
 
 ### Interaction with IndexedDB
 It's possible to interact with IndexedDB database in browser via JavaScript. 
 This interface helps get/update/insert data in existing databases and tables.
 
-__Important: it's necessary to have logging enabled for your webdriver instance, since there's no other way for Selenium to get data from IndexedDB than gather it from the console. Here's how you can enable logging in your webdriver:__
+> [!WARNING]
+> It's necessary to have logging enabled for your webdriver instance, since there's no other way for Selenium to get data from IndexedDB than gather it from the console. The way to enable logs differs between versions of Selenium.
+
+#### Setup - Selenium 3
 ```
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 
+dc = DesiredCapabilities.CHROME
 dc["goog:loggingPrefs"] = {"browser": "ALL"}
 driver = webdriver.Chrome(desired_capabilities=dc)
 ```
 
+#### Setup - Selenium 4
+```
+from selenium import webdriver
+
+options = webdriver.ChromeOptions()
+options.set_capability("goog:loggingPrefs", {"browser": "ALL"})
+```
+
 Example:
 ```
 from seletools.indexeddb import IndexedDB
 
 idb = IndexedDB(driver, "mydb", 3)  # webdriver instance, db name, db version
 # GET value
 value = idb.get_value("keyvaluepairs", "foo")  # table name, key in table
```

### Comparing `seletools-1.4.0/setup.py` & `seletools-1.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("CHANGES", "r", encoding="utf-8") as ch:
     changes = ch.read()
 
 setuptools.setup(
     name="seletools",
-    version="1.4.0",
+    version="1.5.0",
     author="Dmitrii Bormotov",
     author_email="squier7@gmail.com",
     description="Helpful tools for Selenium on Python",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bormando/selenium-tools",
@@ -21,9 +21,9 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=[
         "seletools",
     ],
     package_data={"seletools": ["drag_and_drop.js"]},
-    python_requires=">=3.6",
+    python_requires=">=3.8",
 )
```

