# Comparing `tmp/indralib-0.1.1.tar.gz` & `tmp/indralib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indralib-0.1.1.tar", last modified: Fri May 10 07:34:34 2024, max compression
+gzip compressed data, was "indralib-0.1.2.tar", last modified: Sun May 12 13:40:10 2024, max compression
```

## Comparing `indralib-0.1.1.tar` & `indralib-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-10 07:34:34.898481 indralib-0.1.1/
--rw-r--r--   0 dsc        (501) staff       (20)      627 2024-05-10 07:34:34.898279 indralib-0.1.1/PKG-INFO
--rw-r--r--   0 dsc        (501) staff       (20)       52 2024-05-09 14:18:10.000000 indralib-0.1.1/README.md
--rw-r--r--   0 dsc        (501) staff       (20)      676 2024-05-10 07:32:29.000000 indralib-0.1.1/pyproject.toml
--rw-r--r--   0 dsc        (501) staff       (20)       38 2024-05-10 07:34:34.898536 indralib-0.1.1/setup.cfg
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-10 07:34:34.894432 indralib-0.1.1/src/
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-10 07:34:34.895612 indralib-0.1.1/src/indralib/
--rw-r--r--   0 dsc        (501) staff       (20)        0 2024-05-09 14:14:09.000000 indralib-0.1.1/src/indralib/__init__.py
--rw-r--r--   0 dsc        (501) staff       (20)    23425 2024-05-10 07:33:38.000000 indralib-0.1.1/src/indralib/indra_client.py
--rw-r--r--   0 dsc        (501) staff       (20)    17753 2024-05-09 14:46:36.000000 indralib-0.1.1/src/indralib/indra_downloader.py
--rw-r--r--   0 dsc        (501) staff       (20)     3214 2024-05-09 15:30:32.000000 indralib-0.1.1/src/indralib/indra_event.py
--rw-r--r--   0 dsc        (501) staff       (20)     2720 2024-05-09 14:46:45.000000 indralib-0.1.1/src/indralib/indra_module.py
--rw-r--r--   0 dsc        (501) staff       (20)    13670 2024-05-09 14:46:52.000000 indralib-0.1.1/src/indralib/indra_time.py
-drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-10 07:34:34.898048 indralib-0.1.1/src/indralib.egg-info/
--rw-r--r--   0 dsc        (501) staff       (20)      627 2024-05-10 07:34:34.000000 indralib-0.1.1/src/indralib.egg-info/PKG-INFO
--rw-r--r--   0 dsc        (501) staff       (20)      374 2024-05-10 07:34:34.000000 indralib-0.1.1/src/indralib.egg-info/SOURCES.txt
--rw-r--r--   0 dsc        (501) staff       (20)        1 2024-05-10 07:34:34.000000 indralib-0.1.1/src/indralib.egg-info/dependency_links.txt
--rw-r--r--   0 dsc        (501) staff       (20)       17 2024-05-10 07:34:34.000000 indralib-0.1.1/src/indralib.egg-info/requires.txt
--rw-r--r--   0 dsc        (501) staff       (20)        9 2024-05-10 07:34:34.000000 indralib-0.1.1/src/indralib.egg-info/top_level.txt
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-12 13:40:10.543057 indralib-0.1.2/
+-rw-r--r--   0 dsc        (501) staff       (20)      627 2024-05-12 13:40:10.542868 indralib-0.1.2/PKG-INFO
+-rw-r--r--   0 dsc        (501) staff       (20)       52 2024-05-09 14:18:10.000000 indralib-0.1.2/README.md
+-rw-r--r--   0 dsc        (501) staff       (20)      676 2024-05-12 13:32:07.000000 indralib-0.1.2/pyproject.toml
+-rw-r--r--   0 dsc        (501) staff       (20)       38 2024-05-12 13:40:10.543102 indralib-0.1.2/setup.cfg
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-12 13:40:10.539863 indralib-0.1.2/src/
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-12 13:40:10.541933 indralib-0.1.2/src/indralib/
+-rw-r--r--   0 dsc        (501) staff       (20)        0 2024-05-09 14:14:09.000000 indralib-0.1.2/src/indralib/__init__.py
+-rw-r--r--   0 dsc        (501) staff       (20)    18076 2024-05-12 13:31:39.000000 indralib-0.1.2/src/indralib/indra_client.py
+-rw-r--r--   0 dsc        (501) staff       (20)    17753 2024-05-09 14:46:36.000000 indralib-0.1.2/src/indralib/indra_downloader.py
+-rw-r--r--   0 dsc        (501) staff       (20)     3214 2024-05-09 15:30:32.000000 indralib-0.1.2/src/indralib/indra_event.py
+-rw-r--r--   0 dsc        (501) staff       (20)     2720 2024-05-09 14:46:45.000000 indralib-0.1.2/src/indralib/indra_module.py
+-rw-r--r--   0 dsc        (501) staff       (20)    13670 2024-05-09 14:46:52.000000 indralib-0.1.2/src/indralib/indra_time.py
+-rw-r--r--   0 dsc        (501) staff       (20)     3691 2024-05-12 13:37:46.000000 indralib-0.1.2/src/indralib/server_config.py
+drwxr-xr-x   0 dsc        (501) staff       (20)        0 2024-05-12 13:40:10.542677 indralib-0.1.2/src/indralib.egg-info/
+-rw-r--r--   0 dsc        (501) staff       (20)      627 2024-05-12 13:40:10.000000 indralib-0.1.2/src/indralib.egg-info/PKG-INFO
+-rw-r--r--   0 dsc        (501) staff       (20)      404 2024-05-12 13:40:10.000000 indralib-0.1.2/src/indralib.egg-info/SOURCES.txt
+-rw-r--r--   0 dsc        (501) staff       (20)        1 2024-05-12 13:40:10.000000 indralib-0.1.2/src/indralib.egg-info/dependency_links.txt
+-rw-r--r--   0 dsc        (501) staff       (20)       17 2024-05-12 13:40:10.000000 indralib-0.1.2/src/indralib.egg-info/requires.txt
+-rw-r--r--   0 dsc        (501) staff       (20)        9 2024-05-12 13:40:10.000000 indralib-0.1.2/src/indralib.egg-info/top_level.txt
```

### Comparing `indralib-0.1.1/PKG-INFO` & `indralib-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indralib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Client for the Indrajala system
 Author-email: Dominik Schlösser <dominik.schloesser@gmail.com>
 Project-URL: Homepage, https://github.com/domschl/indrajala
 Project-URL: Bug Tracker, https://github.com/domschl/indrajala/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `indralib-0.1.1/pyproject.toml` & `indralib-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "indralib"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "Dominik Schlösser", email = "dominik.schloesser@gmail.com" }]
 description = "Client for the Indrajala system"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `indralib-0.1.1/src/indralib/indra_client.py` & `indralib-0.1.2/src/indralib/indra_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,24 @@
 import asyncio
 import websockets
 import logging
 import ssl
 import json
-
-try:
-    import tomllib as toml
-except ImportError:
-    import tomli as toml
-
-import os
 import time
-import sys
 
 from indralib.indra_event import IndraEvent
+from indralib.server_config import Profiles
 
 
 class IndraClient:
     def __init__(
         self,
-        uri=None,
-        ca_authority=None,
-        auth_token=None,
-        config_file=None,
+        profile,
         verbose=False,
         module_name=None,
-        profile="default",
         log_handler=None,
     ):
         self.log = logging.getLogger("IndraClient")
         if log_handler is not None:
             self.log.addHandler(log_handler)
         if module_name is None:
             self.module_name = "IndraClient (python)"
@@ -38,167 +27,46 @@
         self.websocket = None
         self.verbose = verbose
         self.trx = {}
         self.recv_queue = asyncio.Queue()
         self.recv_task = None
         self.initialized = False
         self.error_shown = False
-        if profile is not None and profile.lower() in ["default", "none"]:
-            profile = None
-        if config_file is not None and config_file != "":
-            self.initialized = self.get_config(config_file, verbose=self.verbose)
-        elif uri is not None and uri != "":
-            self.initialized = True
-            self.uri = uri
-            if ca_authority is not None and ca_authority != "":
-                self.ca_authority = ca_authority
-            else:
-                self.ca_authority = None
-            if auth_token is not None and auth_token != "":
-                self.auth_token = auth_token
-            else:
-                self.auth_token = None
-            if self.uri.startswith("wss://"):
-                self.use_ssl = True
-            else:
-                self.use_ssl = False
-        elif profile is not None:
-            if os.path.exists("/var/lib/indrajala/config") is True:
-                cfg_path = "/var/lib/indrajala/config"
-            else:
-                cfg_path = "~/.config/indrajala/server_profiles"
-                cfg_path = os.path.expanduser(cfg_path)
-            config_file = os.path.join(cfg_path, profile + ".toml")
-            if os.path.exists(config_file) is True:
-                self.initialized = self.get_config(config_file, verbose=self.verbose)
-            else:
-                self.initialized = False
-                if verbose is True:
-                    self.log.error(
-                        f"Profile {profile} not found in {cfg_path}, alternatively please provide a valid uri, starting with ws:// or wss://, e.g. wss://localhost:8082, or config_file=..."
-                    )
-                return
-        else:
-            if os.path.exists("/var/lib/indrajala/config/server_profiles") is True:
-                cfg_path = "/var/lib/indrajala/config/server_profiles"
-            else:
-                cfg_path = "~/.config/indrajala/server_profiles"
-                cfg_path = os.path.expanduser(cfg_path)
-            prfs = IndraClient.get_profiles()
-
-            if len(prfs) > 0:
-                self.initialized = self.get_config(
-                    os.path.join(cfg_path, prfs[0] + ".toml"), verbose=self.verbose
-                )
-            else:
-                self.initialized = False
-                if verbose is True:
-                    self.log.error(f"No valid profiles found in {cfg_path}")
-                return
-
-    @staticmethod
-    def get_profiles(prefer_ssl=None):
-        """Get profiles"""
-        if os.path.exists("/var/lib/indrajala/config/server_profiles") is True:
-            cfg_path = "/var/lib/indrajala/config/server_profiles"
-        else:
-            cfg_path = "~/.config/indrajala/server_profiles"
-            cfg_path = os.path.expanduser(cfg_path)
-        if os.path.exists(cfg_path) is False:
-            return []
-        profiles = []
-        for f in os.listdir(cfg_path):
-            if f.endswith(".toml"):
-                if prefer_ssl is None:
-                    profiles.append(f[:-5])
-                else:
-                    try:
-                        with open(os.path.join(cfg_path, f), "rb") as f:
-                            config = toml.load(f)
-                        if "uri" in config:
-                            if prefer_ssl is True and config["uri"].startswith(
-                                "wss://"
-                            ):
-                                profiles.append(f[:-5])
-                            elif prefer_ssl is False and config["uri"].startswith(
-                                "ws://"
-                            ):
-                                profiles.append(f[:-5])
-                    except Exception as e:
-                        pass
-        return profiles
-
-    def get_config(self, config_file, verbose=True):
-        """Get config from file"""
-        self.initialized = False
-        try:
-            with open(config_file, "rb") as f:
-                config = toml.load(f)
-            if verbose is True:
-                self.log.debug(f"Loaded config from {config_file}: {config}f")
-        except Exception as e:
-            if verbose is True:
-                self.log.error(f"{config_file} config file not found: {e}")
-            return False
-        if "uri" not in config:
-            if verbose is True:
-                self.log.error(
-                    f"Please provide an uri=ws[s]://host:port in {config_file}"
-                )
-            return False
-        self.uri = config["uri"]
-        if "ca_authority" in config and config["ca_authority"] != "":
-            cert_auth = os.path.expanduser(config["ca_authority"])
-            if os.path.exists(cert_auth) is False:
-                if verbose is True:
-                    self.log.error(f"CA authority file {cert_auth} not found!")
-                return False
-            self.ca_authority = cert_auth
-        else:
-            self.ca_authority = None
-        if "auth_token" in config and config["auth_token"] != "":
-            self.auth_token = config["auth_token"]
-        else:
-            self.auth_token = None
-        if self.uri.startswith("wss://"):
-            self.use_ssl = True
-        else:
-            self.use_ssl = False
-        if verbose is True:
-            self.log.info(
-                f"Initialized IndraClient with uri={self.uri}, ca_authority={self.ca_authority}, auth_token={self.auth_token}"
-            )
+        if Profiles.check_profile(profile) is False:
+            self.log.error("Invalid profile {profile}")
+            self.profile = None
+            return
+        self.profile = profile
         self.initialized = True
-        return True
 
     async def init_connection(self, verbose=False):
         """Initialize connection"""
         if self.initialized is False:
             self.trx = {}
             self.websocket = None
-            if verbose is True:
-                self.log.error(
-                    "Indrajala init_connection(): connection data not initialized!"
-                )
+            self.log.error(
+                "Indrajala init_connection(): connection profile data not initialized!"
+            )
             return None
         if self.websocket is not None:
             if verbose is True:
                 self.log.warning(
                     "Websocket already initialized, please call close_connection() first!"
                 )
             return self.websocket
         self.trx = {}
-        if self.use_ssl is True:
+        self.uri = Profiles.get_uri(self.profile)
+        if self.profile["TLS"] is True:
             ssl_ctx = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
-            if self.ca_authority is not None:
+            if self.profile["ca_authority"] is not None:
                 try:
-                    ssl_ctx.load_verify_locations(cafile=self.ca_authority)
+                    ssl_ctx.load_verify_locations(cafile=self.profile["ca_authority"])
                 except Exception as e:
                     self.log.error(
-                        f"Could not load CA authority file {self.ca_authority}: {e}"
+                        f"Could not load CA authority file {self.profile['ca_authority']}: {e}"
                     )
                     self.websocket = None
                     return None
         try:
             self.websocket = await websockets.connect(self.uri, ssl=ssl_ctx)
         except Exception as e:
             self.log.error(f"Could not connect to {self.uri}: {e}")
```

### Comparing `indralib-0.1.1/src/indralib/indra_downloader.py` & `indralib-0.1.2/src/indralib/indra_downloader.py`

 * *Files identical despite different names*

### Comparing `indralib-0.1.1/src/indralib/indra_event.py` & `indralib-0.1.2/src/indralib/indra_event.py`

 * *Files identical despite different names*

### Comparing `indralib-0.1.1/src/indralib/indra_module.py` & `indralib-0.1.2/src/indralib/indra_module.py`

 * *Files identical despite different names*

### Comparing `indralib-0.1.1/src/indralib/indra_time.py` & `indralib-0.1.2/src/indralib/indra_time.py`

 * *Files identical despite different names*

### Comparing `indralib-0.1.1/src/indralib.egg-info/PKG-INFO` & `indralib-0.1.2/src/indralib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indralib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Client for the Indrajala system
 Author-email: Dominik Schlösser <dominik.schloesser@gmail.com>
 Project-URL: Homepage, https://github.com/domschl/indrajala
 Project-URL: Bug Tracker, https://github.com/domschl/indrajala/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

