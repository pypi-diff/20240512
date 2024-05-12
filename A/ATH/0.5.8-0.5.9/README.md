# Comparing `tmp/ATH-0.5.8.tar.gz` & `tmp/ATH-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ATH-0.5.8.tar", last modified: Tue May  7 09:51:20 2024, max compression
+gzip compressed data, was "ATH-0.5.9.tar", last modified: Sun May 12 17:24:41 2024, max compression
```

## Comparing `ATH-0.5.8.tar` & `ATH-0.5.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 09:51:20.538580 ATH-0.5.8/
-drwxrwxrwx   0        0        0        0 2024-05-07 09:51:20.512020 ATH-0.5.8/ATH/
--rw-rw-rw-   0        0        0     1287 2024-03-03 12:52:16.000000 ATH-0.5.8/ATH/DB_read.py
--rw-rw-rw-   0        0        0      914 2024-03-02 12:38:15.000000 ATH-0.5.8/ATH/DB_send.py
--rw-rw-rw-   0        0        0      440 2024-04-27 18:54:21.000000 ATH-0.5.8/ATH/__init__.py
--rw-rw-rw-   0        0        0      172 2024-03-16 15:51:41.000000 ATH-0.5.8/ATH/abc123_2.py
--rw-rw-rw-   0        0        0      125 2024-03-01 17:00:39.000000 ATH-0.5.8/ATH/arithmetic_average.py
--rw-rw-rw-   0        0        0      528 2024-03-07 17:24:38.000000 ATH-0.5.8/ATH/calculator.py
--rw-rw-rw-   0        0        0      196 2024-03-05 13:23:48.000000 ATH-0.5.8/ATH/env.py
--rw-rw-rw-   0        0        0      368 2024-03-03 20:21:14.000000 ATH-0.5.8/ATH/get_current_time.py
--rw-rw-rw-   0        0        0     1791 2024-05-07 09:49:53.000000 ATH-0.5.8/ATH/owl.py
--rw-rw-rw-   0        0        0      347 2024-03-07 15:18:29.000000 ATH-0.5.8/ATH/qr.py
--rw-rw-rw-   0        0        0      430 2024-02-29 15:58:56.000000 ATH-0.5.8/ATH/safe.py
--rw-rw-rw-   0        0        0      113 2024-02-28 18:40:56.000000 ATH-0.5.8/ATH/scr_shot.py
--rw-rw-rw-   0        0        0      312 2024-03-03 17:45:47.000000 ATH-0.5.8/ATH/scr_shot_telegram.py
--rw-rw-rw-   0        0        0      212 2024-04-16 17:22:17.000000 ATH-0.5.8/ATH/singed.py
--rw-rw-rw-   0        0        0       96 2024-02-29 13:36:04.000000 ATH-0.5.8/ATH/sq_root.py
--rw-rw-rw-   0        0        0      167 2024-04-16 15:53:44.000000 ATH-0.5.8/ATH/telegram.py
--rw-rw-rw-   0        0        0      486 2024-05-06 15:53:19.000000 ATH-0.5.8/ATH/tts.py
--rw-rw-rw-   0        0        0       58 2024-03-03 20:32:05.000000 ATH-0.5.8/ATH/wait.py
--rw-rw-rw-   0        0        0       78 2024-03-06 13:59:40.000000 ATH-0.5.8/ATH/write.py
-drwxrwxrwx   0        0        0        0 2024-05-07 09:51:20.536446 ATH-0.5.8/ATH.egg-info/
--rw-rw-rw-   0        0        0      466 2024-05-07 09:51:20.000000 ATH-0.5.8/ATH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-05-07 09:51:20.000000 ATH-0.5.8/ATH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 09:51:20.000000 ATH-0.5.8/ATH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      140 2024-05-07 09:51:20.000000 ATH-0.5.8/ATH.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-07 09:51:20.000000 ATH-0.5.8/ATH.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      466 2024-05-07 09:51:20.537569 ATH-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-07 09:51:20.540385 ATH-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0      423 2024-05-07 09:51:15.000000 ATH-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 17:24:41.876376 ATH-0.5.9/
+drwxrwxrwx   0        0        0        0 2024-05-12 17:24:41.853289 ATH-0.5.9/ATH/
+-rw-rw-rw-   0        0        0     1287 2024-03-03 12:52:16.000000 ATH-0.5.9/ATH/DB_read.py
+-rw-rw-rw-   0        0        0      914 2024-03-02 12:38:15.000000 ATH-0.5.9/ATH/DB_send.py
+-rw-rw-rw-   0        0        0      462 2024-05-12 16:21:48.000000 ATH-0.5.9/ATH/__init__.py
+-rw-rw-rw-   0        0        0      172 2024-03-16 15:51:41.000000 ATH-0.5.9/ATH/abc123_2.py
+-rw-rw-rw-   0        0        0      125 2024-03-01 17:00:39.000000 ATH-0.5.9/ATH/arithmetic_average.py
+-rw-rw-rw-   0        0        0      528 2024-03-07 17:24:38.000000 ATH-0.5.9/ATH/calculator.py
+-rw-rw-rw-   0        0        0      196 2024-03-05 13:23:48.000000 ATH-0.5.9/ATH/env.py
+-rw-rw-rw-   0        0        0      368 2024-03-03 20:21:14.000000 ATH-0.5.9/ATH/get_current_time.py
+-rw-rw-rw-   0        0        0      984 2024-05-12 17:23:48.000000 ATH-0.5.9/ATH/gmail.py
+-rw-rw-rw-   0        0        0     1791 2024-05-07 09:49:53.000000 ATH-0.5.9/ATH/owl.py
+-rw-rw-rw-   0        0        0      347 2024-03-07 15:18:29.000000 ATH-0.5.9/ATH/qr.py
+-rw-rw-rw-   0        0        0      430 2024-02-29 15:58:56.000000 ATH-0.5.9/ATH/safe.py
+-rw-rw-rw-   0        0        0      113 2024-02-28 18:40:56.000000 ATH-0.5.9/ATH/scr_shot.py
+-rw-rw-rw-   0        0        0      312 2024-03-03 17:45:47.000000 ATH-0.5.9/ATH/scr_shot_telegram.py
+-rw-rw-rw-   0        0        0      212 2024-04-16 17:22:17.000000 ATH-0.5.9/ATH/singed.py
+-rw-rw-rw-   0        0        0       96 2024-02-29 13:36:04.000000 ATH-0.5.9/ATH/sq_root.py
+-rw-rw-rw-   0        0        0      167 2024-04-16 15:53:44.000000 ATH-0.5.9/ATH/telegram.py
+-rw-rw-rw-   0        0        0      486 2024-05-06 15:53:19.000000 ATH-0.5.9/ATH/tts.py
+-rw-rw-rw-   0        0        0       58 2024-03-03 20:32:05.000000 ATH-0.5.9/ATH/wait.py
+-rw-rw-rw-   0        0        0       78 2024-03-06 13:59:40.000000 ATH-0.5.9/ATH/write.py
+drwxrwxrwx   0        0        0        0 2024-05-12 17:24:41.875355 ATH-0.5.9/ATH.egg-info/
+-rw-rw-rw-   0        0        0      466 2024-05-12 17:24:41.000000 ATH-0.5.9/ATH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2024-05-12 17:24:41.000000 ATH-0.5.9/ATH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 17:24:41.000000 ATH-0.5.9/ATH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      140 2024-05-12 17:24:41.000000 ATH-0.5.9/ATH.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-12 17:24:41.000000 ATH-0.5.9/ATH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      466 2024-05-12 17:24:41.876376 ATH-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-12 17:24:41.876376 ATH-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      423 2024-05-12 17:24:10.000000 ATH-0.5.9/setup.py
```

### Comparing `ATH-0.5.8/ATH/DB_read.py` & `ATH-0.5.9/ATH/DB_read.py`

 * *Files identical despite different names*

### Comparing `ATH-0.5.8/ATH/DB_send.py` & `ATH-0.5.9/ATH/DB_send.py`

 * *Files identical despite different names*

### Comparing `ATH-0.5.8/ATH/calculator.py` & `ATH-0.5.9/ATH/calculator.py`

 * *Files identical despite different names*

### Comparing `ATH-0.5.8/ATH/owl.py` & `ATH-0.5.9/ATH/owl.py`

 * *Files identical despite different names*

