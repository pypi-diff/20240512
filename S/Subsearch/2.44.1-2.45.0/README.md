# Comparing `tmp/subsearch-2.44.1.tar.gz` & `tmp/subsearch-2.45.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subsearch-2.44.1.tar", last modified: Thu May  9 13:31:29 2024, max compression
+gzip compressed data, was "subsearch-2.45.0.tar", last modified: Sun May 12 11:33:00 2024, max compression
```

## Comparing `subsearch-2.44.1.tar` & `subsearch-2.45.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.554010 subsearch-2.44.1/
--rw-rw-rw-   0        0        0     1093 2024-05-09 13:29:54.000000 subsearch-2.44.1/LICENSE
--rw-rw-rw-   0        0        0      121 2024-05-09 13:29:54.000000 subsearch-2.44.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7763 2024-05-09 13:31:29.554010 subsearch-2.44.1/PKG-INFO
--rw-rw-rw-   0        0        0     5961 2024-05-09 13:29:54.000000 subsearch-2.44.1/README.md
--rw-rw-rw-   0        0        0     2607 2024-05-09 13:29:54.000000 subsearch-2.44.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 13:31:29.554010 subsearch-2.44.1/setup.cfg
--rw-rw-rw-   0        0        0      114 2024-05-09 13:29:54.000000 subsearch-2.44.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.507138 subsearch-2.44.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.538383 subsearch-2.44.1/src/Subsearch.egg-info/
--rw-rw-rw-   0        0        0     7763 2024-05-09 13:31:29.000000 subsearch-2.44.1/src/Subsearch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2024-05-09 13:31:29.000000 subsearch-2.44.1/src/Subsearch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 13:31:29.000000 subsearch-2.44.1/src/Subsearch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-09 13:31:29.000000 subsearch-2.44.1/src/Subsearch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-09 13:31:29.000000 subsearch-2.44.1/src/Subsearch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      377 2024-05-09 13:31:29.000000 subsearch-2.44.1/src/Subsearch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-09 13:31:29.000000 subsearch-2.44.1/src/Subsearch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.522751 subsearch-2.44.1/src/subsearch/
--rw-rw-rw-   0        0        0     1498 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/__init__.py
--rw-rw-rw-   0        0        0       38 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/__main__.py
--rw-rw-rw-   0        0        0     9400 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/core.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.522751 subsearch-2.44.1/src/subsearch/data/
--rw-rw-rw-   0        0        0       99 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/data/__init__.py
--rw-rw-rw-   0        0        0       53 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/data/guid.py
--rw-rw-rw-   0        0        0     7704 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/data/language_data.toml
--rw-rw-rw-   0        0        0       24 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/data/version.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.522751 subsearch-2.44.1/src/subsearch/globals/
--rw-rw-rw-   0        0        0        0 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/globals/__init__.py
--rw-rw-rw-   0        0        0      513 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/globals/constants.py
--rw-rw-rw-   0        0        0     2505 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/globals/dataclasses.py
--rw-rw-rw-   0        0        0     5622 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/globals/decorators.py
--rw-rw-rw-   0        0        0      980 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/globals/exceptions.py
--rw-rw-rw-   0        0        0      258 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/globals/metaclasses.py
--rw-rw-rw-   0        0        0     1597 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/globals/propagating_thread.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.522751 subsearch-2.44.1/src/subsearch/gui/
--rw-rw-rw-   0        0        0      588 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/__init__.py
--rw-rw-rw-   0        0        0     3180 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/common_utils.py
--rw-rw-rw-   0        0        0     1053 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/resource_loader.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.538383 subsearch-2.44.1/src/subsearch/gui/resources/
--rw-rw-rw-   0        0        0        0 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.538383 subsearch-2.44.1/src/subsearch/gui/resources/assets/
--rw-rw-rw-   0        0        0        0 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/resources/assets/__init__.py
--rw-rw-rw-   0        0        0     7119 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/resources/assets/spritesheet.png
--rw-rw-rw-   0        0        0   105808 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/resources/assets/subsearch.ico
--rw-rw-rw-   0        0        0     1674 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/resources/config.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.538383 subsearch-2.44.1/src/subsearch/gui/resources/styles/
--rw-rw-rw-   0        0        0        0 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/resources/styles/__init__.py
--rw-rw-rw-   0        0        0     1780 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/resources/styles/sprites.tcl
--rw-rw-rw-   0        0        0     7247 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/resources/styles/style_subsearch.tcl
--rw-rw-rw-   0        0        0     1451 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/resources/styles/theme_setter.tcl
--rw-rw-rw-   0        0        0     6957 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/screen_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.538383 subsearch-2.44.1/src/subsearch/gui/screens/
--rw-rw-rw-   0        0        0        0 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/screens/__init__.py
--rw-rw-rw-   0        0        0     5703 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/screens/download_manager.py
--rw-rw-rw-   0        0        0     2935 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/screens/language_options.py
--rw-rw-rw-   0        0        0    15203 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/screens/search_options.py
--rw-rw-rw-   0        0        0    13523 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/screens/subsearch_options.py
--rw-rw-rw-   0        0        0     1270 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/gui/system_tray.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.538383 subsearch-2.44.1/src/subsearch/providers/
--rw-rw-rw-   0        0        0        2 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/providers/__init__.py
--rw-rw-rw-   0        0        0     5927 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/providers/common_utils.py
--rw-rw-rw-   0        0        0     3187 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/providers/opensubtitles.py
--rw-rw-rw-   0        0        0     3330 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/providers/subscene.py
--rw-rw-rw-   0        0        0     2459 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/providers/yifysubtitles.py
-drwxrwxrwx   0        0        0        0 2024-05-09 13:31:29.538383 subsearch-2.44.1/src/subsearch/utils/
--rw-rw-rw-   0        0        0        2 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/utils/__init__.py
--rw-rw-rw-   0        0        0     1797 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/utils/imdb_lookup.py
--rw-rw-rw-   0        0        0     4803 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/utils/io_app.py
--rw-rw-rw-   0        0        0     6415 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/utils/io_file_system.py
--rw-rw-rw-   0        0        0     5967 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/utils/io_log.py
--rw-rw-rw-   0        0        0     4151 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/utils/io_toml.py
--rw-rw-rw-   0        0        0     4397 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/utils/io_winreg.py
--rw-rw-rw-   0        0        0     8426 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/utils/string_parser.py
--rw-rw-rw-   0        0        0     2898 2024-05-09 13:29:54.000000 subsearch-2.44.1/src/subsearch/utils/update.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.238421 subsearch-2.45.0/
+-rw-rw-rw-   0        0        0     1093 2024-05-12 11:32:23.000000 subsearch-2.45.0/LICENSE
+-rw-rw-rw-   0        0        0      121 2024-05-12 11:32:23.000000 subsearch-2.45.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7491 2024-05-12 11:33:00.238421 subsearch-2.45.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5741 2024-05-12 11:32:23.000000 subsearch-2.45.0/README.md
+-rw-rw-rw-   0        0        0     2556 2024-05-12 11:32:23.000000 subsearch-2.45.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 11:33:00.238421 subsearch-2.45.0/setup.cfg
+-rw-rw-rw-   0        0        0      114 2024-05-12 11:32:23.000000 subsearch-2.45.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.191542 subsearch-2.45.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.222795 subsearch-2.45.0/src/Subsearch.egg-info/
+-rw-rw-rw-   0        0        0     7491 2024-05-12 11:33:00.000000 subsearch-2.45.0/src/Subsearch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2078 2024-05-12 11:33:00.000000 subsearch-2.45.0/src/Subsearch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 11:33:00.000000 subsearch-2.45.0/src/Subsearch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-12 11:33:00.000000 subsearch-2.45.0/src/Subsearch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-12 11:32:59.000000 subsearch-2.45.0/src/Subsearch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      377 2024-05-12 11:33:00.000000 subsearch-2.45.0/src/Subsearch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 11:33:00.000000 subsearch-2.45.0/src/Subsearch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.207169 subsearch-2.45.0/src/subsearch/
+-rw-rw-rw-   0        0        0     1487 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/__init__.py
+-rw-rw-rw-   0        0        0       38 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/__main__.py
+-rw-rw-rw-   0        0        0     9540 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/core.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.207169 subsearch-2.45.0/src/subsearch/data/
+-rw-rw-rw-   0        0        0       99 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/data/__init__.py
+-rw-rw-rw-   0        0        0       53 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/data/guid.py
+-rw-rw-rw-   0        0        0     7704 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/data/language_data.toml
+-rw-rw-rw-   0        0        0       24 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/data/version.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.207169 subsearch-2.45.0/src/subsearch/globals/
+-rw-rw-rw-   0        0        0       62 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/globals/__init__.py
+-rw-rw-rw-   0        0        0     6405 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/globals/_logging.py
+-rw-rw-rw-   0        0        0      513 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/globals/constants.py
+-rw-rw-rw-   0        0        0     2505 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/globals/dataclasses.py
+-rw-rw-rw-   0        0        0     5161 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/globals/decorators.py
+-rw-rw-rw-   0        0        0      980 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/globals/exceptions.py
+-rw-rw-rw-   0        0        0      258 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/globals/metaclasses.py
+-rw-rw-rw-   0        0        0     1269 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/globals/thread_handle.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.222795 subsearch-2.45.0/src/subsearch/gui/
+-rw-rw-rw-   0        0        0      588 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/__init__.py
+-rw-rw-rw-   0        0        0     3180 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/common_utils.py
+-rw-rw-rw-   0        0        0     1053 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/resource_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.222795 subsearch-2.45.0/src/subsearch/gui/resources/
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.222795 subsearch-2.45.0/src/subsearch/gui/resources/assets/
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/resources/assets/__init__.py
+-rw-rw-rw-   0        0        0     7119 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/resources/assets/spritesheet.png
+-rw-rw-rw-   0        0        0   105808 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/resources/assets/subsearch.ico
+-rw-rw-rw-   0        0        0     1674 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/resources/config.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.222795 subsearch-2.45.0/src/subsearch/gui/resources/styles/
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/resources/styles/__init__.py
+-rw-rw-rw-   0        0        0     1780 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/resources/styles/sprites.tcl
+-rw-rw-rw-   0        0        0     7247 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/resources/styles/style_subsearch.tcl
+-rw-rw-rw-   0        0        0     1451 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/resources/styles/theme_setter.tcl
+-rw-rw-rw-   0        0        0     6949 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/screen_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.222795 subsearch-2.45.0/src/subsearch/gui/screens/
+-rw-rw-rw-   0        0        0        0 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/screens/__init__.py
+-rw-rw-rw-   0        0        0     5727 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/screens/download_manager.py
+-rw-rw-rw-   0        0        0     2935 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/screens/language_options.py
+-rw-rw-rw-   0        0        0    15230 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/screens/search_options.py
+-rw-rw-rw-   0        0        0    13523 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/screens/subsearch_options.py
+-rw-rw-rw-   0        0        0     1195 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/gui/system_tray.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.222795 subsearch-2.45.0/src/subsearch/providers/
+-rw-rw-rw-   0        0        0        2 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/providers/__init__.py
+-rw-rw-rw-   0        0        0     5947 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/providers/common_utils.py
+-rw-rw-rw-   0        0        0     3172 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/providers/opensubtitles.py
+-rw-rw-rw-   0        0        0     3330 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/providers/subscene.py
+-rw-rw-rw-   0        0        0     2459 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/providers/yifysubtitles.py
+drwxrwxrwx   0        0        0        0 2024-05-12 11:33:00.222795 subsearch-2.45.0/src/subsearch/utils/
+-rw-rw-rw-   0        0        0        2 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/utils/__init__.py
+-rw-rw-rw-   0        0        0     1992 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/utils/imdb_lookup.py
+-rw-rw-rw-   0        0        0     4803 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/utils/io_app.py
+-rw-rw-rw-   0        0        0     6344 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/utils/io_file_system.py
+-rw-rw-rw-   0        0        0     4094 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/utils/io_toml.py
+-rw-rw-rw-   0        0        0     4424 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/utils/io_winreg.py
+-rw-rw-rw-   0        0        0     8453 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/utils/string_parser.py
+-rw-rw-rw-   0        0        0     2890 2024-05-12 11:32:23.000000 subsearch-2.45.0/src/subsearch/utils/update.py
```

### Comparing `subsearch-2.44.1/LICENSE` & `subsearch-2.45.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/PKG-INFO` & `subsearch-2.45.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.44.1
+Version: 2.45.0
 Summary: Subsearch
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subtitles,sub,srt,tool,tools,download,movies,shows,scrape,opensubtitles,subscene,subsearch,subtitles,yifysubtitles
 Platform: win32
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: picologging==0.9.3
 Requires-Dist: cloudscraper==1.2.71
 Requires-Dist: num2words==0.5.13
 Requires-Dist: packaging==24.0
 Requires-Dist: pillow==10.3.0
@@ -45,21 +44,20 @@
 Provides-Extra: type
 Requires-Dist: mypy==1.10.0; extra == "type"
 
 <h1 align="center"><img src="https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/subsearch_v2.png"/></h1>
 
 <div align="center">
 
