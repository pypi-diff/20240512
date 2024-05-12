# Comparing `tmp/nostpy_cli-0.2.2.tar.gz` & `tmp/nostpy_cli-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostpy_cli-0.2.2.tar", last modified: Sun May 12 06:01:20 2024, max compression
+gzip compressed data, was "nostpy_cli-0.3.0.tar", last modified: Sun May 12 06:53:16 2024, max compression
```

## Comparing `nostpy_cli-0.2.2.tar` & `nostpy_cli-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 06:01:20.691237 nostpy_cli-0.2.2/
--rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.2.2/LICENSE
--rw-r--r--   0 tron      (1000) tron      (1000)     3394 2024-05-12 06:01:20.691237 nostpy_cli-0.2.2/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)     2823 2024-05-12 06:00:09.000000 nostpy_cli-0.2.2/README.md
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 06:01:20.691237 nostpy_cli-0.2.2/nostpy_cli/
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.2.2/nostpy_cli/__init__.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     5874 2024-05-12 06:00:09.000000 nostpy_cli-0.2.2/nostpy_cli/create_event.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.2.2/nostpy_cli/kind4.py
--rwxrwxr-x   0 tron      (1000) tron      (1000)     3346 2024-05-12 06:00:09.000000 nostpy_cli-0.2.2/nostpy_cli/main.py
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 06:01:20.691237 nostpy_cli-0.2.2/nostpy_cli.egg-info/
--rw-r--r--   0 tron      (1000) tron      (1000)     3394 2024-05-12 06:01:20.000000 nostpy_cli-0.2.2/nostpy_cli.egg-info/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 06:01:20.000000 nostpy_cli-0.2.2/nostpy_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 06:01:20.000000 nostpy_cli-0.2.2/nostpy_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 06:01:20.000000 nostpy_cli-0.2.2/nostpy_cli.egg-info/entry_points.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 06:01:20.000000 nostpy_cli-0.2.2/nostpy_cli.egg-info/requires.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 06:01:20.000000 nostpy_cli-0.2.2/nostpy_cli.egg-info/top_level.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)      705 2024-05-12 06:01:14.000000 nostpy_cli-0.2.2/pyproject.toml
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 06:01:20.691237 nostpy_cli-0.2.2/setup.cfg
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 06:53:16.345452 nostpy_cli-0.3.0/
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.3.0/LICENSE
+-rw-r--r--   0 tron      (1000) tron      (1000)     4359 2024-05-12 06:53:16.345452 nostpy_cli-0.3.0/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)     3788 2024-05-12 06:49:34.000000 nostpy_cli-0.3.0/README.md
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 06:53:16.345452 nostpy_cli-0.3.0/nostpy_cli/
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.3.0/nostpy_cli/__init__.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     5874 2024-05-12 06:00:09.000000 nostpy_cli-0.3.0/nostpy_cli/create_event.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.3.0/nostpy_cli/kind4.py
+-rwxrwxr-x   0 tron      (1000) tron      (1000)     4061 2024-05-12 06:51:45.000000 nostpy_cli-0.3.0/nostpy_cli/main.py
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 06:53:16.345452 nostpy_cli-0.3.0/nostpy_cli.egg-info/
+-rw-r--r--   0 tron      (1000) tron      (1000)     4359 2024-05-12 06:53:16.000000 nostpy_cli-0.3.0/nostpy_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 06:53:16.000000 nostpy_cli-0.3.0/nostpy_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 06:53:16.000000 nostpy_cli-0.3.0/nostpy_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 06:53:16.000000 nostpy_cli-0.3.0/nostpy_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 06:53:16.000000 nostpy_cli-0.3.0/nostpy_cli.egg-info/requires.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 06:53:16.000000 nostpy_cli-0.3.0/nostpy_cli.egg-info/top_level.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)      705 2024-05-12 06:52:51.000000 nostpy_cli-0.3.0/pyproject.toml
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 06:53:16.345452 nostpy_cli-0.3.0/setup.cfg
```

### Comparing `nostpy_cli-0.2.2/LICENSE` & `nostpy_cli-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.2.2/PKG-INFO` & `nostpy_cli-0.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostpy-cli
-Version: 0.2.2
+Version: 0.3.0
 Summary: CLI tool for handling nostr events
 Author-email: Brian Hartford <bh419@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/UTXOnly/nostpy-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,16 +18,16 @@
 
 # nostpy-cli
 
 `nostpy-cli` is a Command Line Interface tool for sending and querying nostr events by websocket connection.
 
 ## Features
 
