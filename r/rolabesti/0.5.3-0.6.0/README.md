# Comparing `tmp/rolabesti-0.5.3.tar.gz` & `tmp/rolabesti-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rolabesti-0.5.3.tar", last modified: Mon Mar 25 21:23:58 2024, max compression
+gzip compressed data, was "rolabesti-0.6.0.tar", max compression
```

## Comparing `rolabesti-0.5.3.tar` & `rolabesti-0.6.0.tar`

### file list

```diff
@@ -1,31 +1,45 @@
-drwxr-xr-x   0 kinuax    (1001) kinuax    (1001)        0 2024-03-25 21:23:58.000000 rolabesti-0.5.3/
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     7694 2024-03-25 21:23:58.000000 rolabesti-0.5.3/PKG-INFO
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     5603 2024-03-25 20:49:12.000000 rolabesti-0.5.3/README.rst
-drwxr-xr-x   0 kinuax    (1001) kinuax    (1001)        0 2024-03-25 21:23:58.000000 rolabesti-0.5.3/rolabesti/
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)      347 2024-03-25 21:02:19.000000 rolabesti-0.5.3/rolabesti/__init__.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     1958 2024-03-25 20:39:49.000000 rolabesti-0.5.3/rolabesti/__main__.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     6809 2022-01-28 11:15:07.000000 rolabesti-0.5.3/rolabesti/arguments.py
-drwxr-xr-x   0 kinuax    (1001) kinuax    (1001)        0 2024-03-25 21:23:58.000000 rolabesti-0.5.3/rolabesti/conf/
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)        0 2017-02-16 17:53:52.000000 rolabesti-0.5.3/rolabesti/conf/__init__.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     1290 2023-12-26 13:00:11.000000 rolabesti-0.5.3/rolabesti/conf/settings.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)      596 2023-12-26 12:59:59.000000 rolabesti-0.5.3/rolabesti/constants.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)      511 2017-02-24 15:03:10.000000 rolabesti-0.5.3/rolabesti/copier.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     1137 2023-12-26 16:12:57.000000 rolabesti-0.5.3/rolabesti/displayer.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     3912 2024-03-25 20:40:15.000000 rolabesti-0.5.3/rolabesti/mongo.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     2851 2022-01-28 10:39:17.000000 rolabesti-0.5.3/rolabesti/parser.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     2219 2024-03-25 20:41:10.000000 rolabesti-0.5.3/rolabesti/player.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)      618 2024-03-25 20:45:44.000000 rolabesti-0.5.3/rolabesti/slicer.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)      535 2024-03-25 20:46:08.000000 rolabesti-0.5.3/rolabesti/sorter.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     1235 2024-01-13 20:03:55.000000 rolabesti-0.5.3/rolabesti/tagger.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     3644 2024-03-25 20:46:27.000000 rolabesti-0.5.3/rolabesti/utils.py
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     2818 2024-03-25 20:47:00.000000 rolabesti-0.5.3/rolabesti/validator.py
-drwxr-xr-x   0 kinuax    (1001) kinuax    (1001)        0 2024-03-25 21:23:58.000000 rolabesti-0.5.3/rolabesti.egg-info/
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     7694 2024-03-25 21:23:58.000000 rolabesti-0.5.3/rolabesti.egg-info/PKG-INFO
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)      609 2024-03-25 21:23:58.000000 rolabesti-0.5.3/rolabesti.egg-info/SOURCES.txt
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)        1 2024-03-25 21:23:58.000000 rolabesti-0.5.3/rolabesti.egg-info/dependency_links.txt
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)       55 2024-03-25 21:23:58.000000 rolabesti-0.5.3/rolabesti.egg-info/entry_points.txt
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)        1 2024-03-25 21:23:58.000000 rolabesti-0.5.3/rolabesti.egg-info/not-zip-safe
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)       47 2024-03-25 21:23:58.000000 rolabesti-0.5.3/rolabesti.egg-info/requires.txt
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)       10 2024-03-25 21:23:58.000000 rolabesti-0.5.3/rolabesti.egg-info/top_level.txt
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)       96 2024-03-25 21:23:58.000000 rolabesti-0.5.3/setup.cfg
--rw-r--r--   0 kinuax    (1001) kinuax    (1001)     1611 2024-03-25 17:45:47.000000 rolabesti-0.5.3/setup.py
+-rw-r--r--   0        0        0     1068 2024-05-11 16:46:12.377432 rolabesti-0.6.0/LICENSE
+-rw-r--r--   0        0        0     9418 2024-05-12 04:36:42.078675 rolabesti-0.6.0/README.md
+-rw-r--r--   0        0        0     1889 2024-05-12 06:34:45.912927 rolabesti-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      166 2024-05-11 19:12:43.384930 rolabesti-0.6.0/rolabesti/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-12 11:20:10.830762 rolabesti-0.6.0/rolabesti/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:20:10.830762 rolabesti-0.6.0/rolabesti/cli/__init__.py
+-rw-r--r--   0        0        0      141 2024-05-05 18:57:42.420886 rolabesti-0.6.0/rolabesti/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3079 2024-05-12 04:45:21.953629 rolabesti-0.6.0/rolabesti/cli/commands/config.py
+-rw-r--r--   0        0        0     1417 2024-05-12 04:45:21.953629 rolabesti-0.6.0/rolabesti/cli/commands/copy.py
+-rw-r--r--   0        0        0      595 2024-05-05 18:57:42.420886 rolabesti-0.6.0/rolabesti/cli/commands/init.py
+-rw-r--r--   0        0        0      908 2024-05-12 04:45:21.953629 rolabesti-0.6.0/rolabesti/cli/commands/list.py
+-rw-r--r--   0        0        0     1528 2024-05-12 04:45:21.957629 rolabesti-0.6.0/rolabesti/cli/commands/play.py
+-rw-r--r--   0        0        0     1140 2024-05-12 04:45:21.957629 rolabesti-0.6.0/rolabesti/cli/commands/tag.py
+-rw-r--r--   0        0        0      986 2024-05-12 04:45:21.957629 rolabesti-0.6.0/rolabesti/cli/main.py
+-rw-r--r--   0        0        0     2298 2024-05-04 16:51:56.124018 rolabesti-0.6.0/rolabesti/cli/options.py
+-rw-r--r--   0        0        0      741 2024-05-05 16:01:36.477407 rolabesti-0.6.0/rolabesti/cli/utils.py
+-rw-r--r--   0        0        0      118 2024-05-08 07:43:06.230149 rolabesti-0.6.0/rolabesti/config/__init__.py
+-rw-r--r--   0        0        0     2293 2024-05-08 07:43:06.230149 rolabesti-0.6.0/rolabesti/config/settings.py
+-rw-r--r--   0        0        0      672 2024-05-07 11:30:09.189157 rolabesti-0.6.0/rolabesti/config/utils.py
+-rw-r--r--   0        0        0      200 2024-05-05 18:57:42.424886 rolabesti-0.6.0/rolabesti/controllers/__init__.py
+-rw-r--r--   0        0        0     1735 2024-05-08 07:43:06.230149 rolabesti-0.6.0/rolabesti/controllers/config.py
+-rw-r--r--   0        0        0      509 2024-05-08 07:43:06.230149 rolabesti-0.6.0/rolabesti/controllers/controller.py
+-rw-r--r--   0        0        0      422 2024-05-05 18:57:42.424886 rolabesti-0.6.0/rolabesti/controllers/copy.py
+-rw-r--r--   0        0        0     1294 2024-05-07 18:30:29.959704 rolabesti-0.6.0/rolabesti/controllers/init.py
+-rw-r--r--   0        0        0      225 2024-04-26 20:17:28.293354 rolabesti-0.6.0/rolabesti/controllers/list.py
+-rw-r--r--   0        0        0     4560 2024-05-08 07:43:06.230149 rolabesti-0.6.0/rolabesti/controllers/parser.py
+-rw-r--r--   0        0        0      446 2024-04-26 20:17:28.293354 rolabesti-0.6.0/rolabesti/controllers/play.py
+-rw-r--r--   0        0        0     1789 2024-05-05 18:57:42.424886 rolabesti-0.6.0/rolabesti/controllers/search.py
+-rw-r--r--   0        0        0     1720 2024-04-26 20:17:28.293354 rolabesti-0.6.0/rolabesti/controllers/tag.py
+-rw-r--r--   0        0        0      579 2024-04-30 08:19:40.016953 rolabesti-0.6.0/rolabesti/controllers/utils.py
+-rw-r--r--   0        0        0       56 2024-05-01 18:47:11.977674 rolabesti-0.6.0/rolabesti/database/__init__.py
+-rw-r--r--   0        0        0     1020 2024-05-01 18:47:11.977674 rolabesti-0.6.0/rolabesti/database/db.py
+-rw-r--r--   0        0        0     2877 2024-05-05 18:57:42.424886 rolabesti-0.6.0/rolabesti/database/mongodb.py
+-rw-r--r--   0        0        0     1945 2024-05-05 18:57:42.424886 rolabesti-0.6.0/rolabesti/database/tinydb.py
+-rw-r--r--   0        0        0      134 2024-04-25 19:15:21.544296 rolabesti-0.6.0/rolabesti/logger.py
+-rw-r--r--   0        0        0      148 2024-04-24 08:16:47.056256 rolabesti-0.6.0/rolabesti/models/__init__.py
+-rw-r--r--   0        0        0      342 2024-04-24 08:16:47.056256 rolabesti-0.6.0/rolabesti/models/filters.py
+-rw-r--r--   0        0        0      132 2024-04-24 08:16:47.056256 rolabesti-0.6.0/rolabesti/models/id3.py
+-rw-r--r--   0        0        0      107 2024-04-24 08:16:47.056256 rolabesti-0.6.0/rolabesti/models/sortings.py
+-rw-r--r--   0        0        0     1205 2024-04-24 08:16:47.056256 rolabesti-0.6.0/rolabesti/models/track.py
+-rw-r--r--   0        0        0      255 2024-05-03 12:49:49.603921 rolabesti-0.6.0/rolabesti/utils.py
+-rw-r--r--   0        0        0       33 2024-04-25 19:57:36.447931 rolabesti-0.6.0/rolabesti/views/__init__.py
+-rw-r--r--   0        0        0     4680 2024-05-11 19:20:15.304447 rolabesti-0.6.0/rolabesti/views/tracklist.py
+-rw-r--r--   0        0        0     1012 2024-05-11 19:20:15.304447 rolabesti-0.6.0/rolabesti/views/utils.py
+-rw-r--r--   0        0        0    11287 1970-01-01 00:00:00.000000 rolabesti-0.6.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

