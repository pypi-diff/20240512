# Comparing `tmp/aplustools-1.4.8.4.tar.gz` & `tmp/aplustools-1.4.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aplustools-1.4.8.4.tar", last modified: Fri Apr 12 17:07:41 2024, max compression
+gzip compressed data, was "aplustools-1.4.8.5.tar", last modified: Sun May 12 15:41:39 2024, max compression
```

## Comparing `aplustools-1.4.8.4.tar` & `aplustools-1.4.8.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:41.250501 aplustools-1.4.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-04-12 17:07:41.250501 aplustools-1.4.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19488 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:41.238501 aplustools-1.4.8.4/aplustools/
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:41.242501 aplustools-1.4.8.4/aplustools/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28389 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/advanced_imagetools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/database_new.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/faker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/github-updater-cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/github-updater-gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/github-updater-none.py
--rw-r--r--   0 runner    (1001) docker     (127)    29673 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/imagetools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/data/updaters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:41.242501 aplustools-1.4.8.4/aplustools/io/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17184 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/io/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:41.242501 aplustools-1.4.8.4/aplustools/io/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/io/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/io/gui/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    41238 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/io/gui/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)   188419 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/io/gui/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/io/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/io/system_Test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:41.242501 aplustools-1.4.8.4/aplustools/package/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/package/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23987 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/package/argu_mint_old.py
--rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/package/argumint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/package/timid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:41.246501 aplustools-1.4.8.4/aplustools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/tests/test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:41.246501 aplustools-1.4.8.4/aplustools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/utils/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/utils/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)    64497 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/utils/genpass.py
--rw-r--r--   0 runner    (1001) docker     (127)    31397 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/utils/hasher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:41.246501 aplustools-1.4.8.4/aplustools/web/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/web/_direct_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19651 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/web/new_webtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/web/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/web/search.py
--rw-r--r--   0 runner    (1001) docker     (127)   219892 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/aplustools/web/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:07:41.246501 aplustools-1.4.8.4/aplustools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20405 2024-04-12 17:07:41.000000 aplustools-1.4.8.4/aplustools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-12 17:07:41.000000 aplustools-1.4.8.4/aplustools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:07:41.000000 aplustools-1.4.8.4/aplustools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 17:07:41.000000 aplustools-1.4.8.4/aplustools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-12 17:07:41.000000 aplustools-1.4.8.4/aplustools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 17:07:41.000000 aplustools-1.4.8.4/aplustools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-12 17:07:36.000000 aplustools-1.4.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:07:41.250501 aplustools-1.4.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:39.231499 aplustools-1.4.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-05-12 15:41:39.231499 aplustools-1.4.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19837 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:39.219499 aplustools-1.4.8.5/aplustools/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:39.223499 aplustools-1.4.8.5/aplustools/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28416 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/advanced_imagetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13622 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/database_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/faker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/github-updater-cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/github-updater-gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/github-updater-none.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29699 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/imagetools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/data/updaters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:39.223499 aplustools-1.4.8.5/aplustools/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17184 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/io/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:39.223499 aplustools-1.4.8.5/aplustools/io/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/io/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/io/gui/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41238 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/io/gui/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)   188419 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/io/gui/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12346 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/io/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/io/system_Test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:39.223499 aplustools-1.4.8.5/aplustools/package/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/package/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23987 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/package/argu_mint_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19454 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/package/argumint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/package/timid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:39.227499 aplustools-1.4.8.5/aplustools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:39.227499 aplustools-1.4.8.5/aplustools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/utils/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/utils/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64497 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/utils/genpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31397 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/utils/hasher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:39.227499 aplustools-1.4.8.5/aplustools/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/web/_direct_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19651 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/web/new_webtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/web/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/web/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)   219892 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/aplustools/web/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:41:39.227499 aplustools-1.4.8.5/aplustools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-05-12 15:41:39.000000 aplustools-1.4.8.5/aplustools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-12 15:41:39.000000 aplustools-1.4.8.5/aplustools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:41:39.000000 aplustools-1.4.8.5/aplustools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-12 15:41:39.000000 aplustools-1.4.8.5/aplustools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-12 15:41:39.000000 aplustools-1.4.8.5/aplustools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-12 15:41:39.000000 aplustools-1.4.8.5/aplustools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-12 15:41:34.000000 aplustools-1.4.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:41:39.231499 aplustools-1.4.8.5/setup.cfg
```

### Comparing `aplustools-1.4.8.4/LICENSE` & `aplustools-1.4.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/PKG-INFO` & `aplustools-1.4.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplustools
-Version: 1.4.8.4
+Version: 1.4.8.5
 Summary: A collection of helpful tools
 Author-email: Cariel Becker <cariel.becker@gmx.de>
 Maintainer-email: Cariel Becker <cariel.becker@gmx.de>
 License: GPL-3.0-or-later
 Project-URL: Home, https://pypi.org/project/aplustools/
 Project-URL: Repository, https://github.com/adalfarus/aplustools
 Project-URL: Documentation, https://github.com/adalfarus/aplustools/wiki
