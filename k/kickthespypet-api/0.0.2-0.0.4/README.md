# Comparing `tmp/kickthespypet_api-0.0.2.tar.gz` & `tmp/kickthespypet_api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kickthespypet_api-0.0.2.tar", max compression
+gzip compressed data, was "kickthespypet_api-0.0.4.tar", max compression
```

## Comparing `kickthespypet_api-0.0.2.tar` & `kickthespypet_api-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5230 2024-04-26 23:43:47.433331 kickthespypet_api-0.0.2/kickthespypet_api/__init__.py
--rw-r--r--   0        0        0      231 2024-04-26 23:49:39.655614 kickthespypet_api-0.0.2/kickthespypet_api/types.py
--rw-r--r--   0        0        0    17096 2024-04-26 23:56:57.517072 kickthespypet_api-0.0.2/LICENSE
--rw-r--r--   0        0        0      817 2024-04-27 00:08:08.920153 kickthespypet_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      974 2024-04-26 23:53:30.866676 kickthespypet_api-0.0.2/README.md
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 kickthespypet_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5257 2024-05-11 23:18:26.064602 kickthespypet_api-0.0.4/kickthespypet_api/__init__.py
+-rw-r--r--   0        0        0      231 2024-04-26 23:49:39.655614 kickthespypet_api-0.0.4/kickthespypet_api/types.py
+-rw-r--r--   0        0        0    17096 2024-04-26 23:56:57.517072 kickthespypet_api-0.0.4/LICENSE
+-rw-r--r--   0        0        0      792 2024-05-11 23:18:26.065602 kickthespypet_api-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1052 2024-05-11 23:18:26.063103 kickthespypet_api-0.0.4/README.md
+-rw-r--r--   0        0        0     1999 1970-01-01 00:00:00.000000 kickthespypet_api-0.0.4/PKG-INFO
```

### Comparing `kickthespypet_api-0.0.2/kickthespypet_api/__init__.py` & `kickthespypet_api-0.0.4/kickthespypet_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         Keyword arguments:
         id -- A server ID as number, string or `discord.Guild` object
         Return: API data. Raise if API returns status code anything than 200 and 404 for `None`
         """
 
         async with self.client as req:
             async with req.get(
-                "getBot",
+                self.BASE_URL / "getBot",
                 params={"id": id if not isinstance(id, discord.Guild) else id.id},
             ) as resp:
                 if resp.status == 404:  # not found
                     return None
                 resp.raise_for_status()
                 return GetBotAPIResponse(**await resp.json())
 
@@ -116,15 +116,15 @@
 
         Keyword arguments:
         code -- A server invite code as string or `discord.Invite` object
         Return: API data. Raise if API returns status code anything than 200 and 404 for `None`
         """
         async with self.client as req:
             async with req.get(
-                str(self.BASE_URL / "byInv"),
+                self.BASE_URL / "byInv",
                 params={
                     "code": code if not isinstance(code, discord.Invite) else code.id
                 },
             ) as resp:
                 if resp.status == 404:  # not found. again
                     return None
                 resp.raise_for_status()
@@ -135,12 +135,12 @@
 
         Keyword arguments:
         use_orjson -- Uses orjson for faster JSON loading
         Return: Returns a list of user ID
         """
 
         async with self.client as req:
-            async with req.get("ids") as resp:
+            async with req.get(self.BASE_URL / "ids") as resp:
                 resp.raise_for_status()
                 if use_orjson:
                     return orjson.loads(await resp.text())
                 return await resp.json()
```

### Comparing `kickthespypet_api-0.0.2/LICENSE` & `kickthespypet_api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kickthespypet_api-0.0.2/pyproject.toml` & `kickthespypet_api-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kickthespypet-api"
-version = "0.0.2"
+version = "0.0.4"
 description = "kickthespy.pet API wrapper"
 authors = ["timelesnesses <timelessnesses@timelessnesses.me>"]
 readme = "README.md"
 package-mode = true
 license = "MPL-2.0"
 repository = "https://github.com/timelessnesses/kickthespypet-api"
 keywords = [
@@ -14,17 +14,15 @@
     "Development Status :: 4 - Beta",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 aiohttp = "^3.9.5"
-
-[tool.poetry.extras]
-orjson = ["orjson"]
+orjson = "^3.10.3"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/timelessnesses/kickthespypet-api/issues"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
```

### Comparing `kickthespypet_api-0.0.2/README.md` & `kickthespypet_api-0.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ## Installing
 
 ```shell
 pip install git+https://github.com/timelessnesses/kickthespypet-api
 # or
 pip install kickthespypet-api
 ```
+You also need `discord` version of your choice (not installed automatically)
 
 ## Examples
 
 ```python
 import kickthespypet_api
 
 client = kickthespypet_api.KickTheSpyPetAPI()
```

### Comparing `kickthespypet_api-0.0.2/PKG-INFO` & `kickthespypet_api-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: kickthespypet-api
-Version: 0.0.2
+Version: 0.0.4
 Summary: kickthespy.pet API wrapper
 Home-page: https://github.com/timelessnesses/kickthespypet-api
 License: MPL-2.0
 Keywords: async,python3,kickthespy.pet,spy.pet
 Author: timelesnesses
 Author-email: timelessnesses@timelessnesses.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: orjson
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
+Requires-Dist: orjson (>=3.10.3,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/timelessnesses/kickthespypet-api/issues
 Project-URL: Repository, https://github.com/timelessnesses/kickthespypet-api
 Description-Content-Type: text/markdown
 
 # kickthespypet-api
 
@@ -29,14 +29,15 @@
 ## Installing
 
 ```shell
 pip install git+https://github.com/timelessnesses/kickthespypet-api
 # or
 pip install kickthespypet-api
 ```
+You also need `discord` version of your choice (not installed automatically)
 
 ## Examples
 
 ```python
 import kickthespypet_api
 
 client = kickthespypet_api.KickTheSpyPetAPI()
```

