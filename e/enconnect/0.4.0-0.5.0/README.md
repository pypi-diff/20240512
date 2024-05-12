# Comparing `tmp/enconnect-0.4.0.tar.gz` & `tmp/enconnect-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enconnect-0.4.0.tar", last modified: Sun May  5 05:18:47 2024, max compression
+gzip compressed data, was "enconnect-0.5.0.tar", last modified: Sun May 12 09:21:44 2024, max compression
```

## Comparing `enconnect-0.4.0.tar` & `enconnect-0.5.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-04-08 22:20:24.000000 enconnect-0.4.0/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       33 2024-04-08 22:21:35.000000 enconnect-0.4.0/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2828 2024-05-05 05:18:47.162314 enconnect-0.4.0/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2417 2024-05-05 05:12:09.000000 enconnect-0.4.0/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.160314 enconnect-0.4.0/enconnect/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 22:22:18.000000 enconnect-0.4.0/enconnect/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/instagram/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      405 2024-04-13 00:00:49.000000 enconnect-0.4.0/enconnect/instagram/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6092 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/instagram/instagram.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      881 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/instagram/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/instagram/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 04:42:12.000000 enconnect-0.4.0/enconnect/instagram/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3314 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/instagram/test/test_instagram.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/philipshue/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:18.000000 enconnect-0.4.0/enconnect/philipshue/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2254 2024-04-14 11:29:01.000000 enconnect-0.4.0/enconnect/philipshue/bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      955 2024-04-14 11:21:24.000000 enconnect-0.4.0/enconnect/philipshue/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/philipshue/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:44.000000 enconnect-0.4.0/enconnect/philipshue/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1773 2024-04-15 09:01:50.000000 enconnect-0.4.0/enconnect/philipshue/test/test_bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 22:21:56.000000 enconnect-0.4.0/enconnect/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/reddit/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      385 2024-04-13 11:18:53.000000 enconnect-0.4.0/enconnect/reddit/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1197 2024-05-05 04:49:10.000000 enconnect-0.4.0/enconnect/reddit/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    11372 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/reddit/reddit.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/reddit/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-13 07:05:56.000000 enconnect-0.4.0/enconnect/reddit/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4478 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/reddit/test/test_reddit.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.161314 enconnect-0.4.0/enconnect/ubiquiti/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:46.000000 enconnect-0.4.0/enconnect/ubiquiti/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1127 2024-04-14 11:21:29.000000 enconnect-0.4.0/enconnect/ubiquiti/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4376 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/ubiquiti/router.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect/ubiquiti/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:52.000000 enconnect-0.4.0/enconnect/ubiquiti/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2199 2024-04-15 09:01:50.000000 enconnect-0.4.0/enconnect/ubiquiti/test/test_router.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect/utils/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      283 2024-04-29 00:13:14.000000 enconnect-0.4.0/enconnect/utils/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     8682 2024-05-05 04:49:10.000000 enconnect-0.4.0/enconnect/utils/http.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect/utils/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-29 00:13:14.000000 enconnect-0.4.0/enconnect/utils/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2996 2024-05-05 04:49:10.000000 enconnect-0.4.0/enconnect/utils/test/test_http.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-05-05 05:13:11.000000 enconnect-0.4.0/enconnect/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect/youtube/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      391 2024-04-12 07:52:09.000000 enconnect-0.4.0/enconnect/youtube/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      879 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/youtube/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect/youtube/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 07:23:02.000000 enconnect-0.4.0/enconnect/youtube/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3446 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/youtube/test/test_youtube.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7638 2024-05-05 05:10:19.000000 enconnect-0.4.0/enconnect/youtube/youtube.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-05 05:18:47.162314 enconnect-0.4.0/enconnect.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2828 2024-05-05 05:18:47.000000 enconnect-0.4.0/enconnect.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1245 2024-05-05 05:18:47.000000 enconnect-0.4.0/enconnect.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-05-05 05:18:47.000000 enconnect-0.4.0/enconnect.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       24 2024-05-05 05:18:47.000000 enconnect-0.4.0/enconnect.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       10 2024-05-05 05:18:47.000000 enconnect-0.4.0/enconnect.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      529 2024-04-08 22:22:47.000000 enconnect-0.4.0/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       24 2024-04-29 00:13:14.000000 enconnect-0.4.0/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      339 2024-05-05 05:18:47.162314 enconnect-0.4.0/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.193423 enconnect-0.5.0/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-04-08 22:20:24.000000 enconnect-0.5.0/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       33 2024-04-08 22:21:35.000000 enconnect-0.5.0/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2856 2024-05-12 09:21:44.193423 enconnect-0.5.0/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2445 2024-05-12 08:29:25.000000 enconnect-0.5.0/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.191424 enconnect-0.5.0/enconnect/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 22:22:18.000000 enconnect-0.5.0/enconnect/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.192423 enconnect-0.5.0/enconnect/instagram/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      405 2024-04-13 00:00:49.000000 enconnect-0.5.0/enconnect/instagram/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6092 2024-05-05 05:10:19.000000 enconnect-0.5.0/enconnect/instagram/instagram.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      881 2024-05-05 05:10:19.000000 enconnect-0.5.0/enconnect/instagram/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.192423 enconnect-0.5.0/enconnect/instagram/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 04:42:12.000000 enconnect-0.5.0/enconnect/instagram/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3314 2024-05-05 05:10:19.000000 enconnect-0.5.0/enconnect/instagram/test/test_instagram.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.192423 enconnect-0.5.0/enconnect/philipshue/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:18.000000 enconnect-0.5.0/enconnect/philipshue/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2254 2024-04-14 11:29:01.000000 enconnect-0.5.0/enconnect/philipshue/bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      955 2024-04-14 11:21:24.000000 enconnect-0.5.0/enconnect/philipshue/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.192423 enconnect-0.5.0/enconnect/philipshue/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:44.000000 enconnect-0.5.0/enconnect/philipshue/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1773 2024-04-15 09:01:50.000000 enconnect-0.5.0/enconnect/philipshue/test/test_bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 22:21:56.000000 enconnect-0.5.0/enconnect/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.192423 enconnect-0.5.0/enconnect/reddit/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      385 2024-04-13 11:18:53.000000 enconnect-0.5.0/enconnect/reddit/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1197 2024-05-05 04:49:10.000000 enconnect-0.5.0/enconnect/reddit/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    11372 2024-05-05 05:10:19.000000 enconnect-0.5.0/enconnect/reddit/reddit.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.192423 enconnect-0.5.0/enconnect/reddit/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-13 07:05:56.000000 enconnect-0.5.0/enconnect/reddit/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4478 2024-05-05 05:10:19.000000 enconnect-0.5.0/enconnect/reddit/test/test_reddit.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.192423 enconnect-0.5.0/enconnect/ubiquiti/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:46.000000 enconnect-0.5.0/enconnect/ubiquiti/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1127 2024-04-14 11:21:29.000000 enconnect-0.5.0/enconnect/ubiquiti/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4376 2024-05-05 05:10:19.000000 enconnect-0.5.0/enconnect/ubiquiti/router.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.193423 enconnect-0.5.0/enconnect/ubiquiti/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:52.000000 enconnect-0.5.0/enconnect/ubiquiti/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2199 2024-04-15 09:01:50.000000 enconnect-0.5.0/enconnect/ubiquiti/test/test_router.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.193423 enconnect-0.5.0/enconnect/utils/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      283 2024-04-29 00:13:14.000000 enconnect-0.5.0/enconnect/utils/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     8682 2024-05-05 04:49:10.000000 enconnect-0.5.0/enconnect/utils/http.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.193423 enconnect-0.5.0/enconnect/utils/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-29 00:13:14.000000 enconnect-0.5.0/enconnect/utils/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2996 2024-05-05 04:49:10.000000 enconnect-0.5.0/enconnect/utils/test/test_http.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-05-12 09:18:48.000000 enconnect-0.5.0/enconnect/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.193423 enconnect-0.5.0/enconnect/youtube/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      445 2024-05-12 09:18:09.000000 enconnect-0.5.0/enconnect/youtube/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      879 2024-05-05 05:10:19.000000 enconnect-0.5.0/enconnect/youtube/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.193423 enconnect-0.5.0/enconnect/youtube/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 07:23:02.000000 enconnect-0.5.0/enconnect/youtube/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5420 2024-05-12 09:18:09.000000 enconnect-0.5.0/enconnect/youtube/test/test_youtube.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    11126 2024-05-12 09:18:09.000000 enconnect-0.5.0/enconnect/youtube/youtube.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-05-12 09:21:44.193423 enconnect-0.5.0/enconnect.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2856 2024-05-12 09:21:44.000000 enconnect-0.5.0/enconnect.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1245 2024-05-12 09:21:44.000000 enconnect-0.5.0/enconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-05-12 09:21:44.000000 enconnect-0.5.0/enconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       24 2024-05-12 09:21:44.000000 enconnect-0.5.0/enconnect.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       10 2024-05-12 09:21:44.000000 enconnect-0.5.0/enconnect.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      529 2024-04-08 22:22:47.000000 enconnect-0.5.0/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       24 2024-04-29 00:13:14.000000 enconnect-0.5.0/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      339 2024-05-12 09:21:44.193423 enconnect-0.5.0/setup.cfg
```

### Comparing `enconnect-0.4.0/LICENSE` & `enconnect-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/PKG-INFO` & `enconnect-0.5.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: enconnect
-Version: 0.4.0
-Summary: Enasis Network Remote Connect
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: encommon
-Requires-Dist: httpx
-Requires-Dist: requests
-
 # Enasis Network Remote Connect
 
 > :children_crossing: This project has not released its first major version.
 
 Functions and classes for connecting to remote services and whatnot.
 
 [![](https://img.shields.io/github/actions/workflow/status/enasisnetwork/enconnect/build.yml?style=flat-square&label=GitHub%20actions)](https://github.com/enasisnetwork/enconnect/actions)<br>
@@ -27,15 +12,16 @@
 
 ## Documentation
 Documentation is on [Read the Docs](https://enconnect.readthedocs.io).
 Should you venture into the sections below you will be able to use the
 `sphinx` recipe to build documention in the `docs/html` directory.
 
 ## Useful and related links
-- https://developers.facebook.com/docs/instagram-basic-display-api/reference/media
+- [Instagram API](https://developers.facebook.com/docs/instagram-basic-display-api/reference/media)
+- [YouTube API](https://developers.google.com/youtube/v3/docs)
 
 ## Installing the package
 Installing stable from the PyPi repository
 ```
 pip install enconnect
 ```
 Installing latest from GitHub repository
@@ -49,40 +35,37 @@
 git clone https://github.com/enasisnetwork/enconnect.git
 ```
 Set up the Python virtual environments expected by the Makefile.
 ```
 make -s venv-create
 ```
 
-### Execute the linters and tests
-The comprehensive approach is to use the `check` recipe. This will stop on
-any failure that is encountered.
-```
-make -s check
-```
-However you can run the linters in a non-blocking mode.
-```
-make -s linters-pass
-```
-And finally run the various tests to validate the code and produce coverage
-information found in the `htmlcov` folder in the root of the project.
-```
-make -s pytest
-```
+## Version management
+:warning: Ensure that no changes are pending.
 
-## Build and upload to PyPi
-Rebuild the environment.
-```
-make -s check-revenv
-```
-Build the package.
-```
-make -s pypackage
-```
-Upload to the test PyPi.
-```
-make -s pypi-upload-test
-```
-Upload to the prod PyPi.
-```
-make -s pypi-upload-prod
-```
+1. Rebuild the environment.
+   ```
+   make -s check-revenv
+   ```
+
+1. Update the [version.txt](enconnect/version.txt) file.
+
+1. Push to the `main` branch.
+
+1. Create [repository](https://github.com/enasisnetwork/enconnect) release.
+
+1. Build the Python package.<br>
+   ```
+   make -s pypackage
+   ```
+
+1. Upload Python package to PyPi test.
+   ```
+   make -s pypi-upload-test
+   ```
+
+1. Upload Python package to PyPi prod.
+   ```
+   make -s pypi-upload-prod
+   ```
+
+1. Update [Read the Docs](https://enconnect.readthedocs.io) documentation.
```

### Comparing `enconnect-0.4.0/enconnect/__init__.py` & `enconnect-0.5.0/enconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/instagram/instagram.py` & `enconnect-0.5.0/enconnect/instagram/instagram.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/instagram/params.py` & `enconnect-0.5.0/enconnect/instagram/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/instagram/test/test_instagram.py` & `enconnect-0.5.0/enconnect/instagram/test/test_instagram.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/philipshue/bridge.py` & `enconnect-0.5.0/enconnect/philipshue/bridge.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/philipshue/params.py` & `enconnect-0.5.0/enconnect/philipshue/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/philipshue/test/test_bridge.py` & `enconnect-0.5.0/enconnect/philipshue/test/test_bridge.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/reddit/params.py` & `enconnect-0.5.0/enconnect/reddit/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/reddit/reddit.py` & `enconnect-0.5.0/enconnect/reddit/reddit.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/reddit/test/test_reddit.py` & `enconnect-0.5.0/enconnect/reddit/test/test_reddit.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/ubiquiti/params.py` & `enconnect-0.5.0/enconnect/ubiquiti/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/ubiquiti/router.py` & `enconnect-0.5.0/enconnect/ubiquiti/router.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/ubiquiti/test/test_router.py` & `enconnect-0.5.0/enconnect/ubiquiti/test/test_router.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/utils/http.py` & `enconnect-0.5.0/enconnect/utils/http.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/utils/test/test_http.py` & `enconnect-0.5.0/enconnect/utils/test/test_http.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/youtube/params.py` & `enconnect-0.5.0/enconnect/youtube/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/enconnect/youtube/test/test_youtube.py` & `enconnect-0.5.0/enconnect/youtube/test/test_youtube.py`

 * *Files 22% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         social)
 
 
     assert social.params is not None
 
 
 
-def test_YouTube_block(
+def test_YouTube_search_block(
     social: YouTube,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
     :param social: Class instance for connecting to service.
     """
@@ -93,15 +93,15 @@
 
     patched = patch(
         'httpx.Client.request')
 
     with patched as mocker:
 
         source = read_text(
-            f'{SAMPLES}/source.json')
+            f'{SAMPLES}/search/source.json')
 
         mocker.side_effect = [
             Response(
                 status_code=200,
                 content=source,
                 request=_REQGET)]
 
@@ -109,15 +109,15 @@
 
         results = (
             social
             .search_block(payload))
 
 
     sample_path = (
-        f'{SAMPLES}/dumped.json')
+        f'{SAMPLES}/search/dumped.json')
 
     sample = load_sample(
         sample_path,
         [x.model_dump()
          for x in results],
         update=ENPYRWS)
 
@@ -126,15 +126,15 @@
         for x in results])
 
     assert sample == expect
 
 
 
 @mark.asyncio
-async def test_YouTube_async(
+async def test_YouTube_search_async(
     social: YouTube,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
     :param social: Class instance for connecting to service.
     """
@@ -143,15 +143,15 @@
     patched = patch(
         'httpx.AsyncClient.request',
         new_callable=AsyncMock)
 
     with patched as mocker:
 
         source = read_text(
-            f'{SAMPLES}/source.json')
+            f'{SAMPLES}/search/source.json')
 
         mocker.side_effect = [
             Response(
                 status_code=200,
                 content=source,
                 request=_REQGET)]
 
@@ -161,15 +161,115 @@
             social
             .search_async(payload))
 
         results = await waited
 
 
     sample_path = (
-        f'{SAMPLES}/dumped.json')
+        f'{SAMPLES}/search/dumped.json')
+
+    sample = load_sample(
+        sample_path,
+        [x.model_dump()
+         for x in results],
+        update=ENPYRWS)
+
+    expect = prep_sample([
+        x.model_dump()
+        for x in results])
+
+    assert sample == expect
+
+
+
+def test_YouTube_videos_block(
+    social: YouTube,
+) -> None:
+    """
+    Perform various tests associated with relevant routines.
+
+    :param social: Class instance for connecting to service.
+    """
+
+
+    patched = patch(
+        'httpx.Client.request')
+
+    with patched as mocker:
+
+        source = read_text(
+            f'{SAMPLES}/videos/source.json')
+
+        mocker.side_effect = [
+            Response(
+                status_code=200,
+                content=source,
+                request=_REQGET)]
+
+        payload = {'id': 'mocked'}
+
+        results = (
+            social
+            .videos_block(payload))
+
+
+    sample_path = (
+        f'{SAMPLES}/videos/dumped.json')
+
+    sample = load_sample(
+        sample_path,
+        [x.model_dump()
+         for x in results],
+        update=ENPYRWS)
+
+    expect = prep_sample([
+        x.model_dump()
+        for x in results])
+
+    assert sample == expect
+
+
+
+@mark.asyncio
+async def test_YouTube_videos_async(
+    social: YouTube,
+) -> None:
+    """
+    Perform various tests associated with relevant routines.
+
+    :param social: Class instance for connecting to service.
+    """
+
+
+    patched = patch(
+        'httpx.AsyncClient.request',
+        new_callable=AsyncMock)
+
+    with patched as mocker:
+
+        source = read_text(
+            f'{SAMPLES}/videos/source.json')
+
+        mocker.side_effect = [
+            Response(
+                status_code=200,
+                content=source,
+                request=_REQGET)]
+
+        payload = {'id': 'mocked'}
+
+        waited = (
+            social
+            .videos_async(payload))
+
+        results = await waited
+
+
+    sample_path = (
+        f'{SAMPLES}/videos/dumped.json')
 
     sample = load_sample(
         sample_path,
         [x.model_dump()
          for x in results],
         update=ENPYRWS)
```

### Comparing `enconnect-0.4.0/enconnect/youtube/youtube.py` & `enconnect-0.5.0/enconnect/youtube/youtube.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,14 +47,24 @@
     'channelId': 'channel',
     'kind': 'kind',
     'playlistId': 'playlist',
     'videoId': 'video'}
 
 
 
+VIDEO_VALUE = {
+    'channelId': 'channel',
+    'channelTitle': 'channel_title',
+    'description': 'about',
+    'publishedAt': 'published',
+    'thumbnails': 'thumbnail',
+    'title': 'title'}
+
+
+
 class YouTubeResult(BaseModel, extra='ignore'):
     """
     Contains information returned from the upstream response.
 
     .. note::
        Fields are not completely documented for this model.
 
@@ -121,14 +131,75 @@
         data['kind'] = data['kind'][8:]
 
 
         super().__init__(**data)
 
 
 
+class YouTubeVideo(BaseModel, extra='ignore'):
+    """
+    Contains information returned from the upstream response.
+
+    .. note::
+       Fields are not completely documented for this model.
+
+    :param data: Keyword arguments passed to Pydantic model.
+        Parameter is picked up by autodoc, please ignore.
+    """
+
+    kind: RESULT_KINDS
+
+    channel: str
+    video: str
+
+    title: str
+    about: str
+    thumbnail: str
+    published: str
+
+
+    def __init__(
+        self,
+        **data: Any,
+    ) -> None:
+        """
+        Initialize instance for class using provided parameters.
+        """
+
+
+        data['video'] = data['id']
+
+
+        video = data['snippet']
+
+        items = VIDEO_VALUE.items()
+
+        for old, new in items:
+
+            value = video.get(old)
+
+            if value is None:
+                continue  # NOCVR
+
+            data[new] = value
+
+
+        if 'thumbnail' in data:
+            data['thumbnail'] = (
+                data['thumbnail']
+                ['high']['url'])
+
+
+        data['kind'] = data['kind'][8:]
+
+
+        super().__init__(**data)
+
+
+
 class YouTube:
     """
     Interact with the cloud service API with various methods.
 
     :param params: Parameters for instantiating the instance.
     """
 
@@ -345,7 +416,104 @@
 
 
         return [
             YouTubeResult(**x)
             for x in fetched['items']
             if x['id']['kind']
             in _RESULT_KINDS]
+
+
+    def videos(
+        # NOCVR
+        self,
+        params: Optional[dict[str, Any]] = None,
+    ) -> list[YouTubeVideo]:
+        """
+        Return the videos from the provided search parameters.
+
+        :param params: Optional parameters included in request.
+        :returns: Results from the provided search parameters.
+        """
+
+        return self.videos_block(params)
+
+
+    def videos_block(
+        self,
+        params: Optional[dict[str, Any]] = None,
+    ) -> list[YouTubeVideo]:
+        """
+        Return the videos from the provided search parameters.
+
+        :param params: Optional parameters included in request.
+        :returns: Results from the provided search parameters.
+        """
+
+        params = dict(params or {})
+
+
+        if 'maxResults' not in params:
+            params['maxResults'] = 50
+
+        if 'order' not in params:
+            params['order'] = 'date'
+
+        if 'part' not in params:
+            params['part'] = 'snippet,id'
+
+
+        request = self.request_block
+
+        response = request(
+            'get', 'videos', params)
+
+        response.raise_for_status()
+
+        fetched = response.json()
+
+        assert isinstance(fetched, dict)
+
+
+        return [
+            YouTubeVideo(**x)
+            for x in fetched['items']]
+
+
+    async def videos_async(
+        self,
+        params: Optional[dict[str, Any]] = None,
+    ) -> list[YouTubeVideo]:
+        """
+        Return the videos from the provided search parameters.
+
+        :param params: Optional parameters included in request.
+        :returns: Results from the provided search parameters.
+        """
+
+        params = dict(params or {})
+
+
+        if 'maxResults' not in params:
+            params['maxResults'] = 50
+
+        if 'order' not in params:
+            params['order'] = 'date'
+
+        if 'part' not in params:
+            params['part'] = 'snippet,id'
+
+
+        request = self.request_async
+
+        response = await request(
+            'get', 'videos', params)
+
+        response.raise_for_status()
+
+        fetched = response.json()
+
+        assert isinstance(fetched, dict)
+
+
+        return [
+            YouTubeVideo(**x)
+            for x in fetched['items']]
```

### Comparing `enconnect-0.4.0/enconnect.egg-info/SOURCES.txt` & `enconnect-0.5.0/enconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `enconnect-0.4.0/pyproject.toml` & `enconnect-0.5.0/pyproject.toml`

 * *Files identical despite different names*

