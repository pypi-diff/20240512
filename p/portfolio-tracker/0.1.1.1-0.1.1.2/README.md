# Comparing `tmp/portfolio_tracker-0.1.1.1.tar.gz` & `tmp/portfolio_tracker-0.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_tracker-0.1.1.1.tar", last modified: Sun May 12 10:12:55 2024, max compression
+gzip compressed data, was "portfolio_tracker-0.1.1.2.tar", last modified: Sun May 12 11:14:55 2024, max compression
```

## Comparing `portfolio_tracker-0.1.1.1.tar` & `portfolio_tracker-0.1.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 10:12:55.833761 portfolio_tracker-0.1.1.1/
--rw-rw-rw-   0        0        0      350 2024-05-12 10:12:55.832761 portfolio_tracker-0.1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-12 10:12:55.827760 portfolio_tracker-0.1.1.1/portfolio_tracker/
--rw-rw-rw-   0        0        0      129 2024-05-12 10:12:51.000000 portfolio_tracker-0.1.1.1/portfolio_tracker/__init__.py
--rw-rw-rw-   0        0        0    17652 2024-05-12 09:30:40.000000 portfolio_tracker-0.1.1.1/portfolio_tracker/manager.py
--rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.1.1.1/portfolio_tracker/price_repo.py
--rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.1.1.1/portfolio_tracker/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 10:12:55.831761 portfolio_tracker-0.1.1.1/portfolio_tracker.egg-info/
--rw-rw-rw-   0        0        0      350 2024-05-12 10:12:55.000000 portfolio_tracker-0.1.1.1/portfolio_tracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2024-05-12 10:12:55.000000 portfolio_tracker-0.1.1.1/portfolio_tracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 10:12:55.000000 portfolio_tracker-0.1.1.1/portfolio_tracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-12 10:12:55.000000 portfolio_tracker-0.1.1.1/portfolio_tracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-12 10:12:55.000000 portfolio_tracker-0.1.1.1/portfolio_tracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 10:12:55.833761 portfolio_tracker-0.1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-12 10:12:51.000000 portfolio_tracker-0.1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:14:55.267970 portfolio_tracker-0.1.1.2/
+-rw-rw-rw-   0        0        0     3368 2024-05-12 11:14:55.266377 portfolio_tracker-0.1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2906 2024-05-12 09:23:49.000000 portfolio_tracker-0.1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 11:14:55.253406 portfolio_tracker-0.1.1.2/portfolio_tracker/
+-rw-rw-rw-   0        0        0      154 2024-05-12 10:43:36.000000 portfolio_tracker-0.1.1.2/portfolio_tracker/__init__.py
+-rw-rw-rw-   0        0        0    17652 2024-05-12 09:30:40.000000 portfolio_tracker-0.1.1.2/portfolio_tracker/manager.py
+-rw-rw-rw-   0        0        0     4655 2024-05-12 09:13:01.000000 portfolio_tracker-0.1.1.2/portfolio_tracker/price_repo.py
+-rw-rw-rw-   0        0        0     4118 2024-05-12 09:07:54.000000 portfolio_tracker-0.1.1.2/portfolio_tracker/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:14:55.264406 portfolio_tracker-0.1.1.2/portfolio_tracker.egg-info/
+-rw-rw-rw-   0        0        0     3368 2024-05-12 11:14:55.000000 portfolio_tracker-0.1.1.2/portfolio_tracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2024-05-12 11:14:55.000000 portfolio_tracker-0.1.1.2/portfolio_tracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 11:14:55.000000 portfolio_tracker-0.1.1.2/portfolio_tracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-12 11:14:55.000000 portfolio_tracker-0.1.1.2/portfolio_tracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-12 11:14:55.000000 portfolio_tracker-0.1.1.2/portfolio_tracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 11:14:55.267970 portfolio_tracker-0.1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      906 2024-05-12 11:14:47.000000 portfolio_tracker-0.1.1.2/setup.py
```

### Comparing `portfolio_tracker-0.1.1.1/portfolio_tracker/manager.py` & `portfolio_tracker-0.1.1.2/portfolio_tracker/manager.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.1.1/portfolio_tracker/price_repo.py` & `portfolio_tracker-0.1.1.2/portfolio_tracker/price_repo.py`

 * *Files identical despite different names*

### Comparing `portfolio_tracker-0.1.1.1/portfolio_tracker/utils.py` & `portfolio_tracker-0.1.1.2/portfolio_tracker/utils.py`

 * *Files identical despite different names*

