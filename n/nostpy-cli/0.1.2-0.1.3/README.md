# Comparing `tmp/nostpy_cli-0.1.2.tar.gz` & `tmp/nostpy_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostpy_cli-0.1.2.tar", last modified: Sun May 12 04:26:58 2024, max compression
+gzip compressed data, was "nostpy_cli-0.1.3.tar", last modified: Sun May 12 04:33:31 2024, max compression
```

## Comparing `nostpy_cli-0.1.2.tar` & `nostpy_cli-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:26:58.079561 nostpy_cli-0.1.2/
--rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.1.2/LICENSE
--rw-r--r--   0 tron      (1000) tron      (1000)     2364 2024-05-12 04:26:58.079561 nostpy_cli-0.1.2/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)     1792 2024-05-12 04:16:10.000000 nostpy_cli-0.1.2/README.md
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:26:58.079561 nostpy_cli-0.1.2/nostpy_cli/
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.1.2/nostpy_cli/__init__.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     5880 2024-05-12 04:16:10.000000 nostpy_cli-0.1.2/nostpy_cli/create_event.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.1.2/nostpy_cli/kind4.py
--rwxrwxr-x   0 tron      (1000) tron      (1000)     3199 2024-05-12 04:16:10.000000 nostpy_cli-0.1.2/nostpy_cli/main.py
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:26:58.079561 nostpy_cli-0.1.2/nostpy_cli.egg-info/
--rw-r--r--   0 tron      (1000) tron      (1000)     2364 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/entry_points.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/requires.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 04:26:58.000000 nostpy_cli-0.1.2/nostpy_cli.egg-info/top_level.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)      704 2024-05-12 04:26:52.000000 nostpy_cli-0.1.2/pyproject.toml
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:26:58.079561 nostpy_cli-0.1.2/setup.cfg
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:33:31.481315 nostpy_cli-0.1.3/
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.1.3/LICENSE
+-rw-r--r--   0 tron      (1000) tron      (1000)     2396 2024-05-12 04:33:31.481315 nostpy_cli-0.1.3/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1824 2024-05-12 04:33:16.000000 nostpy_cli-0.1.3/README.md
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:33:31.481315 nostpy_cli-0.1.3/nostpy_cli/
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.1.3/nostpy_cli/__init__.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     5880 2024-05-12 04:16:10.000000 nostpy_cli-0.1.3/nostpy_cli/create_event.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.1.3/nostpy_cli/kind4.py
+-rwxrwxr-x   0 tron      (1000) tron      (1000)     3199 2024-05-12 04:16:10.000000 nostpy_cli-0.1.3/nostpy_cli/main.py
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:33:31.481315 nostpy_cli-0.1.3/nostpy_cli.egg-info/
+-rw-r--r--   0 tron      (1000) tron      (1000)     2396 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/requires.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/top_level.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)      704 2024-05-12 04:29:05.000000 nostpy_cli-0.1.3/pyproject.toml
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:33:31.481315 nostpy_cli-0.1.3/setup.cfg
```

### Comparing `nostpy_cli-0.1.2/LICENSE` & `nostpy_cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.2/PKG-INFO` & `nostpy_cli-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostpy-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: CLI tool for handling nostpy events
 Author-email: Brian Hartford <bh419@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/UTXOnly/nostpy-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,41 +18,45 @@
 
 # nostpy-cli
 
 `nostpy-cli` is a Command Line Interface (CLI) tool designed to handle nostpy events efficiently. This tool provides easy-to-use commands to send and query events via a WebSocket connection.
 
 ## Features
 
-- Send events to a specified relay.
-- Query events from a relay.
+- Send events to a specified relays
+- Query events from relays
+- Encode/decode kind4 messages
 
 ## Prerequisites
 
 Before installing `nostpy-cli`, ensure you have Python 3.6 or higher installed on your system. You can check your Python version by running:
 
 ```
 python3 --version
 ```
 ## Installation
+
+### Install Using pip
+To install using `pip` use the command below:
+```
+pip install nostpy-cli
+```
+
 ### Build from source
 Clone the Repository
 First, clone the repository to your local machine:
 
 ```
 git clone https://github.com/UTXOnly/nostpy-cli.git
 cd nostpy-cli
 python3 -m build
 pip install .
 ```
 
