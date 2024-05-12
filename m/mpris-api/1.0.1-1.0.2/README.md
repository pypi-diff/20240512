# Comparing `tmp/mpris-api-1.0.1.tar.gz` & `tmp/mpris-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pawel/workspace/repo/mpris-api/dist/.tmp-2us7dbuc/mpris-api-1.0.1.tar", last modified: Sun May 12 12:14:57 2024, max compression
+gzip compressed data, was "/home/pawel/workspace/repo/mpris-api/dist/.tmp-ghte94w5/mpris-api-1.0.2.tar", last modified: Sun May 12 15:21:26 2024, max compression
```

## Comparing `mpris-api-1.0.1.tar` & `mpris-api-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 12:14:57.000000 mpris-api-1.0.1/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1072 2024-04-06 19:49:23.000000 mpris-api-1.0.1/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       69 2024-05-12 07:49:24.000000 mpris-api-1.0.1/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-12 12:14:57.000000 mpris-api-1.0.1/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2434 2024-05-12 12:01:51.000000 mpris-api-1.0.1/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/mpris_api/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5218 2024-05-12 11:28:20.000000 mpris-api-1.0.1/pkg/mpris_api/MprisService.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1836 2024-05-12 09:34:58.000000 mpris-api-1.0.1/pkg/mpris_api/MprisUpdateNotifier.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-05-12 12:07:59.000000 mpris-api-1.0.1/pkg/mpris_api/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/mpris_api/adapter/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      835 2024-05-12 09:32:33.000000 mpris-api-1.0.1/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2151 2024-05-12 08:39:29.000000 mpris-api-1.0.1/pkg/mpris_api/adapter/IMprisAdapterPlayer.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      945 2024-05-11 08:53:04.000000 mpris-api-1.0.1/pkg/mpris_api/adapter/IMprisAdapterRoot.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      789 2024-05-12 11:03:06.000000 mpris-api-1.0.1/pkg/mpris_api/adapter/IMprisAdapterTrackList.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.0.1/pkg/mpris_api/adapter/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/mpris_api/common/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1485 2024-05-12 11:19:02.000000 mpris-api-1.0.1/pkg/mpris_api/common/DbusObject.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3678 2024-05-12 11:46:26.000000 mpris-api-1.0.1/pkg/mpris_api/common/DbusObjectSpec.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      483 2024-05-12 09:42:57.000000 mpris-api-1.0.1/pkg/mpris_api/common/DbusType.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 18:20:04.000000 mpris-api-1.0.1/pkg/mpris_api/common/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      209 2024-05-12 09:55:02.000000 mpris-api-1.0.1/pkg/mpris_api/common/dbusDecorators.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/mpris_api/interface/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1429 2024-05-12 09:12:24.000000 mpris-api-1.0.1/pkg/mpris_api/interface/MprisInterfaceBase.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2759 2024-05-12 10:04:49.000000 mpris-api-1.0.1/pkg/mpris_api/interface/MprisInterfacePlayLists.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     7286 2024-05-12 11:21:27.000000 mpris-api-1.0.1/pkg/mpris_api/interface/MprisInterfacePlayer.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3437 2024-05-12 09:58:10.000000 mpris-api-1.0.1/pkg/mpris_api/interface/MprisInterfaceRoot.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3439 2024-05-12 11:21:27.000000 mpris-api-1.0.1/pkg/mpris_api/interface/MprisInterfaceTrackList.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.0.1/pkg/mpris_api/interface/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/mpris_api/model/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      254 2024-05-12 11:21:27.000000 mpris-api-1.0.1/pkg/mpris_api/model/MprisConstant.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      201 2024-05-11 07:59:37.000000 mpris-api-1.0.1/pkg/mpris_api/model/MprisLoopStatus.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2576 2024-05-12 11:11:07.000000 mpris-api-1.0.1/pkg/mpris_api/model/MprisMetaData.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      211 2024-05-11 07:59:57.000000 mpris-api-1.0.1/pkg/mpris_api/model/MprisPlaybackStatus.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      656 2024-05-12 10:00:54.000000 mpris-api-1.0.1/pkg/mpris_api/model/MprisPlaylist.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      316 2024-05-11 12:27:27.000000 mpris-api-1.0.1/pkg/mpris_api/model/MprisPlaylistOrdering.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      343 2024-05-12 11:22:22.000000 mpris-api-1.0.1/pkg/mpris_api/model/MprisTrack.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 21:44:38.000000 mpris-api-1.0.1/pkg/mpris_api/model/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2024-05-12 07:49:45.000000 mpris-api-1.0.1/pkg/mpris_api/py.typed
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/mpris_api.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/mpris_api.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1291 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/mpris_api.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/mpris_api.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       10 2024-05-12 12:14:57.000000 mpris-api-1.0.1/pkg/mpris_api.egg-info/top_level.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)      852 2024-05-12 07:55:14.000000 mpris-api-1.0.1/pyproject.toml
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-05-12 12:14:57.000000 mpris-api-1.0.1/setup.cfg
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:21:26.000000 mpris-api-1.0.2/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1072 2024-04-06 19:49:23.000000 mpris-api-1.0.2/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      102 2024-05-12 15:19:56.000000 mpris-api-1.0.2/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-12 15:21:26.000000 mpris-api-1.0.2/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2434 2024-05-12 12:01:51.000000 mpris-api-1.0.2/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/mpris_api/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5218 2024-05-12 11:28:20.000000 mpris-api-1.0.2/pkg/mpris_api/MprisService.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1836 2024-05-12 09:34:58.000000 mpris-api-1.0.2/pkg/mpris_api/MprisUpdateNotifier.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-05-12 15:18:54.000000 mpris-api-1.0.2/pkg/mpris_api/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/mpris_api/adapter/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      835 2024-05-12 09:32:33.000000 mpris-api-1.0.2/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2151 2024-05-12 08:39:29.000000 mpris-api-1.0.2/pkg/mpris_api/adapter/IMprisAdapterPlayer.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      945 2024-05-11 08:53:04.000000 mpris-api-1.0.2/pkg/mpris_api/adapter/IMprisAdapterRoot.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      789 2024-05-12 11:03:06.000000 mpris-api-1.0.2/pkg/mpris_api/adapter/IMprisAdapterTrackList.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.0.2/pkg/mpris_api/adapter/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/mpris_api/common/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1485 2024-05-12 11:19:02.000000 mpris-api-1.0.2/pkg/mpris_api/common/DbusObject.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3678 2024-05-12 11:46:26.000000 mpris-api-1.0.2/pkg/mpris_api/common/DbusObjectSpec.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      483 2024-05-12 09:42:57.000000 mpris-api-1.0.2/pkg/mpris_api/common/DbusType.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 18:20:04.000000 mpris-api-1.0.2/pkg/mpris_api/common/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      209 2024-05-12 09:55:02.000000 mpris-api-1.0.2/pkg/mpris_api/common/dbusDecorators.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/mpris_api/interface/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1429 2024-05-12 09:12:24.000000 mpris-api-1.0.2/pkg/mpris_api/interface/MprisInterfaceBase.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2759 2024-05-12 10:04:49.000000 mpris-api-1.0.2/pkg/mpris_api/interface/MprisInterfacePlayLists.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     7286 2024-05-12 11:21:27.000000 mpris-api-1.0.2/pkg/mpris_api/interface/MprisInterfacePlayer.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3437 2024-05-12 09:58:10.000000 mpris-api-1.0.2/pkg/mpris_api/interface/MprisInterfaceRoot.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3439 2024-05-12 11:21:27.000000 mpris-api-1.0.2/pkg/mpris_api/interface/MprisInterfaceTrackList.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 17:49:43.000000 mpris-api-1.0.2/pkg/mpris_api/interface/__init__.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/mpris_api/model/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      254 2024-05-12 11:21:27.000000 mpris-api-1.0.2/pkg/mpris_api/model/MprisConstant.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      201 2024-05-11 07:59:37.000000 mpris-api-1.0.2/pkg/mpris_api/model/MprisLoopStatus.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2576 2024-05-12 11:11:07.000000 mpris-api-1.0.2/pkg/mpris_api/model/MprisMetaData.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      211 2024-05-11 07:59:57.000000 mpris-api-1.0.2/pkg/mpris_api/model/MprisPlaybackStatus.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      656 2024-05-12 10:00:54.000000 mpris-api-1.0.2/pkg/mpris_api/model/MprisPlaylist.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      316 2024-05-11 12:27:27.000000 mpris-api-1.0.2/pkg/mpris_api/model/MprisPlaylistOrdering.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      343 2024-05-12 11:22:22.000000 mpris-api-1.0.2/pkg/mpris_api/model/MprisTrack.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-05-09 21:44:38.000000 mpris-api-1.0.2/pkg/mpris_api/model/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2024-05-12 07:49:45.000000 mpris-api-1.0.2/pkg/mpris_api/py.typed
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/mpris_api.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     3053 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/mpris_api.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1316 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/mpris_api.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/mpris_api.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       10 2024-05-12 15:21:26.000000 mpris-api-1.0.2/pkg/mpris_api.egg-info/top_level.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      905 2024-05-12 15:18:08.000000 mpris-api-1.0.2/pyproject.toml
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-05-12 15:21:26.000000 mpris-api-1.0.2/requirements/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       51 2024-05-12 12:10:54.000000 mpris-api-1.0.2/requirements/release.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-05-12 15:21:26.000000 mpris-api-1.0.2/setup.cfg
```

### Comparing `mpris-api-1.0.1/LICENSE.txt` & `mpris-api-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/PKG-INFO` & `mpris-api-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpris-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Make your multimedia app discoverable by linux desktop.
 Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
 Project-URL: Repository, https://bitbucket.org/massultidev/mpris-api
 Keywords: mpris,player,multimedia,linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mpris-api-1.0.1/README.md` & `mpris-api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/MprisService.py` & `mpris-api-1.0.2/pkg/mpris_api/MprisService.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/MprisUpdateNotifier.py` & `mpris-api-1.0.2/pkg/mpris_api/MprisUpdateNotifier.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py` & `mpris-api-1.0.2/pkg/mpris_api/adapter/IMprisAdapterPlayLists.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/adapter/IMprisAdapterPlayer.py` & `mpris-api-1.0.2/pkg/mpris_api/adapter/IMprisAdapterPlayer.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/adapter/IMprisAdapterRoot.py` & `mpris-api-1.0.2/pkg/mpris_api/adapter/IMprisAdapterRoot.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/adapter/IMprisAdapterTrackList.py` & `mpris-api-1.0.2/pkg/mpris_api/adapter/IMprisAdapterTrackList.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/common/DbusObject.py` & `mpris-api-1.0.2/pkg/mpris_api/common/DbusObject.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/common/DbusObjectSpec.py` & `mpris-api-1.0.2/pkg/mpris_api/common/DbusObjectSpec.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/interface/MprisInterfaceBase.py` & `mpris-api-1.0.2/pkg/mpris_api/interface/MprisInterfaceBase.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/interface/MprisInterfacePlayLists.py` & `mpris-api-1.0.2/pkg/mpris_api/interface/MprisInterfacePlayLists.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/interface/MprisInterfacePlayer.py` & `mpris-api-1.0.2/pkg/mpris_api/interface/MprisInterfacePlayer.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/interface/MprisInterfaceRoot.py` & `mpris-api-1.0.2/pkg/mpris_api/interface/MprisInterfaceRoot.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/interface/MprisInterfaceTrackList.py` & `mpris-api-1.0.2/pkg/mpris_api/interface/MprisInterfaceTrackList.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/model/MprisMetaData.py` & `mpris-api-1.0.2/pkg/mpris_api/model/MprisMetaData.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api/model/MprisPlaylist.py` & `mpris-api-1.0.2/pkg/mpris_api/model/MprisPlaylist.py`

 * *Files identical despite different names*

### Comparing `mpris-api-1.0.1/pkg/mpris_api.egg-info/PKG-INFO` & `mpris-api-1.0.2/pkg/mpris_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpris-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: Make your multimedia app discoverable by linux desktop.
 Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
 Project-URL: Repository, https://bitbucket.org/massultidev/mpris-api
 Keywords: mpris,player,multimedia,linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mpris-api-1.0.1/pkg/mpris_api.egg-info/SOURCES.txt` & `mpris-api-1.0.2/pkg/mpris_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 pkg/mpris_api/model/MprisConstant.py
 pkg/mpris_api/model/MprisLoopStatus.py
 pkg/mpris_api/model/MprisMetaData.py
 pkg/mpris_api/model/MprisPlaybackStatus.py
 pkg/mpris_api/model/MprisPlaylist.py
 pkg/mpris_api/model/MprisPlaylistOrdering.py
 pkg/mpris_api/model/MprisTrack.py
-pkg/mpris_api/model/__init__.py
+pkg/mpris_api/model/__init__.py
+requirements/release.txt
```

### Comparing `mpris-api-1.0.1/pyproject.toml` & `mpris-api-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -29,7 +29,8 @@
 Repository = 'https://bitbucket.org/massultidev/mpris-api'
 
 [tool.setuptools]
 package-dir = { '' = 'pkg' }
 
 [tool.setuptools.dynamic]
 version = { attr = 'mpris_api.__version__' }
+dependencies = { file = 'requirements/release.txt' }
```