-- Send events to a specified relays
-- Query events from relays
+- Send events to specified relays
+- Query events from specified relays
 - Encode/decode kind4 messages
 - Supports [NIP-50](https://github.com/nostr-protocol/nips/blob/master/50.md) searches
 
 ## Prerequisites
 
 Before installing `nostpy-cli`, ensure you have Python 3.6 or higher installed on your system. You can check your Python version by running:
 
@@ -88,18 +88,46 @@
 `--relay` field required
 
 #### Example
 * Query an event with search
 ```
 nostpy-cli query -kinds "[31990,1]" -search "random_search" -since 1713629501 -authors npub1g5pm4gf8hh7skp2rsnw9h2pvkr32sdnuhkcx9yte7qxmrg6v4txqqudjqv --relay wss://relay.nostpy.lol
 ```
+
+### Decrypt kind4 message content
+Decrypt kind4 message content by providing recipient private key hex, sender public key hex and the message ciphertext, returns the plaintext message
+
+#### Example 
+```
+nostpy-cli decode -content "kP9dCG/stpEGNTjW2/aySQ==?iv=+GCHVOBAiM9X074n1vxiFg==" -priv_key 2b1e4e1f26517dda57458596760bb3bd3bd3717083763166e12983a6421abc18 -sender_pubkey 4503baa127bdfd0b054384dc5ba82cb0e2a8367cbdb0629179f00db1a34caacc 
+```
 ### Help
 To view all available commands and their options, use the help command:
 
 ```
 nostpy-cli -h
 ```
+
+```
+usage: nostpy-cli [-h] {query,send_event,decode} ...
+
+Send and query nostr events
+
+options:
+  -h, --help            show this help message and exit
+
+commands:
+  valid commands
+
+  {query,send_event,decode}
+                        additional help
+    query               Query events
+    send_event          Send an event
+    decode              Decode kind4 content
+
+Example send usage: nostpy-cli send_event -pubkey "abc123..." -privkey "def456..." -content "Hello, world!" --relay "wss://example.com"
+```
 ## Contributing
 Contributions to nostpy-cli are welcome! Please feel free to submit pull requests or open issues to report bugs or suggest enhancements.
 
 ### License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `nostpy_cli-0.2.2/README.md` & `nostpy_cli-0.3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # nostpy-cli
 
 `nostpy-cli` is a Command Line Interface tool for sending and querying nostr events by websocket connection.
 
 ## Features
 
-- Send events to a specified relays
-- Query events from relays
+- Send events to specified relays
+- Query events from specified relays
 - Encode/decode kind4 messages
 - Supports [NIP-50](https://github.com/nostr-protocol/nips/blob/master/50.md) searches
 
 ## Prerequisites
 
 Before installing `nostpy-cli`, ensure you have Python 3.6 or higher installed on your system. You can check your Python version by running:
 
@@ -70,18 +70,46 @@
 `--relay` field required
 
 #### Example
 * Query an event with search
 ```
 nostpy-cli query -kinds "[31990,1]" -search "random_search" -since 1713629501 -authors npub1g5pm4gf8hh7skp2rsnw9h2pvkr32sdnuhkcx9yte7qxmrg6v4txqqudjqv --relay wss://relay.nostpy.lol
 ```
+
+### Decrypt kind4 message content
+Decrypt kind4 message content by providing recipient private key hex, sender public key hex and the message ciphertext, returns the plaintext message
+
+#### Example 
+```
+nostpy-cli decode -content "kP9dCG/stpEGNTjW2/aySQ==?iv=+GCHVOBAiM9X074n1vxiFg==" -priv_key 2b1e4e1f26517dda57458596760bb3bd3bd3717083763166e12983a6421abc18 -sender_pubkey 4503baa127bdfd0b054384dc5ba82cb0e2a8367cbdb0629179f00db1a34caacc 
+```
 ### Help
 To view all available commands and their options, use the help command:
 
 ```
 nostpy-cli -h
 ```
+
+```
+usage: nostpy-cli [-h] {query,send_event,decode} ...
+
+Send and query nostr events
+
+options:
+  -h, --help            show this help message and exit
+
+commands:
+  valid commands
+
+  {query,send_event,decode}
+                        additional help
+    query               Query events
+    send_event          Send an event
+    decode              Decode kind4 content
+
+Example send usage: nostpy-cli send_event -pubkey "abc123..." -privkey "def456..." -content "Hello, world!" --relay "wss://example.com"
+```
 ## Contributing
 Contributions to nostpy-cli are welcome! Please feel free to submit pull requests or open issues to report bugs or suggest enhancements.
 
 ### License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `nostpy_cli-0.2.2/nostpy_cli/create_event.py` & `nostpy_cli-0.3.0/nostpy_cli/create_event.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.2.2/nostpy_cli/kind4.py` & `nostpy_cli-0.3.0/nostpy_cli/kind4.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.2.2/nostpy_cli.egg-info/PKG-INFO` & `nostpy_cli-0.3.0/nostpy_cli.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nostpy-cli
-Version: 0.2.2
+Version: 0.3.0
 Summary: CLI tool for handling nostr events
 Author-email: Brian Hartford <bh419@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/UTXOnly/nostpy-cli
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,16 +18,16 @@
 
 # nostpy-cli
 
 `nostpy-cli` is a Command Line Interface tool for sending and querying nostr events by websocket connection.
 
 ## Features
 
-- Send events to a specified relays
-- Query events from relays
+- Send events to specified relays
+- Query events from specified relays
 - Encode/decode kind4 messages
 - Supports [NIP-50](https://github.com/nostr-protocol/nips/blob/master/50.md) searches
 
 ## Prerequisites
 
 Before installing `nostpy-cli`, ensure you have Python 3.6 or higher installed on your system. You can check your Python version by running:
 
@@ -88,18 +88,46 @@
 `--relay` field required
 
 #### Example
 * Query an event with search
 ```
 nostpy-cli query -kinds "[31990,1]" -search "random_search" -since 1713629501 -authors npub1g5pm4gf8hh7skp2rsnw9h2pvkr32sdnuhkcx9yte7qxmrg6v4txqqudjqv --relay wss://relay.nostpy.lol
 ```
+
+### Decrypt kind4 message content
+Decrypt kind4 message content by providing recipient private key hex, sender public key hex and the message ciphertext, returns the plaintext message
+
+#### Example 
+```
+nostpy-cli decode -content "kP9dCG/stpEGNTjW2/aySQ==?iv=+GCHVOBAiM9X074n1vxiFg==" -priv_key 2b1e4e1f26517dda57458596760bb3bd3bd3717083763166e12983a6421abc18 -sender_pubkey 4503baa127bdfd0b054384dc5ba82cb0e2a8367cbdb0629179f00db1a34caacc 
+```
 ### Help
 To view all available commands and their options, use the help command:
 
 ```
 nostpy-cli -h
 ```
+
+```
+usage: nostpy-cli [-h] {query,send_event,decode} ...
+
+Send and query nostr events
+
+options:
+  -h, --help            show this help message and exit
+
+commands:
+  valid commands
+
+  {query,send_event,decode}
+                        additional help
+    query               Query events
+    send_event          Send an event
+    decode              Decode kind4 content
+
+Example send usage: nostpy-cli send_event -pubkey "abc123..." -privkey "def456..." -content "Hello, world!" --relay "wss://example.com"
+```
 ## Contributing
 Contributions to nostpy-cli are welcome! Please feel free to submit pull requests or open issues to report bugs or suggest enhancements.
 
 ### License
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `nostpy_cli-0.2.2/pyproject.toml` & `nostpy_cli-0.3.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nostpy-cli"
 
-version = "0.2.2"
+version = "0.3.0"
 
 authors = [{ name = "Brian Hartford", email = "bh419@protonmail.com" }]
 description = "CLI tool for handling nostr events"
 readme = "README.md"
 license = { text = "MIT" }
 urls = { homepage = "https://github.com/UTXOnly/nostpy-cli" }
 classifiers = [
```

