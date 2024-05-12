# Comparing `tmp/standard_distutils-3.7.17.tar.gz` & `tmp/standard_distutils-3.8.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "standard_distutils-3.7.17.tar", last modified: Sun May 12 02:24:38 2024, max compression
+gzip compressed data, was "standard_distutils-3.8.19.tar", last modified: Sun May 12 02:27:50 2024, max compression
```

## Comparing `standard_distutils-3.7.17.tar` & `standard_distutils-3.8.19.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:24:38.036895 standard_distutils-3.7.17/
--rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_distutils-3.7.17/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     3814 2024-05-12 02:24:38.036568 standard_distutils-3.7.17/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_distutils-3.7.17/README.rst
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:24:37.998133 standard_distutils-3.7.17/distutils/
--rw-r--r--   0 user       (501) staff       (20)      236 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/__init__.py
--rw-r--r--   0 user       (501) staff       (20)    19870 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/_msvccompiler.py
--rw-r--r--   0 user       (501) staff       (20)     8518 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/archive_util.py
--rw-r--r--   0 user       (501) staff       (20)    14935 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/bcppcompiler.py
--rw-r--r--   0 user       (501) staff       (20)    47433 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/ccompiler.py
--rw-r--r--   0 user       (501) staff       (20)    18079 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/cmd.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:24:38.014948 standard_distutils-3.7.17/distutils/command/
--rw-r--r--   0 user       (501) staff       (20)      799 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     5562 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/bdist.py
--rw-r--r--   0 user       (501) staff       (20)     4913 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/bdist_dumb.py
--rw-r--r--   0 user       (501) staff       (20)    35233 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/bdist_msi.py
--rw-r--r--   0 user       (501) staff       (20)    21671 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/bdist_rpm.py
--rw-r--r--   0 user       (501) staff       (20)    15560 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/command/bdist_wininst.py
--rw-r--r--   0 user       (501) staff       (20)     5767 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/command/build.py
--rw-r--r--   0 user       (501) staff       (20)     8022 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/build_clib.py
--rw-r--r--   0 user       (501) staff       (20)    30421 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/command/build_ext.py
--rw-r--r--   0 user       (501) staff       (20)    17164 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/build_py.py
--rw-r--r--   0 user       (501) staff       (20)     6232 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/build_scripts.py
--rw-r--r--   0 user       (501) staff       (20)     5599 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/command/check.py
--rw-r--r--   0 user       (501) staff       (20)     2776 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/clean.py
--rw-r--r--   0 user       (501) staff       (20)    13086 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/config.py
--rw-r--r--   0 user       (501) staff       (20)    26737 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/install.py
--rw-r--r--   0 user       (501) staff       (20)     2822 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/install_data.py
--rw-r--r--   0 user       (501) staff       (20)     2603 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/install_egg_info.py
--rw-r--r--   0 user       (501) staff       (20)     1298 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/install_headers.py
--rw-r--r--   0 user       (501) staff       (20)     8397 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/install_lib.py
--rw-r--r--   0 user       (501) staff       (20)     2017 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/install_scripts.py
--rw-r--r--   0 user       (501) staff       (20)    11712 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/register.py
--rw-r--r--   0 user       (501) staff       (20)    18999 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/command/sdist.py
--rw-r--r--   0 user       (501) staff       (20)     7261 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/command/upload.py
--rw-r--r--   0 user       (501) staff       (20)     4827 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/config.py
--rw-r--r--   0 user       (501) staff       (20)     8876 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/core.py
--rw-r--r--   0 user       (501) staff       (20)    16478 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/cygwinccompiler.py
--rw-r--r--   0 user       (501) staff       (20)      139 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/debug.py
--rw-r--r--   0 user       (501) staff       (20)     3491 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/dep_util.py
--rw-r--r--   0 user       (501) staff       (20)     7778 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/dir_util.py
--rw-r--r--   0 user       (501) staff       (20)    50385 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/dist.py
--rw-r--r--   0 user       (501) staff       (20)     3577 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/errors.py
--rw-r--r--   0 user       (501) staff       (20)    10515 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/extension.py
--rw-r--r--   0 user       (501) staff       (20)    17784 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/fancy_getopt.py
--rw-r--r--   0 user       (501) staff       (20)     8148 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/file_util.py
--rw-r--r--   0 user       (501) staff       (20)    12832 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/filelist.py
--rw-r--r--   0 user       (501) staff       (20)     1969 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/log.py
--rw-r--r--   0 user       (501) staff       (20)    30511 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/msvc9compiler.py
--rw-r--r--   0 user       (501) staff       (20)    23564 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/msvccompiler.py
--rw-r--r--   0 user       (501) staff       (20)     7835 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/spawn.py
--rw-r--r--   0 user       (501) staff       (20)    20453 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/sysconfig.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:24:38.035333 standard_distutils-3.7.17/distutils/tests/
--rw-r--r--   0 user       (501) staff       (20)     1327 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     6533 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/support.py
--rw-r--r--   0 user       (501) staff       (20)    14301 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/test_archive_util.py
--rw-r--r--   0 user       (501) staff       (20)     1680 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_bdist.py
--rw-r--r--   0 user       (501) staff       (20)     2905 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_bdist_dumb.py
--rw-r--r--   0 user       (501) staff       (20)      728 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_bdist_msi.py
--rw-r--r--   0 user       (501) staff       (20)     5008 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_bdist_rpm.py
--rw-r--r--   0 user       (501) staff       (20)     1158 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_bdist_wininst.py
--rw-r--r--   0 user       (501) staff       (20)     1965 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_build.py
--rw-r--r--   0 user       (501) staff       (20)     4675 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_build_clib.py
--rw-r--r--   0 user       (501) staff       (20)    19547 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/test_build_ext.py
--rw-r--r--   0 user       (501) staff       (20)     6335 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_build_py.py
--rw-r--r--   0 user       (501) staff       (20)     3593 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_build_scripts.py
--rw-r--r--   0 user       (501) staff       (20)     5711 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/test_check.py
--rw-r--r--   0 user       (501) staff       (20)     1441 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_clean.py
--rw-r--r--   0 user       (501) staff       (20)     3835 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_cmd.py
--rw-r--r--   0 user       (501) staff       (20)     3843 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_config.py
--rw-r--r--   0 user       (501) staff       (20)     2782 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_config_cmd.py
--rw-r--r--   0 user       (501) staff       (20)     4077 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_core.py
--rw-r--r--   0 user       (501) staff       (20)     5636 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_cygwinccompiler.py
--rw-r--r--   0 user       (501) staff       (20)     2820 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_dep_util.py
--rw-r--r--   0 user       (501) staff       (20)     4654 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_dir_util.py
--rw-r--r--   0 user       (501) staff       (20)    19095 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/test_dist.py
--rw-r--r--   0 user       (501) staff       (20)     2768 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_extension.py
--rw-r--r--   0 user       (501) staff       (20)     4413 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/test_file_util.py
--rw-r--r--   0 user       (501) staff       (20)    11475 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_filelist.py
--rw-r--r--   0 user       (501) staff       (20)     8535 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_install.py
--rw-r--r--   0 user       (501) staff       (20)     2577 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_install_data.py
--rw-r--r--   0 user       (501) staff       (20)     1238 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_install_headers.py
--rw-r--r--   0 user       (501) staff       (20)     3974 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_install_lib.py
--rw-r--r--   0 user       (501) staff       (20)     2625 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_install_scripts.py
--rw-r--r--   0 user       (501) staff       (20)     1864 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_log.py
--rw-r--r--   0 user       (501) staff       (20)     6038 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_msvc9compiler.py
--rw-r--r--   0 user       (501) staff       (20)     2845 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/test_msvccompiler.py
--rw-r--r--   0 user       (501) staff       (20)     9765 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_register.py
--rw-r--r--   0 user       (501) staff       (20)    17047 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_sdist.py
--rw-r--r--   0 user       (501) staff       (20)     5666 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/test_spawn.py
--rw-r--r--   0 user       (501) staff       (20)    11045 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/test_sysconfig.py
--rw-r--r--   0 user       (501) staff       (20)     3436 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_text_file.py
--rw-r--r--   0 user       (501) staff       (20)     4628 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/test_unixccompiler.py
--rw-r--r--   0 user       (501) staff       (20)     6535 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_upload.py
--rw-r--r--   0 user       (501) staff       (20)    11572 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/tests/test_util.py
--rw-r--r--   0 user       (501) staff       (20)     2614 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_version.py
--rw-r--r--   0 user       (501) staff       (20)      280 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/tests/test_versionpredicate.py
--rw-r--r--   0 user       (501) staff       (20)    12483 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/text_file.py
--rw-r--r--   0 user       (501) staff       (20)    14696 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/unixccompiler.py
--rw-r--r--   0 user       (501) staff       (20)    20384 2024-05-12 02:24:30.000000 standard_distutils-3.7.17/distutils/util.py
--rw-r--r--   0 user       (501) staff       (20)    12345 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/version.py
--rw-r--r--   0 user       (501) staff       (20)     5133 2024-05-12 01:52:39.000000 standard_distutils-3.7.17/distutils/versionpredicate.py
--rw-r--r--   0 user       (501) staff       (20)      717 2024-05-12 02:24:29.000000 standard_distutils-3.7.17/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2024-05-12 02:24:38.037034 standard_distutils-3.7.17/setup.cfg
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:24:38.036250 standard_distutils-3.7.17/standard_distutils.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     3814 2024-05-12 02:24:37.000000 standard_distutils-3.7.17/standard_distutils.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3047 2024-05-12 02:24:37.000000 standard_distutils-3.7.17/standard_distutils.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2024-05-12 02:24:37.000000 standard_distutils-3.7.17/standard_distutils.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       10 2024-05-12 02:24:37.000000 standard_distutils-3.7.17/standard_distutils.egg-info/top_level.txt
-drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:24:38.036056 standard_distutils-3.7.17/tests/
--rw-r--r--   0 user       (501) staff       (20)      375 2024-05-12 02:24:32.000000 standard_distutils-3.7.17/tests/test_distutils.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:27:50.629682 standard_distutils-3.8.19/
+-rw-r--r--   0 user       (501) staff       (20)     2569 2024-04-21 15:02:43.000000 standard_distutils-3.8.19/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     3814 2024-05-12 02:27:50.629314 standard_distutils-3.8.19/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      334 2024-04-21 16:58:55.000000 standard_distutils-3.8.19/README.rst
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:27:50.610215 standard_distutils-3.8.19/distutils/
+-rw-r--r--   0 user       (501) staff       (20)      236 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)    20050 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/_msvccompiler.py
+-rw-r--r--   0 user       (501) staff       (20)     8572 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/archive_util.py
+-rw-r--r--   0 user       (501) staff       (20)    14935 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/bcppcompiler.py
+-rw-r--r--   0 user       (501) staff       (20)    47433 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/ccompiler.py
+-rw-r--r--   0 user       (501) staff       (20)    18079 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/cmd.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:27:50.614332 standard_distutils-3.8.19/distutils/command/
+-rw-r--r--   0 user       (501) staff       (20)      799 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     5562 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/bdist.py
+-rw-r--r--   0 user       (501) staff       (20)     4913 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/bdist_dumb.py
+-rw-r--r--   0 user       (501) staff       (20)    35295 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/command/bdist_msi.py
+-rw-r--r--   0 user       (501) staff       (20)    21577 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/command/bdist_rpm.py
+-rw-r--r--   0 user       (501) staff       (20)    16043 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/command/bdist_wininst.py
+-rw-r--r--   0 user       (501) staff       (20)     5767 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/command/build.py
+-rw-r--r--   0 user       (501) staff       (20)     8022 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/build_clib.py
+-rw-r--r--   0 user       (501) staff       (20)    31568 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/command/build_ext.py
+-rw-r--r--   0 user       (501) staff       (20)    17190 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/command/build_py.py
+-rw-r--r--   0 user       (501) staff       (20)     6232 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/build_scripts.py
+-rw-r--r--   0 user       (501) staff       (20)     5599 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/command/check.py
+-rw-r--r--   0 user       (501) staff       (20)     2776 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/clean.py
+-rw-r--r--   0 user       (501) staff       (20)    13117 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/command/config.py
+-rw-r--r--   0 user       (501) staff       (20)    26731 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/command/install.py
+-rw-r--r--   0 user       (501) staff       (20)     2822 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/install_data.py
+-rw-r--r--   0 user       (501) staff       (20)     2603 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/install_egg_info.py
+-rw-r--r--   0 user       (501) staff       (20)     1298 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/install_headers.py
+-rw-r--r--   0 user       (501) staff       (20)     8397 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/install_lib.py
+-rw-r--r--   0 user       (501) staff       (20)     2017 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/install_scripts.py
+-rw-r--r--   0 user       (501) staff       (20)    11712 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/command/register.py
+-rw-r--r--   0 user       (501) staff       (20)    19005 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/command/sdist.py
+-rw-r--r--   0 user       (501) staff       (20)     7001 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/command/upload.py
+-rw-r--r--   0 user       (501) staff       (20)     4827 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/config.py
+-rw-r--r--   0 user       (501) staff       (20)     8876 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/core.py
+-rw-r--r--   0 user       (501) staff       (20)    16478 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/cygwinccompiler.py
+-rw-r--r--   0 user       (501) staff       (20)      139 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/debug.py
+-rw-r--r--   0 user       (501) staff       (20)     3491 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/dep_util.py
+-rw-r--r--   0 user       (501) staff       (20)     7778 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/dir_util.py
+-rw-r--r--   0 user       (501) staff       (20)    50385 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/dist.py
+-rw-r--r--   0 user       (501) staff       (20)     3577 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/errors.py
+-rw-r--r--   0 user       (501) staff       (20)    10515 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/extension.py
+-rw-r--r--   0 user       (501) staff       (20)    17784 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/fancy_getopt.py
+-rw-r--r--   0 user       (501) staff       (20)     8148 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/file_util.py
+-rw-r--r--   0 user       (501) staff       (20)    12832 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/filelist.py
+-rw-r--r--   0 user       (501) staff       (20)     1969 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/log.py
+-rw-r--r--   0 user       (501) staff       (20)    30511 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/msvc9compiler.py
+-rw-r--r--   0 user       (501) staff       (20)    23564 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/msvccompiler.py
+-rw-r--r--   0 user       (501) staff       (20)     7843 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/spawn.py
+-rw-r--r--   0 user       (501) staff       (20)    20390 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/sysconfig.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:27:50.626695 standard_distutils-3.8.19/distutils/tests/
+-rw-r--r--   0 user       (501) staff       (20)     1344 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/tests/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     6540 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/tests/support.py
+-rw-r--r--   0 user       (501) staff       (20)    14301 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/tests/test_archive_util.py
+-rw-r--r--   0 user       (501) staff       (20)     1893 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/tests/test_bdist.py
+-rw-r--r--   0 user       (501) staff       (20)     2905 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_bdist_dumb.py
+-rw-r--r--   0 user       (501) staff       (20)      728 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_bdist_msi.py
+-rw-r--r--   0 user       (501) staff       (20)     5008 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_bdist_rpm.py
+-rw-r--r--   0 user       (501) staff       (20)     1390 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/tests/test_bdist_wininst.py
+-rw-r--r--   0 user       (501) staff       (20)     1965 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_build.py
+-rw-r--r--   0 user       (501) staff       (20)     4675 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_build_clib.py
+-rw-r--r--   0 user       (501) staff       (20)    20633 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/tests/test_build_ext.py
+-rw-r--r--   0 user       (501) staff       (20)     6335 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_build_py.py
+-rw-r--r--   0 user       (501) staff       (20)     3593 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_build_scripts.py
+-rw-r--r--   0 user       (501) staff       (20)     5711 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/tests/test_check.py
+-rw-r--r--   0 user       (501) staff       (20)     1441 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_clean.py
+-rw-r--r--   0 user       (501) staff       (20)     3835 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_cmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3892 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/tests/test_config.py
+-rw-r--r--   0 user       (501) staff       (20)     3045 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/tests/test_config_cmd.py
+-rw-r--r--   0 user       (501) staff       (20)     4077 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_core.py
+-rw-r--r--   0 user       (501) staff       (20)     5636 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_cygwinccompiler.py
+-rw-r--r--   0 user       (501) staff       (20)     2820 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_dep_util.py
+-rw-r--r--   0 user       (501) staff       (20)     4654 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_dir_util.py
+-rw-r--r--   0 user       (501) staff       (20)    19102 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/tests/test_dist.py
+-rw-r--r--   0 user       (501) staff       (20)     2768 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_extension.py
+-rw-r--r--   0 user       (501) staff       (20)     4413 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/tests/test_file_util.py
+-rw-r--r--   0 user       (501) staff       (20)    11475 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_filelist.py
+-rw-r--r--   0 user       (501) staff       (20)     8535 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_install.py
+-rw-r--r--   0 user       (501) staff       (20)     2577 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_install_data.py
+-rw-r--r--   0 user       (501) staff       (20)     1238 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_install_headers.py
+-rw-r--r--   0 user       (501) staff       (20)     3974 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_install_lib.py
+-rw-r--r--   0 user       (501) staff       (20)     2625 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_install_scripts.py
+-rw-r--r--   0 user       (501) staff       (20)     1864 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_log.py
+-rw-r--r--   0 user       (501) staff       (20)     6038 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_msvc9compiler.py
+-rw-r--r--   0 user       (501) staff       (20)     2845 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/tests/test_msvccompiler.py
+-rw-r--r--   0 user       (501) staff       (20)     9765 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_register.py
+-rw-r--r--   0 user       (501) staff       (20)    17047 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_sdist.py
+-rw-r--r--   0 user       (501) staff       (20)     5666 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/tests/test_spawn.py
+-rw-r--r--   0 user       (501) staff       (20)    11045 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/tests/test_sysconfig.py
+-rw-r--r--   0 user       (501) staff       (20)     3436 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_text_file.py
+-rw-r--r--   0 user       (501) staff       (20)     4628 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/tests/test_unixccompiler.py
+-rw-r--r--   0 user       (501) staff       (20)     6535 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_upload.py
+-rw-r--r--   0 user       (501) staff       (20)    11572 2024-05-12 02:24:30.000000 standard_distutils-3.8.19/distutils/tests/test_util.py
+-rw-r--r--   0 user       (501) staff       (20)     2614 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_version.py
+-rw-r--r--   0 user       (501) staff       (20)      280 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/tests/test_versionpredicate.py
+-rw-r--r--   0 user       (501) staff       (20)    12483 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/text_file.py
+-rw-r--r--   0 user       (501) staff       (20)    14754 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/unixccompiler.py
+-rw-r--r--   0 user       (501) staff       (20)    20892 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/distutils/util.py
+-rw-r--r--   0 user       (501) staff       (20)    12345 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/version.py
+-rw-r--r--   0 user       (501) staff       (20)     5133 2024-05-12 01:52:39.000000 standard_distutils-3.8.19/distutils/versionpredicate.py
+-rw-r--r--   0 user       (501) staff       (20)      717 2024-05-12 02:27:44.000000 standard_distutils-3.8.19/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2024-05-12 02:27:50.629767 standard_distutils-3.8.19/setup.cfg
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:27:50.628831 standard_distutils-3.8.19/standard_distutils.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     3814 2024-05-12 02:27:50.000000 standard_distutils-3.8.19/standard_distutils.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3047 2024-05-12 02:27:50.000000 standard_distutils-3.8.19/standard_distutils.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2024-05-12 02:27:50.000000 standard_distutils-3.8.19/standard_distutils.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       10 2024-05-12 02:27:50.000000 standard_distutils-3.8.19/standard_distutils.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2024-05-12 02:27:50.628444 standard_distutils-3.8.19/tests/
+-rw-r--r--   0 user       (501) staff       (20)      375 2024-05-12 02:27:45.000000 standard_distutils-3.8.19/tests/test_distutils.py
```

### Comparing `standard_distutils-3.7.17/LICENSE` & `standard_distutils-3.8.19/LICENSE`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/PKG-INFO` & `standard_distutils-3.8.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-distutils
-Version: 3.7.17
+Version: 3.8.19
 Summary: Standard library distutils redistribution. "dead battery".
 Author-email: Python Developers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_distutils-3.7.17/distutils/_msvccompiler.py` & `standard_distutils-3.8.19/distutils/_msvccompiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,21 @@
 
     path = os.path.join(path, "VC", "Auxiliary", "Build")
     if os.path.isdir(path):
         return 15, path
 
     return None, None
 
+PLAT_SPEC_TO_RUNTIME = {
+    'x86' : 'x86',
+    'x86_amd64' : 'x64',
+    'x86_arm' : 'arm',
+    'x86_arm64' : 'arm64'
+}
+
 def _find_vcvarsall(plat_spec):
     # bpo-38597: Removed vcruntime return value
     _, best_dir = _find_vc2017()
 
     if not best_dir:
         best_version, best_dir = _find_vc2015()
 
@@ -156,14 +163,16 @@
 
 # A map keyed by get_platform() return values to values accepted by
 # 'vcvarsall.bat'. Always cross-compile from x86 to work with the
 # lighter-weight MSVC installs that do not include native 64-bit tools.
 PLAT_TO_VCVARS = {
     'win32' : 'x86',
     'win-amd64' : 'x86_amd64',
+    'win-arm32' : 'x86_arm',
+    'win-arm64' : 'x86_arm64'
 }
 
 class MSVCCompiler(CCompiler) :
     """Concrete class that implements an interface to Microsoft Visual C++,
        as defined by the CCompiler abstract class."""
 
     compiler_type = 'msvc'
```

