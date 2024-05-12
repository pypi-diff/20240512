# Comparing `tmp/nostpy_cli-0.1.4.tar.gz` & `tmp/nostpy_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nostpy_cli-0.1.4.tar", last modified: Sun May 12 04:42:50 2024, max compression
+gzip compressed data, was "nostpy_cli-0.2.0.tar", last modified: Sun May 12 05:48:24 2024, max compression
```

## Comparing `nostpy_cli-0.1.4.tar` & `nostpy_cli-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:42:50.702123 nostpy_cli-0.1.4/
--rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.1.4/LICENSE
--rw-r--r--   0 tron      (1000) tron      (1000)     2401 2024-05-12 04:42:50.702123 nostpy_cli-0.1.4/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)     1829 2024-05-12 04:40:45.000000 nostpy_cli-0.1.4/README.md
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:42:50.702123 nostpy_cli-0.1.4/nostpy_cli/
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.1.4/nostpy_cli/__init__.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     5880 2024-05-12 04:16:10.000000 nostpy_cli-0.1.4/nostpy_cli/create_event.py
--rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.1.4/nostpy_cli/kind4.py
--rwxrwxr-x   0 tron      (1000) tron      (1000)     3199 2024-05-12 04:16:10.000000 nostpy_cli-0.1.4/nostpy_cli/main.py
-drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 04:42:50.702123 nostpy_cli-0.1.4/nostpy_cli.egg-info/
--rw-r--r--   0 tron      (1000) tron      (1000)     2401 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/PKG-INFO
--rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/entry_points.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/requires.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 04:42:50.000000 nostpy_cli-0.1.4/nostpy_cli.egg-info/top_level.txt
--rw-rw-r--   0 tron      (1000) tron      (1000)      704 2024-05-12 04:42:10.000000 nostpy_cli-0.1.4/pyproject.toml
--rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 04:42:50.702123 nostpy_cli-0.1.4/setup.cfg
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 05:48:24.359669 nostpy_cli-0.2.0/
+-rw-rw-r--   0 tron      (1000) tron      (1000)     1071 2024-04-30 02:27:44.000000 nostpy_cli-0.2.0/LICENSE
+-rw-r--r--   0 tron      (1000) tron      (1000)     3395 2024-05-12 05:48:24.359669 nostpy_cli-0.2.0/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)     2823 2024-05-12 05:39:18.000000 nostpy_cli-0.2.0/README.md
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 05:48:24.355669 nostpy_cli-0.2.0/nostpy_cli/
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 04:16:10.000000 nostpy_cli-0.2.0/nostpy_cli/__init__.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     5874 2024-05-12 05:24:48.000000 nostpy_cli-0.2.0/nostpy_cli/create_event.py
+-rw-rw-r--   0 tron      (1000) tron      (1000)     3544 2024-05-12 04:16:10.000000 nostpy_cli-0.2.0/nostpy_cli/kind4.py
+-rwxrwxr-x   0 tron      (1000) tron      (1000)     3346 2024-05-12 05:39:02.000000 nostpy_cli-0.2.0/nostpy_cli/main.py
+drwxrwxr-x   0 tron      (1000) tron      (1000)        0 2024-05-12 05:48:24.359669 nostpy_cli-0.2.0/nostpy_cli.egg-info/
+-rw-r--r--   0 tron      (1000) tron      (1000)     3395 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 tron      (1000) tron      (1000)      327 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)        1 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       52 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/requires.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)       11 2024-05-12 05:48:24.000000 nostpy_cli-0.2.0/nostpy_cli.egg-info/top_level.txt
+-rw-rw-r--   0 tron      (1000) tron      (1000)      704 2024-05-12 05:48:17.000000 nostpy_cli-0.2.0/pyproject.toml
+-rw-rw-r--   0 tron      (1000) tron      (1000)       38 2024-05-12 05:48:24.359669 nostpy_cli-0.2.0/setup.cfg
```

### Comparing `nostpy_cli-0.1.4/LICENSE` & `nostpy_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.4/PKG-INFO` & `nostpy_cli-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: nostpy-cli
-Version: 0.1.4
-Summary: CLI tool for handling nostpy events
-Author-email: Brian Hartford <bh419@protonmail.com>
-License: MIT
-Project-URL: homepage, https://github.com/UTXOnly/nostpy-cli
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: argparse
-Requires-Dist: asyncio
-Requires-Dist: secp256k1
-Requires-Dist: websockets
-
 # nostpy-cli
 
 `nostpy-cli` is a Command Line Interface tool for sending and querying nostr events by websocket connection.
 
 ## Features
 
 - Send events to a specified relays
@@ -52,31 +34,50 @@
 python3 -m build
 pip install .
 ```
 
 
 
 ## Usage
-Once installed, you can run nostpy-cli from the command line. Below are some examples of how to use the CLI tool:
+Once installed, you can run `nostpy-cli` from the command line as shown below:
 
 ### Send Event
 To send an event, you would use a command similar to the following:
 
 ```
