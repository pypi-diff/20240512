# Comparing `tmp/connectlife-0.0.2.tar.gz` & `tmp/connectlife-0.0.3.tar.gz`

## Comparing `connectlife-0.0.2.tar` & `connectlife-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,24 @@
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 connectlife-0.0.2/.github/workflows/python-publish.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 connectlife-0.0.2/connectlife/__init__.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 connectlife-0.0.2/connectlife/api.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 connectlife-0.0.2/connectlife/appliance.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 connectlife-0.0.2/connectlife/dump.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 connectlife-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 connectlife-0.0.2/LICENSE
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 connectlife-0.0.2/README.md
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 connectlife-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 connectlife-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 connectlife-0.0.3/.github/workflows/python-publish.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 connectlife-0.0.3/connectlife/__init__.py
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 connectlife-0.0.3/connectlife/api.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 connectlife-0.0.3/connectlife/appliance.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 connectlife-0.0.3/connectlife/dump.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_dishwasher.json
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_hood_1.json
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_hood_2.json
+-rw-r--r--   0        0        0    14445 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_induction_hob_1.json
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_induction_hob_2.json
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_professional_tumble_dryer.json
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Asko_professional_washing_machine.json
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Gorenje_dishwasher.json
+-rw-r--r--   0        0        0     6891 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Gorenje_washing_machine.json
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Heat_pump.json
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Oven_type_1.json
+-rw-r--r--   0        0        0    15989 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/Oven_type_2.json
+-rw-r--r--   0        0        0   587306 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 connectlife-0.0.3/dumps/format.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 connectlife-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 connectlife-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 connectlife-0.0.3/README.md
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 connectlife-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 connectlife-0.0.3/PKG-INFO
```

### Comparing `connectlife-0.0.2/connectlife/api.py` & `connectlife-0.0.3/connectlife/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 OAUTH2_REDIRECT = "https://api.connectlife.io/swagger/oauth2-redirect.html"
 OAUTH2_AUTHORIZE = "https://oauth.hijuconn.com/oauth/authorize"
 OAUTH2_TOKEN = "https://oauth.hijuconn.com/oauth/token"
 
 APPLIANCES_URL = "https://connectlife.bapi.ovh/appliances"
 
-_LOGGER = logging.getLogger("connectlife")
+_LOGGER = logging.getLogger(__name__)
 
 
 class LifeConnectError(Exception):
     pass
 
 
 class LifeConnectAuthError(Exception):
@@ -72,15 +72,14 @@
         """Make a request and return the response as text."""
         await self._fetch_access_token()
         async with aiohttp.ClientSession() as session:
             async with session.get(APPLIANCES_URL, headers={
                 "User-Agent": "connectlife-api-connector 2.1.4",
                 "X-Token": self._access_token
             }) as response:
-                print(response.headers)
                 return await response.json()
 
 
     async def _fetch_access_token(self):
         if self._expires is None:
             await self._initial_access_token()
         elif self._expires < dt.datetime.now():
```

### Comparing `connectlife-0.0.2/connectlife/dump.py` & `connectlife-0.0.3/connectlife/dump.py`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.2/LICENSE` & `connectlife-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.2/README.md` & `connectlife-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `connectlife-0.0.2/pyproject.toml` & `connectlife-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "connectlife"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Øyvind Matheson Wergeland", email="oyvind@wergeland.org" },
 ]
 description = "A Python library for communicating with the ConnectLife API"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `connectlife-0.0.2/PKG-INFO` & `connectlife-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: connectlife
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python library for communicating with the ConnectLife API
 Project-URL: Homepage, https://github.com/oyvindwe/connectlife
 Project-URL: Issues, https://github.com/oyvindwe/connectlife/issues
 Author-email: Øyvind Matheson Wergeland <oyvind@wergeland.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

