# Comparing `tmp/algobase-0.9.2.tar.gz` & `tmp/algobase-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algobase-0.9.2.tar", max compression
+gzip compressed data, was "algobase-0.9.3.tar", max compression
```

## Comparing `algobase-0.9.2.tar` & `algobase-0.9.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10886 2024-01-31 11:56:38.775754 algobase-0.9.2/LICENSE
--rw-r--r--   0        0        0    10354 2024-01-31 11:56:38.775754 algobase-0.9.2/README.md
--rw-r--r--   0        0        0       74 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/__init__.py
--rw-r--r--   0        0        0     1069 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/choices.py
--rw-r--r--   0        0        0       28 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/data/__init__.py
--rw-r--r--   0        0        0     2523 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/data/ipfs.toml
--rw-r--r--   0        0        0      556 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/functional.py
--rw-r--r--   0        0        0       19 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/ipfs/__init__.py
--rw-r--r--   0        0        0     2503 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/ipfs/client_base.py
--rw-r--r--   0        0        0     3791 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/ipfs/nft_storage.py
--rw-r--r--   0        0        0       60 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/models/__init__.py
--rw-r--r--   0        0        0     6842 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/models/arc3.py
--rw-r--r--   0        0        0     7933 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/models/asa.py
--rw-r--r--   0        0        0     2457 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/models/asset_params.py
--rw-r--r--   0        0        0       26 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/types/__init__.py
--rw-r--r--   0        0        0     3603 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/types/annotated.py
--rw-r--r--   0        0        0       38 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/utils/__init__.py
--rw-r--r--   0        0        0      553 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/utils/hash.py
--rw-r--r--   0        0        0      606 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/utils/read.py
--rw-r--r--   0        0        0      727 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/utils/url.py
--rw-r--r--   0        0        0     8848 2024-01-31 11:56:38.775754 algobase-0.9.2/algobase/utils/validate.py
--rw-r--r--   0        0        0     3565 2024-01-31 11:56:38.779754 algobase-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    11710 1970-01-01 00:00:00.000000 algobase-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    10886 2024-01-31 23:36:42.092809 algobase-0.9.3/LICENSE
+-rw-r--r--   0        0        0    10354 2024-01-31 23:36:42.092809 algobase-0.9.3/README.md
+-rw-r--r--   0        0        0       74 2024-01-31 23:36:42.092809 algobase-0.9.3/algobase/__init__.py
+-rw-r--r--   0        0        0     1069 2024-01-31 23:36:42.092809 algobase-0.9.3/algobase/choices.py
+-rw-r--r--   0        0        0       28 2024-01-31 23:36:42.092809 algobase-0.9.3/algobase/data/__init__.py
+-rw-r--r--   0        0        0     2523 2024-01-31 23:36:42.092809 algobase-0.9.3/algobase/data/ipfs.toml
+-rw-r--r--   0        0        0      556 2024-01-31 23:36:42.092809 algobase-0.9.3/algobase/functional.py
+-rw-r--r--   0        0        0       19 2024-01-31 23:36:42.092809 algobase-0.9.3/algobase/ipfs/__init__.py
+-rw-r--r--   0        0        0     2407 2024-01-31 23:36:42.092809 algobase-0.9.3/algobase/ipfs/client_base.py
+-rw-r--r--   0        0        0     3622 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/ipfs/nft_storage.py
+-rw-r--r--   0        0        0       60 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/models/__init__.py
+-rw-r--r--   0        0        0     6842 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/models/arc3.py
+-rw-r--r--   0        0        0     7933 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/models/asa.py
+-rw-r--r--   0        0        0     2457 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/models/asset_params.py
+-rw-r--r--   0        0        0       26 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/types/__init__.py
+-rw-r--r--   0        0        0     3603 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/types/annotated.py
+-rw-r--r--   0        0        0       38 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/utils/__init__.py
+-rw-r--r--   0        0        0      553 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/utils/hash.py
+-rw-r--r--   0        0        0      606 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/utils/read.py
+-rw-r--r--   0        0        0      727 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/utils/url.py
+-rw-r--r--   0        0        0     8848 2024-01-31 23:36:42.096809 algobase-0.9.3/algobase/utils/validate.py
+-rw-r--r--   0        0        0     3565 2024-01-31 23:36:42.096809 algobase-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    11710 1970-01-01 00:00:00.000000 algobase-0.9.3/PKG-INFO
```

### Comparing `algobase-0.9.2/LICENSE` & `algobase-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/README.md` & `algobase-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/choices.py` & `algobase-0.9.3/algobase/choices.py`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/data/ipfs.toml` & `algobase-0.9.3/algobase/data/ipfs.toml`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/functional.py` & `algobase-0.9.3/algobase/functional.py`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/ipfs/client_base.py` & `algobase-0.9.3/algobase/ipfs/client_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Abstract base class for IPFS clients."""
 
 from abc import ABC, abstractmethod
 
+import httpx
 from decouple import UndefinedValueError, config
 
 from algobase.choices import IpfsPinStatusChoice, IpfsProviderChoice
 from algobase.functional import maybe_bind
 
 
 class IpfsClient(ABC):
@@ -26,15 +27,15 @@
     @abstractmethod
     def api_version(self) -> str:
         """The version of the IPFS provider's API."""
         ...  # pragma: no cover
 
     @property
     @abstractmethod
-    def base_url(self) -> str:
+    def base_url(self) -> httpx.URL:
         """The base URL of the IPFS provider's API."""
         ...  # pragma: no cover
 
     @property
     @abstractmethod
     def is_api_key_required(self) -> bool:
         """Whether the IPFS provider requires an API key."""
@@ -54,29 +55,29 @@
         """Checks that the IPFS provider's API key is present."""
         if self.is_api_key_required and self.api_key is None:
             raise UndefinedValueError(
                 f"`{self.api_key_name}` must be defined in .env file."
             )
 
     @abstractmethod
-    def store_json(self, json: str) -> str | None:
+    def store_json(self, json: str) -> str:
         """Stores JSON data in IPFS.
 
         Args:
             json (str): The JSON to store.
 
         Returns:
-            str | None: The IPFS CID of the stored data, or None if the data could not be stored.
+            str: The IPFS CID of the stored data.
         """
         ...  # pragma: no cover
 
     @abstractmethod
-    def fetch_pin_status(self, cid: str) -> IpfsPinStatusChoice | None:
+    def fetch_pin_status(self, cid: str) -> IpfsPinStatusChoice:
         """Returns the pinning status of a file, by CID.
 
         Args:
             cid (str): The CID of the file to check.
 
         Returns:
-            IpfsPinStatusChoice | None: The pin status of the CID, or None if the status could not be retrieved.
+            IpfsPinStatusChoice: The pin status of the CID.
         """
         ...  # pragma: no cover
```