-### Install Using pip
-To install using `pip` use the command below:
-```
-pip install nostpy-cli
-```
+
 
 ## Usage
 Once installed, you can run nostpy-cli from the command line. Below are some examples of how to use the CLI tool:
 
 ### Send Event
 To send an event, you would use a command similar to the following:
```

### Comparing `nostpy_cli-0.1.2/README.md` & `nostpy_cli-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 # nostpy-cli
 
 `nostpy-cli` is a Command Line Interface (CLI) tool designed to handle nostpy events efficiently. This tool provides easy-to-use commands to send and query events via a WebSocket connection.
 
 ## Features
 
-- Send events to a specified relay.
-- Query events from a relay.
+- Send events to a specified relays
+- Query events from relays
+- Encode/decode kind4 messages
 
 ## Prerequisites
 
 Before installing `nostpy-cli`, ensure you have Python 3.6 or higher installed on your system. You can check your Python version by running:
 
 ```
 python3 --version
 ```
 ## Installation
+
+### Install Using pip
+To install using `pip` use the command below:
+```
+pip install nostpy-cli
+```
+
 ### Build from source
 Clone the Repository
 First, clone the repository to your local machine:
 
 ```
 git clone https://github.com/UTXOnly/nostpy-cli.git
 cd nostpy-cli
 python3 -m build
 pip install .
 ```
 
-### Install Using pip
-To install using `pip` use the command below:
-```
-pip install nostpy-cli
-```
+
 
 ## Usage
 Once installed, you can run nostpy-cli from the command line. Below are some examples of how to use the CLI tool:
 
 ### Send Event
 To send an event, you would use a command similar to the following:
```

### Comparing `nostpy_cli-0.1.2/nostpy_cli/create_event.py` & `nostpy_cli-0.1.3/nostpy_cli/create_event.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.2/nostpy_cli/kind4.py` & `nostpy_cli-0.1.3/nostpy_cli/kind4.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.2/nostpy_cli/main.py` & `nostpy_cli-0.1.3/nostpy_cli/main.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.2/nostpy_cli.egg-info/PKG-INFO` & `nostpy_cli-0.1.3/nostpy_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostpy-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: CLI tool for handling nostpy events
 Author-email: Brian Hartford <bh419@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/UTXOnly/nostpy-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,41 +18,45 @@
 
 # nostpy-cli
 
 `nostpy-cli` is a Command Line Interface (CLI) tool designed to handle nostpy events efficiently. This tool provides easy-to-use commands to send and query events via a WebSocket connection.
 
 ## Features
 
-- Send events to a specified relay.
-- Query events from a relay.
+- Send events to a specified relays
+- Query events from relays
+- Encode/decode kind4 messages
 
 ## Prerequisites
 
 Before installing `nostpy-cli`, ensure you have Python 3.6 or higher installed on your system. You can check your Python version by running:
 
 ```
 python3 --version
 ```
 ## Installation
+
+### Install Using pip
+To install using `pip` use the command below:
+```
+pip install nostpy-cli
+```
+
 ### Build from source
 Clone the Repository
 First, clone the repository to your local machine:
 
 ```
 git clone https://github.com/UTXOnly/nostpy-cli.git
 cd nostpy-cli
 python3 -m build
 pip install .
 ```
 
-### Install Using pip
-To install using `pip` use the command below:
-```
-pip install nostpy-cli
-```
+
 
 ## Usage
 Once installed, you can run nostpy-cli from the command line. Below are some examples of how to use the CLI tool:
 
 ### Send Event
 To send an event, you would use a command similar to the following:
```

### Comparing `nostpy_cli-0.1.2/pyproject.toml` & `nostpy_cli-0.1.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nostpy-cli"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{ name = "Brian Hartford", email = "bh419@protonmail.com" }]
 description = "CLI tool for handling nostpy events"
 readme = "README.md"
 license = { text = "MIT" }
 urls = { homepage = "https://github.com/UTXOnly/nostpy-cli" }
 classifiers = [
     "Development Status :: 4 - Beta",
```

