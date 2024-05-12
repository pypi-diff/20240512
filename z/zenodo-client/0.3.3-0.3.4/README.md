# Comparing `tmp/zenodo_client-0.3.3.tar.gz` & `tmp/zenodo_client-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenodo_client-0.3.3.tar", last modified: Thu Mar 28 16:16:47 2024, max compression
+gzip compressed data, was "zenodo_client-0.3.4.tar", last modified: Sun May 12 10:20:32 2024, max compression
```

## Comparing `zenodo_client-0.3.3.tar` & `zenodo_client-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-28 16:16:47.438650 zenodo_client-0.3.3/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2024-03-11 09:20:33.000000 zenodo_client-0.3.3/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      429 2024-03-11 09:20:33.000000 zenodo_client-0.3.3/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)    10275 2024-03-28 16:16:47.438557 zenodo_client-0.3.3/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     8522 2024-03-11 09:20:33.000000 zenodo_client-0.3.3/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-28 16:16:47.430012 zenodo_client-0.3.3/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-28 16:16:47.433617 zenodo_client-0.3.3/docs/source/
--rw-r--r--   0 cthoyt     (501) staff       (20)      246 2023-08-14 13:18:21.000000 zenodo_client-0.3.3/docs/source/cli.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     6988 2024-03-28 16:16:46.000000 zenodo_client-0.3.3/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      275 2023-08-14 13:18:21.000000 zenodo_client-0.3.3/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      534 2023-08-14 13:18:21.000000 zenodo_client-0.3.3/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      693 2024-01-18 17:06:02.000000 zenodo_client-0.3.3/docs/source/usage.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      386 2024-03-28 16:10:47.000000 zenodo_client-0.3.3/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2422 2024-03-28 16:16:47.439046 zenodo_client-0.3.3/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-28 16:16:47.430162 zenodo_client-0.3.3/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-28 16:16:47.435701 zenodo_client-0.3.3/src/zenodo_client/
--rw-r--r--   0 cthoyt     (501) staff       (20)      265 2024-01-18 17:06:02.000000 zenodo_client-0.3.3/src/zenodo_client/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      330 2023-08-14 13:18:21.000000 zenodo_client-0.3.3/src/zenodo_client/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    15543 2024-03-28 16:14:06.000000 zenodo_client-0.3.3/src/zenodo_client/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1611 2023-08-14 13:18:21.000000 zenodo_client-0.3.3/src/zenodo_client/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-03-11 09:20:33.000000 zenodo_client-0.3.3/src/zenodo_client/py.typed
--rw-r--r--   0 cthoyt     (501) staff       (20)     3974 2024-03-11 09:20:33.000000 zenodo_client-0.3.3/src/zenodo_client/struct.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1028 2024-03-28 16:16:46.000000 zenodo_client-0.3.3/src/zenodo_client/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-28 16:16:47.438060 zenodo_client-0.3.3/src/zenodo_client.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)    10275 2024-03-28 16:16:47.000000 zenodo_client-0.3.3/src/zenodo_client.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)      691 2024-03-28 16:16:47.000000 zenodo_client-0.3.3/src/zenodo_client.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-03-28 16:16:47.000000 zenodo_client-0.3.3/src/zenodo_client.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       57 2024-03-28 16:16:47.000000 zenodo_client-0.3.3/src/zenodo_client.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-09-13 06:14:54.000000 zenodo_client-0.3.3/src/zenodo_client.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      137 2024-03-28 16:16:47.000000 zenodo_client-0.3.3/src/zenodo_client.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       14 2024-03-28 16:16:47.000000 zenodo_client-0.3.3/src/zenodo_client.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-28 16:16:47.437754 zenodo_client-0.3.3/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       63 2023-09-13 06:07:52.000000 zenodo_client-0.3.3/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5810 2024-03-28 16:14:18.000000 zenodo_client-0.3.3/tests/test_lifecycle.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-05-12 10:20:32.150638 zenodo_client-0.3.4/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2024-05-09 15:40:48.000000 zenodo_client-0.3.4/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      429 2024-05-09 15:40:48.000000 zenodo_client-0.3.4/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10261 2024-05-12 10:20:32.150557 zenodo_client-0.3.4/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8508 2024-05-09 16:18:05.000000 zenodo_client-0.3.4/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-05-12 10:20:32.146961 zenodo_client-0.3.4/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-05-12 10:20:32.148138 zenodo_client-0.3.4/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      246 2024-05-09 15:40:48.000000 zenodo_client-0.3.4/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6988 2024-05-12 10:20:31.000000 zenodo_client-0.3.4/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      275 2024-05-09 15:40:48.000000 zenodo_client-0.3.4/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      534 2024-05-09 15:40:48.000000 zenodo_client-0.3.4/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2002 2024-05-09 16:20:49.000000 zenodo_client-0.3.4/docs/source/usage.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      386 2024-05-09 15:40:48.000000 zenodo_client-0.3.4/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2422 2024-05-12 10:20:32.150968 zenodo_client-0.3.4/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-05-12 10:20:32.147104 zenodo_client-0.3.4/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-05-12 10:20:32.149043 zenodo_client-0.3.4/src/zenodo_client/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      285 2024-05-09 16:15:03.000000 zenodo_client-0.3.4/src/zenodo_client/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      330 2024-05-09 15:40:48.000000 zenodo_client-0.3.4/src/zenodo_client/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      328 2024-05-09 16:14:53.000000 zenodo_client-0.3.4/src/zenodo_client/_pydantic_compat.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    16981 2024-05-09 16:16:42.000000 zenodo_client-0.3.4/src/zenodo_client/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1611 2024-05-09 15:40:48.000000 zenodo_client-0.3.4/src/zenodo_client/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-05-09 15:40:48.000000 zenodo_client-0.3.4/src/zenodo_client/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4142 2024-05-09 16:14:53.000000 zenodo_client-0.3.4/src/zenodo_client/struct.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1028 2024-05-12 10:20:31.000000 zenodo_client-0.3.4/src/zenodo_client/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-05-12 10:20:32.150111 zenodo_client-0.3.4/src/zenodo_client.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10261 2024-05-12 10:20:32.000000 zenodo_client-0.3.4/src/zenodo_client.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)      729 2024-05-12 10:20:32.000000 zenodo_client-0.3.4/src/zenodo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-05-12 10:20:32.000000 zenodo_client-0.3.4/src/zenodo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       57 2024-05-12 10:20:32.000000 zenodo_client-0.3.4/src/zenodo_client.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-05-09 15:48:52.000000 zenodo_client-0.3.4/src/zenodo_client.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      137 2024-05-12 10:20:32.000000 zenodo_client-0.3.4/src/zenodo_client.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       14 2024-05-12 10:20:32.000000 zenodo_client-0.3.4/src/zenodo_client.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-05-12 10:20:32.149964 zenodo_client-0.3.4/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       63 2024-05-09 15:40:48.000000 zenodo_client-0.3.4/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7546 2024-05-09 16:15:03.000000 zenodo_client-0.3.4/tests/test_lifecycle.py
```

### Comparing `zenodo_client-0.3.3/LICENSE` & `zenodo_client-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zenodo_client-0.3.3/PKG-INFO` & `zenodo_client-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: zenodo_client
-Version: 0.3.3
+Version: 0.3.4
 Summary: A wrapper for the Zenodo API.
 Home-page: https://github.com/cthoyt/zenodo-client
 Download-URL: https://github.com/cthoyt/zenodo-client/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/cthoyt/zenodo-client/issues
 Project-URL: Source, https://github.com/cthoyt/zenodo-client