-nostpy-cli send_event --pubkey "your_public_key" --privkey "your_private_key" --content "your plaintext message" --tags "[['tag1', 'value1']]" --kind 4 --relay "wss://yourrelayurl.com"
+nostpy-cli send_event -pubkey "your_public_key_hex" -privkey "your_private_key_hex" -content "your plaintext message" -tags "[['tag1', 'value1']]" -kind 4 --relay "wss://yourrelayurl.com" "wss://yoursecondrelayurl.com"
 ```
 `--pubkey` , `--priv_key` and `--relay` arguments are required, all else are optional
 
+#### Example
+* Send a kind 1 event with tags
+
+```
+nostpy-cli send_event -pubkey 5ce5b352f1ef76b1dffc5694dd5b34126137184cc9a7d78cba841c0635e17952 -privkey 2b1e4e1f26517dda57458596760bb3bd3bd3717083763166e12983a6421abc18 -content test27 -tags "[
+['t', 'vvfdvfd'], ['v', 'v2']]" -kind 1 --relay wss://relay.nostpy.lol wss://relay.damus.io wss://nos.lol
+```
+
+* Send a kind 4 direct message
+```
+nostpy-cli send_event -pubkey 5ce5b352f1ef76b1dffc5694dd5b34126137184cc9a7d78cba841c0635e17952 -privkey 2b1e4e1f26517dda57458596760bb3bd3bd3717083763166e12983a6421abc18 -content "This is my plaintext message" -tags "[['p', '4503baa127bdfd0b054384dc5ba82cb0e2a8367cbdb0629179f00db1a34caacc']]" -kind 4 --relay wss://relay.nostpy.lol wss://relay.damus.io wss://nos.lol
+```
+
 ### Query Event
 To query events, use the following command:
 
 ```
-nostpy-cli query --kinds "[1,9075]" --relay "wss://yourrelayurl.com"
+nostpy-cli query --kinds "[1,9735]" --relay "wss://yourrelayurl.com"
 ```
 `--relay` field required
+
+#### Example
+* Query an event with search
+```
+nostpy-cli query -kinds "[31990,1]" -search "random_search" -since 1713629501 -authors npub1g5pm4gf8hh7skp2rsnw9h2pvkr32sdnuhkcx9yte7qxmrg6v4txqqudjqv --relay wss://relay.nostpy.lol
+```
 ### Help
 To view all available commands and their options, use the help command:
 
 ```
 nostpy-cli -h
 ```
 ## Contributing
```

### Comparing `nostpy_cli-0.1.4/nostpy_cli/create_event.py` & `nostpy_cli-0.2.0/nostpy_cli/create_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             return False
 
     async def send_event(self, public_key, private_key_hex, content, kind, tags):
         try:
             event_data = self.create_event(
                 public_key, private_key_hex, content, kind, tags
             )
-            for ws_relay in self.relays_kind4:
+            for ws_relay in self.relays:
                 async with websockets.connect(ws_relay) as ws:
                     event_json = ("EVENT", event_data)
                     print("Sending event:")
                     self.print_color(f"{event_json}", "32")
                     print(f"to {ws_relay}")
                     await ws.send(json.dumps(event_json))
                     response = await asyncio.wait_for(ws.recv(), timeout=10)
```

### Comparing `nostpy_cli-0.1.4/nostpy_cli/kind4.py` & `nostpy_cli-0.2.0/nostpy_cli/kind4.py`

 * *Files identical despite different names*

### Comparing `nostpy_cli-0.1.4/nostpy_cli/main.py` & `nostpy_cli-0.2.0/nostpy_cli/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         args.content = kind4_codec.encrypt_message(args.content)
     await event.send_event(
         args.public_key, args.private_key, args.content, args.kind, args.tags
     )
 
 
 def main():
-    parser = argparse.ArgumentParser(description="Send events via WebSocket.")
+    parser = argparse.ArgumentParser(description="Send and query nostr events")
     subparsers = parser.add_subparsers(
         title="commands", description="valid commands", help="additional help"
     )
 
     # Subparser for the "query" command
     query_parser = subparsers.add_parser("query", help="Query events")
     query_parser.add_argument(
@@ -51,15 +51,15 @@
     query_parser.add_argument(
         "-since", "--since", type=int, help="Collect events since"
     )
     query_parser.add_argument(
         "-until", "--until", type=int, help="Collect events until"
     )
     query_parser.add_argument(
-        "-authors", "--authors", type=ast.literal_eval, help="List of authors e.g. []"
+        "-authors", "--authors", type=str, help="List of authors e.g. []"
     )
     query_parser.add_argument(
         "-limit",
         "--limit",
         type=ast.literal_eval,
         help="Limit on number of results returned",
     )
@@ -88,14 +88,16 @@
     )
     send_event_parser.add_argument("-kind", "--kind", type=int, help="Event kind")
     send_event_parser.add_argument(
         "--relay", nargs="+", required=True, help="WebSocket relay URLs"
     )
     send_event_parser.set_defaults(func=handle_send_event)
 
+    parser.epilog = 'Example send usage: nostpy-cli send_event -pubkey "abc123..." -privkey "def456..." -content "Hello, world!" --relay "wss://example.com"'
+
     args = parser.parse_args()
     if hasattr(args, "func"):
         asyncio.run(args.func(args))
     else:
         parser.print_help()
```

### Comparing `nostpy_cli-0.1.4/pyproject.toml` & `nostpy_cli-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nostpy-cli"
-version = "0.1.4"
+version = "0.2.0"
 authors = [{ name = "Brian Hartford", email = "bh419@protonmail.com" }]
 description = "CLI tool for handling nostpy events"
 readme = "README.md"
 license = { text = "MIT" }
 urls = { homepage = "https://github.com/UTXOnly/nostpy-cli" }
 classifiers = [
     "Development Status :: 4 - Beta",
```

