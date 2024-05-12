# Comparing `tmp/rootdir-0.1.0.tar.gz` & `tmp/rootdir-0.1.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootdir-0.1.0.tar", last modified: Sun May 12 15:53:57 2024, max compression
+gzip compressed data, was "rootdir-0.1.2.post1.tar", last modified: Sun May 12 16:36:01 2024, max compression
```

## Comparing `rootdir-0.1.0.tar` & `rootdir-0.1.2.post1.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 15:53:57.020949 rootdir-0.1.0/
--rw-rw-rw-   0        0        0      351 2024-05-12 15:53:57.019949 rootdir-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      112 2024-05-11 07:40:55.000000 rootdir-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 15:53:57.011951 rootdir-0.1.0/rootdir.egg-info/
--rw-rw-rw-   0        0        0      351 2024-05-12 15:53:56.000000 rootdir-0.1.0/rootdir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-05-12 15:53:56.000000 rootdir-0.1.0/rootdir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 15:53:56.000000 rootdir-0.1.0/rootdir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-12 15:53:56.000000 rootdir-0.1.0/rootdir.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 15:53:57.020949 rootdir-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      479 2024-05-12 15:53:47.000000 rootdir-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 15:53:57.016959 rootdir-0.1.0/src/
--rw-rw-rw-   0        0        0      503 2024-05-12 15:53:29.000000 rootdir-0.1.0/src/RootDir.py
--rw-rw-rw-   0        0        0        0 2024-05-11 07:37:50.000000 rootdir-0.1.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:36:01.779822 rootdir-0.1.2.post1/
+-rw-rw-rw-   0        0        0      666 2024-05-12 16:36:01.778823 rootdir-0.1.2.post1/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-12 16:03:46.000000 rootdir-0.1.2.post1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:36:01.779822 rootdir-0.1.2.post1/setup.cfg
+-rw-rw-rw-   0        0        0      472 2024-05-12 16:35:52.000000 rootdir-0.1.2.post1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:36:01.757821 rootdir-0.1.2.post1/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 16:36:01.776822 rootdir-0.1.2.post1/src/rootdir.egg-info/
+-rw-rw-rw-   0        0        0      666 2024-05-12 16:36:01.000000 rootdir-0.1.2.post1/src/rootdir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2024-05-12 16:36:01.000000 rootdir-0.1.2.post1/src/rootdir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:36:01.000000 rootdir-0.1.2.post1/src/rootdir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:36:01.000000 rootdir-0.1.2.post1/src/rootdir.egg-info/top_level.txt
```