### Comparing `algobase-0.9.2/algobase/ipfs/nft_storage.py` & `algobase-0.9.3/algobase/ipfs/nft_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """IPFS client for nft.storage."""
 
 from dataclasses import dataclass
-from urllib.parse import urljoin
 
 import httpx
 
 from algobase.choices import (
     IpfsPinStatus,
     IpfsPinStatusChoice,
     IpfsProvider,
@@ -28,40 +27,40 @@
 
     @property
     def api_version(self) -> str:
         """The version of the IPFS provider's API."""
         return "1.0"
 
     @property
-    def base_url(self) -> str:
+    def base_url(self) -> httpx.URL:
         """The base URL of the IPFS provider's API."""
-        return "https://api.nft.storage"
+        return httpx.URL("https://api.nft.storage")
 
     @property
     def is_api_key_required(self) -> bool:
         """Whether the IPFS provider requires an API key."""
         return True
 
     @property
     def headers(self) -> dict[str, str]:
         """The headers to use for the HTTP requests."""
         return {"Authorization": f"Bearer {self.api_key}"}
 
-    def store_json(self, json: str) -> str | None:
+    def store_json(self, json: str) -> str:
         """Stores JSON data in IPFS.
 
         Args:
             json (str): The JSON to store.
 
         Returns:
-            str | None: The IPFS CID of the stored data, or None if the data could not be stored.
+            str: The IPFS CID of the stored data.
         """
         with httpx.Client() as client:
             response = client.post(
-                url=urljoin(self.base_url, "upload"),
+                url=self.base_url.join("upload"),
                 json=json,
                 headers=self.headers,
                 timeout=10.0,
             )
             data = response.json()
             if response.status_code == httpx.codes.OK:
                 if (
@@ -74,27 +73,26 @@
                         f"HTTP Exception for {response.request.url}: Failed to store JSON in IPFS using {self.ipfs_provider_name}."
                     )
             else:
                 raise httpx.HTTPError(
                     f"HTTP Exception for {response.request.url}: {response.status_code} {data.get('error').get('message')}"
                 )
 
-    def fetch_pin_status(self, cid: str) -> IpfsPinStatusChoice | None:
+    def fetch_pin_status(self, cid: str) -> IpfsPinStatusChoice:
         """Returns the pinning status of a file, by CID.
 
         Args:
             cid (str): The CID of the file to check.
 
         Returns:
-            IpfsPinStatusChoice | None: The pin status of the CID, or None if the status could not be retrieved.
+            IpfsPinStatusChoice: The pin status of the CID.
         """
         with httpx.Client() as client:
             response = client.get(
-                url=urljoin(self.base_url, "check"),
-                params={"cid": cid},
+                url=self.base_url.join(f"check/{cid}"),
                 headers=self.headers,
                 timeout=10.0,
             )
             data = response.json()
             if response.status_code == httpx.codes.OK:
                 pin_status = data.get("value").get("pin").get("status")
                 if (
```

### Comparing `algobase-0.9.2/algobase/models/arc3.py` & `algobase-0.9.3/algobase/models/arc3.py`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/models/asa.py` & `algobase-0.9.3/algobase/models/asa.py`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/models/asset_params.py` & `algobase-0.9.3/algobase/models/asset_params.py`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/types/annotated.py` & `algobase-0.9.3/algobase/types/annotated.py`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/utils/hash.py` & `algobase-0.9.3/algobase/utils/hash.py`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/utils/read.py` & `algobase-0.9.3/algobase/utils/read.py`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/utils/url.py` & `algobase-0.9.3/algobase/utils/url.py`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/algobase/utils/validate.py` & `algobase-0.9.3/algobase/utils/validate.py`

 * *Files identical despite different names*

### Comparing `algobase-0.9.2/pyproject.toml` & `algobase-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "algobase"
-version = "0.9.2"
+version = "0.9.3"
 description = "A type-safe Python library for interacting with assets on Algorand."
 readme = "README.md"
 authors = ["algobase <alexandercodes@proton.me>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/code-alexander/algobase"
 homepage = "https://github.com/code-alexander/algobase"
```

### Comparing `algobase-0.9.2/PKG-INFO` & `algobase-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algobase
-Version: 0.9.2
+Version: 0.9.3
 Summary: A type-safe Python library for interacting with assets on Algorand.
 Home-page: https://github.com/code-alexander/algobase
 License: Apache Software License 2.0
 Author: algobase
 Author-email: alexandercodes@proton.me
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

