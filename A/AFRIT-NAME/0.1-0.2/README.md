# Comparing `tmp/AFRIT_NAME-0.1.tar.gz` & `tmp/AFRIT_NAME-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AFRIT_NAME-0.1.tar", last modified: Sun May 12 00:15:02 2024, max compression
+gzip compressed data, was "AFRIT_NAME-0.2.tar", last modified: Sun May 12 00:48:15 2024, max compression
```

## Comparing `AFRIT_NAME-0.1.tar` & `AFRIT_NAME-0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 00:15:02.254162 AFRIT_NAME-0.1/
-drwxrwxrwx   0        0        0        0 2024-05-12 00:15:02.245189 AFRIT_NAME-0.1/AFRIT_NAME.egg-info/
--rw-rw-rw-   0        0        0      345 2024-05-12 00:15:02.000000 AFRIT_NAME-0.1/AFRIT_NAME.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-12 00:15:02.000000 AFRIT_NAME-0.1/AFRIT_NAME.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 00:15:02.000000 AFRIT_NAME-0.1/AFRIT_NAME.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-12 00:15:02.000000 AFRIT_NAME-0.1/AFRIT_NAME.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       31 2024-03-26 01:45:26.000000 AFRIT_NAME-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      345 2024-05-12 00:15:02.253163 AFRIT_NAME-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-12 00:15:02.252164 AFRIT_NAME-0.1/name_afrit/
--rw-rw-rw-   0        0        0      680 2024-05-11 23:59:01.000000 AFRIT_NAME-0.1/name_afrit/OS.py
--rw-rw-rw-   0        0        0      394 2024-05-12 00:04:11.000000 AFRIT_NAME-0.1/name_afrit/__init__.py
--rw-rw-rw-   0        0        0      721 2024-05-12 00:10:29.000000 AFRIT_NAME-0.1/name_afrit/momo.py
--rw-rw-rw-   0        0        0       42 2024-05-12 00:15:02.255162 AFRIT_NAME-0.1/setup.cfg
--rw-rw-rw-   0        0        0      348 2024-05-12 00:10:27.000000 AFRIT_NAME-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 00:48:15.480927 AFRIT_NAME-0.2/
+drwxrwxrwx   0        0        0        0 2024-05-12 00:48:15.472359 AFRIT_NAME-0.2/AFRIT_NAME.egg-info/
+-rw-rw-rw-   0        0        0      345 2024-05-12 00:48:15.000000 AFRIT_NAME-0.2/AFRIT_NAME.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-05-12 00:48:15.000000 AFRIT_NAME-0.2/AFRIT_NAME.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 00:48:15.000000 AFRIT_NAME-0.2/AFRIT_NAME.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-12 00:48:15.000000 AFRIT_NAME-0.2/AFRIT_NAME.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       31 2024-03-26 01:45:26.000000 AFRIT_NAME-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      345 2024-05-12 00:48:15.479922 AFRIT_NAME-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-12 00:48:15.477353 AFRIT_NAME-0.2/name_afrit/
+-rw-rw-rw-   0        0        0      680 2024-05-11 23:59:01.000000 AFRIT_NAME-0.2/name_afrit/OS.py
+-rw-rw-rw-   0        0        0      258 2024-05-12 00:47:53.000000 AFRIT_NAME-0.2/name_afrit/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-12 00:48:15.480927 AFRIT_NAME-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      348 2024-05-12 00:47:46.000000 AFRIT_NAME-0.2/setup.py
```

### Comparing `AFRIT_NAME-0.1/name_afrit/OS.py` & `AFRIT_NAME-0.2/name_afrit/OS.py`

 * *Files identical despite different names*

