# Comparing `tmp/fetchdep-0.0.0.tar.gz` & `tmp/fetchdep-0.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetchdep-0.0.0.tar", last modified: Sat May 11 23:35:01 2024, max compression
+gzip compressed data, was "fetchdep-0.0.0.dev0.tar", last modified: Mon May  6 01:17:39 2024, max compression
```

## Comparing `fetchdep-0.0.0.tar` & `fetchdep-0.0.0.dev0.tar`

### file list

```diff
@@ -1,121 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.657878 fetchdep-0.0.0/
--rw-r--r--   0 root         (0) root         (0)     1270 2024-05-11 23:34:57.000000 fetchdep-0.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       90 2024-05-11 23:34:57.000000 fetchdep-0.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5761 2024-05-11 23:35:01.657878 fetchdep-0.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4526 2024-05-11 23:34:57.000000 fetchdep-0.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.645878 fetchdep-0.0.0/fetchdep/
--rw-r--r--   0 root         (0) root         (0)      108 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5072 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/__main__.py
--rw-r--r--   0 root         (0) root         (0)     3702 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/config.py
--rw-r--r--   0 root         (0) root         (0)     1367 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/database.py
--rw-r--r--   0 root         (0) root         (0)     1139 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/defs.py
--rw-r--r--   0 root         (0) root         (0)     3052 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/dependency.py
--rw-r--r--   0 root         (0) root         (0)    10561 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/engine.py
--rw-r--r--   0 root         (0) root         (0)     2419 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.645878 fetchdep-0.0.0/fetchdep/fetch/
--rw-r--r--   0 root         (0) root         (0)     1830 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/fetch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1817 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/fetch/cvs.py
--rw-r--r--   0 root         (0) root         (0)      862 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/fetch/git.py
--rw-r--r--   0 root         (0) root         (0)      881 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/fetch/mercurial.py
--rw-r--r--   0 root         (0) root         (0)     1448 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/fetch/mkdir.py
--rw-r--r--   0 root         (0) root         (0)      847 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/fetch/svn.py
--rw-r--r--   0 root         (0) root         (0)     4892 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/opts.py
--rw-r--r--   0 root         (0) root         (0)     4212 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.645878 fetchdep-0.0.0/fetchdep/tool/
--rw-r--r--   0 root         (0) root         (0)     5600 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/tool/__init__.py
--rw-r--r--   0 root         (0) root         (0)      457 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/tool/cvs.py
--rw-r--r--   0 root         (0) root         (0)      542 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/tool/git.py
--rw-r--r--   0 root         (0) root         (0)      467 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/tool/hg.py
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/tool/svn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.649878 fetchdep-0.0.0/fetchdep/util/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)      764 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/util/compat.py
--rw-r--r--   0 root         (0) root         (0)      568 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/util/enum.py
--rw-r--r--   0 root         (0) root         (0)    12455 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/util/io.py
--rw-r--r--   0 root         (0) root         (0)     7482 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/util/log.py
--rw-r--r--   0 root         (0) root         (0)      729 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/util/string.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/util/tags.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-05-11 23:34:57.000000 fetchdep-0.0.0/fetchdep/util/win32.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/fetchdep.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5761 2024-05-11 23:35:01.000000 fetchdep-0.0.0/fetchdep.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2853 2024-05-11 23:35:01.000000 fetchdep-0.0.0/fetchdep.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 23:35:01.000000 fetchdep-0.0.0/fetchdep.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-11 23:35:01.000000 fetchdep-0.0.0/fetchdep.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-11 23:35:01.000000 fetchdep-0.0.0/fetchdep.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-11 23:35:01.000000 fetchdep-0.0.0/fetchdep.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1349 2024-05-11 23:34:57.000000 fetchdep-0.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      392 2024-05-11 23:35:01.657878 fetchdep-0.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      177 2024-05-11 23:34:57.000000 fetchdep-0.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.649878 fetchdep-0.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)    14737 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4236 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.649878 fetchdep-0.0.0/tests/example/
--rw-r--r--   0 root         (0) root         (0)      390 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/example/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.649878 fetchdep-0.0.0/tests/extract-tests/
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/extract-tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2159 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/extract-tests/test_cvs.py
--rw-r--r--   0 root         (0) root         (0)     1906 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/extract-tests/test_git.py
--rw-r--r--   0 root         (0) root         (0)     2040 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/extract-tests/test_mercurial.py
--rw-r--r--   0 root         (0) root         (0)     1707 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/extract-tests/test_svn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.649878 fetchdep-0.0.0/tests/unit-tests/
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.649878 fetchdep-0.0.0/tests/unit-tests/assets/
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/.gitattributes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/badcfg-no-name/
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/badcfg-no-name/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/badcfg-no-site/
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/badcfg-no-site/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/badcfg-yaml-notfetchdep/
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/badcfg-yaml-notfetchdep/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/badcfg-yaml-syntax/
--rw-r--r--   0 root         (0) root         (0)        2 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/badcfg-yaml-syntax/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/cfgname-type01/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/cfgname-type01/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/cfgname-type02/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/cfgname-type02/.fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/cfgname-type03/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/cfgname-type03/.fetchdep
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/large-set/
--rw-r--r--   0 root         (0) root         (0)     1000 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/large-set/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/missing/
--rw-r--r--   0 root         (0) root         (0)       75 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/missing/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/no-config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/no-config/.empty
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/recursive/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/recursive/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/tags/
--rw-r--r--   0 root         (0) root         (0)      361 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/tags/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/unicode/
--rw-r--r--   0 root         (0) root         (0)       62 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/unicode/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/vcs-cvs01/
--rw-r--r--   0 root         (0) root         (0)       95 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/vcs-cvs01/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/vcs-cvs02/
--rw-r--r--   0 root         (0) root         (0)      105 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/vcs-cvs02/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/vcs-git01/
--rw-r--r--   0 root         (0) root         (0)       72 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/vcs-git01/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/vcs-git02/
--rw-r--r--   0 root         (0) root         (0)       87 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/vcs-git02/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/vcs-git03/
--rw-r--r--   0 root         (0) root         (0)       79 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/vcs-git03/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/vcs-mercurial/
--rw-r--r--   0 root         (0) root         (0)       74 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/vcs-mercurial/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/vcs-multiple/
--rw-r--r--   0 root         (0) root         (0)      298 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/vcs-multiple/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/vcs-svn/
--rw-r--r--   0 root         (0) root         (0)       72 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/vcs-svn/fetchdep.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 23:35:01.653879 fetchdep-0.0.0/tests/unit-tests/assets/vcs-unknown/
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/assets/vcs-unknown/fetchdep.yml
--rw-r--r--   0 root         (0) root         (0)     1979 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_config_bad.py
--rw-r--r--   0 root         (0) root         (0)     1432 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_config_find.py
--rw-r--r--   0 root         (0) root         (0)      742 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_config_unicode.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_config_vcs.py
--rw-r--r--   0 root         (0) root         (0)     4167 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_engine_run_args.py
--rw-r--r--   0 root         (0) root         (0)     1375 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_engine_run_defaults.py
--rw-r--r--   0 root         (0) root         (0)      687 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_engine_run_environ_config.py
--rw-r--r--   0 root         (0) root         (0)     1014 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_engine_run_large.py
--rw-r--r--   0 root         (0) root         (0)      988 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_engine_run_missing.py
--rw-r--r--   0 root         (0) root         (0)     1502 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_engine_run_recursive.py
--rw-r--r--   0 root         (0) root         (0)      369 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_engine_run_required.py
--rw-r--r--   0 root         (0) root         (0)     3604 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_tags.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_util_io_resolve_dirname.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-11 23:34:57.000000 fetchdep-0.0.0/tests/unit-tests/test_util_tag_resolve_tag.py
+drwxrwxrwx   0        0        0        0 2024-05-06 01:17:39.066721 fetchdep-0.0.0.dev0/
+-rw-rw-rw-   0        0        0     1232 2024-05-06 01:17:39.065722 fetchdep-0.0.0.dev0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 01:17:39.052726 fetchdep-0.0.0.dev0/fetchdep/
+-rw-rw-rw-   0        0        0      118 2024-05-06 01:14:54.000000 fetchdep-0.0.0.dev0/fetchdep/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 01:17:39.064722 fetchdep-0.0.0.dev0/fetchdep.egg-info/
+-rw-rw-rw-   0        0        0     1232 2024-05-06 01:17:39.000000 fetchdep-0.0.0.dev0/fetchdep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-05-06 01:17:39.000000 fetchdep-0.0.0.dev0/fetchdep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 01:17:39.000000 fetchdep-0.0.0.dev0/fetchdep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-06 01:17:39.000000 fetchdep-0.0.0.dev0/fetchdep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1306 2024-05-06 01:16:29.000000 fetchdep-0.0.0.dev0/pyproject.toml
+-rw-rw-rw-   0        0        0      242 2024-05-06 01:17:39.071720 fetchdep-0.0.0.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      186 2024-05-06 01:15:12.000000 fetchdep-0.0.0.dev0/setup.py
```

