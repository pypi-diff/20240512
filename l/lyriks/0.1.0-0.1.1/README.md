# Comparing `tmp/lyriks-0.1.0.tar.gz` & `tmp/lyriks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyriks-0.1.0.tar", last modified: Sun May 12 21:21:36 2024, max compression
+gzip compressed data, was "lyriks-0.1.1.tar", last modified: Sun May 12 21:49:30 2024, max compression
```

## Comparing `lyriks-0.1.0.tar` & `lyriks-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-12 21:21:36.688278 lyriks-0.1.0/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-12 21:21:36.688278 lyriks-0.1.0/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-12 21:20:32.000000 lyriks-0.1.0/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-12 21:21:36.684945 lyriks-0.1.0/lyriks/
--rw-r--r--   0 max       (1000) max       (1000)      536 2024-05-12 15:25:28.000000 lyriks-0.1.0/lyriks/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)     2770 2024-05-12 20:18:56.000000 lyriks-0.1.0/lyriks/genie_client.py
--rw-r--r--   0 max       (1000) max       (1000)     1134 2024-05-12 20:20:30.000000 lyriks-0.1.0/lyriks/lyrics.py
--rw-r--r--   0 max       (1000) max       (1000)     3968 2024-05-12 19:07:56.000000 lyriks-0.1.0/lyriks/lyrics_fetcher.py
--rw-r--r--   0 max       (1000) max       (1000)     1942 2024-05-12 20:20:30.000000 lyriks-0.1.0/lyriks/mb_client.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-12 21:21:36.688278 lyriks-0.1.0/lyriks.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-12 21:21:36.000000 lyriks-0.1.0/lyriks.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      310 2024-05-12 21:21:36.000000 lyriks-0.1.0/lyriks.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-12 21:21:36.000000 lyriks-0.1.0/lyriks.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-12 21:21:36.000000 lyriks-0.1.0/lyriks.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-12 21:21:36.000000 lyriks-0.1.0/lyriks.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-12 21:21:36.000000 lyriks-0.1.0/lyriks.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-12 16:40:13.000000 lyriks-0.1.0/pyproject.toml
--rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-12 21:21:36.688278 lyriks-0.1.0/setup.cfg
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-12 21:49:30.353587 lyriks-0.1.1/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-12 21:49:30.353587 lyriks-0.1.1/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     1501 2024-05-12 21:48:33.000000 lyriks-0.1.1/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-12 21:49:30.353587 lyriks-0.1.1/lyriks/
+-rw-r--r--   0 max       (1000) max       (1000)      536 2024-05-12 15:25:28.000000 lyriks-0.1.1/lyriks/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)     2770 2024-05-12 20:18:56.000000 lyriks-0.1.1/lyriks/genie_client.py
+-rw-r--r--   0 max       (1000) max       (1000)     1134 2024-05-12 20:20:30.000000 lyriks-0.1.1/lyriks/lyrics.py
+-rw-r--r--   0 max       (1000) max       (1000)     3971 2024-05-12 21:46:34.000000 lyriks-0.1.1/lyriks/lyrics_fetcher.py
+-rw-r--r--   0 max       (1000) max       (1000)     1942 2024-05-12 21:48:33.000000 lyriks-0.1.1/lyriks/mb_client.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2024-05-12 21:49:30.353587 lyriks-0.1.1/lyriks.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     1958 2024-05-12 21:49:30.000000 lyriks-0.1.1/lyriks.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      310 2024-05-12 21:49:30.000000 lyriks-0.1.1/lyriks.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2024-05-12 21:49:30.000000 lyriks-0.1.1/lyriks.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       39 2024-05-12 21:49:30.000000 lyriks-0.1.1/lyriks.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       29 2024-05-12 21:49:30.000000 lyriks-0.1.1/lyriks.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        7 2024-05-12 21:49:30.000000 lyriks-0.1.1/lyriks.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)      530 2024-05-12 21:48:22.000000 lyriks-0.1.1/pyproject.toml
+-rw-r--r--   0 max       (1000) max       (1000)       38 2024-05-12 21:49:30.353587 lyriks-0.1.1/setup.cfg
```

### Comparing `lyriks-0.1.0/PKG-INFO` & `lyriks-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command line tool to fetch lyrics from Genie
 Author-email: Maxr1998 <max@maxr1998.de>
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -18,15 +18,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.1.0-py3-none-any.whl
+pip install dist/lyriks-0.1.1-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.1.0/README.md` & `lyriks-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.1.0-py3-none-any.whl
+pip install dist/lyriks-0.1.1-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.1.0/lyriks/__init__.py` & `lyriks-0.1.1/lyriks/__init__.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.1.0/lyriks/genie_client.py` & `lyriks-0.1.1/lyriks/genie_client.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.1.0/lyriks/lyrics.py` & `lyriks-0.1.1/lyriks/lyrics.py`

 * *Files identical despite different names*

### Comparing `lyriks-0.1.0/lyriks/lyrics_fetcher.py` & `lyriks-0.1.1/lyriks/lyrics_fetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,13 +112,13 @@
         rg_releases = get_releases_by_release_group(rg_mbid)
         if not rg_releases:
             return None
 
         for rg_release in rg_releases:
             if rg_release.get_track_count() != release.get_track_count():
                 continue
-            album_id = release.get_genie_album_id()
+            album_id = rg_release.get_genie_album_id()
             if album_id is not None:
                 return album_id
 
         print(f'No Genie URL found for release {release.title} [{release.id}]')
         return None
```

### Comparing `lyriks-0.1.0/lyriks/mb_client.py` & `lyriks-0.1.1/lyriks/mb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import time
 
 import requests
 from requests import JSONDecodeError
 
 API_URL = 'https://musicbrainz.org/ws/2'
-USER_AGENT = 'lyriks/0.1.0 ( max@maxr1998.de )'
+USER_AGENT = 'lyriks/0.1.1 ( max@maxr1998.de )'
 
 last_request_time = 0
 
 
 class Release:
     def __init__(self, data: dict):
         self.data = data
```

### Comparing `lyriks-0.1.0/lyriks.egg-info/PKG-INFO` & `lyriks-0.1.1/lyriks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lyriks
-Version: 0.1.0
+Version: 0.1.1
 Summary: A command line tool to fetch lyrics from Genie
 Author-email: Maxr1998 <max@maxr1998.de>
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -18,15 +18,15 @@
 
 ### Installation
 
 Build the wheel and install it with pip:
 
 ```bash
 python -m build --wheel
-pip install dist/lyriks-0.1.0-py3-none-any.whl
+pip install dist/lyriks-0.1.1-py3-none-any.whl
 ```
 
 Alternatively, you can directly run the script from the repository:
 
 ```bash
 `./lyriks.py /path/to/music/folder`
 ```
```

### Comparing `lyriks-0.1.0/pyproject.toml` & `lyriks-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lyriks"
-version = "0.1.0"
+version = "0.1.1"
 description = "A command line tool to fetch lyrics from Genie"
 authors = [
     { name = "Maxr1998", email = "max@maxr1998.de" },
 ]
 license = { text = "GPLv3" }
 readme = "README.md"
 classifiers = [
```