@@ -567,14 +567,23 @@
 ...     def hello_word(self):
 ...             print("Hello, you!")
 ... test = Test()
 ... test.hello_word()
 ... end
 Hello, you!
 ```
+These can also be used in e.g. batch files like this
+```batch
+@echo off
+set /p id=Enter ID: 
+upype from aplustools.utils.genpass import GeneratePasswords; print(GeneratePasswords.generate_custom_sentence_based_password_v1("""%id%""", random_case=True, extra_char="""_""", char_position=0, num_length=5, special_chars_length=2))
+pause
+
+```
+
 ### apt
 Can currently run tests with ```apt tests run``` and show a basic help using ```apt help```.
 
 
 For more detailed usage and examples, check out our [documentation](https://github.com/adalfarus/aplustools/wiki).
 
 ## Naming convention, dependencies and more
```

### Comparing `aplustools-1.4.8.4/README.md` & `aplustools-1.4.8.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -530,14 +530,23 @@
 ...     def hello_word(self):
 ...             print("Hello, you!")
 ... test = Test()
 ... test.hello_word()
 ... end
 Hello, you!
 ```
+These can also be used in e.g. batch files like this
+```batch
+@echo off
+set /p id=Enter ID: 
+upype from aplustools.utils.genpass import GeneratePasswords; print(GeneratePasswords.generate_custom_sentence_based_password_v1("""%id%""", random_case=True, extra_char="""_""", char_position=0, num_length=5, special_chars_length=2))
+pause
+
+```
+
 ### apt
 Can currently run tests with ```apt tests run``` and show a basic help using ```apt help```.
 
 
 For more detailed usage and examples, check out our [documentation](https://github.com/adalfarus/aplustools/wiki).
 
 ## Naming convention, dependencies and more
```

### Comparing `aplustools-1.4.8.4/aplustools/__init__.py` & `aplustools-1.4.8.5/aplustools/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # aplustools __init__
-__version__ = "1.4.8.4"
+__version__ = "1.4.8.5"
 
 
 from aplustools.package import LazyModuleLoader as _LazyModuleLoader
 
 # Lazy loading modules
 io = _LazyModuleLoader('aplustools.io')
 data = _LazyModuleLoader('aplustools.data')
```

### Comparing `aplustools-1.4.8.4/aplustools/_direct_functions.py` & `aplustools-1.4.8.5/aplustools/_direct_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     """Simulates a hard user CTRL+C exit. This means it skips any try ... except KeyboardInterrupts"""
     exit(-1073741510)  # 130 / 0xC000013A
 
 
 def install_all_dependencies():
     success = _install_dependencies_lst(["requests==2.31.0", "Pillow==10.3.0", "BeautifulSoup4==4.12.3",
                                          "duckduckgo_search==3.9.3", "cryptography==42.0.5", "PySide6==6.6.1",
-                                         "aiohttp==3.9.3", "opencv-python==4.9.0.80", "brotli==1.1.0",
+                                         "aiohttp==3.9.4", "opencv-python==4.9.0.80", "brotli==1.1.0",
                                          "zstandard==0.22.0", "py7zr==0.21.0", "pillow_heif==0.15.0", "numpy==1.26.4"])
     if not success:
         return
     print("Done, all possible dependencies installed ...")
 
 
 def set_dir_to_ex():
