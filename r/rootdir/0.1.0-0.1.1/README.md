# Comparing `tmp/rootdir-0.1.0.tar.gz` & `tmp/rootdir-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rootdir-0.1.0.tar", last modified: Sun May 12 15:53:57 2024, max compression
+gzip compressed data, was "rootdir-0.1.1.tar", last modified: Sun May 12 16:14:31 2024, max compression
```

## Comparing `rootdir-0.1.0.tar` & `rootdir-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
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
+drwxrwxrwx   0        0        0        0 2024-05-12 16:14:30.999845 rootdir-0.1.1/
+-rw-rw-rw-   0        0        0      660 2024-05-12 16:14:30.998846 rootdir-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-12 16:03:46.000000 rootdir-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 16:14:30.993844 rootdir-0.1.1/rootdir.egg-info/
+-rw-rw-rw-   0        0        0      660 2024-05-12 16:14:30.000000 rootdir-0.1.1/rootdir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2024-05-12 16:14:30.000000 rootdir-0.1.1/rootdir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:14:30.000000 rootdir-0.1.1/rootdir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:14:30.000000 rootdir-0.1.1/rootdir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:14:31.000844 rootdir-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      482 2024-05-12 16:13:21.000000 rootdir-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:14:30.969845 rootdir-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 16:14:30.996843 rootdir-0.1.1/src/rootdir/
+-rw-rw-rw-   0        0        0        0 2024-05-12 16:09:07.000000 rootdir-0.1.1/src/rootdir/__init__.py
+-rw-rw-rw-   0        0        0      502 2024-05-12 16:09:24.000000 rootdir-0.1.1/src/rootdir/rootdir.py
```

