# Comparing `tmp/v2share-0.1.0a5.tar.gz` & `tmp/v2share-0.1.0a6.tar.gz`

## Comparing `v2share-0.1.0a5.tar` & `v2share-0.1.0a6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 v2share-0.1.0a5/requirements.txt
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 v2share-0.1.0a5/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a5/tests/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a5/tests/test_config.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/_version.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/clash.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/clashmeta.py
--rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/data.py
--rw-r--r--   0        0        0     6759 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/singbox.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/templates/clash.yml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 v2share-0.1.0a5/v2share/templates/singbox.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 v2share-0.1.0a5/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a5/README.md
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 v2share-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 v2share-0.1.0a6/requirements.txt
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 v2share-0.1.0a6/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a6/tests/__init__.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 v2share-0.1.0a6/tests/test_links.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 v2share-0.1.0a6/v2share/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 v2share-0.1.0a6/v2share/_version.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 v2share-0.1.0a6/v2share/clash.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 v2share-0.1.0a6/v2share/clashmeta.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 v2share-0.1.0a6/v2share/data.py
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 v2share-0.1.0a6/v2share/singbox.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 v2share-0.1.0a6/v2share/templates/clash.yml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 v2share-0.1.0a6/v2share/templates/singbox.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 v2share-0.1.0a6/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0a6/README.md
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 v2share-0.1.0a6/PKG-INFO
```

### Comparing `v2share-0.1.0a5/.github/workflows/python-tests.yml` & `v2share-0.1.0a6/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a5/v2share/clash.py` & `v2share-0.1.0a6/v2share/clash.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from v2share.data import V2Data
 
 
 class ClashConfig:
     def __init__(self, template_path: Optional[str] = None):
         if not template_path:
-            template_path = (resources.files("v2share.templates") / "clash.yml")
+            template_path = resources.files("v2share.templates") / "clash.yml"
         with open(template_path, "r") as f:
             self.template_data = f.read()
         self.data = {
             "proxies": [],
             "proxy-groups": [],
             "rules": [],
         }
@@ -133,8 +133,7 @@
             self.data["proxies"].append(node)
             self.proxy_remarks.append(config.remark)
         elif config.protocol == "shadowsocks":
             node["password"] = config.password
             node["cipher"] = config.shadowsocks_method
             self.data["proxies"].append(node)
             self.proxy_remarks.append(config.remark)
-
```

### Comparing `v2share-0.1.0a5/v2share/clashmeta.py` & `v2share-0.1.0a6/v2share/clashmeta.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,18 +68,15 @@
             node["cipher"] = "auto"
             self.data["proxies"].append(node)
             self.proxy_remarks.append(config.remark)
 
         if config.protocol == "vless":
             node["uuid"] = str(config.uuid)
 
-            if (
-                config.transport_type in ("tcp", "kcp")
-                and config.header_type != "http"
-            ):
+            if config.transport_type in ("tcp", "kcp") and config.header_type != "http":
                 node["flow"] = config.flow
 
             self.data["proxies"].append(node)
             self.proxy_remarks.append(config.remark)
 
         if config.protocol == "trojan":
             node["password"] = config.password
```

### Comparing `v2share-0.1.0a5/v2share/data.py` & `v2share-0.1.0a6/v2share/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import json
+import urllib.parse as urlparse
 from dataclasses import dataclass
 from typing import Optional
 from uuid import UUID
-import urllib.parse as urlparse
 
 
 @dataclass
 class V2Data:
     protocol: str
     remark: str
     address: str
@@ -67,15 +67,15 @@
             )
         elif self.protocol == "vmess":
             payload = {
                 "add": self.address,
                 "aid": "0",
                 "host": self.host,
                 "id": str(self.uuid),
-                "transport_type": self.transport_type,
+                "net": self.transport_type,
                 "path": self.path,
                 "port": self.port,
                 "ps": self.remark,
                 "scy": "auto",
                 "tls": self.tls,
                 "type": self.header_type,
                 "v": "2",
```

### Comparing `v2share-0.1.0a5/v2share/singbox.py` & `v2share-0.1.0a6/v2share/singbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from v2share.data import V2Data
 
 
 class SingBoxConfig(str):
     def __init__(self, template_path: str = None):
         if not template_path:
-            template_path = (resources.files("v2share.templates") / "singbox.json")
+            template_path = resources.files("v2share.templates") / "singbox.json"
         with open(template_path, "r") as f:
             self._template_data = f.read()
         self._outbounds = []
 
     def render(self):
         result = json.loads(self._template_data)
         result["outbounds"].extend(self._outbounds)
```

### Comparing `v2share-0.1.0a5/v2share/templates/singbox.json` & `v2share-0.1.0a6/v2share/templates/singbox.json`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a5/.gitignore` & `v2share-0.1.0a6/.gitignore`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0a5/pyproject.toml` & `v2share-0.1.0a6/pyproject.toml`

 * *Files identical despite different names*