```

### Comparing `aplustools-1.4.8.4/aplustools/cli.py` & `aplustools-1.4.8.5/aplustools/cli.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/data/__init__.py` & `aplustools-1.4.8.5/aplustools/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/data/advanced_imagetools.py` & `aplustools-1.4.8.5/aplustools/data/advanced_imagetools.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,18 +64,18 @@
         """
         if self.use_async:
             asyncio.run(self._add_images_async(images_info))
         else:
             for image_class, args, kwargs in images_info:
                 kwargs["base_location"] = kwargs.get("base_location") or self.base_location
                 kwargs["_use_async"] = False
-                self.images.append(image_class(**kwargs))
+                self.images.append(image_class(*args, **kwargs))
 
     async def _add_images_async(self, images_info):
-        tasks = [ImageClass(*args, **{**kwargs, "_use_async": True,
+        tasks = [self.create_async(ImageClass, *args, **{**kwargs, "_use_async": True,
                                       "base_location": kwargs.get("base_location") or self.base_location})
                  for ImageClass, args, kwargs in images_info]
         self.images.extend(await asyncio.gather(*tasks))
 
     def add_image_object(self, image_object: Union['OfflineImage', 'OnlineImage']) -> int:
         """Adds image objects."""
         self.images.append(image_object)
@@ -604,8 +604,8 @@
         print(f"An exception occurred during testing: {e}")
         return False
     print("Test completed successfully.")
     return True
 
 
 if __name__ == "__main__":
-    local_test()
+    local_test()
```

### Comparing `aplustools-1.4.8.4/aplustools/data/compressor.py` & `aplustools-1.4.8.5/aplustools/data/compressor.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/data/database.py` & `aplustools-1.4.8.5/aplustools/data/database.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/data/database_new.py` & `aplustools-1.4.8.5/aplustools/data/database_new.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/data/faker.py` & `aplustools-1.4.8.5/aplustools/data/faker.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/data/github-updater-cmd.py` & `aplustools-1.4.8.5/aplustools/data/github-updater-cmd.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/data/github-updater-gui.py` & `aplustools-1.4.8.5/aplustools/data/github-updater-gui.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/data/github-updater-none.py` & `aplustools-1.4.8.5/aplustools/data/github-updater-none.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/data/imagetools.py` & `aplustools-1.4.8.5/aplustools/data/imagetools.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,18 +61,18 @@
         """
         if self.use_async:
             asyncio.run(self._add_images_async(images_info))
         else:
             for image_class, args, kwargs in images_info:
                 kwargs["base_location"] = kwargs.get("base_location") or self.base_location
                 kwargs["_use_async"] = False
-                self.images.append(image_class(**kwargs))
+                self.images.append(image_class(*args, **kwargs))
 
     async def _add_images_async(self, images_info):