### Comparing `standard_distutils-3.7.17/distutils/archive_util.py` & `standard_distutils-3.8.19/distutils/archive_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,29 +162,29 @@
             try:
                 zip = zipfile.ZipFile(zip_filename, "w",
                                       compression=zipfile.ZIP_DEFLATED)
             except RuntimeError:
                 zip = zipfile.ZipFile(zip_filename, "w",
                                       compression=zipfile.ZIP_STORED)
 
-            if base_dir != os.curdir:
-                path = os.path.normpath(os.path.join(base_dir, ''))
-                zip.write(path, path)
-                log.info("adding '%s'", path)
-            for dirpath, dirnames, filenames in os.walk(base_dir):
-                for name in dirnames:
-                    path = os.path.normpath(os.path.join(dirpath, name, ''))
+            with zip:
+                if base_dir != os.curdir:
+                    path = os.path.normpath(os.path.join(base_dir, ''))
                     zip.write(path, path)
                     log.info("adding '%s'", path)
-                for name in filenames:
-                    path = os.path.normpath(os.path.join(dirpath, name))
-                    if os.path.isfile(path):
+                for dirpath, dirnames, filenames in os.walk(base_dir):
+                    for name in dirnames:
+                        path = os.path.normpath(os.path.join(dirpath, name, ''))
                         zip.write(path, path)
                         log.info("adding '%s'", path)