-Project-URL: Documentation, https://zenodo_client.readthedocs.io
+Project-URL: Documentation, https://zenodo-client.readthedocs.io
 Keywords: cookiecutter,snekpack,Zenodo
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
@@ -64,15 +64,15 @@
     </a>
     <a href="https://pypi.org/project/zenodo_client">
         <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/zenodo_client" />
     </a>
     <a href="https://github.com/cthoyt/zenodo-client/blob/main/LICENSE">
         <img alt="PyPI - License" src="https://img.shields.io/pypi/l/zenodo_client" />
     </a>
-    <a href='https://zenodo_client.readthedocs.io/en/latest/?badge=latest'>
+    <a href='https://zenodo-client.readthedocs.io/en/latest'>
         <img src='https://readthedocs.org/projects/zenodo_client/badge/?version=latest' alt='Documentation Status' />
     </a>
     <a href="https://codecov.io/gh/cthoyt/zenodo-client/branch/main">
         <img src="https://codecov.io/gh/cthoyt/zenodo-client/branch/main/graph/badge.svg" alt="Codecov status" />
     </a>  
     <a href="https://github.com/cthoyt/cookiecutter-python-package">
         <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-snekpack-blue" />
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: zenodo_client Version: 0.3.3 Summary: A wrapper for
+Metadata-Version: 2.1 Name: zenodo_client Version: 0.3.4 Summary: A wrapper for
 the Zenodo API. Home-page: https://github.com/cthoyt/zenodo-client Download-
 URL: https://github.com/cthoyt/zenodo-client/releases Author: Charles Tapley
 Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt Maintainer-
 email: cthoyt@gmail.com License: MIT Project-URL: Tracker, https://github.com/
 cthoyt/zenodo-client/issues Project-URL: Source, https://github.com/cthoyt/
