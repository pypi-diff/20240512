# Comparing `tmp/nostpy_cli-0.1.3.tar.gz` & `tmp/nostpy_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostpy_cli-0.1.3.tar", last modified: Sun May 12 04:33:31 2024, max compression
+gzip compressed data, was "nostpy_cli-0.1.4.tar", last modified: Sun May 12 04:42:50 2024, max compression
```

## Comparing `nostpy_cli-0.1.3.tar` & `nostpy_cli-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:33:31.481315 nostpy_cli-0.1.3/
--rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.1.3/LICENSE
--rw-r--r--   0 tron      (1000) tron      (1000)     2396 2024-05-12 04:33:31.481315 nostpy_cli-0.1.3/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)     1824 2024-05-12 04:33:16.000000 nostpy_cli-0.1.3/README.md
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:33:31.481315 nostpy_cli-0.1.3/nostpy_cli/
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.1.3/nostpy_cli/__init__.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     5880 2024-05-12 04:16:10.000000 nostpy_cli-0.1.3/nostpy_cli/create_event.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.1.3/nostpy_cli/kind4.py
--rwxrwxr-x   0 tron      (1000) tron      (1000)     3199 2024-05-12 04:16:10.000000 nostpy_cli-0.1.3/nostpy_cli/main.py
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:33:31.481315 nostpy_cli-0.1.3/nostpy_cli.egg-info/
--rw-r--r--   0 tron      (1000) tron      (1000)     2396 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/entry_points.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/requires.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 04:33:31.000000 nostpy_cli-0.1.3/nostpy_cli.egg-info/top_level.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)      704 2024-05-12 04:29:05.000000 nostpy_cli-0.1.3/pyproject.toml
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:33:31.481315 nostpy_cli-0.1.3/setup.cfg
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:42:50.702123 nostpy_cli-0.1.4/
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.1.4/LICENSE
+-rw-r--r--   0 tron      (1000) tron      (1000)     2401 2024-05-12 04:42:50.702123 nostpy_cli-0.1.4/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1829 2024-05-12 04:40:45.000000 nostpy_cli-0.1.4/README.md
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:42:50.702123 nostpy_cli-0.1.4/nostpy_cli/
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.1.4/nostpy_cli/__init__.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     5880 2024-05-12 04:16:10.000000 nostpy_cli-0.1.4/nostpy_cli/create_event.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.1.4/nostpy_cli/kind4.py
+-rwxrwxr-x   0 tron      (1000) tron      (1000)     3199 2024-05-12 04:16:10.000000 nostpy_cli-0.1.4/nostpy_cli/main.py
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:42:50.702123 nostpy_cli-0.1.4/nostpy_cli.egg-info/
+-rw-r--r--   0 tron      (1000) tron      (1000)     2401 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/requires.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/top_level.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)      704 2024-05-12 04:42:10.000000 nostpy_cli-0.1.4/pyproject.toml
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:42:50.702123 nostpy_cli-0.1.4/setup.cfg
```

### Comparing `nostpy_cli-0.1.3/LICENSE` & `nostpy_cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.3/PKG-INFO` & `nostpy_cli-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostpy-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: CLI tool for handling nostpy events
 Author-email: Brian Hartford <bh419@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/UTXOnly/nostpy-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,21 +14,22 @@
 Requires-Dist: argparse
 Requires-Dist: asyncio
 Requires-Dist: secp256k1
 Requires-Dist: websockets
 
 # nostpy-cli
 
-`nostpy-cli` is a Command Line Interface (CLI) tool designed to handle nostpy events efficiently. This tool provides easy-to-use commands to send and query events via a WebSocket connection.
+`nostpy-cli` is a Command Line Interface tool for sending and querying nostr events by websocket connection.
 
 ## Features
 
 - Send events to a specified relays
 - Query events from relays
 - Encode/decode kind4 messages
+- Supports [NIP-50](https://github.com/nostr-protocol/nips/blob/master/50.md) searches
 
 ## Prerequisites
 
 Before installing `nostpy-cli`, ensure you have Python 3.6 or higher installed on your system. You can check your Python version by running:
 
 ```
 python3 --version
```

### Comparing `nostpy_cli-0.1.3/README.md` & `nostpy_cli-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # nostpy-cli
 
-`nostpy-cli` is a Command Line Interface (CLI) tool designed to handle nostpy events efficiently. This tool provides easy-to-use commands to send and query events via a WebSocket connection.
+`nostpy-cli` is a Command Line Interface tool for sending and querying nostr events by websocket connection.
 
 ## Features
 
 - Send events to a specified relays
 - Query events from relays
 - Encode/decode kind4 messages
+- Supports [NIP-50](https://github.com/nostr-protocol/nips/blob/master/50.md) searches
 
 ## Prerequisites
 
 Before installing `nostpy-cli`, ensure you have Python 3.6 or higher installed on your system. You can check your Python version by running:
 
 ```
 python3 --version
```

### Comparing `nostpy_cli-0.1.3/nostpy_cli/create_event.py` & `nostpy_cli-0.1.4/nostpy_cli/create_event.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.3/nostpy_cli/kind4.py` & `nostpy_cli-0.1.4/nostpy_cli/kind4.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.3/nostpy_cli/main.py` & `nostpy_cli-0.1.4/nostpy_cli/main.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.3/nostpy_cli.egg-info/PKG-INFO` & `nostpy_cli-0.1.4/nostpy_cli.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostpy-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: CLI tool for handling nostpy events
 Author-email: Brian Hartford <bh419@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/UTXOnly/nostpy-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -14,21 +14,22 @@
 Requires-Dist: argparse
 Requires-Dist: asyncio
 Requires-Dist: secp256k1
 Requires-Dist: websockets
 
 # nostpy-cli
 
-`nostpy-cli` is a Command Line Interface (CLI) tool designed to handle nostpy events efficiently. This tool provides easy-to-use commands to send and query events via a WebSocket connection.
+`nostpy-cli` is a Command Line Interface tool for sending and querying nostr events by websocket connection.
 
 ## Features
 
 - Send events to a specified relays
 - Query events from relays
 - Encode/decode kind4 messages
+- Supports [NIP-50](https://github.com/nostr-protocol/nips/blob/master/50.md) searches
 
 ## Prerequisites
 
 Before installing `nostpy-cli`, ensure you have Python 3.6 or higher installed on your system. You can check your Python version by running:
 
 ```
 python3 --version
```

### Comparing `nostpy_cli-0.1.3/pyproject.toml` & `nostpy_cli-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nostpy-cli"
-version = "0.1.3"
+version = "0.1.4"
 authors = [{ name = "Brian Hartford", email = "bh419@protonmail.com" }]
 description = "CLI tool for handling nostpy events"
 readme = "README.md"
 license = { text = "MIT" }
 urls = { homepage = "https://github.com/UTXOnly/nostpy-cli" }
 classifiers = [
     "Development Status :: 4 - Beta",
```