-            zip.close()
+                    for name in filenames:
+                        path = os.path.normpath(os.path.join(dirpath, name))
+                        if os.path.isfile(path):
+                            zip.write(path, path)
+                            log.info("adding '%s'", path)
 
     return zip_filename
 
 ARCHIVE_FORMATS = {
     'gztar': (make_tarball, [('compress', 'gzip')], "gzip'ed tar-file"),
     'bztar': (make_tarball, [('compress', 'bzip2')], "bzip2'ed tar-file"),
     'xztar': (make_tarball, [('compress', 'xz')], "xz'ed tar-file"),
```

### Comparing `standard_distutils-3.7.17/distutils/bcppcompiler.py` & `standard_distutils-3.8.19/distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/ccompiler.py` & `standard_distutils-3.8.19/distutils/ccompiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -541,15 +541,15 @@
 
         'debug' is a boolean; if true, the compiler will be instructed to
         output debug symbols in (or alongside) the object file(s).
 
         'extra_preargs' and 'extra_postargs' are implementation- dependent.
         On platforms that have the notion of a command-line (e.g. Unix,
         DOS/Windows), they are most likely lists of strings: extra
-        command-line arguments to prepand/append to the compiler command
+        command-line arguments to prepend/append to the compiler command
         line.  On other platforms, consult the implementation class
         documentation.  In any event, they are intended as an escape hatch
         for those occasions when the abstract compiler framework doesn't
         cut the mustard.
 
         'depends', if given, is a list of filenames that all targets
         depend on.  If a source file is older than any file in
```

### Comparing `standard_distutils-3.7.17/distutils/cmd.py` & `standard_distutils-3.8.19/distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/__init__.py` & `standard_distutils-3.8.19/distutils/command/__init__.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/bdist.py` & `standard_distutils-3.8.19/distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/bdist_dumb.py` & `standard_distutils-3.8.19/distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/bdist_msi.py` & `standard_distutils-3.8.19/distutils/command/bdist_msi.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,26 +386,26 @@
                         [(install_action, "&Python%s=3" % ver, start)])
                 start += 1
         # XXX pre-install scripts are currently refused in finalize_options()
         #     but if this feature is completed, it will also need to add
         #     entries for each version as the above code does
         if self.pre_install_script:
             scriptfn = os.path.join(self.bdist_dir, "preinstall.bat")