-zenodo-client Project-URL: Documentation, https://zenodo_client.readthedocs.io
+zenodo-client Project-URL: Documentation, https://zenodo-client.readthedocs.io
 Keywords: cookiecutter,snekpack,Zenodo Classifier: Development Status :: 1 -
 Planning Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Framework :: Pytest Classifier:
 Framework :: tox Classifier: Framework :: Sphinx Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `zenodo_client-0.3.3/README.md` & `zenodo_client-0.3.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     </a>
     <a href="https://pypi.org/project/zenodo_client">
         <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/zenodo_client" />
     </a>
     <a href="https://github.com/cthoyt/zenodo-client/blob/main/LICENSE">
         <img alt="PyPI - License" src="https://img.shields.io/pypi/l/zenodo_client" />
     </a>
-    <a href='https://zenodo_client.readthedocs.io/en/latest/?badge=latest'>
+    <a href='https://zenodo-client.readthedocs.io/en/latest'>
         <img src='https://readthedocs.org/projects/zenodo_client/badge/?version=latest' alt='Documentation Status' />
     </a>
     <a href="https://codecov.io/gh/cthoyt/zenodo-client/branch/main">
         <img src="https://codecov.io/gh/cthoyt/zenodo-client/branch/main/graph/badge.svg" alt="Codecov status" />
     </a>  
     <a href="https://github.com/cthoyt/cookiecutter-python-package">
         <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-snekpack-blue" />
```

### Comparing `zenodo_client-0.3.3/docs/source/conf.py` & `zenodo_client-0.3.4/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "zenodo_client"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.3.3"
+release = "0.3.4"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `zenodo_client-0.3.3/docs/source/installation.rst` & `zenodo_client-0.3.4/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `zenodo_client-0.3.3/setup.cfg` & `zenodo_client-0.3.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = zenodo_client
-version = 0.3.3
+version = 0.3.4
 description = A wrapper for the Zenodo API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/zenodo-client
 download_url = https://github.com/cthoyt/zenodo-client/releases
 project_urls = 
 	Tracker = https://github.com/cthoyt/zenodo-client/issues
 	Source = https://github.com/cthoyt/zenodo-client
-	Documentation = https://zenodo_client.readthedocs.io
+	Documentation = https://zenodo-client.readthedocs.io
 author = Charles Tapley Hoyt
 author_email = cthoyt@gmail.com
 maintainer = Charles Tapley Hoyt
 maintainer_email = cthoyt@gmail.com
 license = MIT
 license_files = 
 	LICENSE
