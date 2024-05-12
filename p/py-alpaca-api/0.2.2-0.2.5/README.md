# Comparing `tmp/py_alpaca_api-0.2.2.tar.gz` & `tmp/py_alpaca_api-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.2.2.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.2.5.tar", max compression
```

## Comparing `py_alpaca_api-0.2.2.tar` & `py_alpaca_api-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.2.2/LICENSE
--rw-r--r--   0        0        0    12345 2024-05-12 02:10:59.952064 py_alpaca_api-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.2.2/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0    20598 2024-05-12 02:10:59.962064 py_alpaca_api-0.2.2/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0    10308 2024-05-11 22:19:24.885819 py_alpaca_api-0.2.2/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     1159 2024-05-12 02:19:18.691926 py_alpaca_api-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    13030 1970-01-01 00:00:00.000000 py_alpaca_api-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-11 23:37:32.674625 py_alpaca_api-0.2.5/LICENSE
+-rw-r--r--   0        0        0    12576 2024-05-12 02:52:40.341369 py_alpaca_api-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.2.5/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0    43735 2024-05-12 16:00:21.371412 py_alpaca_api-0.2.5/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0    17342 2024-05-12 16:00:21.371412 py_alpaca_api-0.2.5/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     1225 2024-05-12 16:00:21.371412 py_alpaca_api-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    13337 1970-01-01 00:00:00.000000 py_alpaca_api-0.2.5/PKG-INFO
```

### Comparing `py_alpaca_api-0.2.2/LICENSE` & `py_alpaca_api-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.2.2/README.md` & `py_alpaca_api-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 </details>
 <hr>
 
 ##  Overview
 
 The py-alpaca-api project is a Python library that simplifies interaction with the Alpaca API. It provides a robust interface, encapsulated in the `PyAlpacaApi` class, enabling developers to access Alpaca Market API trading functionalities effortlessly. By utilizing data classes for orders, assets, and accounts, the project abstracts away complexities, enhancing flexibility in processing API responses. With clear metadata management through Poetry, this project serves as a valuable tool for those looking to integrate Alpaca trading capabilities seamlessly into their applications.
 
+This project is still in development. New functionality will be added and updated daily. Hopefully this project will help make communicating with Alpaca Markets API, much easier for some. Any input or help would be appreciated.
+
 ---
 
 ##  Features
 
 |    |   Feature         | Description |
 |----|-------------------|---------------------------------------------------------------|
 | ⚙️  | **Architecture**  | Designed with a clear separation of concerns, utilizing data classes for enhanced abstraction and maintainability. Follows a modular approach to interact with the Alpaca API efficiently. |
@@ -174,15 +176,15 @@
 ---
 
 ##  Contributing
 
 Contributions are welcome! Here are several ways you can contribute:
 
 - **[Report Issues](https://github.com/TexasCoding/py-alpaca-api/issues)**: Submit bugs found or log feature requests for the `py-alpaca-api` project.
-- **[Submit Pull Requests](https://github.com/TexasCoding/py-alpaca-api/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
+- **[Submit Pull Requests](https://github.com/TexasCoding/py-alpaca-api/blob/master/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
 - **[Join the Discussions](https://github.com/TexasCoding/py-alpaca-api/discussions)**: Share your insights, provide feedback, or ask questions.
 
 <details closed>
 <summary>Contributing Guidelines</summary>
 
 1. **Fork the Repository**: Start by forking the project repository to your github account.
 2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
```

### Comparing `py_alpaca_api-0.2.2/pyproject.toml` & `py_alpaca_api-0.2.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.2.2"
+version = "0.2.5"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
+documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
 keywords = ["alpaca", "python"]
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pandas = "^2.2.2"
 requests = "^2.31.0"
 numpy = "^1.26.4"
```

### Comparing `py_alpaca_api-0.2.2/PKG-INFO` & `py_alpaca_api-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.2.2
+Version: 0.2.5
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Documentation, https://py-alpaca-api.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/TexasCoding/py-alpaca-api
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" alt="project-logo">
 </p>
 <p align="center">
@@ -55,14 +56,16 @@
 </details>
 <hr>
 
 ##  Overview
 
 The py-alpaca-api project is a Python library that simplifies interaction with the Alpaca API. It provides a robust interface, encapsulated in the `PyAlpacaApi` class, enabling developers to access Alpaca Market API trading functionalities effortlessly. By utilizing data classes for orders, assets, and accounts, the project abstracts away complexities, enhancing flexibility in processing API responses. With clear metadata management through Poetry, this project serves as a valuable tool for those looking to integrate Alpaca trading capabilities seamlessly into their applications.
 
+This project is still in development. New functionality will be added and updated daily. Hopefully this project will help make communicating with Alpaca Markets API, much easier for some. Any input or help would be appreciated.
+
 ---
 
 ##  Features
 
 |    |   Feature         | Description |
 |----|-------------------|---------------------------------------------------------------|
 | ⚙️  | **Architecture**  | Designed with a clear separation of concerns, utilizing data classes for enhanced abstraction and maintainability. Follows a modular approach to interact with the Alpaca API efficiently. |
@@ -193,15 +196,15 @@
 ---
 
 ##  Contributing
 
 Contributions are welcome! Here are several ways you can contribute:
 
 - **[Report Issues](https://github.com/TexasCoding/py-alpaca-api/issues)**: Submit bugs found or log feature requests for the `py-alpaca-api` project.
-- **[Submit Pull Requests](https://github.com/TexasCoding/py-alpaca-api/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
+- **[Submit Pull Requests](https://github.com/TexasCoding/py-alpaca-api/blob/master/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.
 - **[Join the Discussions](https://github.com/TexasCoding/py-alpaca-api/discussions)**: Share your insights, provide feedback, or ask questions.
 
 <details closed>
 <summary>Contributing Guidelines</summary>
 
 1. **Fork the Repository**: Start by forking the project repository to your github account.
 2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
```