-            f = open(scriptfn, "w")
-            # The batch file will be executed with [PYTHON], so that %1
-            # is the path to the Python interpreter; %0 will be the path
-            # of the batch file.
-            # rem ="""
-            # %1 %0
-            # exit
-            # """
-            # <actual script>
-            f.write('rem ="""\n%1 %0\nexit\n"""\n')
-            f.write(open(self.pre_install_script).read())
-            f.close()
+            with open(scriptfn, "w") as f:
+                # The batch file will be executed with [PYTHON], so that %1
+                # is the path to the Python interpreter; %0 will be the path
+                # of the batch file.
+                # rem ="""
+                # %1 %0
+                # exit
+                # """
+                # <actual script>
+                f.write('rem ="""\n%1 %0\nexit\n"""\n')
+                with open(self.pre_install_script) as fin:
+                    f.write(fin.read())
             add_data(self.db, "Binary",
                 [("PreInstall", msilib.Binary(scriptfn))
                 ])
             add_data(self.db, "CustomAction",
                 [("PreInstall", 2, "PreInstall", None)
                 ])
             add_data(self.db, "InstallExecuteSequence",
```

### Comparing `standard_distutils-3.7.17/distutils/command/bdist_rpm.py` & `standard_distutils-3.8.19/distutils/command/bdist_rpm.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,18 +305,15 @@
                 self.copy_file(self.icon, source_dir)
             else:
                 raise DistutilsFileError(
                       "icon file '%s' does not exist" % self.icon)
 
         # build package
         log.info("building RPMs")
-        rpm_cmd = ['rpm']
-        if os.path.exists('/usr/bin/rpmbuild') or \
-           os.path.exists('/bin/rpmbuild'):
-            rpm_cmd = ['rpmbuild']
+        rpm_cmd = ['rpmbuild']
 
         if self.source_only: # what kind of RPMs?
             rpm_cmd.append('-bs')
         elif self.binary_only:
             rpm_cmd.append('-bb')
         else:
             rpm_cmd.append('-ba')
@@ -533,15 +530,16 @@
             # use 'default' as contents of script
             val = getattr(self, attr)
             if val or default:
                 spec_file.extend([
                     '',
                     '%' + rpm_opt,])
                 if val:
-                    spec_file.extend(open(val, 'r').read().split('\n'))
+                    with open(val) as f:
+                        spec_file.extend(f.read().split('\n'))
                 else:
                     spec_file.append(default)
 
 
         # files section
         spec_file.extend([
             '',
```

### Comparing `standard_distutils-3.7.17/distutils/command/bdist_wininst.py` & `standard_distutils-3.8.19/distutils/command/bdist_wininst.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """distutils.command.bdist_wininst
 
 Implements the Distutils 'bdist_wininst' command: create a windows installer
 exe-program."""
 
-import sys, os
+import os
+import sys
+import warnings
 from distutils.core import Command
 from distutils.util import get_platform
 from distutils.dir_util import create_tree, remove_tree
 from distutils.errors import *
 from distutils.sysconfig import get_python_version
 from distutils import log
 
@@ -54,14 +56,20 @@
 
     boolean_options = ['keep-temp', 'no-target-compile', 'no-target-optimize',
                        'skip-build']
 
     # bpo-10945: bdist_wininst requires mbcs encoding only available on Windows
     _unsupported = (sys.platform != "win32")
 
+    def __init__(self, *args, **kw):
+        super().__init__(*args, **kw)
+        warnings.warn("bdist_wininst command is deprecated since Python 3.8, "
+                      "use bdist_wheel (wheel packages) instead",
+                      DeprecationWarning, 2)
+
     def initialize_options(self):
         self.bdist_dir = None
         self.plat_name = None
         self.keep_temp = 0
         self.no_target_compile = 0
         self.no_target_optimize = 0
         self.target_version = None
@@ -246,55 +254,57 @@
 
         cfgdata = self.get_inidata()
 
         installer_name = self.get_installer_filename(fullname)
         self.announce("creating %s" % installer_name)
 
         if bitmap:
-            bitmapdata = open(bitmap, "rb").read()
+            with open(bitmap, "rb") as f:
+                bitmapdata = f.read()
             bitmaplen = len(bitmapdata)
         else:
             bitmaplen = 0
 
-        file = open(installer_name, "wb")
-        file.write(self.get_exe_bytes())
-        if bitmap:
-            file.write(bitmapdata)
+        with open(installer_name, "wb") as file:
+            file.write(self.get_exe_bytes())
+            if bitmap:
+                file.write(bitmapdata)
+
+            # Convert cfgdata from unicode to ascii, mbcs encoded
+            if isinstance(cfgdata, str):
+                cfgdata = cfgdata.encode("mbcs")
 
-        # Convert cfgdata from unicode to ascii, mbcs encoded
-        if isinstance(cfgdata, str):
-            cfgdata = cfgdata.encode("mbcs")
-
-        # Append the pre-install script
-        cfgdata = cfgdata + b"\0"
-        if self.pre_install_script:
-            # We need to normalize newlines, so we open in text mode and
-            # convert back to bytes. "latin-1" simply avoids any possible
-            # failures.
-            with open(self.pre_install_script, "r",
-                encoding="latin-1") as script:
-                script_data = script.read().encode("latin-1")
-            cfgdata = cfgdata + script_data + b"\n\0"
-        else:
-            # empty pre-install script
+            # Append the pre-install script
             cfgdata = cfgdata + b"\0"
-        file.write(cfgdata)
-
-        # The 'magic number' 0x1234567B is used to make sure that the
-        # binary layout of 'cfgdata' is what the wininst.exe binary
-        # expects.  If the layout changes, increment that number, make
-        # the corresponding changes to the wininst.exe sources, and
-        # recompile them.
-        header = struct.pack("<iii",
-                             0x1234567B,       # tag
-                             len(cfgdata),     # length
-                             bitmaplen,        # number of bytes in bitmap
-                             )
-        file.write(header)
-        file.write(open(arcname, "rb").read())
+            if self.pre_install_script:
+                # We need to normalize newlines, so we open in text mode and
+                # convert back to bytes. "latin-1" simply avoids any possible
+                # failures.
+                with open(self.pre_install_script, "r",
+                          encoding="latin-1") as script:
+                    script_data = script.read().encode("latin-1")
+                cfgdata = cfgdata + script_data + b"\n\0"
+            else:
+                # empty pre-install script
+                cfgdata = cfgdata + b"\0"
+            file.write(cfgdata)
+
+            # The 'magic number' 0x1234567B is used to make sure that the
+            # binary layout of 'cfgdata' is what the wininst.exe binary
+            # expects.  If the layout changes, increment that number, make
+            # the corresponding changes to the wininst.exe sources, and
+            # recompile them.
+            header = struct.pack("<iii",
+                                0x1234567B,       # tag
+                                len(cfgdata),     # length
+                                bitmaplen,        # number of bytes in bitmap
+                                )
+            file.write(header)
+            with open(arcname, "rb") as f:
+                file.write(f.read())
 
     def get_installer_filename(self, fullname):
         # Factored out to allow overriding in subclasses
         if self.target_version:
             # if we create an installer for a specific python version,
             # it's better to include this in the name
             installer_name = os.path.join(self.dist_dir,
```

### Comparing `standard_distutils-3.7.17/distutils/command/build.py` & `standard_distutils-3.8.19/distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/build_clib.py` & `standard_distutils-3.8.19/distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/build_ext.py` & `standard_distutils-3.8.19/distutils/command/build_ext.py`

 * *Files 6% similar despite different names*

```diff
@@ -684,15 +684,23 @@
 
     def get_export_symbols(self, ext):
         """Return the list of symbols that a shared extension has to
         export.  This either uses 'ext.export_symbols' or, if it's not
         provided, "PyInit_" + module_name.  Only relevant on Windows, where
         the .pyd file (DLL) must export the module "PyInit_" function.
         """
-        initfunc_name = "PyInit_" + ext.name.split('.')[-1]
+        suffix = '_' + ext.name.split('.')[-1]
+        try:
+            # Unicode module name support as defined in PEP-489
+            # https://www.python.org/dev/peps/pep-0489/#export-hook-name
+            suffix.encode('ascii')
+        except UnicodeEncodeError:
+            suffix = 'U' + suffix.encode('punycode').replace(b'-', b'_').decode('ascii')
+
+        initfunc_name = "PyInit" + suffix
         if initfunc_name not in ext.export_symbols:
             ext.export_symbols.append(initfunc_name)
         return ext.export_symbols
 
     def get_libraries(self, ext):
         """Return the list of libraries to link against when building a
         shared extension.  On most platforms, this is just 'ext.libraries';
@@ -710,24 +718,36 @@
                 if self.debug:
                     template = template + '_d'
                 pythonlib = (template %
                        (sys.hexversion >> 24, (sys.hexversion >> 16) & 0xff))
                 # don't extend ext.libraries, it may be shared with other
                 # extensions, it is a reference to the original list
                 return ext.libraries + [pythonlib]
-            else:
-                return ext.libraries
-        elif sys.platform == 'darwin':
-            # Don't use the default code below
-            return ext.libraries
-        elif sys.platform[:3] == 'aix':
-            # Don't use the default code below
-            return ext.libraries
         else:
-            from distutils import sysconfig
-            if sysconfig.get_config_var('Py_ENABLE_SHARED'):
-                pythonlib = 'python{}.{}{}'.format(
-                    sys.hexversion >> 24, (sys.hexversion >> 16) & 0xff,
-                    sysconfig.get_config_var('ABIFLAGS'))
-                return ext.libraries + [pythonlib]
-            else:
-                return ext.libraries
+            # On Android only the main executable and LD_PRELOADs are considered
+            # to be RTLD_GLOBAL, all the dependencies of the main executable
+            # remain RTLD_LOCAL and so the shared libraries must be linked with
+            # libpython when python is built with a shared python library (issue
+            # bpo-21536).
+            # On Cygwin (and if required, other POSIX-like platforms based on
+            # Windows like MinGW) it is simply necessary that all symbols in
+            # shared libraries are resolved at link time.
+            from distutils.sysconfig import get_config_var
+            link_libpython = False
+            if get_config_var('Py_ENABLE_SHARED'):
+                # A native build on an Android device or on Cygwin
+                if hasattr(sys, 'getandroidapilevel'):
+                    link_libpython = True
+                elif sys.platform == 'cygwin':
+                    link_libpython = True
+                elif '_PYTHON_HOST_PLATFORM' in os.environ:
+                    # We are cross-compiling for one of the relevant platforms
+                    if get_config_var('ANDROID_API_LEVEL') != 0:
+                        link_libpython = True
+                    elif get_config_var('MACHDEP') == 'cygwin':
+                        link_libpython = True
+
+            if link_libpython:
+                ldversion = get_config_var('LDVERSION')
+                return ext.libraries + ['python' + ldversion]
+
+        return ext.libraries
```

### Comparing `standard_distutils-3.7.17/distutils/command/build_py.py` & `standard_distutils-3.8.19/distutils/command/build_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """distutils.command.build_py
 
 Implements the Distutils 'build_py' command."""
 
 import os
 import importlib.util
 import sys
-from glob import glob
+import glob
 
 from distutils.core import Command
 from distutils.errors import *
 from distutils.util import convert_path, Mixin2to3
 from distutils import log
 
 class build_py (Command):
@@ -121,15 +121,15 @@
     def find_data_files(self, package, src_dir):
         """Return filenames for package's data files in 'src_dir'"""
         globs = (self.package_data.get('', [])
                  + self.package_data.get(package, []))
         files = []
         for pattern in globs:
             # Each pattern has to be converted to a platform-specific path
-            filelist = glob(os.path.join(src_dir, convert_path(pattern)))
+            filelist = glob.glob(os.path.join(glob.escape(src_dir), convert_path(pattern)))
             # Files that match more than one pattern are only added once
             files.extend([fn for fn in filelist if fn not in files
                 and os.path.isfile(fn)])
         return files
 
     def build_package_data(self):
         """Copy data files into build directory"""
@@ -212,15 +212,15 @@
             log.warn("file %s (for module %s) not found", module_file, module)
             return False
         else:
             return True
 
     def find_package_modules(self, package, package_dir):
         self.check_package(package, package_dir)
-        module_files = glob(os.path.join(package_dir, "*.py"))
+        module_files = glob.glob(os.path.join(glob.escape(package_dir), "*.py"))
         modules = []
         setup_script = os.path.abspath(self.distribution.script_name)
 
         for f in module_files:
             abs_f = os.path.abspath(f)
             if abs_f != setup_script:
                 module = os.path.splitext(os.path.basename(f))[0]
```

### Comparing `standard_distutils-3.7.17/distutils/command/build_scripts.py` & `standard_distutils-3.8.19/distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/check.py` & `standard_distutils-3.8.19/distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/clean.py` & `standard_distutils-3.8.19/distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/config.py` & `standard_distutils-3.8.19/distutils/command/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,23 +102,22 @@
             if self.libraries:
                 self.compiler.set_libraries(self.libraries)
             if self.library_dirs:
                 self.compiler.set_library_dirs(self.library_dirs)
 
     def _gen_temp_sourcefile(self, body, headers, lang):
         filename = "_configtest" + LANG_EXT[lang]
-        file = open(filename, "w")
-        if headers:
-            for header in headers:
-                file.write("#include <%s>\n" % header)
-            file.write("\n")
-        file.write(body)
-        if body[-1] != "\n":
-            file.write("\n")
-        file.close()
+        with open(filename, "w") as file:
+            if headers:
+                for header in headers:
+                    file.write("#include <%s>\n" % header)
+                file.write("\n")
+            file.write(body)
+            if body[-1] != "\n":
+                file.write("\n")
         return filename
 
     def _preprocess(self, body, headers, include_dirs, lang):
         src = self._gen_temp_sourcefile(body, headers, lang)
         out = "_configtest.i"
         self.temp_files.extend([src, out])
         self.compiler.preprocess(src, out, include_dirs=include_dirs)
@@ -199,25 +198,24 @@
         """
         self._check_compiler()
         src, out = self._preprocess(body, headers, include_dirs, lang)
 
         if isinstance(pattern, str):
             pattern = re.compile(pattern)
 
-        file = open(out)
-        match = False
-        while True:
-            line = file.readline()
-            if line == '':
-                break
-            if pattern.search(line):
-                match = True
-                break
+        with open(out) as file:
+            match = False
+            while True:
+                line = file.readline()
+                if line == '':
+                    break
+                if pattern.search(line):
+                    match = True
+                    break
 
-        file.close()
         self._clean()
         return match
 
     def try_compile(self, body, headers=None, include_dirs=None, lang="c"):
         """Try to compile a source file built from 'body' and 'headers'.
         Return true on success, false otherwise.
         """
@@ -326,15 +324,14 @@
         """Determine if the system header file named by 'header_file'
         exists and can be found by the preprocessor; return true if so,
         false otherwise.
         """
         return self.try_cpp(body="/* No body */", headers=[header],
                             include_dirs=include_dirs)
 
-
 def dump_file(filename, head=None):
     """Dumps a file content into log.info.
 
     If head is not None, will be dumped before the file content.
     """
     if head is None:
         log.info('%s', filename)
```

### Comparing `standard_distutils-3.7.17/distutils/command/install.py` & `standard_distutils-3.8.19/distutils/command/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
     # (This is rather more involved than for most commands,
     # because this is where the policy for installing third-
     # party Python modules on various platforms given a wide
     # array of user input is decided.  Yes, it's quite complex!)
 
     def finalize_options(self):
         """Finalizes options."""
-        # This method (and its pliant slaves, like 'finalize_unix()',
+        # This method (and its helpers, like 'finalize_unix()',
         # 'finalize_other()', and 'select_scheme()') is where the default
         # installation directories for modules, extension modules, and
         # anything else we care to install from a Python module
         # distribution.  Thus, this code makes a pretty important policy
         # statement about how third-party stuff is added to a Python
         # installation!  Note that the actual work of installation is done
         # by the relatively simple 'install_*' commands; they just take
```

### Comparing `standard_distutils-3.7.17/distutils/command/install_data.py` & `standard_distutils-3.8.19/distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/install_egg_info.py` & `standard_distutils-3.8.19/distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/install_headers.py` & `standard_distutils-3.8.19/distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/install_lib.py` & `standard_distutils-3.8.19/distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/install_scripts.py` & `standard_distutils-3.8.19/distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/register.py` & `standard_distutils-3.8.19/distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/command/sdist.py` & `standard_distutils-3.8.19/distutils/command/sdist.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,22 +403,21 @@
 
     def read_manifest(self):
         """Read the manifest file (named by 'self.manifest') and use it to
         fill in 'self.filelist', the list of files to include in the source
         distribution.
         """
         log.info("reading manifest file '%s'", self.manifest)
-        manifest = open(self.manifest)
-        for line in manifest:
-            # ignore comments and blank lines
-            line = line.strip()
-            if line.startswith('#') or not line:
-                continue
-            self.filelist.append(line)
-        manifest.close()
+        with open(self.manifest) as manifest:
+            for line in manifest:
+                # ignore comments and blank lines
+                line = line.strip()
+                if line.startswith('#') or not line:
+                    continue
+                self.filelist.append(line)
 
     def make_release_tree(self, base_dir, files):
         """Create the directory tree that will become the source
         distribution archive.  All directories implied by the filenames in
         'files' are created under 'base_dir', and then we hard link or copy
         (if hard linking is unavailable) those files into place.
         Essentially, this duplicates the developer's source tree, but in a
```

### Comparing `standard_distutils-3.7.17/distutils/command/upload.py` & `standard_distutils-3.8.19/distutils/command/upload.py`

 * *Files 7% similar despite different names*

```diff
@@ -117,26 +117,21 @@
             'classifiers': meta.get_classifiers(),
             'download_url': meta.get_download_url(),
             # PEP 314
             'provides': meta.get_provides(),
             'requires': meta.get_requires(),
             'obsoletes': meta.get_obsoletes(),
             }
-        comment = ''
-        if command == 'bdist_rpm':
-            dist, version, id = platform.dist()
-            if dist:
-                comment = 'built for %s %s' % (dist, version)
-        elif command == 'bdist_dumb':
-            comment = 'built for %s' % platform.platform(terse=1)
-        data['comment'] = comment
+
+        data['comment'] = ''
 
         if self.sign:
-            data['gpg_signature'] = (os.path.basename(filename) + ".asc",
-                                     open(filename+".asc", "rb").read())
+            with open(filename + ".asc", "rb") as f:
+                data['gpg_signature'] = (os.path.basename(filename) + ".asc",
+                                         f.read())
 
         # set up the authentication
         user_pass = (self.username + ":" + self.password).encode('ascii')
         # The exact encoding of the authentication string is debated.
         # Anyway PyPI only accepts ascii for both username or password.
         auth = "Basic " + standard_b64encode(user_pass).decode('ascii')
```

### Comparing `standard_distutils-3.7.17/distutils/config.py` & `standard_distutils-3.8.19/distutils/config.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/core.py` & `standard_distutils-3.8.19/distutils/core.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/cygwinccompiler.py` & `standard_distutils-3.8.19/distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/dep_util.py` & `standard_distutils-3.8.19/distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/dir_util.py` & `standard_distutils-3.8.19/distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/dist.py` & `standard_distutils-3.8.19/distutils/dist.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/errors.py` & `standard_distutils-3.8.19/distutils/errors.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/extension.py` & `standard_distutils-3.8.19/distutils/extension.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/fancy_getopt.py` & `standard_distutils-3.8.19/distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/file_util.py` & `standard_distutils-3.8.19/distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/filelist.py` & `standard_distutils-3.8.19/distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/log.py` & `standard_distutils-3.8.19/distutils/log.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/msvc9compiler.py` & `standard_distutils-3.8.19/distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/msvccompiler.py` & `standard_distutils-3.8.19/distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/spawn.py` & `standard_distutils-3.8.19/distutils/spawn.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,28 +77,28 @@
             # and this reflects the command running but failing
             if not DEBUG:
                 cmd = executable
             raise DistutilsExecError(
                   "command %r failed with exit status %d" % (cmd, rc))
 
 if sys.platform == 'darwin':
-    from distutils import sysconfig
     _cfg_target = None
     _cfg_target_split = None
 
 def _spawn_posix(cmd, search_path=1, verbose=0, dry_run=0):
     log.info(' '.join(cmd))
     if dry_run:
         return
     executable = cmd[0]
     exec_fn = search_path and os.execvp or os.execv
     env = None
     if sys.platform == 'darwin':
         global _cfg_target, _cfg_target_split
         if _cfg_target is None:
+            from distutils import sysconfig
             _cfg_target = sysconfig.get_config_var(
                                   'MACOSX_DEPLOYMENT_TARGET') or ''
             if _cfg_target:
                 _cfg_target_split = [int(x) for x in _cfg_target.split('.')]
         if _cfg_target:
             # ensure that the deployment target of build process is not less
             # than that used when the interpreter was built. This ensures
```

### Comparing `standard_distutils-3.7.17/distutils/sysconfig.py` & `standard_distutils-3.8.19/distutils/sysconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 import _imp
 import os
 import re
 import sys
 
 from .errors import DistutilsPlatformError
+from .util import get_platform, get_host_platform
 
 # These are needed in a couple of spots, so just compute them once.
 PREFIX = os.path.normpath(sys.prefix)
 EXEC_PREFIX = os.path.normpath(sys.exec_prefix)
 BASE_PREFIX = os.path.normpath(sys.base_prefix)
 BASE_EXEC_PREFIX = os.path.normpath(sys.base_exec_prefix)
 
@@ -35,18 +36,16 @@
         # unable to retrieve the real program name
         project_base = os.getcwd()
 
 
 # python_build: (Boolean) if true, we're either building Python or
 # building an extension with an un-installed Python, so we use
 # different (hard-wired) directories.
-# Setup.local is available for Makefile builds including VPATH builds,
-# Setup.dist is available on Windows
 def _is_python_source_dir(d):
-    for fn in ("Setup.dist", "Setup.local"):
+    for fn in ("Setup", "Setup.local"):
         if os.path.isfile(os.path.join(d, "Modules", fn)):
             return True
     return False
 
 _sys_home = getattr(sys, '_home', None)
 
 if os.name == 'nt':
```

### Comparing `standard_distutils-3.7.17/distutils/tests/__init__.py` & `standard_distutils-3.8.19/distutils/tests/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,32 +11,30 @@
 by import rather than matching pre-defined names.
 
 """
 
 import os
 import sys
 import unittest
-import warnings
-from test.support import run_unittest
+from test.support import run_unittest, save_restore_warnings_filters
 
 
 here = os.path.dirname(__file__) or os.curdir
 
 
 def test_suite():
-    old_filters = warnings.filters[:]
     suite = unittest.TestSuite()
     for fn in os.listdir(here):
         if fn.startswith("test") and fn.endswith(".py"):
             modname = "distutils.tests." + fn[:-3]
-            __import__(modname)
+            # bpo-40055: Save/restore warnings filters to leave them unchanged.
+            # Importing tests imports docutils which imports pkg_resources
+            # which adds a warnings filter.
+            with save_restore_warnings_filters():
+                __import__(modname)
             module = sys.modules[modname]
             suite.addTest(module.test_suite())
-    # bpo-40055: Save/restore warnings filters to leave them unchanged.
-    # Importing tests imports docutils which imports pkg_resources which adds a
-    # warnings filter.
-    warnings.filters[:] = old_filters
     return suite
 
 
 if __name__ == "__main__":
     run_unittest(test_suite())
```

### Comparing `standard_distutils-3.7.17/distutils/tests/support.py` & `standard_distutils-3.8.19/distutils/tests/support.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import sys
 import shutil
 import tempfile
 import unittest
 import sysconfig
 from copy import deepcopy
+import test.support
 
 from distutils import log
 from distutils.log import DEBUG, INFO, WARN, ERROR, FATAL
 from distutils.core import Distribution
 
 
 class LoggingSilencer(object):
@@ -60,16 +61,16 @@
 
     def tearDown(self):
         # Restore working dir, for Solaris and derivatives, where rmdir()
         # on the current directory fails.
         os.chdir(self.old_cwd)
         super().tearDown()
         while self.tempdirs:
-            d = self.tempdirs.pop()
-            shutil.rmtree(d, os.name in ('nt', 'cygwin'))
+            tmpdir = self.tempdirs.pop()
+            test.support.rmtree(tmpdir)
 
     def mkdtemp(self):
         """Create a temporary directory that will be cleaned up.
 
         Returns the path of the directory.
         """
         d = tempfile.mkdtemp()
```

### Comparing `standard_distutils-3.7.17/distutils/tests/test_archive_util.py` & `standard_distutils-3.8.19/distutils/tests/test_archive_util.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_bdist.py` & `standard_distutils-3.8.19/distutils/tests/test_bdist.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for distutils.command.bdist."""
 import os
 import unittest
 from test.support import run_unittest
+import warnings
 
 from distutils.command.bdist import bdist
 from distutils.tests import support
 
 
 class BuildTestCase(support.TempdirManager,
                     unittest.TestCase):
@@ -34,15 +35,18 @@
         dist.command_obj['bdist'] = cmd
 
         names = ['bdist_dumb', 'bdist_wininst']  # bdist_rpm does not support --skip-build
         if os.name == 'nt':
             names.append('bdist_msi')
 
         for name in names:
-            subcmd = cmd.get_finalized_command(name)
+            with warnings.catch_warnings():
+                warnings.filterwarnings('ignore', 'bdist_wininst command is deprecated',
+                                        DeprecationWarning)
+                subcmd = cmd.get_finalized_command(name)
             if getattr(subcmd, '_unsupported', False):
                 # command is not supported on this build
                 continue
             self.assertTrue(subcmd.skip_build,
                             '%s should take --skip-build from bdist' % name)
```

### Comparing `standard_distutils-3.7.17/distutils/tests/test_bdist_dumb.py` & `standard_distutils-3.8.19/distutils/tests/test_bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_bdist_msi.py` & `standard_distutils-3.8.19/distutils/tests/test_bdist_msi.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_bdist_rpm.py` & `standard_distutils-3.8.19/distutils/tests/test_bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_bdist_wininst.py` & `standard_distutils-3.8.19/distutils/tests/test_bdist_wininst.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 """Tests for distutils.command.bdist_wininst."""
+import sys
+import platform
 import unittest
-from test.support import run_unittest
+from test.support import run_unittest, check_warnings
 
 from distutils.command.bdist_wininst import bdist_wininst
 from distutils.tests import support
 
+@unittest.skipIf(sys.platform == 'win32' and platform.machine() == 'ARM64',
+    'bdist_wininst is not supported in this install')
 @unittest.skipIf(getattr(bdist_wininst, '_unsupported', False),
     'bdist_wininst is not supported in this install')
 class BuildWinInstTestCase(support.TempdirManager,
                            support.LoggingSilencer,
                            unittest.TestCase):
 
     def test_get_exe_bytes(self):
 
         # issue5731: command was broken on non-windows platforms
         # this test makes sure it works now for every platform
         # let's create a command
         pkg_pth, dist = self.create_dist()
-        cmd = bdist_wininst(dist)
+        with check_warnings(("", DeprecationWarning)):
+            cmd = bdist_wininst(dist)
         cmd.ensure_finalized()
 
         # let's run the code that finds the right wininst*.exe file
         # and make sure it finds it and returns its content
         # no matter what platform we have
         exe_file = cmd.get_exe_bytes()
         self.assertGreater(len(exe_file), 10)
```

### Comparing `standard_distutils-3.7.17/distutils/tests/test_build.py` & `standard_distutils-3.8.19/distutils/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_build_clib.py` & `standard_distutils-3.8.19/distutils/tests/test_build_clib.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_build_ext.py` & `standard_distutils-3.8.19/distutils/tests/test_build_ext.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,48 +11,42 @@
 from distutils.extension import Extension
 from distutils.errors import (
     CompileError, DistutilsPlatformError, DistutilsSetupError,
     UnknownFileError)
 
 import unittest
 from test import support
+from test.support.script_helper import assert_python_ok
 
 # http://bugs.python.org/issue4373
 # Don't load the xx module more than once.
 ALREADY_TESTED = False
 
 
 class BuildExtTestCase(TempdirManager,
                        LoggingSilencer,
                        unittest.TestCase):
     def setUp(self):
         # Create a simple test environment
-        # Note that we're making changes to sys.path
         super(BuildExtTestCase, self).setUp()
         self.tmp_dir = self.mkdtemp()
-        self.sys_path = sys.path, sys.path[:]
-        sys.path.append(self.tmp_dir)
         import site
         self.old_user_base = site.USER_BASE
         site.USER_BASE = self.mkdtemp()
         from distutils.command import build_ext
         build_ext.USER_BASE = site.USER_BASE
 
         # bpo-30132: On Windows, a .pdb file may be created in the current
         # working directory. Create a temporary working directory to cleanup
         # everything at the end of the test.
-        self.temp_cwd = support.temp_cwd()
-        self.temp_cwd.__enter__()
-        self.addCleanup(self.temp_cwd.__exit__, None, None, None)
+        change_cwd = support.change_cwd(self.tmp_dir)
+        change_cwd.__enter__()
+        self.addCleanup(change_cwd.__exit__, None, None, None)
 
     def tearDown(self):
-        # Get everything back to normal
-        support.unload('xx')
-        sys.path = self.sys_path[0]
-        sys.path[:] = self.sys_path[1]
         import site
         site.USER_BASE = self.old_user_base
         from distutils.command import build_ext
         build_ext.USER_BASE = self.old_user_base
         super(BuildExtTestCase, self).tearDown()
 
     def build_ext(self, *args, **kwargs):
@@ -84,27 +78,42 @@
             sys.stdout = old_stdout
 
         if ALREADY_TESTED:
             self.skipTest('Already tested in %s' % ALREADY_TESTED)
         else:
             ALREADY_TESTED = type(self).__name__
 
-        import xx
+        code = textwrap.dedent(f"""
+            tmp_dir = {self.tmp_dir!r}
 
-        for attr in ('error', 'foo', 'new', 'roj'):
-            self.assertTrue(hasattr(xx, attr))
-
-        self.assertEqual(xx.foo(2, 5), 7)
-        self.assertEqual(xx.foo(13,15), 28)
-        self.assertEqual(xx.new().demo(), None)
-        if support.HAVE_DOCSTRINGS:
-            doc = 'This is a template module just for instruction.'
-            self.assertEqual(xx.__doc__, doc)
-        self.assertIsInstance(xx.Null(), xx.Null)
-        self.assertIsInstance(xx.Str(), xx.Str)
+            import sys
+            import unittest
+            from test import support
+
+            sys.path.insert(0, tmp_dir)
+            import xx
+
+            class Tests(unittest.TestCase):
+                def test_xx(self):
+                    for attr in ('error', 'foo', 'new', 'roj'):
+                        self.assertTrue(hasattr(xx, attr))
+
+                    self.assertEqual(xx.foo(2, 5), 7)
+                    self.assertEqual(xx.foo(13,15), 28)
+                    self.assertEqual(xx.new().demo(), None)
+                    if support.HAVE_DOCSTRINGS:
+                        doc = 'This is a template module just for instruction.'
+                        self.assertEqual(xx.__doc__, doc)
+                    self.assertIsInstance(xx.Null(), xx.Null)
+                    self.assertIsInstance(xx.Str(), xx.Str)
+
+
+            unittest.main()
+        """)
+        assert_python_ok('-c', code)
 
     def test_solaris_enable_shared(self):
         dist = Distribution({'name': 'xx'})
         cmd = self.build_ext(dist)
         old = sys.platform
 
         sys.platform = 'sunos' # fooling finalize_options
@@ -291,14 +300,27 @@
     def test_get_source_files(self):
         modules = [Extension('foo', ['xxx'], optional=False)]
         dist = Distribution({'name': 'xx', 'ext_modules': modules})
         cmd = self.build_ext(dist)
         cmd.ensure_finalized()
         self.assertEqual(cmd.get_source_files(), ['xxx'])
 
+    def test_unicode_module_names(self):
+        modules = [
+            Extension('foo', ['aaa'], optional=False),
+            Extension('föö', ['uuu'], optional=False),
+        ]
+        dist = Distribution({'name': 'xx', 'ext_modules': modules})
+        cmd = self.build_ext(dist)
+        cmd.ensure_finalized()
+        self.assertRegex(cmd.get_ext_filename(modules[0].name), r'foo(_d)?\..*')
+        self.assertRegex(cmd.get_ext_filename(modules[1].name), r'föö(_d)?\..*')
+        self.assertEqual(cmd.get_export_symbols(modules[0]), ['PyInit_foo'])
+        self.assertEqual(cmd.get_export_symbols(modules[1]), ['PyInitU_f_gkaa'])
+
     def test_compiler_option(self):
         # cmd.compiler is an option and
         # should not be overridden by a compiler instance
         # when the command is run
         dist = Distribution()
         cmd = self.build_ext(dist)
         cmd.compiler = 'unix'
@@ -471,15 +493,19 @@
         # Availability Macros.  We can't use the macro names since
         # at least one value we test with will not exist yet.
         if target[:2] < (10, 10):
             # for 10.1 through 10.9.x -> "10n0"
             target = '%02d%01d0' % target
         else:
             # for 10.10 and beyond -> "10nn00"
-            target = '%02d%02d00' % target
+            if len(target) >= 2:
+                target = '%02d%02d00' % target
+            else:
+                # 11 and later can have no minor version (11 instead of 11.0)
+                target = '%02d0000' % target
         deptarget_ext = Extension(
             'deptarget',
             [deptarget_c],
             extra_compile_args=['-DTARGET=%s'%(target,)],
         )
         dist = Distribution({
             'name': 'deptarget',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `standard_distutils-3.7.17/distutils/tests/test_build_py.py` & `standard_distutils-3.8.19/distutils/tests/test_build_py.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_build_scripts.py` & `standard_distutils-3.8.19/distutils/tests/test_build_scripts.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_check.py` & `standard_distutils-3.8.19/distutils/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_clean.py` & `standard_distutils-3.8.19/distutils/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_cmd.py` & `standard_distutils-3.8.19/distutils/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_config.py` & `standard_distutils-3.8.19/distutils/tests/test_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,15 @@
                             unittest.TestCase):
 
     def setUp(self):
         """Patches the environment."""
         super(BasePyPIRCCommandTestCase, self).setUp()
         self.tmp_dir = self.mkdtemp()
         os.environ['HOME'] = self.tmp_dir
+        os.environ['USERPROFILE'] = self.tmp_dir
         self.rc = os.path.join(self.tmp_dir, '.pypirc')
         self.dist = Distribution()
 
         class command(PyPIRCCommand):
             def __init__(self, dist):
                 PyPIRCCommand.__init__(self, dist)
             def initialize_options(self):
```

### Comparing `standard_distutils-3.7.17/distutils/tests/test_config_cmd.py` & `standard_distutils-3.8.19/distutils/tests/test_config_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,19 +35,24 @@
             f.close()
 
         dump_file(this_file, 'I am the header')
         self.assertEqual(len(self._logs), numlines+1)
 
     @unittest.skipIf(sys.platform == 'win32', "can't test on Windows")
     def test_search_cpp(self):
+        import shutil
         cmd = missing_compiler_executable(['preprocessor'])
         if cmd is not None:
             self.skipTest('The %r command is not found' % cmd)
         pkg_dir, dist = self.create_dist()
         cmd = config(dist)
+        cmd._check_compiler()
+        compiler = cmd.compiler
+        if sys.platform[:3] == "aix" and "xlc" in compiler.preprocessor[0].lower():
+            self.skipTest('xlc: The -E option overrides the -P, -o, and -qsyntaxonly options')
 
         # simple pattern searches
         match = cmd.search_cpp(pattern='xxx', body='/* xxx */')
         self.assertEqual(match, 0)
 
         match = cmd.search_cpp(pattern='_configtest', body='/* xxx */')
         self.assertEqual(match, 1)
```

### Comparing `standard_distutils-3.7.17/distutils/tests/test_core.py` & `standard_distutils-3.8.19/distutils/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_cygwinccompiler.py` & `standard_distutils-3.8.19/distutils/tests/test_cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_dep_util.py` & `standard_distutils-3.8.19/distutils/tests/test_dep_util.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_dir_util.py` & `standard_distutils-3.8.19/distutils/tests/test_dir_util.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_dist.py` & `standard_distutils-3.8.19/distutils/tests/test_dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,15 @@
                 os.environ['HOME'] = temp_dir
                 files = dist.find_config_files()
                 self.assertIn(user_filename, files)
 
             # win32-style
             if sys.platform == 'win32':
                 # home drive should be found
-                os.environ['HOME'] = temp_dir
+                os.environ['USERPROFILE'] = temp_dir
                 files = dist.find_config_files()
                 self.assertIn(user_filename, files,
                               '%r not found in %r' % (user_filename, files))
         finally:
             os.remove(user_filename)
 
     def test_fix_help_options(self):
```

### Comparing `standard_distutils-3.7.17/distutils/tests/test_extension.py` & `standard_distutils-3.8.19/distutils/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_file_util.py` & `standard_distutils-3.8.19/distutils/tests/test_file_util.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_filelist.py` & `standard_distutils-3.8.19/distutils/tests/test_filelist.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_install.py` & `standard_distutils-3.8.19/distutils/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_install_data.py` & `standard_distutils-3.8.19/distutils/tests/test_install_data.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_install_headers.py` & `standard_distutils-3.8.19/distutils/tests/test_install_headers.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_install_lib.py` & `standard_distutils-3.8.19/distutils/tests/test_install_lib.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_install_scripts.py` & `standard_distutils-3.8.19/distutils/tests/test_install_scripts.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_log.py` & `standard_distutils-3.8.19/distutils/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_msvc9compiler.py` & `standard_distutils-3.8.19/distutils/tests/test_msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_msvccompiler.py` & `standard_distutils-3.8.19/distutils/tests/test_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_register.py` & `standard_distutils-3.8.19/distutils/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_sdist.py` & `standard_distutils-3.8.19/distutils/tests/test_sdist.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_spawn.py` & `standard_distutils-3.8.19/distutils/tests/test_spawn.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_sysconfig.py` & `standard_distutils-3.8.19/distutils/tests/test_sysconfig.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_text_file.py` & `standard_distutils-3.8.19/distutils/tests/test_text_file.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_unixccompiler.py` & `standard_distutils-3.8.19/distutils/tests/test_unixccompiler.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_upload.py` & `standard_distutils-3.8.19/distutils/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_util.py` & `standard_distutils-3.8.19/distutils/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/tests/test_version.py` & `standard_distutils-3.8.19/distutils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/text_file.py` & `standard_distutils-3.8.19/distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/unixccompiler.py` & `standard_distutils-3.8.19/distutils/unixccompiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,15 @@
             #       MacOSX.platform/Developer/SDKs/MacOSX10.11.sdk/
             #       usr/lib/libedit.tbd
             # vs
             #   /usr/lib/libedit.dylib
             cflags = sysconfig.get_config_var('CFLAGS')
             m = re.search(r'-isysroot\s*(\S+)', cflags)
             if m is None:
-                sysroot = '/'
+                sysroot = _osx_support._default_sysroot(sysconfig.get_config_var('CC'))
             else:
                 sysroot = m.group(1)
 
 
 
         for dir in dirs:
             shared = os.path.join(dir, shared_f)
```

### Comparing `standard_distutils-3.7.17/distutils/util.py` & `standard_distutils-3.8.19/distutils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import sys
 from distutils.errors import DistutilsPlatformError
 from distutils.dep_util import newer
 from distutils.spawn import spawn
 from distutils import log
 from distutils.errors import DistutilsByteCompileError
 
-def get_platform ():
+def get_host_platform():
     """Return a string that identifies the current platform.  This is used mainly to
     distinguish platform-specific build directories and platform-specific built
     distributions.  Typically includes the OS name and version and the
     architecture (as supplied by 'os.uname()'), although the exact information
     included depends on the OS; eg. on Linux, the kernel version isn't
     particularly important.
 
@@ -34,14 +34,18 @@
 
     For other non-POSIX platforms, currently just returns 'sys.platform'.
 
     """
     if os.name == 'nt':
         if 'amd64' in sys.version.lower():
             return 'win-amd64'
+        if '(arm)' in sys.version.lower():
+            return 'win-arm32'
+        if '(arm64)' in sys.version.lower():
+            return 'win-arm64'
         return sys.platform
 
     # Set for cross builds explicitly
     if "_PYTHON_HOST_PLATFORM" in os.environ:
         return os.environ["_PYTHON_HOST_PLATFORM"]
 
     if os.name != "posix" or not hasattr(os, 'uname'):
@@ -86,16 +90,24 @@
         import _osx_support, distutils.sysconfig
         osname, release, machine = _osx_support.get_platform_osx(
                                         distutils.sysconfig.get_config_vars(),
                                         osname, release, machine)
 
     return "%s-%s-%s" % (osname, release, machine)
 
-# get_platform ()
-
+def get_platform():
+    if os.name == 'nt':
+        TARGET_TO_PLAT = {
+            'x86' : 'win32',
+            'x64' : 'win-amd64',
+            'arm' : 'win-arm32',
+        }
+        return TARGET_TO_PLAT.get(os.environ.get('VSCMD_ARG_TGT_ARCH')) or get_host_platform()
+    else:
+        return get_host_platform()
 
 def convert_path (pathname):
     """Return 'pathname' as a name that will work on the native filesystem,
     i.e. split it on '/' and put it back together again using the current
     directory separator.  Needed because filenames in the setup script are
     always supplied in Unix style, and have to be converted to the local
     convention before we can actually use them in the filesystem.  Raises
@@ -374,43 +386,42 @@
         log.info("writing byte-compilation script '%s'", script_name)
         if not dry_run:
             if script_fd is not None:
                 script = os.fdopen(script_fd, "w")
             else:
                 script = open(script_name, "w")
 
-            script.write("""\
+            with script:
+                script.write("""\
 from distutils.util import byte_compile
 files = [
 """)
 
-            # XXX would be nice to write absolute filenames, just for
-            # safety's sake (script should be more robust in the face of
-            # chdir'ing before running it).  But this requires abspath'ing
-            # 'prefix' as well, and that breaks the hack in build_lib's
-            # 'byte_compile()' method that carefully tacks on a trailing
-            # slash (os.sep really) to make sure the prefix here is "just
-            # right".  This whole prefix business is rather delicate -- the
-            # problem is that it's really a directory, but I'm treating it
-            # as a dumb string, so trailing slashes and so forth matter.
-
-            #py_files = map(os.path.abspath, py_files)
-            #if prefix:
-            #    prefix = os.path.abspath(prefix)
+                # XXX would be nice to write absolute filenames, just for
+                # safety's sake (script should be more robust in the face of
+                # chdir'ing before running it).  But this requires abspath'ing
+                # 'prefix' as well, and that breaks the hack in build_lib's
+                # 'byte_compile()' method that carefully tacks on a trailing
+                # slash (os.sep really) to make sure the prefix here is "just
+                # right".  This whole prefix business is rather delicate -- the
+                # problem is that it's really a directory, but I'm treating it
+                # as a dumb string, so trailing slashes and so forth matter.
+
+                #py_files = map(os.path.abspath, py_files)
+                #if prefix:
+                #    prefix = os.path.abspath(prefix)
 
-            script.write(",\n".join(map(repr, py_files)) + "]\n")
-            script.write("""
+                script.write(",\n".join(map(repr, py_files)) + "]\n")
+                script.write("""
 byte_compile(files, optimize=%r, force=%r,
              prefix=%r, base_dir=%r,
              verbose=%r, dry_run=0,
              direct=1)
 """ % (optimize, force, prefix, base_dir, verbose))
 
-            script.close()
-
         cmd = [sys.executable]
         cmd.extend(subprocess._optim_args_from_interpreter_flags())
         cmd.append(script_name)
         spawn(cmd, dry_run=dry_run)
         execute(os.remove, (script_name,), "removing %s" % script_name,
                 dry_run=dry_run)
```

### Comparing `standard_distutils-3.7.17/distutils/version.py` & `standard_distutils-3.8.19/distutils/version.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/distutils/versionpredicate.py` & `standard_distutils-3.8.19/distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `standard_distutils-3.7.17/pyproject.toml` & `standard_distutils-3.8.19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "standard-distutils"
-version = "3.7.17"
+version = "3.8.19"
 description = "Standard library distutils redistribution. \"dead battery\"."
 keywords = ["stdlib"]
 authors = [
     { name = "Python Developers", email = "python-deadlib@youknowone.org" }
 ]
 readme = "README.rst"
 license = {name = "PSF", file = "LICENSE"}
```

### Comparing `standard_distutils-3.7.17/standard_distutils.egg-info/PKG-INFO` & `standard_distutils-3.8.19/standard_distutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: standard-distutils
-Version: 3.7.17
+Version: 3.8.19
 Summary: Standard library distutils redistribution. "dead battery".
 Author-email: Python Developers <python-deadlib@youknowone.org>
 License: Copyright © 2001-2023 Python Software Foundation; All Rights Reserved
         
         This code originally taken from the Python 3.11.3 distribution
         and it is therefore now released under the following Python-style
         license:
```

### Comparing `standard_distutils-3.7.17/standard_distutils.egg-info/SOURCES.txt` & `standard_distutils-3.8.19/standard_distutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