-        tasks = [ImageClass(*args, **{**kwargs, "_use_async": True,
+        tasks = [self.create_async(ImageClass, *args, **{**kwargs, "_use_async": True,
                                       "base_location": kwargs.get("base_location") or self.base_location})
                  for ImageClass, args, kwargs in images_info]
         self.images.extend(await asyncio.gather(*tasks))
 
     def add_image_object(self, image_object: Union['OfflineImage', 'OnlineImage']) -> int:
         """Adds image objects."""
         self.images.append(image_object)
```

### Comparing `aplustools-1.4.8.4/aplustools/data/updaters.py` & `aplustools-1.4.8.5/aplustools/data/updaters.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/io/environment.py` & `aplustools-1.4.8.5/aplustools/io/environment.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/io/gui/__init__.py` & `aplustools-1.4.8.5/aplustools/io/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/io/gui/calendar.py` & `aplustools-1.4.8.5/aplustools/io/gui/calendar.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/io/gui/chat.py` & `aplustools-1.4.8.5/aplustools/io/gui/chat.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/io/loggers.py` & `aplustools-1.4.8.5/aplustools/io/loggers.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/io/system_Test.py` & `aplustools-1.4.8.5/aplustools/io/system_Test.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/package/__init__.py` & `aplustools-1.4.8.5/aplustools/package/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/package/_direct_functions.py` & `aplustools-1.4.8.5/aplustools/package/_direct_functions.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/package/argu_mint_old.py` & `aplustools-1.4.8.5/aplustools/package/argu_mint_old.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/package/argumint.py` & `aplustools-1.4.8.5/aplustools/package/argumint.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/package/timid.py` & `aplustools-1.4.8.5/aplustools/package/timid.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/tests/test_data.py` & `aplustools-1.4.8.5/aplustools/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/utils/__init__.py` & `aplustools-1.4.8.5/aplustools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/utils/_direct_functions.py` & `aplustools-1.4.8.5/aplustools/utils/_direct_functions.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/utils/dummy.py` & `aplustools-1.4.8.5/aplustools/utils/dummy.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/utils/genpass.py` & `aplustools-1.4.8.5/aplustools/utils/genpass.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/utils/hasher.py` & `aplustools-1.4.8.5/aplustools/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/web/__init__.py` & `aplustools-1.4.8.5/aplustools/web/__init__.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/web/new_webtools.py` & `aplustools-1.4.8.5/aplustools/web/new_webtools.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/web/request.py` & `aplustools-1.4.8.5/aplustools/web/request.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/web/search.py` & `aplustools-1.4.8.5/aplustools/web/search.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools/web/utils.py` & `aplustools-1.4.8.5/aplustools/web/utils.py`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/aplustools.egg-info/PKG-INFO` & `aplustools-1.4.8.5/aplustools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplustools
-Version: 1.4.8.4
+Version: 1.4.8.5
 Summary: A collection of helpful tools
 Author-email: Cariel Becker <cariel.becker@gmx.de>
 Maintainer-email: Cariel Becker <cariel.becker@gmx.de>
 License: GPL-3.0-or-later
 Project-URL: Home, https://pypi.org/project/aplustools/
 Project-URL: Repository, https://github.com/adalfarus/aplustools
 Project-URL: Documentation, https://github.com/adalfarus/aplustools/wiki
@@ -567,14 +567,23 @@
 ...     def hello_word(self):
 ...             print("Hello, you!")
 ... test = Test()
 ... test.hello_word()
 ... end
 Hello, you!
 ```
+These can also be used in e.g. batch files like this
+```batch
+@echo off
+set /p id=Enter ID: 
+upype from aplustools.utils.genpass import GeneratePasswords; print(GeneratePasswords.generate_custom_sentence_based_password_v1("""%id%""", random_case=True, extra_char="""_""", char_position=0, num_length=5, special_chars_length=2))
+pause
+
+```
+
 ### apt
 Can currently run tests with ```apt tests run``` and show a basic help using ```apt help```.
 
 
 For more detailed usage and examples, check out our [documentation](https://github.com/adalfarus/aplustools/wiki).
 
 ## Naming convention, dependencies and more
```

### Comparing `aplustools-1.4.8.4/aplustools.egg-info/SOURCES.txt` & `aplustools-1.4.8.5/aplustools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aplustools-1.4.8.4/pyproject.toml` & `aplustools-1.4.8.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["aplustools", "aplustools.data", "aplustools.io", "aplustools.utils", "aplustools.web", "aplustools.package", "aplustools.tests", "aplustools.io.gui"]
 
 [project]
 name = "aplustools"
-version = "1.4.8.4"
+version = "1.4.8.5"
 dependencies = [
   "requests>=2.31.0",
   "BeautifulSoup4>=4.12.2",
 #   "win32api; os_name == 'nt'",
 ]
 requires-python = ">= 3.9"
 authors = [
```