```

### Comparing `zenodo_client-0.3.3/src/zenodo_client/api.py` & `zenodo_client-0.3.4/src/zenodo_client/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from .struct import Metadata
 
 __all__ = [
     "ensure_zenodo",
     "update_zenodo",
     "create_zenodo",
+    "publish_zenodo",
     "download_zenodo",
     "download_zenodo_latest",
     "Zenodo",
 ]
 
 logger = logging.getLogger(__name__)
 
@@ -33,22 +34,27 @@
 
 
 def ensure_zenodo(key: str, data: Data, paths: Paths, **kwargs) -> requests.Response:
     """Create a Zenodo record if it doesn't exist, or update one that does."""
     return Zenodo(**kwargs).ensure(key=key, data=data, paths=paths)
 
 
-def create_zenodo(data: Data, paths: Paths, **kwargs) -> requests.Response:
+def create_zenodo(data: Data, paths: Paths, *, publish: bool = True, **kwargs) -> requests.Response:
     """Create a Zenodo record."""
-    return Zenodo(**kwargs).create(data, paths)
+    return Zenodo(**kwargs).create(data, paths, publish=publish)
 
 
-def update_zenodo(deposition_id: str, paths: Paths, **kwargs) -> requests.Response:
+def update_zenodo(deposition_id: str, paths: Paths, *, publish: bool = True, **kwargs) -> requests.Response:
     """Update a Zenodo record."""
-    return Zenodo(**kwargs).update(deposition_id, paths)
+    return Zenodo(**kwargs).update(deposition_id, paths, publish=publish)
+
+
+def publish_zenodo(deposition_id: str, *, sleep: bool = True, **kwargs) -> requests.Response:
+    """Publish a Zenodo record."""
+    return Zenodo(**kwargs).publish(deposition_id, sleep=sleep)
 
 
 def download_zenodo(deposition_id: str, name: str, force: bool = False, **kwargs) -> Path:
     """Download a Zenodo record."""
     return Zenodo(**kwargs).download(deposition_id, name=name, force=force)
 
 
@@ -100,19 +106,20 @@
 
         res = self.create(data=data, paths=paths)
         # Write the ID to the key in the local configuration
         # so it doesn't need to be created from scratch next time
         pystow.write_config(self.module, key, str(res.json()["id"]))
         return res
 
