# Comparing `tmp/webflask-0.2.tar.gz` & `tmp/webflask-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webflask-0.2.tar", last modified: Sun May 12 14:50:23 2024, max compression
+gzip compressed data, was "webflask-0.2.1.tar", last modified: Sun May 12 15:02:09 2024, max compression
```

## Comparing `webflask-0.2.tar` & `webflask-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 14:50:23.492029 webflask-0.2/
--rw-rw-rw-   0        0        0       53 2024-05-12 14:50:23.488025 webflask-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 14:50:23.492029 webflask-0.2/setup.cfg
--rw-rw-rw-   0        0        0      337 2024-05-12 14:50:04.000000 webflask-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:50:23.482008 webflask-0.2/webflask.egg-info/
--rw-rw-rw-   0        0        0       53 2024-05-12 14:50:23.000000 webflask-0.2/webflask.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-05-12 14:50:23.000000 webflask-0.2/webflask.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 14:50:23.000000 webflask-0.2/webflask.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 14:50:23.000000 webflask-0.2/webflask.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 15:02:09.160667 webflask-0.2.1/
+-rw-rw-rw-   0        0        0       55 2024-05-12 15:02:09.158662 webflask-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-12 14:04:29.000000 webflask-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 15:02:09.160667 webflask-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      336 2024-05-12 15:01:59.000000 webflask-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:02:09.106397 webflask-0.2.1/webflask/
+-rw-rw-rw-   0        0        0      721 2024-05-12 12:55:59.000000 webflask-0.2.1/webflask/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:02:09.155508 webflask-0.2.1/webflask.egg-info/
+-rw-rw-rw-   0        0        0       55 2024-05-12 15:02:08.000000 webflask-0.2.1/webflask.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2024-05-12 15:02:08.000000 webflask-0.2.1/webflask.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 15:02:08.000000 webflask-0.2.1/webflask.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 15:02:08.000000 webflask-0.2.1/webflask.egg-info/top_level.txt
```