-![Tests](https://img.shields.io/github/actions/workflow/status/vagabondhustler/subsearch/ci.yml?style=flat-square&labelColor=1e1e2e&label=ci)
-![Tags](https://img.shields.io/github/v/tag/vagabondhustler/subsearch?style=flat-square&labelColor=1e1e2e)
-![GitHub commit activity](https://img.shields.io/github/commit-activity/m/vagabondhustler/subsearch?&style=flat-square&labelColor=1e1e2e)
-![License](https://img.shields.io/github/license/vagabondhustler/SUbSearch?&style=flat-square&labelColor=1e1e2e)
-
-![downloads-total)](https://img.shields.io/github/downloads/vagabondhustler/subsearch/total?style=flat-square&label=downloads%40total&labelColor=%231e1e2e)
-![downloads-latest)](https://img.shields.io/github/downloads/vagabondhustler/subsearch/latest/total?style=flat-square&label=downloads%40latest&labelColor=%231e1e2e)
+![tests](https://img.shields.io/github/actions/workflow/status/vagabondhustler/subsearch/ci.yml?style=flat-square&labelColor=1e1e2e&label=ci)
+![github_commit_activity](https://img.shields.io/github/last-commit/vagabondhustler/subsearch?&style=flat-square&labelColor=1e1e2e&label=commit%20activity)
+![python_version](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FvagabondHustler%2Fsubsearch%2Fmain%2Fpyproject.toml&style=flat-square&labelColor=1e1e2e)
+![release](https://img.shields.io/github/v/tag/vagabondhustler/subsearch?style=flat-square&labelColor=1e1e2e&label=latest%20release)
+![downloads-total)](https://img.shields.io/github/downloads/vagabondhustler/subsearch/total?style=flat-square&labelColor=%231e1e2e&label=downloads)
+![license](https://img.shields.io/github/license/vagabondhustler/subsearch?&style=flat-square&labelColor=1e1e2e)
 
 </div>
 
 #### Readme Table of Contents
 
 - [About](#about)
 - [Preview of GUI](#preview)
@@ -115,41 +113,33 @@
 
 </div>
 
 ## Installation and usage <a name = "getting_started_src"></a>
 
 #### Install from pypi: <a name = "pypi"></a>
 
-Requires Python 3.10+
-
 - Install Subsearch by running `pip install subsearch` in the command prompt.
 - Launch the app by running `subsearch` in the command prompt.
 
 #### Clone from github <a name = "clone"></a>
 
-Requires Python *3.10+
-
 - Clone the Subsearch repository by running `git clone https://github.com/vagabondHustler/subsearch.git`.
 - Install Subsearch by running `pip install -e .` or *`pip install -e .[build,lint,tests,tools,type]` for optional dependencies.
 - Build the executable and MSI installer by running `python -m tools.cx_freeze_build bdist_msi`.
 
-> [!IMPORTANT]  
-> ###### If you are using Python 3.12+ and cx_Freeze, please refer to [this issue](https://github.com/marcelotduarte/cx_Freeze/issues/2153).
-
 #### Windows installer <a name = "msi"></a>
 
 Requires windows 10/11, probably works on 8.
 
 - Download the windows installer "Subsearch-x.x.x-win64.msi" from [here](https://github.com/vagabondHustler/subsearch/releases).
 - Run the installer.
 - If you receive a PUA message, click "More info" → "Run anyway".
 - Run Subsearch at least once for all the context menu options to appear
 
-> [!NOTE]  
-> ###### Development builds can be located in the [release](https://github.com/vagabondHustler/subsearch/actions/workflows/release.yml) action job, within the generated artifacts.
+###### Development builds can be located in the [release](https://github.com/vagabondHustler/subsearch/actions/workflows/release.yml) action job, within the generated artifacts.
 
 <details>
 <summary>Screenshots of PUA message<a name = "pua"></a></summary>
 
 ![prtsc_moreinfo](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/moreinfo.png)
 
 ![prtsc_runanyway](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/runanyway.png)
@@ -158,12 +148,12 @@
 
 </details>
 
 More about potentially unwanted applications (PUA) can be found [here](https://support.microsoft.com/en-us/windows/protect-your-pc-from-potentially-unwanted-applications-c7668a25-174e-3b78-0191-faf0607f7a6e) on Microsoft's support page.
 
 ## Acknowledgements<a name = "thanks"></a>
 
-I would like to express my gratitude to the following repositories for providing templates, scripts, inspiration, themes, and solutions to similar problems:
+The following repositories provided templates, scripts, inspiration, themes, etc:
 
 - [zavoloklom/material-design-iconic-font](https://github.com/zavoloklom/material-design-iconic-font) // icons
 - [rdbende/Sun-Valley-ttk-theme](https://github.com/rdbende/Sun-Valley-ttk-theme) // base theme
 - [TransparentLC](https://github.com/TransparentLC) // spritesheet_generator.js
```

### Comparing `subsearch-2.44.1/README.md` & `subsearch-2.45.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 <h1 align="center"><img src="https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/subsearch_v2.png"/></h1>
 
 <div align="center">
 
-![Tests](https://img.shields.io/github/actions/workflow/status/vagabondhustler/subsearch/ci.yml?style=flat-square&labelColor=1e1e2e&label=ci)
-![Tags](https://img.shields.io/github/v/tag/vagabondhustler/subsearch?style=flat-square&labelColor=1e1e2e)
-![GitHub commit activity](https://img.shields.io/github/commit-activity/m/vagabondhustler/subsearch?&style=flat-square&labelColor=1e1e2e)
-![License](https://img.shields.io/github/license/vagabondhustler/SUbSearch?&style=flat-square&labelColor=1e1e2e)
-
-![downloads-total)](https://img.shields.io/github/downloads/vagabondhustler/subsearch/total?style=flat-square&label=downloads%40total&labelColor=%231e1e2e)
-![downloads-latest)](https://img.shields.io/github/downloads/vagabondhustler/subsearch/latest/total?style=flat-square&label=downloads%40latest&labelColor=%231e1e2e)
+![tests](https://img.shields.io/github/actions/workflow/status/vagabondhustler/subsearch/ci.yml?style=flat-square&labelColor=1e1e2e&label=ci)
+![github_commit_activity](https://img.shields.io/github/last-commit/vagabondhustler/subsearch?&style=flat-square&labelColor=1e1e2e&label=commit%20activity)
+![python_version](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FvagabondHustler%2Fsubsearch%2Fmain%2Fpyproject.toml&style=flat-square&labelColor=1e1e2e)
+![release](https://img.shields.io/github/v/tag/vagabondhustler/subsearch?style=flat-square&labelColor=1e1e2e&label=latest%20release)
+![downloads-total)](https://img.shields.io/github/downloads/vagabondhustler/subsearch/total?style=flat-square&labelColor=%231e1e2e&label=downloads)
+![license](https://img.shields.io/github/license/vagabondhustler/subsearch?&style=flat-square&labelColor=1e1e2e)
 
 </div>
 
 #### Readme Table of Contents
 
 - [About](#about)
 - [Preview of GUI](#preview)
@@ -68,41 +67,33 @@
 
 </div>
 
 ## Installation and usage <a name = "getting_started_src"></a>
 
 #### Install from pypi: <a name = "pypi"></a>
 
-Requires Python 3.10+
-
 - Install Subsearch by running `pip install subsearch` in the command prompt.
 - Launch the app by running `subsearch` in the command prompt.
 
 #### Clone from github <a name = "clone"></a>
 
-Requires Python *3.10+
-
 - Clone the Subsearch repository by running `git clone https://github.com/vagabondHustler/subsearch.git`.
 - Install Subsearch by running `pip install -e .` or *`pip install -e .[build,lint,tests,tools,type]` for optional dependencies.
 - Build the executable and MSI installer by running `python -m tools.cx_freeze_build bdist_msi`.
 
-> [!IMPORTANT]  
-> ###### If you are using Python 3.12+ and cx_Freeze, please refer to [this issue](https://github.com/marcelotduarte/cx_Freeze/issues/2153).
-
 #### Windows installer <a name = "msi"></a>
 
 Requires windows 10/11, probably works on 8.
 
 - Download the windows installer "Subsearch-x.x.x-win64.msi" from [here](https://github.com/vagabondHustler/subsearch/releases).
 - Run the installer.
 - If you receive a PUA message, click "More info" → "Run anyway".
 - Run Subsearch at least once for all the context menu options to appear
 
-> [!NOTE]  
-> ###### Development builds can be located in the [release](https://github.com/vagabondHustler/subsearch/actions/workflows/release.yml) action job, within the generated artifacts.
+###### Development builds can be located in the [release](https://github.com/vagabondHustler/subsearch/actions/workflows/release.yml) action job, within the generated artifacts.
 
 <details>
 <summary>Screenshots of PUA message<a name = "pua"></a></summary>
 
 ![prtsc_moreinfo](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/moreinfo.png)
 
 ![prtsc_runanyway](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/runanyway.png)
@@ -111,12 +102,12 @@
 
 </details>
 
 More about potentially unwanted applications (PUA) can be found [here](https://support.microsoft.com/en-us/windows/protect-your-pc-from-potentially-unwanted-applications-c7668a25-174e-3b78-0191-faf0607f7a6e) on Microsoft's support page.
 
 ## Acknowledgements<a name = "thanks"></a>
 
-I would like to express my gratitude to the following repositories for providing templates, scripts, inspiration, themes, and solutions to similar problems:
+The following repositories provided templates, scripts, inspiration, themes, etc:
 
 - [zavoloklom/material-design-iconic-font](https://github.com/zavoloklom/material-design-iconic-font) // icons
 - [rdbende/Sun-Valley-ttk-theme](https://github.com/rdbende/Sun-Valley-ttk-theme) // base theme
 - [TransparentLC](https://github.com/TransparentLC) // spritesheet_generator.js
```

### Comparing `subsearch-2.44.1/pyproject.toml` & `subsearch-2.45.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -22,142 +22,139 @@
 00000150: 7365 7273 2f44 6573 6b74 6f70 222c 0d0a  sers/Desktop",..
 00000160: 2020 2020 2020 2020 224f 7065 7261 7469          "Operati
 00000170: 6e67 2053 7973 7465 6d20 3a3a 204d 6963  ng System :: Mic
 00000180: 726f 736f 6674 203a 3a20 5769 6e64 6f77  rosoft :: Window
 00000190: 7322 2c0d 0a20 2020 2020 2020 2022 5072  s",..        "Pr
 000001a0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 000001b0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001c0: 332e 3130 222c 0d0a 2020 2020 2020 2020  3.10",..        
-000001d0: 2250 726f 6772 616d 6d69 6e67 204c 616e  "Programming Lan
-000001e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000001f0: 3a3a 2033 2e31 3122 2c0d 0a20 2020 2020  :: 3.11",..     
-00000200: 2020 2022 546f 7069 6320 3a3a 204d 756c     "Topic :: Mul
-00000210: 7469 6d65 6469 6120 3a3a 2056 6964 656f  timedia :: Video
-00000220: 222c 0d0a 2020 2020 2020 2020 2254 6f70  ",..        "Top
-00000230: 6963 203a 3a20 5574 696c 6974 6965 7322  ic :: Utilities"
-00000240: 2c0d 0a20 2020 205d 0d0a 2020 2020 6465  ,..    ]..    de
-00000250: 7065 6e64 656e 6369 6573 203d 205b 0d0a  pendencies = [..
-00000260: 2020 2020 2020 2020 2270 6963 6f6c 6f67          "picolog
-00000270: 6769 6e67 3d3d 302e 392e 3322 2c0d 0a20  ging==0.9.3",.. 
-00000280: 2020 2020 2020 2022 636c 6f75 6473 6372         "cloudscr
-00000290: 6170 6572 3d3d 312e 322e 3731 222c 0d0a  aper==1.2.71",..
-000002a0: 2020 2020 2020 2020 226e 756d 3277 6f72          "num2wor
-000002b0: 6473 3d3d 302e 352e 3133 222c 0d0a 2020  ds==0.5.13",..  
-000002c0: 2020 2020 2020 2270 6163 6b61 6769 6e67        "packaging
-000002d0: 3d3d 3234 2e30 222c 0d0a 2020 2020 2020  ==24.0",..      
-000002e0: 2020 2270 696c 6c6f 773d 3d31 302e 332e    "pillow==10.3.
-000002f0: 3022 2c0d 0a20 2020 2020 2020 2022 7079  0",..        "py
-00000300: 7374 7261 793d 3d30 2e31 392e 3522 2c0d  stray==0.19.5",.
-00000310: 0a20 2020 2020 2020 2022 7265 7175 6573  .        "reques
-00000320: 7473 3d3d 322e 3331 2e30 222c 0d0a 2020  ts==2.31.0",..  
-00000330: 2020 2020 2020 2273 656c 6563 746f 6c61        "selectola
-00000340: 783d 3d30 2e33 2e32 3122 2c0d 0a20 2020  x==0.3.21",..   
-00000350: 2020 2020 2022 746f 6d6c 3d3d 302e 3130       "toml==0.10
-00000360: 2e32 222c 0d0a 2020 2020 5d0d 0a20 2020  .2",..    ]..   
-00000370: 2064 6573 6372 6970 7469 6f6e 203d 2022   description = "
-00000380: 5375 6273 6561 7263 6822 0d0a 2020 2020  Subsearch"..    
-00000390: 6479 6e61 6d69 6320 3d20 5b22 7665 7273  dynamic = ["vers
-000003a0: 696f 6e22 5d0d 0a20 2020 206b 6579 776f  ion"]..    keywo
-000003b0: 7264 7320 3d20 5b0d 0a20 2020 2020 2020  rds = [..       
-000003c0: 2022 7375 6274 6974 6c65 7322 2c0d 0a20   "subtitles",.. 
-000003d0: 2020 2020 2020 2022 7375 6222 2c0d 0a20         "sub",.. 
-000003e0: 2020 2020 2020 2022 7372 7422 2c0d 0a20         "srt",.. 
-000003f0: 2020 2020 2020 2022 746f 6f6c 222c 0d0a         "tool",..
-00000400: 2020 2020 2020 2020 2274 6f6f 6c73 222c          "tools",
-00000410: 0d0a 2020 2020 2020 2020 2264 6f77 6e6c  ..        "downl
-00000420: 6f61 6422 2c0d 0a20 2020 2020 2020 2022  oad",..        "
-00000430: 6d6f 7669 6573 222c 0d0a 2020 2020 2020  movies",..      
-00000440: 2020 2273 686f 7773 222c 0d0a 2020 2020    "shows",..    
-00000450: 2020 2020 2273 6372 6170 6522 2c0d 0a20      "scrape",.. 
-00000460: 2020 2020 2020 2022 6f70 656e 7375 6274         "opensubt
-00000470: 6974 6c65 7322 2c0d 0a20 2020 2020 2020  itles",..       
-00000480: 2022 7375 6273 6365 6e65 222c 0d0a 2020   "subscene",..  
-00000490: 2020 2020 2020 2273 7562 7365 6172 6368        "subsearch
-000004a0: 222c 0d0a 2020 2020 2020 2020 2273 7562  ",..        "sub
-000004b0: 7469 746c 6573 222c 0d0a 2020 2020 2020  titles",..      
-000004c0: 2020 2279 6966 7973 7562 7469 746c 6573    "yifysubtitles
-000004d0: 222c 0d0a 2020 2020 5d0d 0a20 2020 206c  ",..    ]..    l
-000004e0: 6963 656e 7365 203d 207b 7465 7874 203d  icense = {text =
-000004f0: 2022 4d49 5420 6c69 6365 6e73 6522 7d0d   "MIT license"}.
-00000500: 0a20 2020 206e 616d 6520 3d20 2253 7562  .    name = "Sub
-00000510: 7365 6172 6368 220d 0a20 2020 2072 6561  search"..    rea
-00000520: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
-00000530: 220d 0a20 2020 2072 6571 7569 7265 732d  "..    requires-
-00000540: 7079 7468 6f6e 203d 2022 3e3d 332e 3130  python = ">=3.10
-00000550: 220d 0a0d 0a5b 7072 6f6a 6563 742e 7572  "....[project.ur
-00000560: 6c73 5d0d 0a20 2020 2072 6570 6f73 6974  ls]..    reposit
-00000570: 6f72 7920 3d20 2268 7474 7073 3a2f 2f67  ory = "https://g
-00000580: 6974 6875 622e 636f 6d2f 7661 6761 626f  ithub.com/vagabo
-00000590: 6e64 4875 7374 6c65 722f 7375 6273 6561  ndHustler/subsea
-000005a0: 7263 6822 0d0a 0d0a 5b70 726f 6a65 6374  rch"....[project
-000005b0: 2e73 6372 6970 7473 5d0d 0a20 2020 2073  .scripts]..    s
-000005c0: 7562 7365 6172 6368 203d 2022 7375 6273  ubsearch = "subs
-000005d0: 6561 7263 683a 6d61 696e 220d 0a0d 0a5b  earch:main"....[
-000005e0: 746f 6f6c 2e73 6574 7570 746f 6f6c 735d  tool.setuptools]
-000005f0: 0d0a 2020 2020 706c 6174 666f 726d 7320  ..    platforms 
-00000600: 3d20 5b22 7769 6e33 3222 5d0d 0a20 2020  = ["win32"]..   
-00000610: 207a 6970 2d73 6166 6520 3d20 6661 6c73   zip-safe = fals
-00000620: 650d 0a0d 0a5b 746f 6f6c 2e73 6574 7570  e....[tool.setup
-00000630: 746f 6f6c 732e 7061 636b 6167 6573 2e66  tools.packages.f
-00000640: 696e 645d 0d0a 2020 2020 6578 636c 7564  ind]..    exclud
-00000650: 6520 3d20 5b22 6578 616d 706c 6573 2a22  e = ["examples*"
-00000660: 2c20 2273 7562 7365 6172 6368 2e74 6573  , "subsearch.tes
-00000670: 742a 222c 2022 746f 6f6c 732a 225d 0d0a  t*", "tools*"]..
-00000680: 2020 2020 696e 636c 7564 6520 3d20 5b22      include = ["
-00000690: 7375 6273 6561 7263 682a 225d 0d0a 2020  subsearch*"]..  
-000006a0: 2020 7768 6572 6520 3d20 5b22 7372 6322    where = ["src"
-000006b0: 5d0d 0a0d 0a5b 746f 6f6c 2e73 6574 7570  ]....[tool.setup
-000006c0: 746f 6f6c 732e 6479 6e61 6d69 635d 0d0a  tools.dynamic]..
-000006d0: 2020 2020 7665 7273 696f 6e20 3d20 7b61      version = {a
-000006e0: 7474 7220 3d20 2273 7562 7365 6172 6368  ttr = "subsearch
-000006f0: 2e64 6174 612e 5f5f 7665 7273 696f 6e5f  .data.__version_
-00000700: 5f22 7d0d 0a0d 0a5b 7072 6f6a 6563 742e  _"}....[project.
-00000710: 6f70 7469 6f6e 616c 2d64 6570 656e 6465  optional-depende
-00000720: 6e63 6965 735d 0d0a 2020 2020 6275 696c  ncies]..    buil
-00000730: 6420 3d20 5b0d 0a20 2020 2020 2020 2022  d = [..        "
-00000740: 6275 696c 643d 3d31 2e32 2e31 222c 0d0a  build==1.2.1",..
-00000750: 2020 2020 2020 2020 2263 785f 4672 6565          "cx_Free
-00000760: 7a65 3d3d 372e 302e 3022 2c0d 0a20 2020  ze==7.0.0",..   
-00000770: 2020 2020 2022 7477 696e 653d 3d35 2e30       "twine==5.0
-00000780: 2e30 222c 0d0a 2020 2020 2020 2020 2270  .0",..        "p
-00000790: 7375 7469 6c3d 3d35 2e39 2e38 222c 0d0a  sutil==5.9.8",..
-000007a0: 2020 2020 5d0d 0a20 2020 206c 696e 7420      ]..    lint 
-000007b0: 3d20 5b22 626c 6163 6b3d 3d32 342e 342e  = ["black==24.4.
-000007c0: 3222 2c20 2269 736f 7274 3d3d 352e 3133  2", "isort==5.13
-000007d0: 2e32 225d 0d0a 2020 2020 7465 7374 7320  .2"]..    tests 
-000007e0: 3d20 5b0d 0a20 2020 2020 2020 2022 7079  = [..        "py
-000007f0: 7465 7374 2d63 6f76 3d3d 352e 302e 3022  test-cov==5.0.0"
-00000800: 2c0d 0a20 2020 2020 2020 2022 7079 7465  ,..        "pyte
-00000810: 7374 3d3d 382e 322e 3022 2c0d 0a20 2020  st==8.2.0",..   
-00000820: 2020 2020 2022 746f 783d 3d34 2e31 352e       "tox==4.15.
-00000830: 3022 2c0d 0a20 2020 2020 2020 2022 7079  0",..        "py
-00000840: 7468 6f6e 2d64 6f74 656e 763d 3d31 2e30  thon-dotenv==1.0
-00000850: 2e31 222c 0d0a 2020 2020 5d0d 0a20 2020  .1",..    ]..   
-00000860: 2074 6f6f 6c73 203d 205b 2270 7970 6572   tools = ["pyper
-00000870: 636c 6970 3d3d 312e 382e 3222 5d0d 0a20  clip==1.8.2"].. 
-00000880: 2020 2074 7970 6520 3d20 5b22 6d79 7079     type = ["mypy
-00000890: 3d3d 312e 3130 2e30 225d 0d0a 0d0a 5b74  ==1.10.0"]....[t
-000008a0: 6f6f 6c2e 7079 7465 7374 2e69 6e69 5f6f  ool.pytest.ini_o
-000008b0: 7074 696f 6e73 5d0d 0a20 2020 2061 6464  ptions]..    add
-000008c0: 6f70 7473 203d 2022 2d2d 636f 763d 7372  opts = "--cov=sr
-000008d0: 632f 7375 6273 6561 7263 6822 0d0a 2020  c/subsearch"..  
-000008e0: 2020 6669 6c74 6572 7761 726e 696e 6773    filterwarnings
-000008f0: 203d 205b 2769 676e 6f72 653a 3a44 6570   = ['ignore::Dep
-00000900: 7265 6361 7469 6f6e 5761 726e 696e 6727  recationWarning'
-00000910: 5d0d 0a20 2020 206c 6f67 5f63 6c69 203d  ]..    log_cli =
-00000920: 2074 7275 650d 0a20 2020 206c 6f67 5f63   true..    log_c
-00000930: 6c69 5f6c 6576 656c 203d 2027 4445 4255  li_level = 'DEBU
-00000940: 4727 0d0a 2020 2020 7465 7374 7061 7468  G'..    testpath
-00000950: 7320 3d20 5b22 7465 7374 7322 5d0d 0a0d  s = ["tests"]...
-00000960: 0a5b 746f 6f6c 2e62 6c61 636b 5d0d 0a20  .[tool.black].. 
-00000970: 2020 206c 696e 652d 6c65 6e67 7468 203d     line-length =
-00000980: 2031 3230 0d0a 0d0a 5b74 6f6f 6c2e 6973   120....[tool.is
-00000990: 6f72 745d 0d0a 2020 2020 7072 6f66 696c  ort]..    profil
-000009a0: 6520 3d20 2262 6c61 636b 220d 0a0d 0a5b  e = "black"....[
-000009b0: 746f 6f6c 2e6d 7970 795d 0d0a 2020 2020  tool.mypy]..    
-000009c0: 6368 6563 6b5f 756e 7479 7065 645f 6465  check_untyped_de
-000009d0: 6673 203d 2074 7275 650d 0a20 2020 2069  fs = true..    i
-000009e0: 676e 6f72 655f 6d69 7373 696e 675f 696d  gnore_missing_im
-000009f0: 706f 7274 7320 3d20 7472 7565 0d0a 2020  ports = true..  
-00000a00: 2020 6d79 7079 5f70 6174 6820 3d20 2273    mypy_path = "s
-00000a10: 7263 220d 0a20 2020 2077 6172 6e5f 6e6f  rc"..    warn_no
-00000a20: 5f72 6574 7572 6e20 3d20 6661 6c73 65    _return = false
+000001c0: 332e 3132 222c 0d0a 2020 2020 2020 2020  3.12",..        
+000001d0: 2254 6f70 6963 203a 3a20 4d75 6c74 696d  "Topic :: Multim
+000001e0: 6564 6961 203a 3a20 5669 6465 6f22 2c0d  edia :: Video",.
+000001f0: 0a20 2020 2020 2020 2022 546f 7069 6320  .        "Topic 
+00000200: 3a3a 2055 7469 6c69 7469 6573 222c 0d0a  :: Utilities",..
+00000210: 2020 2020 5d0d 0a20 2020 2064 6570 656e      ]..    depen
+00000220: 6465 6e63 6965 7320 3d20 5b0d 0a20 2020  dencies = [..   
+00000230: 2020 2020 2022 7069 636f 6c6f 6767 696e       "picologgin
+00000240: 673d 3d30 2e39 2e33 222c 0d0a 2020 2020  g==0.9.3",..    
+00000250: 2020 2020 2263 6c6f 7564 7363 7261 7065      "cloudscrape
+00000260: 723d 3d31 2e32 2e37 3122 2c0d 0a20 2020  r==1.2.71",..   
+00000270: 2020 2020 2022 6e75 6d32 776f 7264 733d       "num2words=
+00000280: 3d30 2e35 2e31 3322 2c0d 0a20 2020 2020  =0.5.13",..     
+00000290: 2020 2022 7061 636b 6167 696e 673d 3d32     "packaging==2
+000002a0: 342e 3022 2c0d 0a20 2020 2020 2020 2022  4.0",..        "
+000002b0: 7069 6c6c 6f77 3d3d 3130 2e33 2e30 222c  pillow==10.3.0",
+000002c0: 0d0a 2020 2020 2020 2020 2270 7973 7472  ..        "pystr
+000002d0: 6179 3d3d 302e 3139 2e35 222c 0d0a 2020  ay==0.19.5",..  
+000002e0: 2020 2020 2020 2272 6571 7565 7374 733d        "requests=
+000002f0: 3d32 2e33 312e 3022 2c0d 0a20 2020 2020  =2.31.0",..     
+00000300: 2020 2022 7365 6c65 6374 6f6c 6178 3d3d     "selectolax==
+00000310: 302e 332e 3231 222c 0d0a 2020 2020 2020  0.3.21",..      
+00000320: 2020 2274 6f6d 6c3d 3d30 2e31 302e 3222    "toml==0.10.2"
+00000330: 2c0d 0a20 2020 205d 0d0a 2020 2020 6465  ,..    ]..    de
+00000340: 7363 7269 7074 696f 6e20 3d20 2253 7562  scription = "Sub
+00000350: 7365 6172 6368 220d 0a20 2020 2064 796e  search"..    dyn
+00000360: 616d 6963 203d 205b 2276 6572 7369 6f6e  amic = ["version
+00000370: 225d 0d0a 2020 2020 6b65 7977 6f72 6473  "]..    keywords
+00000380: 203d 205b 0d0a 2020 2020 2020 2020 2273   = [..        "s
+00000390: 7562 7469 746c 6573 222c 0d0a 2020 2020  ubtitles",..    
+000003a0: 2020 2020 2273 7562 222c 0d0a 2020 2020      "sub",..    
+000003b0: 2020 2020 2273 7274 222c 0d0a 2020 2020      "srt",..    
+000003c0: 2020 2020 2274 6f6f 6c22 2c0d 0a20 2020      "tool",..   
+000003d0: 2020 2020 2022 746f 6f6c 7322 2c0d 0a20       "tools",.. 
+000003e0: 2020 2020 2020 2022 646f 776e 6c6f 6164         "download
+000003f0: 222c 0d0a 2020 2020 2020 2020 226d 6f76  ",..        "mov
+00000400: 6965 7322 2c0d 0a20 2020 2020 2020 2022  ies",..        "
+00000410: 7368 6f77 7322 2c0d 0a20 2020 2020 2020  shows",..       
+00000420: 2022 7363 7261 7065 222c 0d0a 2020 2020   "scrape",..    
+00000430: 2020 2020 226f 7065 6e73 7562 7469 746c      "opensubtitl
+00000440: 6573 222c 0d0a 2020 2020 2020 2020 2273  es",..        "s
+00000450: 7562 7363 656e 6522 2c0d 0a20 2020 2020  ubscene",..     
+00000460: 2020 2022 7375 6273 6561 7263 6822 2c0d     "subsearch",.
+00000470: 0a20 2020 2020 2020 2022 7375 6274 6974  .        "subtit
+00000480: 6c65 7322 2c0d 0a20 2020 2020 2020 2022  les",..        "
+00000490: 7969 6679 7375 6274 6974 6c65 7322 2c0d  yifysubtitles",.
+000004a0: 0a20 2020 205d 0d0a 2020 2020 6c69 6365  .    ]..    lice
+000004b0: 6e73 6520 3d20 7b74 6578 7420 3d20 224d  nse = {text = "M
+000004c0: 4954 206c 6963 656e 7365 227d 0d0a 2020  IT license"}..  
+000004d0: 2020 6e61 6d65 203d 2022 5375 6273 6561    name = "Subsea
+000004e0: 7263 6822 0d0a 2020 2020 7265 6164 6d65  rch"..    readme
+000004f0: 203d 2022 5245 4144 4d45 2e6d 6422 0d0a   = "README.md"..
+00000500: 2020 2020 7265 7175 6972 6573 2d70 7974      requires-pyt
+00000510: 686f 6e20 3d20 223e 3d33 2e31 3222 0d0a  hon = ">=3.12"..
+00000520: 0d0a 5b70 726f 6a65 6374 2e75 726c 735d  ..[project.urls]
+00000530: 0d0a 2020 2020 7265 706f 7369 746f 7279  ..    repository
+00000540: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
+00000550: 7562 2e63 6f6d 2f76 6167 6162 6f6e 6448  ub.com/vagabondH
+00000560: 7573 746c 6572 2f73 7562 7365 6172 6368  ustler/subsearch
+00000570: 220d 0a0d 0a5b 7072 6f6a 6563 742e 7363  "....[project.sc
+00000580: 7269 7074 735d 0d0a 2020 2020 7375 6273  ripts]..    subs
+00000590: 6561 7263 6820 3d20 2273 7562 7365 6172  earch = "subsear
+000005a0: 6368 3a6d 6169 6e22 0d0a 0d0a 5b74 6f6f  ch:main"....[too
+000005b0: 6c2e 7365 7475 7074 6f6f 6c73 5d0d 0a20  l.setuptools].. 
+000005c0: 2020 2070 6c61 7466 6f72 6d73 203d 205b     platforms = [
+000005d0: 2277 696e 3332 225d 0d0a 2020 2020 7a69  "win32"]..    zi
+000005e0: 702d 7361 6665 203d 2066 616c 7365 0d0a  p-safe = false..
+000005f0: 0d0a 5b74 6f6f 6c2e 7365 7475 7074 6f6f  ..[tool.setuptoo
+00000600: 6c73 2e70 6163 6b61 6765 732e 6669 6e64  ls.packages.find
+00000610: 5d0d 0a20 2020 2065 7863 6c75 6465 203d  ]..    exclude =
+00000620: 205b 2265 7861 6d70 6c65 732a 222c 2022   ["examples*", "
+00000630: 7375 6273 6561 7263 682e 7465 7374 2a22  subsearch.test*"
+00000640: 2c20 2274 6f6f 6c73 2a22 5d0d 0a20 2020  , "tools*"]..   
+00000650: 2069 6e63 6c75 6465 203d 205b 2273 7562   include = ["sub
+00000660: 7365 6172 6368 2a22 5d0d 0a20 2020 2077  search*"]..    w
+00000670: 6865 7265 203d 205b 2273 7263 225d 0d0a  here = ["src"]..
+00000680: 0d0a 5b74 6f6f 6c2e 7365 7475 7074 6f6f  ..[tool.setuptoo
+00000690: 6c73 2e64 796e 616d 6963 5d0d 0a20 2020  ls.dynamic]..   
+000006a0: 2076 6572 7369 6f6e 203d 207b 6174 7472   version = {attr
+000006b0: 203d 2022 7375 6273 6561 7263 682e 6461   = "subsearch.da
+000006c0: 7461 2e5f 5f76 6572 7369 6f6e 5f5f 227d  ta.__version__"}
+000006d0: 0d0a 0d0a 5b70 726f 6a65 6374 2e6f 7074  ....[project.opt
+000006e0: 696f 6e61 6c2d 6465 7065 6e64 656e 6369  ional-dependenci
+000006f0: 6573 5d0d 0a20 2020 2062 7569 6c64 203d  es]..    build =
+00000700: 205b 0d0a 2020 2020 2020 2020 2262 7569   [..        "bui
+00000710: 6c64 3d3d 312e 322e 3122 2c0d 0a20 2020  ld==1.2.1",..   
+00000720: 2020 2020 2022 6378 5f46 7265 657a 653d       "cx_Freeze=
+00000730: 3d37 2e30 2e30 222c 0d0a 2020 2020 2020  =7.0.0",..      
+00000740: 2020 2274 7769 6e65 3d3d 352e 302e 3022    "twine==5.0.0"
+00000750: 2c0d 0a20 2020 2020 2020 2022 7073 7574  ,..        "psut
+00000760: 696c 3d3d 352e 392e 3822 2c0d 0a20 2020  il==5.9.8",..   
+00000770: 205d 0d0a 2020 2020 6c69 6e74 203d 205b   ]..    lint = [
+00000780: 2262 6c61 636b 3d3d 3234 2e34 2e32 222c  "black==24.4.2",
+00000790: 2022 6973 6f72 743d 3d35 2e31 332e 3222   "isort==5.13.2"
+000007a0: 5d0d 0a20 2020 2074 6573 7473 203d 205b  ]..    tests = [
+000007b0: 0d0a 2020 2020 2020 2020 2270 7974 6573  ..        "pytes
+000007c0: 742d 636f 763d 3d35 2e30 2e30 222c 0d0a  t-cov==5.0.0",..
+000007d0: 2020 2020 2020 2020 2270 7974 6573 743d          "pytest=
+000007e0: 3d38 2e32 2e30 222c 0d0a 2020 2020 2020  =8.2.0",..      
+000007f0: 2020 2274 6f78 3d3d 342e 3135 2e30 222c    "tox==4.15.0",
+00000800: 0d0a 2020 2020 2020 2020 2270 7974 686f  ..        "pytho
+00000810: 6e2d 646f 7465 6e76 3d3d 312e 302e 3122  n-dotenv==1.0.1"
+00000820: 2c0d 0a20 2020 205d 0d0a 2020 2020 746f  ,..    ]..    to
+00000830: 6f6c 7320 3d20 5b22 7079 7065 7263 6c69  ols = ["pypercli
+00000840: 703d 3d31 2e38 2e32 225d 0d0a 2020 2020  p==1.8.2"]..    
+00000850: 7479 7065 203d 205b 226d 7970 793d 3d31  type = ["mypy==1
+00000860: 2e31 302e 3022 5d0d 0a0d 0a5b 746f 6f6c  .10.0"]....[tool
+00000870: 2e70 7974 6573 742e 696e 695f 6f70 7469  .pytest.ini_opti
+00000880: 6f6e 735d 0d0a 2020 2020 6164 646f 7074  ons]..    addopt
+00000890: 7320 3d20 222d 2d63 6f76 3d73 7263 2f73  s = "--cov=src/s
+000008a0: 7562 7365 6172 6368 220d 0a20 2020 2066  ubsearch"..    f
+000008b0: 696c 7465 7277 6172 6e69 6e67 7320 3d20  ilterwarnings = 
+000008c0: 5b27 6967 6e6f 7265 3a3a 4465 7072 6563  ['ignore::Deprec
+000008d0: 6174 696f 6e57 6172 6e69 6e67 275d 0d0a  ationWarning']..
+000008e0: 2020 2020 6c6f 675f 636c 6920 3d20 7472      log_cli = tr
+000008f0: 7565 0d0a 2020 2020 6c6f 675f 636c 695f  ue..    log_cli_
+00000900: 6c65 7665 6c20 3d20 2744 4542 5547 270d  level = 'DEBUG'.
+00000910: 0a20 2020 2074 6573 7470 6174 6873 203d  .    testpaths =
+00000920: 205b 2274 6573 7473 225d 0d0a 0d0a 5b74   ["tests"]....[t
+00000930: 6f6f 6c2e 626c 6163 6b5d 0d0a 2020 2020  ool.black]..    
+00000940: 6c69 6e65 2d6c 656e 6774 6820 3d20 3132  line-length = 12
+00000950: 300d 0a0d 0a5b 746f 6f6c 2e69 736f 7274  0....[tool.isort
+00000960: 5d0d 0a20 2020 2070 726f 6669 6c65 203d  ]..    profile =
+00000970: 2022 626c 6163 6b22 0d0a 0d0a 5b74 6f6f   "black"....[too
+00000980: 6c2e 6d79 7079 5d0d 0a20 2020 2063 6865  l.mypy]..    che
+00000990: 636b 5f75 6e74 7970 6564 5f64 6566 7320  ck_untyped_defs 
+000009a0: 3d20 7472 7565 0d0a 2020 2020 6967 6e6f  = true..    igno
+000009b0: 7265 5f6d 6973 7369 6e67 5f69 6d70 6f72  re_missing_impor
+000009c0: 7473 203d 2074 7275 650d 0a20 2020 206d  ts = true..    m
+000009d0: 7970 795f 7061 7468 203d 2022 7372 6322  ypy_path = "src"
+000009e0: 0d0a 2020 2020 7761 726e 5f6e 6f5f 7265  ..    warn_no_re
+000009f0: 7475 726e 203d 2066 616c 7365            turn = false
```

### Comparing `subsearch-2.44.1/src/Subsearch.egg-info/PKG-INFO` & `subsearch-2.45.0/src/Subsearch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: Subsearch
-Version: 2.44.1
+Version: 2.45.0
 Summary: Subsearch
 Author: vagabondHustler
 Author-email: vagabondHustler.github@gmail.com
 License: MIT license
 Project-URL: repository, https://github.com/vagabondHustler/subsearch
 Keywords: subtitles,sub,srt,tool,tools,download,movies,shows,scrape,opensubtitles,subscene,subsearch,subtitles,yifysubtitles
 Platform: win32
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Utilities
-Requires-Python: >=3.10
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: picologging==0.9.3
 Requires-Dist: cloudscraper==1.2.71
 Requires-Dist: num2words==0.5.13
 Requires-Dist: packaging==24.0
 Requires-Dist: pillow==10.3.0
@@ -45,21 +44,20 @@
 Provides-Extra: type
 Requires-Dist: mypy==1.10.0; extra == "type"
 
 <h1 align="center"><img src="https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/subsearch_v2.png"/></h1>
 
 <div align="center">
 
-![Tests](https://img.shields.io/github/actions/workflow/status/vagabondhustler/subsearch/ci.yml?style=flat-square&labelColor=1e1e2e&label=ci)
-![Tags](https://img.shields.io/github/v/tag/vagabondhustler/subsearch?style=flat-square&labelColor=1e1e2e)
-![GitHub commit activity](https://img.shields.io/github/commit-activity/m/vagabondhustler/subsearch?&style=flat-square&labelColor=1e1e2e)
-![License](https://img.shields.io/github/license/vagabondhustler/SUbSearch?&style=flat-square&labelColor=1e1e2e)
-
-![downloads-total)](https://img.shields.io/github/downloads/vagabondhustler/subsearch/total?style=flat-square&label=downloads%40total&labelColor=%231e1e2e)
-![downloads-latest)](https://img.shields.io/github/downloads/vagabondhustler/subsearch/latest/total?style=flat-square&label=downloads%40latest&labelColor=%231e1e2e)
+![tests](https://img.shields.io/github/actions/workflow/status/vagabondhustler/subsearch/ci.yml?style=flat-square&labelColor=1e1e2e&label=ci)
+![github_commit_activity](https://img.shields.io/github/last-commit/vagabondhustler/subsearch?&style=flat-square&labelColor=1e1e2e&label=commit%20activity)
+![python_version](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2FvagabondHustler%2Fsubsearch%2Fmain%2Fpyproject.toml&style=flat-square&labelColor=1e1e2e)
+![release](https://img.shields.io/github/v/tag/vagabondhustler/subsearch?style=flat-square&labelColor=1e1e2e&label=latest%20release)
+![downloads-total)](https://img.shields.io/github/downloads/vagabondhustler/subsearch/total?style=flat-square&labelColor=%231e1e2e&label=downloads)
+![license](https://img.shields.io/github/license/vagabondhustler/subsearch?&style=flat-square&labelColor=1e1e2e)
 
 </div>
 
 #### Readme Table of Contents
 
 - [About](#about)
 - [Preview of GUI](#preview)
@@ -115,41 +113,33 @@
 
 </div>
 
 ## Installation and usage <a name = "getting_started_src"></a>
 
 #### Install from pypi: <a name = "pypi"></a>
 
-Requires Python 3.10+
-
 - Install Subsearch by running `pip install subsearch` in the command prompt.
 - Launch the app by running `subsearch` in the command prompt.
 
 #### Clone from github <a name = "clone"></a>
 
-Requires Python *3.10+
-
 - Clone the Subsearch repository by running `git clone https://github.com/vagabondHustler/subsearch.git`.
 - Install Subsearch by running `pip install -e .` or *`pip install -e .[build,lint,tests,tools,type]` for optional dependencies.
 - Build the executable and MSI installer by running `python -m tools.cx_freeze_build bdist_msi`.
 
-> [!IMPORTANT]  
-> ###### If you are using Python 3.12+ and cx_Freeze, please refer to [this issue](https://github.com/marcelotduarte/cx_Freeze/issues/2153).
-
 #### Windows installer <a name = "msi"></a>
 
 Requires windows 10/11, probably works on 8.
 
 - Download the windows installer "Subsearch-x.x.x-win64.msi" from [here](https://github.com/vagabondHustler/subsearch/releases).
 - Run the installer.
 - If you receive a PUA message, click "More info" → "Run anyway".
 - Run Subsearch at least once for all the context menu options to appear
 
-> [!NOTE]  
-> ###### Development builds can be located in the [release](https://github.com/vagabondHustler/subsearch/actions/workflows/release.yml) action job, within the generated artifacts.
+###### Development builds can be located in the [release](https://github.com/vagabondHustler/subsearch/actions/workflows/release.yml) action job, within the generated artifacts.
 
 <details>
 <summary>Screenshots of PUA message<a name = "pua"></a></summary>
 
 ![prtsc_moreinfo](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/moreinfo.png)
 
 ![prtsc_runanyway](https://raw.githubusercontent.com/vagabondHustler/SubSearch/main/assets/runanyway.png)
@@ -158,12 +148,12 @@
 
 </details>
 
 More about potentially unwanted applications (PUA) can be found [here](https://support.microsoft.com/en-us/windows/protect-your-pc-from-potentially-unwanted-applications-c7668a25-174e-3b78-0191-faf0607f7a6e) on Microsoft's support page.
 
 ## Acknowledgements<a name = "thanks"></a>
 
-I would like to express my gratitude to the following repositories for providing templates, scripts, inspiration, themes, and solutions to similar problems:
+The following repositories provided templates, scripts, inspiration, themes, etc:
 
 - [zavoloklom/material-design-iconic-font](https://github.com/zavoloklom/material-design-iconic-font) // icons
 - [rdbende/Sun-Valley-ttk-theme](https://github.com/rdbende/Sun-Valley-ttk-theme) // base theme
 - [TransparentLC](https://github.com/TransparentLC) // spritesheet_generator.js
```

### Comparing `subsearch-2.44.1/src/Subsearch.egg-info/SOURCES.txt` & `subsearch-2.45.0/src/Subsearch.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 src/subsearch/__main__.py
 src/subsearch/core.py
 src/subsearch/data/__init__.py
 src/subsearch/data/guid.py
 src/subsearch/data/language_data.toml
 src/subsearch/data/version.py
 src/subsearch/globals/__init__.py
+src/subsearch/globals/_logging.py
 src/subsearch/globals/constants.py
 src/subsearch/globals/dataclasses.py
 src/subsearch/globals/decorators.py
 src/subsearch/globals/exceptions.py
 src/subsearch/globals/metaclasses.py
-src/subsearch/globals/propagating_thread.py
+src/subsearch/globals/thread_handle.py
 src/subsearch/gui/__init__.py
 src/subsearch/gui/common_utils.py
 src/subsearch/gui/resource_loader.py
 src/subsearch/gui/screen_manager.py
 src/subsearch/gui/system_tray.py
 src/subsearch/gui/resources/__init__.py
 src/subsearch/gui/resources/config.py
@@ -48,12 +49,11 @@
 src/subsearch/providers/opensubtitles.py
 src/subsearch/providers/subscene.py
 src/subsearch/providers/yifysubtitles.py
 src/subsearch/utils/__init__.py
 src/subsearch/utils/imdb_lookup.py
 src/subsearch/utils/io_app.py
 src/subsearch/utils/io_file_system.py
-src/subsearch/utils/io_log.py
 src/subsearch/utils/io_toml.py
 src/subsearch/utils/io_winreg.py
 src/subsearch/utils/string_parser.py
 src/subsearch/utils/update.py
```

### Comparing `subsearch-2.44.1/src/subsearch/__init__.py` & `subsearch-2.45.0/src/subsearch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 import time
 from pathlib import Path
 
-
 from subsearch import core
 from subsearch.globals import decorators
 
 PREF_COUNTER = time.perf_counter()
 PACKAGE_PATH = Path(__file__).resolve().parent.as_posix()
 HOME_PATH = Path(PACKAGE_PATH).parent.as_posix()
 sys.path.append(HOME_PATH)
@@ -14,15 +13,15 @@
 
 
 class Subsearch:
     def __init__(self) -> None:
         self.subsearch_core = core.SubsearchCore(PREF_COUNTER)
 
     def search_for_subtitles(self) -> None:
-        self.subsearch_core.search_for_subtitles(
+        self.subsearch_core.init_search(
             self.provider_opensubtitles,
             self.provider_subscene,
             self.provider_yifysubtitles,
         )
 
     def provider_opensubtitles(self) -> None:
         self.subsearch_core.opensubtitles()
```

### Comparing `subsearch-2.44.1/src/subsearch/core.py` & `subsearch-2.45.0/src/subsearch/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,64 @@
 import ctypes
 import time
 from pathlib import Path
-from subsearch.globals import propagating_thread
-from subsearch.globals.constants import APP_PATHS, DEVICE_INFO, FILE_PATHS, VIDEO_FILE, VERSION
+from typing import Callable
+
+from subsearch.globals import decorators, log, thread_handle
+from subsearch.globals.constants import APP_PATHS, DEVICE_INFO, FILE_PATHS, VIDEO_FILE
 from subsearch.globals.dataclasses import Subtitle
-from subsearch.globals import decorators
 from subsearch.gui import screen_manager, system_tray
 from subsearch.gui.screens import download_manager
 from subsearch.providers import opensubtitles, subscene, yifysubtitles
-from subsearch.utils import (
-    io_file_system,
-    io_log,
-    io_toml,
-    string_parser,
-)
+from subsearch.utils import io_file_system, io_toml, string_parser
 
 
 class Initializer:
     def __init__(self, pref_counter: float) -> None:
-        io_log.log.brackets("Initializing")
-        io_log.log.stdout(f"Loading components...", level="info", end_new_line=True)
+        log.brackets("Initializing")
+        log.stdout(f"Loading components...", level="info", end_new_line=True)
         self.file_exist = True if VIDEO_FILE else False
         self.setup_file_system()
         self.start = pref_counter
 
         self.app_config = io_toml.get_app_config(FILE_PATHS.config)
-        io_log.log.dataclass(DEVICE_INFO, level="debug", print_allowed=False)
-        io_log.log.dataclass(self.app_config, level="debug", print_allowed=False)
+        log.dataclass(DEVICE_INFO, level="debug", print_allowed=False)
+        log.dataclass(self.app_config, level="debug", print_allowed=False)
         decorators.enable_system_tray = self.app_config.system_tray
         self.system_tray = system_tray.SystemTray()
         self.system_tray.start()
 
         if self.file_exist:
             VIDEO_FILE.file_hash = io_file_system.get_file_hash(VIDEO_FILE.file_path)
-            io_log.log.dataclass(VIDEO_FILE, level="debug", print_allowed=False)
+            log.dataclass(VIDEO_FILE, level="debug", print_allowed=False)
             io_file_system.create_directory(VIDEO_FILE.file_directory)
 
         self.downloaded_subtitles = 0
         self.ran_download_tab = False
         self.accepted_subtitles: list[Subtitle] = []
         self.rejected_subtitles: list[Subtitle] = []
         self.manually_accepted_subtitles: list[Subtitle] = []
         self.language_data = io_toml.load_toml_data(FILE_PATHS.language_data)
 
         if self.file_exist:
             self.release_data = string_parser.get_release_data(VIDEO_FILE.filename)
-            io_log.log.dataclass(self.release_data, level="debug", print_allowed=False)
+            log.dataclass(self.release_data, level="debug", print_allowed=False)
             provider_urls = string_parser.CreateProviderUrls(self.app_config, self.release_data, self.language_data)
             self.provider_urls = provider_urls.retrieve_urls()
-            io_log.log.dataclass(self.provider_urls, level="debug", print_allowed=False)
+            log.dataclass(self.provider_urls, level="debug", print_allowed=False)
             self.search_kwargs = dict(
                 release_data=self.release_data,
                 app_config=self.app_config,
                 provider_urls=self.provider_urls,
                 language_data=self.language_data,
             )
-        io_log.log.task_completed()
+        log.task_completed()
 
     def setup_file_system(self) -> None:
-        io_log.log.stdout("Verifing files and paths", level="debug")
+        log.stdout("Verifing files and paths", level="debug")
         io_file_system.create_directory(APP_PATHS.tmp_dir)
         io_file_system.create_directory(APP_PATHS.appdata_subsearch)
         io_toml.resolve_on_integrity_failure()
         io_file_system.del_directory_content(APP_PATHS.tmp_dir)
         if self.file_exist:
             io_file_system.create_directory(VIDEO_FILE.subs_dir)
             io_file_system.create_directory(VIDEO_FILE.tmp_dir)
@@ -79,28 +75,37 @@
 
 
 class SubsearchCore(Initializer):
     def __init__(self, pref_counter: float) -> None:
         Initializer.__init__(self, pref_counter)
         ctypes.windll.kernel32.SetConsoleTitleW(f"subsearch - {DEVICE_INFO.subsearch}")
         if not self.file_exist:
-            io_log.log.brackets("GUI")
+            log.brackets("GUI")
             screen_manager.open_screen("search_options")
-            io_log.log.stdout("Exiting GUI", level="debug")
+            log.stdout("Exiting GUI", level="debug")
             return None
 
         if " " in VIDEO_FILE.filename:
-            io_log.log.stdout(f"{VIDEO_FILE.filename} contains spaces, result may vary", level="warning")
+            log.stdout(f"{VIDEO_FILE.filename} contains spaces, result may vary", level="warning")
 
         if not self.all_providers_disabled():
-            io_log.log.brackets("Search started")
+            log.brackets("Search started")
 
-    def search_for_subtitles(self, *tasks) -> None:
-        propagating_thread.handle_tasks(*tasks)
-        io_log.log.task_completed()
+    @decorators.call_func
+    def init_search(self, *providers: Callable[..., None]) -> None:
+        self._create_threads(*providers)
+        log.task_completed()
+
+    def _create_threads(self, *tasks) -> None:
+        for thread_count, target in enumerate(tasks, start=1):
+            func_name = str(target.__name__).split("_")[-1]
+            name = f"thread_{thread_count}_{func_name}"
+            task_thread = thread_handle.CreateThread(target=target, name=name)
+            task_thread.start()
+            task_thread.join()
 
     def start_search(self, provider, flag: str = "") -> None:
         search_provider = provider(**self.search_kwargs)
         if flag:
             search_provider.start_search(flag=flag)
         else:
             search_provider.start_search()
@@ -118,94 +123,94 @@
 
     @decorators.call_func
     def yifysubtitles(self) -> None:
         self.start_search(provider=yifysubtitles.YifiSubtitles)
 
     @decorators.call_func
     def download_files(self) -> None:
-        io_log.log.brackets(f"Downloading subtitles")
+        log.brackets(f"Downloading subtitles")
         index_size = len(self.accepted_subtitles)
         for enum, subtitle in enumerate(self.accepted_subtitles, 1):
             io_file_system.download_subtitle(subtitle, enum, index_size)
             self.downloaded_subtitles += 1
-        io_log.log.task_completed()
+        log.task_completed()
 
     @decorators.call_func
     def download_manager(self) -> None:
-        io_log.log.brackets(f"Download Manager")
+        log.brackets(f"Download Manager")
         subtitles = self.rejected_subtitles + self.accepted_subtitles
         screen_manager.open_screen("download_manager", subtitles=subtitles)
         self.manually_accepted_subtitles.extend(download_manager.DownloadManager.downloaded_subtitle)
-        io_log.log.task_completed()
+        log.task_completed()
 
     @decorators.call_func
     def extract_files(self) -> None:
-        io_log.log.brackets("Extracting downloads")
+        log.brackets("Extracting downloads")
         io_file_system.extract_files_in_dir(VIDEO_FILE.tmp_dir, VIDEO_FILE.subs_dir)
-        io_log.log.task_completed()
+        log.task_completed()
 
     @decorators.call_func
     def subtitle_post_processing(self):
         target = self.app_config.subtitle_post_processing["target_path"]
         resolution = self.app_config.subtitle_post_processing["path_resolution"]
         target_path = io_file_system.create_path_from_string(target, resolution)
         self.subtitle_rename()
         self.subtitle_move_best(target_path)
         self.subtitle_move_all(target_path)
 
     @decorators.call_func
     def subtitle_rename(self) -> None:
-        io_log.log.brackets("Renaming best match")
+        log.brackets("Renaming best match")
         new_name = io_file_system.autoload_rename(VIDEO_FILE.filename, ".srt")
         self.autoload_src = new_name
-        io_log.log.task_completed()
+        log.task_completed()
 
     @decorators.call_func
     def subtitle_move_best(self, target: Path) -> None:
-        io_log.log.brackets("Move best match")
+        log.brackets("Move best match")
         io_file_system.move_and_replace(self.autoload_src, target)
-        io_log.log.task_completed()
+        log.task_completed()
 
     @decorators.call_func
     def subtitle_move_all(self, target: Path) -> None:
-        io_log.log.brackets("Move all")
+        log.brackets("Move all")
         io_file_system.move_all(VIDEO_FILE.subs_dir, target)
-        io_log.log.task_completed()
+        log.task_completed()
 
     @decorators.call_func
     def summary_notification(self, elapsed) -> None:
-        io_log.log.brackets("Summary toast")
+        log.brackets("Summary toast")
         elapsed_summary = f"Finished in {elapsed} seconds"
         tot_num_of_subtitles = len(self.accepted_subtitles) + len(self.rejected_subtitles)
         matches_downloaded = f"Downloaded: {self.downloaded_subtitles}/{tot_num_of_subtitles}"
         if self.downloaded_subtitles > 0:
             msg = "Search Succeeded", f"{matches_downloaded}\n{elapsed_summary}"
-            io_log.log.stdout(matches_downloaded, hex_color="#a6e3a1")
+            log.stdout(matches_downloaded, hex_color="#a6e3a1")
             self.system_tray.display_toast(*msg)
         elif self.downloaded_subtitles == 0:
             msg = "Search Failed", f"{matches_downloaded}\n{elapsed_summary}"
-            io_log.log.stdout(matches_downloaded, hex_color="#f38ba8")
+            log.stdout(matches_downloaded, hex_color="#f38ba8")
             self.system_tray.display_toast(*msg)
 
     @decorators.call_func
     def clean_up(self) -> None:
-        io_log.log.brackets("Cleaning up")
+        log.brackets("Cleaning up")
         io_file_system.del_file_type(VIDEO_FILE.subs_dir, ".nfo")
         io_file_system.del_directory_content(APP_PATHS.tmp_dir)
         io_file_system.del_directory(VIDEO_FILE.tmp_dir)
         if io_file_system.directory_is_empty(VIDEO_FILE.subs_dir):
             io_file_system.del_directory(VIDEO_FILE.subs_dir)
-        io_log.log.task_completed()
+        log.task_completed()
 
     def core_on_exit(self) -> None:
-        io_log.log.brackets("Exit")
+        log.brackets("Exit")
         elapsed = time.perf_counter() - self.start
         self.summary_notification(elapsed)
         self.system_tray.stop()
-        io_log.log.stdout(f"Finished in {elapsed} seconds", hex_color="#f2cdcd")
+        log.stdout(f"Finished in {elapsed} seconds", hex_color="#f2cdcd")
         if not self.app_config.show_terminal:
             return None
         if DEVICE_INFO.mode == "executable":
             return None
 
         try:
             input("Enter to exit")
```

### Comparing `subsearch-2.44.1/src/subsearch/data/language_data.toml` & `subsearch-2.45.0/src/subsearch/data/language_data.toml`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/globals/constants.py` & `subsearch-2.45.0/src/subsearch/globals/constants.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/globals/dataclasses.py` & `subsearch-2.45.0/src/subsearch/globals/dataclasses.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/globals/decorators.py` & `subsearch-2.45.0/src/subsearch/globals/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import ctypes
-from datetime import datetime
-import inspect
 import sys
 from typing import Any, Callable, Union
 
 from subsearch import core
 from subsearch.globals import exceptions
 from subsearch.globals.constants import FILE_PATHS, GUID
 from subsearch.utils import io_toml
@@ -87,14 +85,15 @@
 
         open_dm_senario_1 = len(acc_subs) == 0 and len(rej_subs) >= 1 and cfg.open_on_no_matches
         open_dm_senario_2 = len(acc_subs) >= 1 and cfg.always_open and cfg.no_automatic_downloads
         open_dm_senario_3 = len(rej_subs) >= 1 and cfg.always_open
 
         func_name = kwargs["func_name"]
         conditions: dict[str, list[bool]] = {
+            "add_providers": [],
             "opensubtitles": [
                 _CoreSubsearchFuncCondtitons.language_compatibility("opensubtitles"),
                 cfg.providers["opensubtitles_hash"] or cfg.providers["opensubtitles_site"],
             ],
             "subscene": [
                 _CoreSubsearchFuncCondtitons.language_compatibility("subscene"),
                 cfg.providers["subscene_site"],
@@ -122,27 +121,14 @@
             "subtitle_move_all": [cfg.subtitle_post_processing["move_all"], cls.downloaded_subtitles > 1],
             "summary_notification": [cfg.summary_notification],
             "clean_up": [],
         }
         return _CoreSubsearchFuncCondtitons.eval_all_true(conditions[func_name])
 
 
-def capture_call_info(func):
-    def wrapper(*args, **kwargs):
-        frame = inspect.currentframe().f_back
-        current_time = datetime.now().time()
-        call_time = current_time.strftime("%H:%M:%S.%f")[:-3]
-        kwargs["call_module"] = frame.f_globals["__name__"].split(".")[-1]
-        kwargs["call_lineno"] = frame.f_lineno
-        kwargs["call_ct"] = call_time
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
 def system_tray_conditions(func) -> Callable:
     def wrapper(*args, **kwargs) -> Any:
         if enable_system_tray:
             return func(*args, **kwargs)
 
     return wrapper
```

### Comparing `subsearch-2.44.1/src/subsearch/globals/exceptions.py` & `subsearch-2.45.0/src/subsearch/globals/exceptions.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/globals/propagating_thread.py` & `subsearch-2.45.0/src/subsearch/globals/thread_handle.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,35 @@
+import threading
 from typing import Any
-from subsearch.utils import io_log
 
-import threading
+from subsearch.globals import log
 
 
-class PropagatingThread(threading.Thread):
+class CreateThread(threading.Thread):
     def __init__(self, *args, **kwargs) -> None:
         self._target = None
         self._args = ()
-        self._kwargs = {}
+        self._kwargs = {}  # type: ignore
         super().__init__(*args, **kwargs)
         self.exception = None
         self.return_value = None
         assert self._target
 
     def run(self) -> None:
         try:
-            io_log.log.stdout(f"Thread {self.name} started", level="debug", print_allowed=False)
+            log.stdout(f"Thread {self.name} started", level="debug", print_allowed=False)
             if self._target:
                 self.return_value = self._target(*self._args, **self._kwargs)
         except Exception as e:
-            self.exception = e
+            self.exception = e  # type: ignore
         finally:
             del self._target, self._args, self._kwargs
 
     def join(self, timeout=None) -> Any:
         super().join(timeout)
         if self.exception:
             msg = f"\nError occurred in thread {self.name}\n\tTraceback (most recent call last):\n\t\t{self.exception}"
-            io_log.log.stdout(msg, level="error", print_allowed=False)
+            log.stdout(msg, level="error", print_allowed=False)
             raise self.exception
         else:
-            io_log.log.stdout(f"Thread {self.name} finnished", level="debug", print_allowed=False)
+            log.stdout(f"Thread {self.name} finnished", level="debug", print_allowed=False)
         return self.return_value
-
-
-def handle_tasks(*tasks) -> None:
-    for thread_count, target in enumerate(tasks, start=1):
-        func_name = str(target.__name__).split("_")[-1]
-        name = f"thread_{thread_count}_{func_name}"
-        task_thread = PropagatingThread(target=target, name=name)
-        task_thread.start()
-        task_thread.join()
```

### Comparing `subsearch-2.44.1/src/subsearch/gui/__init__.py` & `subsearch-2.45.0/src/subsearch/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/common_utils.py` & `subsearch-2.45.0/src/subsearch/gui/common_utils.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/resource_loader.py` & `subsearch-2.45.0/src/subsearch/gui/resource_loader.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/resources/assets/spritesheet.png` & `subsearch-2.45.0/src/subsearch/gui/resources/assets/spritesheet.png`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/resources/assets/subsearch.ico` & `subsearch-2.45.0/src/subsearch/gui/resources/assets/subsearch.ico`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/resources/config.py` & `subsearch-2.45.0/src/subsearch/gui/resources/config.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/resources/styles/sprites.tcl` & `subsearch-2.45.0/src/subsearch/gui/resources/styles/sprites.tcl`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/resources/styles/style_subsearch.tcl` & `subsearch-2.45.0/src/subsearch/gui/resources/styles/style_subsearch.tcl`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/resources/styles/theme_setter.tcl` & `subsearch-2.45.0/src/subsearch/gui/resources/styles/theme_setter.tcl`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/screen_manager.py` & `subsearch-2.45.0/src/subsearch/gui/screen_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import tkinter as tk
 from typing import Any
 
+from subsearch.globals import log
 from subsearch.globals.dataclasses import Subtitle
 from subsearch.gui import common_utils, resource_loader, root
 from subsearch.gui.resources import config as cfg
 from subsearch.gui.screens import (
     download_manager,
     language_options,
     search_options,
     subsearch_options,
 )
-from subsearch.utils import io_log
 
 
 class ScreenManager(tk.Frame):
     def __init__(self, parent, available_screens: dict[str, Any], active_screen: str) -> None:
         tk.Frame.__init__(self, parent)
         self.configure(bg=cfg.color.default_bg_dark, width=cfg.size.width, height=82)
         relx_value = 0.0
@@ -136,14 +136,14 @@
         "language_options": LanguageOptions(root),
         "search_options": SearchOptions(root),
         "subsearch_options": SubsearchOptions(root),
         "download_manager": DownloadManager(root, **kwargs),
     }
     manager = ScreenManager(root, screens, tab_name.lower())
     manager.place(y=cfg.size.height - 82)
-    io_log.log.stdout("GUI is running", level="debug")
+    log.stdout("GUI is running", level="debug")
     root.mainloop()
 
 
 def close_mainloop(event):
     if event.keysym == "Escape":
         root.quit()
```

### Comparing `subsearch-2.44.1/src/subsearch/gui/screens/download_manager.py` & `subsearch-2.45.0/src/subsearch/gui/screens/download_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import tkinter as tk
 from tkinter import ttk
 
-from subsearch.globals.constants import VIDEO_FILE, FILE_PATHS
+from subsearch.globals import log
+from subsearch.globals.constants import FILE_PATHS, VIDEO_FILE
 from subsearch.globals.dataclasses import Subtitle
 from subsearch.gui.resources import config as cfg
 from subsearch.providers import common_utils
-from subsearch.utils import io_file_system, io_log, io_toml, string_parser
+from subsearch.utils import io_file_system, io_toml, string_parser
 
 
 class DownloadManager(ttk.LabelFrame):
     downloaded_subtitle: list[Subtitle] = []
 
     def __init__(self, parent, **kwargs) -> None:
         ttk.Labelframe.__init__(self, parent)
@@ -50,17 +51,17 @@
             self.nothing_label = tk.Label(
                 self,
                 text="It's very empty...\n\n:(",
                 font=cfg.font.cas20b,
                 fg=cfg.color.default_fg,
                 bg=cfg.color.default_bg,
                 anchor="center",
-                justify="center"
+                justify="center",
             )
-            self.nothing_label.place(x=cfg.size.height //2, y=cfg.size.width//4, anchor="center")
+            self.nothing_label.place(x=cfg.size.height // 2, y=cfg.size.width // 4, anchor="center")
 
     def fill_listbox(self) -> None:
         accept_threshold = io_toml.load_toml_value(FILE_PATHS.config, "subtitle_filters.accept_threshold")
         no_automatic_downloads = io_toml.load_toml_value(FILE_PATHS.config, "download_manager.no_automatic_downloads")
         self.listbox_index: dict[int, Subtitle] = {}
         for enum, subtitle in enumerate(self.subtitles):
             self.sub_listbox.insert(tk.END, f"{subtitle.pct_result}% {subtitle.release_name}\n")
@@ -98,15 +99,15 @@
             zip_archive = VIDEO_FILE.tmp_dir / f"{subtitle.provider}_{subtitle.release_name}_{self.download_number}.zip"
             zip_archive.unlink()
             self.update_text(selection, "✓", subtitle, cfg.color.green)
             self.download_number += 1
             self.download_index_size += 1
             self.downloaded_subtitle.append(subtitle)
         except Exception as e:
-            io_log.log.stdout(str(e), level="error")
+            log.stdout(str(e), level="error")
             self.update_text(selection, "⨯", subtitle, cfg.color.red)
             self.failed_subtitle_downloads.append(subtitle)
         finally:
             self.sub_listbox.bind("<ButtonPress-1>", self.mouse_b1_press)
 
     def update_text(self, selection: int, symbol: str, subtitle: Subtitle, color: str) -> None:
         self.sub_listbox.delete(int(selection))
```

### Comparing `subsearch-2.44.1/src/subsearch/gui/screens/language_options.py` & `subsearch-2.45.0/src/subsearch/gui/screens/language_options.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/screens/search_options.py` & `subsearch-2.45.0/src/subsearch/gui/screens/search_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import tkinter as tk
 from tkinter import ttk
 
+from subsearch.globals import log
 from subsearch.globals.constants import FILE_PATHS
 from subsearch.gui import common_utils
 from subsearch.gui.resources import config as cfg
-from subsearch.utils import io_log, io_toml, string_parser
+from subsearch.utils import io_toml, string_parser
 
 
 class Providers(ttk.Labelframe):
     def __init__(self, parent) -> None:
         ttk.Labelframe.__init__(self, parent)
         self.configure(text="Subtitle providers", padding=10)
         self.data = io_toml.load_toml_data(FILE_PATHS.config)
```

### Comparing `subsearch-2.44.1/src/subsearch/gui/screens/subsearch_options.py` & `subsearch-2.45.0/src/subsearch/gui/screens/subsearch_options.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/gui/system_tray.py` & `subsearch-2.45.0/src/subsearch/gui/system_tray.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import threading
 
 import pystray
 from PIL import Image
 
+from subsearch.globals import decorators, log, metaclasses
 from subsearch.globals.constants import APP_PATHS, VERSION
-from subsearch.globals import decorators
-from subsearch.globals import metaclasses
-from subsearch.utils import io_log
 
 
 class SystemTray(metaclass=metaclasses.Singleton):
     @decorators.system_tray_conditions
     def __init__(self) -> None:
         title = f"Subsearch {VERSION}"
         icon = Image.open(APP_PATHS.gui_assets / "subsearch.ico")
@@ -20,18 +18,18 @@
     @decorators.system_tray_conditions
     def display_toast(self, title: str, msg: str) -> None:
         self.tray.title
         self.tray.notify(msg, title)
 
     @decorators.system_tray_conditions
     def start(self) -> None:
-        io_log.log.stdout("Subsearch was added to the system tray", level="debug")
+        log.stdout("Subsearch was added to the system tray", level="debug")
         self.thread_tray.start()
 
     @decorators.system_tray_conditions
     def stop(self) -> None:
         self.tray.stop()
         self.thread_tray.join()
-        io_log.log.stdout("Subsearch was removed from the system tray", level="debug")
+        log.stdout("Subsearch was removed from the system tray", level="debug")
 
     def _run_pystray(self) -> None:
         self.tray.run()
```

### Comparing `subsearch-2.44.1/src/subsearch/providers/common_utils.py` & `subsearch-2.45.0/src/subsearch/providers/common_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import cloudscraper
 from selectolax.parser import HTMLParser
 
+from subsearch.globals import log
 from subsearch.globals.constants import FILE_PATHS, VIDEO_FILE
 from subsearch.globals.dataclasses import (
     AppConfig,
     LanguageData,
     ProviderUrls,
     ReleaseData,
     SubsceneCookie,
     Subtitle,
 )
-from subsearch.utils import io_log, io_toml, string_parser
+from subsearch.utils import io_toml, string_parser
 
 
 class CustomSubsceneHeader:
     def __init__(self, app_config: AppConfig) -> None:
         self.app_config = app_config
 
     def _get_hearing_impaired_int(self) -> int:
@@ -96,15 +97,15 @@
 
     def _process_subtitle_data(self, provider_name: str, subtitle_data: dict[str, str]):
         if not subtitle_data:
             return None
 
         for subtitle_name, subtitle_url in subtitle_data.items():
             pct_result = string_parser.calculate_match(subtitle_name, self.release)
-            io_log.log.subtitle_match(
+            log.subtitle_match(
                 provider=provider_name,
                 subtitle_name=subtitle_name,
                 result=pct_result,
                 threshold=self.app_config.accept_threshold,
             )
             if is_threshold_met(self, pct_result):
                 if provider_name == "subscene":
```

### Comparing `subsearch-2.44.1/src/subsearch/providers/opensubtitles.py` & `subsearch-2.45.0/src/subsearch/providers/opensubtitles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import re
 from typing import Any
 
+from subsearch.globals import log
 from subsearch.globals.dataclasses import Subtitle
 from subsearch.providers import common_utils
-from subsearch.utils import io_log
 
 
 class OpenSubtitlesScraper(common_utils.ProviderHelper):
     def __init__(self, **kwargs) -> None:
         common_utils.ProviderHelper.__init__(self, **kwargs)
 
     def is_opensubtitles_down(self, tree: Any) -> bool:
         is_offline = tree.css_matches("pre")
         if is_offline is False:
             return False
         offline_text = tree.css_first("pre").text()
         if offline_text.startswith("Site will be online soon"):
-            io_log.log.stdout(f"opensubtitles is down: {offline_text}", level="error")
+            log.stdout(f"opensubtitles is down: {offline_text}", level="error")
             return True
         return False
 
     def get_subtitles(self, url: str) -> dict[str, str]:
         subtitles: dict[str, str] = {}
         tree = common_utils.get_html_parser(url)
         items = tree.css("item")
@@ -57,15 +57,15 @@
 
     def search_hash(self) -> None:
         subtitle_data = self.with_hash(self.url_opensubtitles_hash, self.release)
 
         if not subtitle_data:
             return None
 
-        io_log.log.subtitle_match(
+        log.subtitle_match(
             provider=self.provider_name,
             subtitle_name=self.release,
             result=100,
             threshold=self.app_config.accept_threshold,
         )
         self._process_subtitle_data(self.provider_name, subtitle_data)
```

### Comparing `subsearch-2.44.1/src/subsearch/providers/subscene.py` & `subsearch-2.45.0/src/subsearch/providers/subscene.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/providers/yifysubtitles.py` & `subsearch-2.45.0/src/subsearch/providers/yifysubtitles.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/utils/imdb_lookup.py` & `subsearch-2.45.0/src/subsearch/utils/imdb_lookup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import re
 from typing import no_type_check
 
 from subsearch.providers import common_utils
 
 
 class AdvTitleSearch:
     def __init__(self, title: str, year: int) -> None:
@@ -48,17 +47,22 @@
 
         product = tree.css("a.ipc-title-link-wrapper h3.ipc-title__text")
 
         for item in product:
             href_ = item.parent.attrs["href"]
             imdb_id = href_.split("/")[2]
             title_ = item.text().split(". ")[-1]
-            year_ = int(item.parent.parent.next.child.child.html)
+            _year = item.parent.parent.next.child.child.html
+            release_year = self._handle_ongoing_show(_year)
 
             if self.title != title_.lower():
                 continue
 
-            if self.year != year_ and (self.year - 1) != year_:
+            if self.year != release_year and (self.year - 1) != release_year:
                 continue
 
             self.id = imdb_id
             break
+
+    def _handle_ongoing_show(self, year: str) -> int:
+        release_year = year.split("–")[0]
+        return int(release_year)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `subsearch-2.44.1/src/subsearch/utils/io_app.py` & `subsearch-2.45.0/src/subsearch/utils/io_app.py`

 * *Files identical despite different names*

### Comparing `subsearch-2.44.1/src/subsearch/utils/io_file_system.py` & `subsearch-2.45.0/src/subsearch/utils/io_file_system.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import time
 import zipfile
 from io import BufferedReader
 from pathlib import Path
 
 import requests
 
+from subsearch.globals import log
 from subsearch.globals.constants import VIDEO_FILE
 from subsearch.globals.dataclasses import Subtitle
 from subsearch.providers.common_utils import get_cloudscraper
-from subsearch.utils import io_log, string_parser
+from subsearch.utils import string_parser
 
 
 def create_path_from_string(string: str, path_resolution: str) -> Path:
     if path_resolution == "relative":
         if string == ".":
             path = VIDEO_FILE.file_directory
         elif string.startswith(".\\") and len(string) > 2:
@@ -27,93 +28,93 @@
         path = Path(string)
 
     path.mkdir(parents=True, exist_ok=True)
     return path
 
 
 def download_subtitle(subtitle: Subtitle, index_position: int, index_size: int):
-    io_log.log.stdout(f"{subtitle.provider}: {index_position}/{index_size}: {subtitle.release_name}")
+    log.stdout(f"{subtitle.provider}: {index_position}/{index_size}: {subtitle.release_name}")
     scraper = get_cloudscraper()
     r = scraper.get(subtitle.download_url, stream=True)
     file_name = f"{subtitle.provider}_{subtitle.release_name}_{index_position}.zip"
     download_path = VIDEO_FILE.tmp_dir / file_name
     with open(download_path, "wb") as fd:
         for chunk in r.iter_content(chunk_size=1024):
             fd.write(chunk)
 
 
 def extract_files_in_dir(src: Path, dst: Path, extension: str = ".zip") -> None:
     for file in src.glob(f"*{extension}"):
         filename = src / file
-        io_log.log.file_system_action(action_type="extract", src=file, dst=dst)
+        log.file_system_action(action_type="extract", src=file, dst=dst)
         zip_ref = zipfile.ZipFile(filename)
         zip_ref.extractall(dst)
         zip_ref.close()
 
 
 def autoload_rename(release_name: str, extension: str = ".srt") -> Path:
     best_match = (0, Path("."))
     for file in VIDEO_FILE.subs_dir.glob(f"*{extension}"):
         value = string_parser.calculate_match(file.name, release_name)
         if value >= best_match[0]:
             best_match = value, file
 
     old_file_path = best_match[1]
     new_file_path = old_file_path.with_name(f"{release_name}{extension}")
-    io_log.log.file_system_action(action_type="rename", src=old_file_path, dst=new_file_path)
+    log.file_system_action(action_type="rename", src=old_file_path, dst=new_file_path)
     old_file_path.rename(new_file_path)
     return new_file_path
 
 
 def move_all(src: Path, dst: Path, extension: str = ".srt"):
     for file in src.glob(f"*{extension}"):
         move_and_replace(file.absolute(), dst)
 
 
 def move_and_replace(source_file: Path, destination_directory: Path) -> None:
     source_file.replace(destination_directory / source_file.name)
-    io_log.log.file_system_action(action_type="move", src=source_file, dst=destination_directory)
+    log.file_system_action(action_type="move", src=source_file, dst=destination_directory)
 
 
 def del_file_type(cwd: Path, extension: str) -> None:
     for file in Path(cwd).glob(f"*{extension}"):
-        io_log.log.file_system_action(action_type="remove", src=file)
+        log.file_system_action(action_type="remove", src=file)
         file_path = Path(cwd) / file
         file_path.unlink()
 
 
 def del_directory(directory: Path) -> None:
-    io_log.log.file_system_action(action_type="remove", src=directory)
+    log.file_system_action(action_type="remove", src=directory)
     shutil.rmtree(directory)
 
 
 def directory_is_empty(directory: Path) -> bool:
     if not any(directory.iterdir()):
         return True
     return False
 
 
 def del_directory_content(directory: Path) -> None:
     for item in directory.iterdir():
         if not item.is_file():
             return None
-        io_log.log.file_system_action(action_type="remove", src=item)
+        log.file_system_action(action_type="remove", src=item)
         if item.is_file():
             item.unlink()
         if item.is_dir():
             shutil.rmtree(item)
 
 
 def create_directory(path: Path) -> None:
-    io_log.log.stdout(f"Creating {path}", level="debug")
+    log.stdout(f"Creating {path}", level="debug")
     path.mkdir(parents=True, exist_ok=True)
 
 
 def get_file_hash(file_path: Path) -> str:
-    io_log.log.stdout("Calculating hash of video file", level="debug")
+    log.stdout("Calculating hash of video file", level="debug")
     if not file_path:
         return ""
 
     hash_algorithm = MPCHashAlgorithm(file_path)
     return hash_algorithm.get_hash()
 
 
@@ -134,15 +135,15 @@
             self.update_hash_chunk(file)
             file.seek(max(0, self.file_size - self.chunk_size), 0)
             self.update_hash_chunk(file)
         return "%016x" % self.hash_chunk
 
     def valid_file_size(self) -> bool:
         if self.file_size < self.chunk_size * 2:
-            io_log.log.stdout(f"Invalid file size, {self.file_size} bytes", level="warning")
+            log.stdout(f"Invalid file size, {self.file_size} bytes", level="warning")
             return False
         return True
 
     def update_hash_chunk(self, file: BufferedReader) -> None:
         for _ in range(self.chunk_size // self.byte_size):
             buffer = file.read(self.byte_size)
             (chunk_value,) = struct.unpack("<q", buffer)
@@ -154,18 +155,18 @@
 
 
 def download_response(msi_package_path: Path, response: requests.Response):
     start_time = time.time()
     with open(msi_package_path, "wb") as msi_file:
         total_size = int(response.headers.get("content-length", 0))
         downloaded_size = 0
-        io_log.log.stdout(f"Download started for {msi_package_path.name}")
-        io_log.log.stdout(f"Downloading 0%")
+        log.stdout(f"Download started for {msi_package_path.name}")
+        log.stdout(f"Downloading 0%")
         for chunk in response.iter_content(chunk_size=128):
             msi_file.write(chunk)
             downloaded_size += len(chunk)
             progress_percentage = (downloaded_size / total_size) * 100
             elapsed_time = time.time() - start_time
             if elapsed_time >= 0.5:
-                io_log.log.stdout(f"Downloading {progress_percentage:.2f}%")
+                log.stdout(f"Downloading {progress_percentage:.2f}%")
                 start_time = time.time()
-        io_log.log.stdout(f"Download complete.")
+        log.stdout(f"Download complete.")
```

### Comparing `subsearch-2.44.1/src/subsearch/utils/io_log.py` & `subsearch-2.45.0/src/subsearch/globals/_logging.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,35 @@
 import dataclasses
-import picologging as logging
-from pathlib import Path
+import inspect
 import threading
+from datetime import datetime
+from pathlib import Path
 from typing import Optional, TypeVar
 
+import picologging as logging
 
-from subsearch.globals import decorators, metaclasses
-from subsearch.globals.constants import FILE_PATHS, APP_PATHS
+from subsearch.globals import metaclasses
+from subsearch.globals.constants import APP_PATHS, FILE_PATHS
 
 DATACLASS = TypeVar("DATACLASS")
 
 
+def capture_call_info(func):
+    def wrapper(*args, **kwargs):
+        frame = inspect.currentframe().f_back  # type: ignore
+        current_time = datetime.now().time()
+        call_time = current_time.strftime("%H:%M:%S.%f")[:-3]
+        kwargs["call_module"] = frame.f_globals["__name__"].split(".")[-1]  # type: ignore
+        kwargs["call_lineno"] = frame.f_lineno  # type: ignore
+        kwargs["call_ct"] = call_time
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
 class ANSIEscapeSequences:
     """
     ANSI escape sequences for text colors
     """
 
     RESET = "\033[0m"
     BOLD = "\033[1m"
@@ -92,30 +107,30 @@
 
     def log(self, message: str, **kwargs) -> None:
         end_new_line = kwargs.get("end_new_line", False)
         self._logger.log(message, **kwargs)
         if end_new_line:
             self._logger.log("", **kwargs)
 
-    @decorators.capture_call_info
+    @capture_call_info
     def stdout(self, message: str, **kwargs) -> None:
         self(message, **kwargs)
 
-    @decorators.capture_call_info
+    @capture_call_info
     def brackets(self, message: str, **kwargs) -> None:
         self(f"--- [{message}] ---", hex_color="#fab387", style="bold", **kwargs)
 
-    @decorators.capture_call_info
+    @capture_call_info
     def subtitle_match(self, provider: str, subtitle_name: str, result: int, threshold: int, **kwargs) -> None:
         if result >= threshold:
             self(f"{provider:<14}{result:>3}% {subtitle_name}", hex_color="#a6e3a1", **kwargs)
         else:
             self(f"{provider:<14}{result:>3}% {subtitle_name}", **kwargs)
 
-    @decorators.capture_call_info
+    @capture_call_info
     def file_system_action(self, action_type: str, src: Path, dst: Optional[Path] = None, **kwargs) -> None:
         if src.is_file():
             type_ = "file"
         elif src.is_dir():
             type_ = "directory"
         else:
             type_ = "item"
@@ -133,25 +148,22 @@
         message = action_messages.get(action_type)
 
         if not message:
             raise ValueError("Invalid action type")
 
         self(message, **kwargs)
 
-    @decorators.capture_call_info
+    @capture_call_info
     def dataclass(self, instance: DATACLASS, **kwargs) -> None:
         if not dataclasses.is_dataclass(instance):
             raise ValueError("Input is not a dataclass instance.")
         instance_name = f"--- [{instance.__class__.__name__}] ---"
         self(instance_name, hex_color="#fab387", style="bold", **kwargs)
         for field in dataclasses.fields(instance):
             key = field.name
             value = getattr(instance, key)
             padding = " " * (30 - len(key))
             self(f"{key}:{padding}{value}", **kwargs)
 
-    @decorators.capture_call_info
+    @capture_call_info
     def task_completed(self, **kwargs) -> None:
         self("Task completed", level="info", hex_color="#89b4fa", **kwargs)
-
-
-log = StdoutHandler()
```

### Comparing `subsearch-2.44.1/src/subsearch/utils/io_toml.py` & `subsearch-2.45.0/src/subsearch/utils/io_toml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import functools
 from pathlib import Path
 from typing import Any, Union
 
 import toml
 
+from subsearch.globals import log
 from subsearch.globals.constants import DEFAULT_CONFIG, FILE_PATHS
 from subsearch.globals.dataclasses import AppConfig
-from subsearch.utils import io_log
 
 
 def load_toml_data(toml_file_path: Path) -> dict[str, Any]:
     with open(toml_file_path, "r") as f:
         return toml.load(f)
 
 
@@ -37,23 +37,23 @@
     toml_data = load_toml_data(toml_file_path)
     keys = key.split(".")
     functools.reduce(dict.get, keys[:-1], toml_data).pop(keys[-1], None)  # type: ignore
     dump_toml_data(toml_file_path, toml_data)
 
 
 def repair_toml_config(toml_file_path: Path, valid_config_keys: list[str], config_keys: list[str]) -> None:
-    io_log.log.stdout(f"Reparing config", level="debug")
+    log.stdout(f"Reparing config", level="debug")
     obsolete_keys = [key for key in config_keys if key not in valid_config_keys]
     for key in obsolete_keys:
-        io_log.log.stdout(f"Removing obsolete key {key}", level="debug")
+        log.stdout(f"Removing obsolete key {key}", level="debug")
         del_toml_key(toml_file_path, key)
 
     missing_keys = [key for key in valid_config_keys if key not in config_keys]
     for key in missing_keys:
-        io_log.log.stdout(f"Adding missing key {key}", level="debug")
+        log.stdout(f"Adding missing key {key}", level="debug")
         keys = key.split(".")
         value = functools.reduce(dict.get, keys, DEFAULT_CONFIG)  # type: ignore
         update_toml_key(FILE_PATHS.config, key, value)
 
 
 def get_keys_recursively(dictionary: dict, prefix="", keys=None) -> list[str]:
     if keys is None:
@@ -74,31 +74,31 @@
     valid_config_keys.sort()
     config_keys.sort()
     return config_keys == valid_config_keys
 
 
 def resolve_on_integrity_failure() -> None:
     if not FILE_PATHS.config.exists():
-        io_log.log.stdout(f"No config.toml exsist, creating default at {FILE_PATHS.config}", level="debug")
+        log.stdout(f"No config.toml exsist, creating default at {FILE_PATHS.config}", level="debug")
         dump_toml_data(FILE_PATHS.config, DEFAULT_CONFIG)
         return None
     valid_config_keys = get_keys_recursively(DEFAULT_CONFIG)
     config_keys = get_keys_recursively(load_toml_data(FILE_PATHS.config))
     valid = valid_config(valid_config_keys, config_keys)
     if valid:
-        io_log.log.stdout(f"Config is valid", level="debug")
+        log.stdout(f"Config is valid", level="debug")
         return None
     try:
-        io_log.log.stdout(f"Config not valid", level="debug")
+        log.stdout(f"Config not valid", level="debug")
         repair_toml_config(FILE_PATHS.config, valid_config_keys, config_keys)
     except Exception:
-        io_log.log.stdout(f"Repair faild, creating default at {FILE_PATHS.config}", level="debug")
+        log.stdout(f"Repair faild, creating default at {FILE_PATHS.config}", level="debug")
         FILE_PATHS.config.unlink()
         dump_toml_data(FILE_PATHS.config, DEFAULT_CONFIG)
-    io_log.log.stdout(f"Repair succeeded", level="debug")
+    log.stdout(f"Repair succeeded", level="debug")
 
 
 def get_app_config(toml_file_path: Path) -> AppConfig:
     data = load_toml_data(toml_file_path)
     user_data = AppConfig(
         **data["subtitle_filters"],
         **data["gui"],
```

### Comparing `subsearch-2.44.1/src/subsearch/utils/io_winreg.py` & `subsearch-2.45.0/src/subsearch/utils/io_winreg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sys
 import winreg
 from pathlib import Path
 
+from subsearch.globals import log
 from subsearch.globals.constants import (
     APP_PATHS,
     COMPUTER_NAME,
     DEVICE_INFO,
     FILE_PATHS,
     REGISTRY_PATHS,
 )
-from subsearch.utils import io_log, io_toml
+from subsearch.utils import io_toml
 
 
 class LaunchOptions:
     def __init__(self) -> None:
         self.show_terminal = io_toml.load_toml_value(FILE_PATHS.config, "gui.show_terminal")
         self.python_path = Path(sys.executable).parent
         self.console_title = "import ctypes; ctypes.windll.kernel32.SetConsoleTitleW('subsearch');"
```

### Comparing `subsearch-2.44.1/src/subsearch/utils/string_parser.py` & `subsearch-2.45.0/src/subsearch/utils/string_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import re
 from typing import Any
 
 from num2words import num2words
 
+from subsearch.globals import log
 from subsearch.globals.constants import VIDEO_FILE
 from subsearch.globals.dataclasses import (
     AppConfig,
     LanguageData,
     ProviderUrls,
     ReleaseData,
 )
-from subsearch.utils import imdb_lookup, io_log
+from subsearch.utils import imdb_lookup
 
 
 def find_year(string: str) -> int:
     re_year = re.findall(r"^.*\.([1-2][0-9]{3})\.", string)
     if re_year:
         year = re_year[0]
         return int(year)
```

### Comparing `subsearch-2.44.1/src/subsearch/utils/update.py` & `subsearch-2.45.0/src/subsearch/utils/update.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from pathlib import Path
 import re
 import subprocess
+import sys
+from pathlib import Path
 
 import cloudscraper
+import requests
 from packaging.version import Version
 
-from subsearch.globals.constants import VERSION, APP_PATHS
-import requests
-import sys
-from subsearch.utils import io_file_system, io_log
+from subsearch.globals import log
+from subsearch.globals.constants import APP_PATHS, VERSION
+from subsearch.utils import io_file_system
 
 
 def find_semantic_version(version: str) -> str:
     # semantic expression https://regex101.com/r/M4qItH/
     pattern = r'(?<=__version__ = ")(\d+\.\d+\.\d+[a-zA-Z]*\d*).*?(?=")'
     version_semantic = "".join(re.findall(pattern, version)[0])
     return version_semantic
@@ -50,29 +51,29 @@
 
 def run_installer(msi_package_path: Path) -> None:
     command = f"msiexec.exe /i {msi_package_path}"
     subprocess.Popen(command, shell=True, creationflags=subprocess.DETACHED_PROCESS)
 
 
 def download_and_update():
-    io_log.log.brackets("Updating Application")
+    log.brackets("Updating Application")
     latest_version = get_latest_version()
     latest_msi = get_latest_msi_url(latest_version)
     if Version(VERSION) > Version(latest_version):
-        io_log.log.stdout(f"No new version available")
+        log.stdout(f"No new version available")
         return None
 
-    io_log.log.stdout(f"New version available")
+    log.stdout(f"New version available")
     if not APP_PATHS.tmp_dir.exists():
         APP_PATHS.tmp_dir.mkdir(parents=True, exist_ok=True)
     msi_package_path = APP_PATHS.tmp_dir / f"Subsearch-{latest_version}-win64.msi"
     response = requests.get(latest_msi, stream=True)
     if response.status_code == 200:
         io_file_system.download_response(msi_package_path, response)
         msg = f"MSI file downloaded to: {msi_package_path}"
-        io_log.log.stdout(f"MSI file downloaded to: {msi_package_path}")
+        log.stdout(f"MSI file downloaded to: {msi_package_path}")
     else:
         msg = f"Failed to download MSI file. HTTP Status Code: {response.status_code}"
-        io_log.log.stdout(msg, level="error")
+        log.stdout(msg, level="error")
         raise Exception(response.status_code)
     run_installer(msi_package_path)
     sys.exit()
```

