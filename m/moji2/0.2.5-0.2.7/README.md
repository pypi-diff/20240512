# Comparing `tmp/moji2-0.2.5.tar.gz` & `tmp/moji2-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moji2-0.2.5.tar", last modified: Sat May 11 23:15:30 2024, max compression
+gzip compressed data, was "moji2-0.2.7.tar", last modified: Sat May 11 23:56:18 2024, max compression
```

## Comparing `moji2-0.2.5.tar` & `moji2-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 23:15:30.419205 moji2-0.2.5/
--rw-rw-rw-   0        0        0      722 2024-05-11 23:15:30.418205 moji2-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-04-16 09:39:02.000000 moji2-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 23:15:30.395509 moji2-0.2.5/moji/
--rw-rw-rw-   0        0        0        0 2024-04-16 09:36:55.000000 moji2-0.2.5/moji/__init__.py
--rw-rw-rw-   0        0        0       78 2024-05-02 22:50:10.000000 moji2-0.2.5/moji/moji.py
-drwxrwxrwx   0        0        0        0 2024-05-11 23:15:30.416465 moji2-0.2.5/moji2.egg-info/
--rw-rw-rw-   0        0        0      722 2024-05-11 23:15:30.000000 moji2-0.2.5/moji2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-05-11 23:15:30.000000 moji2-0.2.5/moji2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 23:15:30.000000 moji2-0.2.5/moji2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-11 23:15:30.000000 moji2-0.2.5/moji2.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-11 23:15:30.000000 moji2-0.2.5/moji2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 23:15:30.420207 moji2-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1353 2024-05-11 23:15:25.000000 moji2-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:56:18.086895 moji2-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-11 23:56:18.086895 moji2-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 23:56:14.000000 moji2-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:56:18.082895 moji2-0.2.7/moji/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:56:14.000000 moji2-0.2.7/moji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-11 23:56:14.000000 moji2-0.2.7/moji/moji.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:56:18.086895 moji2-0.2.7/moji2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-11 23:56:18.000000 moji2-0.2.7/moji2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-11 23:56:18.000000 moji2-0.2.7/moji2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:56:18.000000 moji2-0.2.7/moji2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 23:56:18.000000 moji2-0.2.7/moji2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-11 23:56:18.000000 moji2-0.2.7/moji2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:56:18.086895 moji2-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-11 23:56:14.000000 moji2-0.2.7/setup.py
```

### Comparing `moji2-0.2.5/PKG-INFO` & `moji2-0.2.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1
-Name: moji2
-Version: 0.2.5
-Summary: Demo library
-Author: Joffrey Bienvenu
-Author-email: example@email.com
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-
-# moji Karimi
+Metadata-Version: 2.1
+Name: moji2
+Version: 0.2.7
+Summary: Demo library
+Author: Joffrey Bienvenu
+Author-email: example@email.com
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+
+# moji Karimi
```

### Comparing `moji2-0.2.5/moji2.egg-info/PKG-INFO` & `moji2-0.2.7/moji2.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1
-Name: moji2
-Version: 0.2.5
-Summary: Demo library
-Author: Joffrey Bienvenu
-Author-email: example@email.com
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-
-# moji Karimi
+Metadata-Version: 2.1
+Name: moji2
+Version: 0.2.7
+Summary: Demo library
+Author: Joffrey Bienvenu
+Author-email: example@email.com
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+
+# moji Karimi
```