-    def create(self, data: Data, paths: Paths) -> requests.Response:
+    def create(self, data: Data, paths: Paths, *, publish: bool = True) -> requests.Response:
         """Create a record.
 
         :param data: The JSON data to send to the new data
         :param paths: Paths to local files to upload
+        :param publish: Publish the deposit after creation
         :return: The response JSON from the Zenodo API
         :raises ValueError: if the response is missing a "bucket"
         """
         if isinstance(data, Metadata):
             logger.debug("serializing metadata")
             data = {
                 "metadata": {key: value for key, value in data.dict(exclude_none=True).items() if value},
@@ -132,14 +139,17 @@
         if bucket is None:
             raise ValueError(f"No bucket in response. Got: {res_json}")
 
         logger.info("uploading files to bucket %s", bucket)
         self._upload_files(bucket=bucket, paths=paths)
 
         deposition_id = res_json["id"]
+        if not publish:
+            return self._get_deposition(deposition_id)
+
         logger.info("publishing files to deposition %s", deposition_id)
         return self.publish(deposition_id)
 
     def edit(self, deposition_id: str, sleep: bool = True) -> requests.Response:
         """Unlock already submitted deposition for editing, see https://developers.zenodo.org/#edit.
 
         :param deposition_id: The identifier of the deposition on Zenodo.
@@ -195,24 +205,55 @@
         res = requests.post(
             f"{self.depositions_base}/{deposition_id}/actions/{action}",
             params={"access_token": self.access_token},
         )
         res.raise_for_status()
         return res
 
-    def update(self, deposition_id: str, paths: Paths) -> requests.Response:
+    def _get_deposition(self, deposition_id: str) -> requests.Response:
+        """Get the metadata for a deposition."""
+        url = f"{self.depositions_base}/{deposition_id}"
+        res = requests.get(url, params={"access_token": self.access_token})
+        res.raise_for_status()
+        return res
+
+    def update(self, deposition_id: str, paths: Paths, publish: bool = True) -> requests.Response:
         """Update a record, including creating a new version of the given record, with the given files.
 
-        :param deposition_id: The identifier of the deposition on Zenodo. It should be in edit mode.
+        :param deposition_id: The identifier of the deposition on Zenodo.
         :param paths: Paths to local files to upload; existing files with matching hashes will not be uploaded.
+        :param publish: Publish the deposition after the update.
         :return: The response JSON from the Zenodo API
         """
-        url = f"{self.depositions_base}/{deposition_id}"
-        res = requests.get(url, params={"access_token": self.access_token})
-        res.raise_for_status()
+        res = self._get_deposition(deposition_id)
+
+        deposition_data = res.json()
+        if deposition_data["submitted"]:
+            new_deposition_id, new_deposition_data = self._update_submitted_deposition_metadata(deposition_id, res)
+        else:
+            new_deposition_id, new_deposition_data = deposition_data["id"], deposition_data
+
+        bucket = new_deposition_data["links"]["bucket"]
+
+        # Upload new files. It calculates the hash on all of these, and if no files have changed,
+        #  there will be no update
+        self._upload_files(bucket=bucket, paths=paths)
+
+        # Get the new metadata with the files
+        res = self._get_deposition(deposition_id)
+
+        if not publish:
+            # Return the response with latest metadata
+            return res
+
+        # Send the publish command
+        return self.publish(new_deposition_id)
+
+    def _update_submitted_deposition_metadata(self, deposition_id: str, res: requests.Response) -> tuple:
+        res = self._get_deposition(deposition_id)
         old_version = res.json()["metadata"]["version"]
         new_version = _prepare_new_version(old_version)
 
         res = self.new_version(deposition_id, sleep=False)
         # Parse out the new version (@zenodo please give this as its own field!)
         new_deposition_id = res.json()["links"]["latest_draft"].split("/")[-1]
 
@@ -220,35 +261,28 @@
         # see: https://developers.zenodo.org/#retrieve
         res = requests.get(
             f"{self.depositions_base}/{new_deposition_id}",
             params={"access_token": self.access_token},
         )
         res.raise_for_status()
         new_deposition_data = res.json()
-        # Update the version
+        # Update the version and date
         new_deposition_data["metadata"]["version"] = new_version
         new_deposition_data["metadata"]["publication_date"] = datetime.datetime.today().strftime("%Y-%m-%d")
 
         # Update the deposition for the new version
         # see: https://developers.zenodo.org/#update
         res = requests.put(
             f"{self.depositions_base}/{new_deposition_id}",
             json={"metadata": new_deposition_data["metadata"]},
             params={"access_token": self.access_token},
         )
         res.raise_for_status()
 
-        bucket = new_deposition_data["links"]["bucket"]
-
-        # Upload new files. It calculates the hash on all of these, and if no files have changed,
-        #  there will be no update
-        self._upload_files(bucket=bucket, paths=paths)
-
-        # Send the publish command
-        return self.publish(new_deposition_id)
+        return new_deposition_id, new_deposition_data
 
     def _upload_files(self, *, bucket: str, paths: Paths) -> List[requests.Response]:
         _paths = [paths] if isinstance(paths, (str, Path)) else paths
         rv = []
         # see https://developers.zenodo.org/#quickstart-upload
         for path in _paths:
             with open(path, "rb") as file:
```

### Comparing `zenodo_client-0.3.3/src/zenodo_client/cli.py` & `zenodo_client-0.3.4/src/zenodo_client/cli.py`

 * *Files identical despite different names*

### Comparing `zenodo_client-0.3.3/src/zenodo_client/struct.py` & `zenodo_client-0.3.4/src/zenodo_client/struct.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import datetime
 from typing import List, Optional, Sequence
 
 from pydantic import BaseModel, Field
 from typing_extensions import Literal
 
+from ._pydantic_compat import field_validator
+
 __all__ = [
     "Creator",
     "Metadata",
 ]
 
 
 # https://developers.zenodo.org/#rest-api
@@ -45,17 +47,20 @@
         return f"https://orcid.org/{self.orcid}" if self.orcid else None
 
     @property
     def gnd_url(self) -> Optional[str]:
         """Get the GND identifier as a URL."""
         return f"https://d-nb.info/gnd/{self.gnd}" if self.gnd else None
 
-    def __post_init__(self):  # noqa:D105
-        if "," not in self.name:
+    @field_validator("name")  # type:ignore
+    def comma_in_name(cls, v: str) -> str:  # noqa:N805
+        """Check that a comma appears in the name."""
+        if "," not in v:
             raise ValueError("name should be in format Family name, given names")
+        return v
 
 
 UploadType = Literal[
     "publication",
     "poster",
     "presentation",
     "dataset",
```

### Comparing `zenodo_client-0.3.3/src/zenodo_client/version.py` & `zenodo_client-0.3.4/src/zenodo_client/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.3.3"
+VERSION = "0.3.4"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`zenodo_client` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `zenodo_client-0.3.3/src/zenodo_client.egg-info/PKG-INFO` & `zenodo_client-0.3.4/src/zenodo_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: zenodo_client
-Version: 0.3.3
+Version: 0.3.4
 Summary: A wrapper for the Zenodo API.
 Home-page: https://github.com/cthoyt/zenodo-client
 Download-URL: https://github.com/cthoyt/zenodo-client/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
 License: MIT
 Project-URL: Tracker, https://github.com/cthoyt/zenodo-client/issues
 Project-URL: Source, https://github.com/cthoyt/zenodo-client
-Project-URL: Documentation, https://zenodo_client.readthedocs.io
+Project-URL: Documentation, https://zenodo-client.readthedocs.io
 Keywords: cookiecutter,snekpack,Zenodo
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
@@ -64,15 +64,15 @@
     </a>
     <a href="https://pypi.org/project/zenodo_client">
         <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/zenodo_client" />
     </a>
     <a href="https://github.com/cthoyt/zenodo-client/blob/main/LICENSE">
         <img alt="PyPI - License" src="https://img.shields.io/pypi/l/zenodo_client" />
     </a>
-    <a href='https://zenodo_client.readthedocs.io/en/latest/?badge=latest'>
+    <a href='https://zenodo-client.readthedocs.io/en/latest'>
         <img src='https://readthedocs.org/projects/zenodo_client/badge/?version=latest' alt='Documentation Status' />
     </a>
     <a href="https://codecov.io/gh/cthoyt/zenodo-client/branch/main">
         <img src="https://codecov.io/gh/cthoyt/zenodo-client/branch/main/graph/badge.svg" alt="Codecov status" />
     </a>  
     <a href="https://github.com/cthoyt/cookiecutter-python-package">
         <img alt="Cookiecutter template from @cthoyt" src="https://img.shields.io/badge/Cookiecutter-snekpack-blue" />
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: zenodo_client Version: 0.3.3 Summary: A wrapper for
+Metadata-Version: 2.1 Name: zenodo_client Version: 0.3.4 Summary: A wrapper for
 the Zenodo API. Home-page: https://github.com/cthoyt/zenodo-client Download-
 URL: https://github.com/cthoyt/zenodo-client/releases Author: Charles Tapley
 Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt Maintainer-
 email: cthoyt@gmail.com License: MIT Project-URL: Tracker, https://github.com/
 cthoyt/zenodo-client/issues Project-URL: Source, https://github.com/cthoyt/
-zenodo-client Project-URL: Documentation, https://zenodo_client.readthedocs.io
+zenodo-client Project-URL: Documentation, https://zenodo-client.readthedocs.io
 Keywords: cookiecutter,snekpack,Zenodo Classifier: Development Status :: 1 -
 Planning Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Framework :: Pytest Classifier:
 Framework :: tox Classifier: Framework :: Sphinx Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `zenodo_client-0.3.3/src/zenodo_client.egg-info/SOURCES.txt` & `zenodo_client-0.3.4/src/zenodo_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 docs/source/cli.rst
 docs/source/conf.py
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/usage.rst
 src/zenodo_client/__init__.py
 src/zenodo_client/__main__.py
+src/zenodo_client/_pydantic_compat.py
 src/zenodo_client/api.py
 src/zenodo_client/cli.py
 src/zenodo_client/py.typed
 src/zenodo_client/struct.py
 src/zenodo_client/version.py
 src/zenodo_client.egg-info/PKG-INFO
 src/zenodo_client.egg-info/SOURCES.txt
```

### Comparing `zenodo_client-0.3.3/tests/test_lifecycle.py` & `zenodo_client-0.3.4/tests/test_lifecycle.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Tests for the upload and revision lifecyle."""
 
 import datetime
+import hashlib
 import logging
 import tempfile
 import unittest
 from pathlib import Path
 from uuid import uuid4
 
 import requests
@@ -23,14 +24,23 @@
     affiliation="Northeastern University",
     orcid="0000-0003-4423-4370",
     # Note: zenodo has some problem validating my GND. Skip it for now
     # gnd="1203140533",
 )
 
 
+class TestStruct(unittest.TestCase):
+    """Tests for data structures."""
+
+    def test_name(self):
+        """Test name errors."""
+        with self.assertRaises(ValueError):
+            Creator(name="Charles Tapley Hoyt")
+
+
 class TestLifecycle(unittest.TestCase):
     """Test case for zenodo client."""
 
     def setUp(self) -> None:
         """Set up the test case with a zenodo client."""
         self.zenodo = Zenodo(sandbox=True)
         self.assertIsInstance(self.zenodo.access_token, str)
@@ -129,7 +139,44 @@
         res_json = res.json()
         # print(f"\n\nSEE V1 ON ZENODO: {res_json['links']['record_html']}")
         self.assertEqual(True, res_json["submitted"])
         self.assertEqual("done", res_json["state"])
         self.assertEqual("dataset", res_json["metadata"]["upload_type"])
         self.assertEqual(data.title, res_json["metadata"]["title"])
         self.assertEqual(data.version, res_json["metadata"]["version"])
+
+    def test_create_without_publish(self):
+        """Test create without publishing."""
+        data = Metadata(
+            title="Test Upload",
+            upload_type="dataset",
+            description="Test create without publishing",
+            creators=[
+                Creator(
+                    name="Hoyt, Charles Tapley",
+                    affiliation="Harvard Medical School",
+                    orcid="0000-0003-4423-4370",
+                ),
+            ],
+        )
+
+        res = self.zenodo.create(data=data, paths=[], publish=False)
+        res_create_json = res.json()
+        deposition_id = res_create_json["id"]
+
+        self.assertEqual(False, res_create_json["submitted"])
+        self.assertEqual("unsubmitted", res_create_json["state"])
+        self.assertEqual(0, len(res_create_json["files"]))
+
+        path = self.directory.joinpath("doi.txt")
+        path.write_text("this record will have DOI %s" % res_create_json["metadata"]["prereserve_doi"]["doi"])
+
+        res = self.zenodo.update(deposition_id, paths=[path], publish=False)
+        res_update_json = res.json()
+
+        path_hash = hashlib.md5(path.read_bytes()).hexdigest()  # noqa:S324,S303
+        self.assertEqual(path_hash, res_update_json["files"][0]["checksum"])
+        self.assertEqual(deposition_id, res_update_json["id"])
+
+        res = self.zenodo.publish(deposition_id=deposition_id)
+        res_publish_json = res.json()
+        self.assertEqual(deposition_id, res_publish_json["id"])
```

