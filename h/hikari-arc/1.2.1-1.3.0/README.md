# Comparing `tmp/hikari-arc-1.2.1.tar.gz` & `tmp/hikari_arc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari-arc-1.2.1.tar", last modified: Tue Feb  6 15:53:26 2024, max compression
+gzip compressed data, was "hikari_arc-1.3.0.tar", last modified: Sun May 12 19:49:36 2024, max compression
```

## Comparing `hikari-arc-1.2.1.tar` & `hikari_arc-1.3.0.tar`

### file list

```diff
@@ -1,88 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.038520 hikari-arc-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-02-06 15:53:26.038520 hikari-arc-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.026520 hikari-arc-1.2.1/arc/
--rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.030521 hikari-arc-1.2.1/arc/abc/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48291 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/abc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28429 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/abc/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/abc/concurrency_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/abc/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/abc/hookable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/abc/limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/abc/option.py
--rw-r--r--   0 runner    (1001) docker     (127)    19699 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/abc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17850 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.030521 hikari-arc-1.2.1/arc/command/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.030521 hikari-arc-1.2.1/arc/command/option/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/option/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/option/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/option/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/option/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/option/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/option/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/option/mentionable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/option/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/option/str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/option/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    35285 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/slash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/command/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.030521 hikari-arc-1.2.1/arc/context/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/context/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    38472 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.030521 hikari-arc-1.2.1/arc/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.034520 hikari-arc-1.2.1/arc/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/internal/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/internal/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/internal/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13095 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/internal/sigparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12587 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/internal/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/internal/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.034520 hikari-arc-1.2.1/arc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/utils/concurrency_limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.034520 hikari-arc-1.2.1/arc/utils/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/utils/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/utils/hooks/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/utils/hooks/limiters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/utils/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/arc/utils/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/cron_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/doc_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.034520 hikari-arc-1.2.1/hikari_arc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-02-06 15:53:26.000000 hikari-arc-1.2.1/hikari_arc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-02-06 15:53:26.000000 hikari-arc-1.2.1/hikari_arc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 15:53:26.000000 hikari-arc-1.2.1/hikari_arc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 15:53:25.000000 hikari-arc-1.2.1/hikari_arc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-06 15:53:26.000000 hikari-arc-1.2.1/hikari_arc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-06 15:53:26.000000 hikari-arc-1.2.1/hikari_arc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/rest_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 15:53:26.038520 hikari-arc-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 15:53:26.034520 hikari-arc-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/tests/test_context_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/tests/test_di.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/tests/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/tests/test_sigparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-02-06 15:53:16.000000 hikari-arc-1.2.1/tests/test_slash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.047094 hikari_arc-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-12 19:49:36.047094 hikari_arc-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.035094 hikari_arc-1.3.0/arc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.035094 hikari_arc-1.3.0/arc/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54162 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28769 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/concurrency_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/hookable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19703 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.035094 hikari_arc-1.3.0/arc/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.035094 hikari_arc-1.3.0/arc/command/option/
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/command/option/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/custom/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/custom/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/mentionable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35485 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/slash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/context/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39977 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/sigparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/concurrency_limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/utils/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/hooks/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/hooks/limiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/cron_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/doc_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.043094 hikari_arc-1.3.0/hikari_arc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-12 19:49:36.000000 hikari_arc-1.3.0/hikari_arc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-12 19:49:36.000000 hikari_arc-1.3.0/hikari_arc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:49:36.000000 hikari_arc-1.3.0/hikari_arc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:49:35.000000 hikari_arc-1.3.0/hikari_arc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-12 19:49:36.000000 hikari_arc-1.3.0/hikari_arc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-12 19:49:36.000000 hikari_arc-1.3.0/hikari_arc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/rest_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:49:36.047094 hikari_arc-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.043094 hikari_arc-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_context_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_di.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_sigparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_slash.py
```

### Comparing `hikari-arc-1.2.1/LICENSE` & `hikari_arc-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/PKG-INFO` & `hikari_arc-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-arc
-Version: 1.2.1
+Version: 1.3.0
 Summary: A command handler for hikari with a focus on type-safety and correctness.
 Home-page: https://github.com/hypergonial/hikari-arc
 Author: hypergonial
 Author-email: git@hypergonial.com
 Maintainer: hypergonial
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,37 +20,37 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10.0,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hikari>=2.0.0.dev122
-Requires-Dist: alluka>=0.1.4
+Requires-Dist: alluka<0.4,>=0.3.0
 Requires-Dist: attrs>=23.1
 Requires-Dist: colorama; sys_platform == "win32"
 Provides-Extra: docs
-Requires-Dist: mkdocs-material[imaging]~=9.5.7; extra == "docs"
-Requires-Dist: mkdocs~=1.5.3; extra == "docs"
-Requires-Dist: mkdocstrings-python~=1.8.0; extra == "docs"
-Requires-Dist: black~=24.1.1; extra == "docs"
+Requires-Dist: mkdocs-material[imaging]~=9.5.21; extra == "docs"
+Requires-Dist: mkdocs~=1.6.0; extra == "docs"
+Requires-Dist: mkdocstrings-python~=1.10.0; extra == "docs"
+Requires-Dist: black~=24.4.2; extra == "docs"
 Requires-Dist: griffe-inherited-docstrings~=1.0.0; extra == "docs"
-Requires-Dist: mkdocs-glightbox~=0.3.7; extra == "docs"
+Requires-Dist: mkdocs-glightbox~=0.4.0; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: ruff==0.1.14; extra == "dev"
-Requires-Dist: pyright==1.1.350; extra == "dev"
-Requires-Dist: nox==2023.4.22; extra == "dev"
-Requires-Dist: typing_extensions==4.9.0; extra == "dev"
-Requires-Dist: pytest==7.4.4; extra == "dev"
-Requires-Dist: pytest-asyncio==0.23.4; extra == "dev"
-Requires-Dist: slotscheck==0.17.1; extra == "dev"
+Requires-Dist: ruff==0.4.4; extra == "dev"
+Requires-Dist: pyright==1.1.362; extra == "dev"
+Requires-Dist: nox==2024.4.15; extra == "dev"
+Requires-Dist: typing_extensions==4.11.0; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "dev"
+Requires-Dist: slotscheck==0.19.0; extra == "dev"
 Provides-Extra: rest
 Requires-Dist: hikari[server]>=2.0.0.dev122; extra == "rest"
 Provides-Extra: cron
-Requires-Dist: croniter==2.0.1; extra == "cron"
-Requires-Dist: types-croniter==2.0.0.20240106; extra == "cron"
+Requires-Dist: croniter==2.0.5; extra == "cron"
+Requires-Dist: types-croniter==2.0.0.20240423; extra == "cron"
 
 # hikari-arc
 
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/hikari-arc)](https://pypi.org/project/hikari-arc)
 [![CI](https://github.com/hypergonial/hikari-arc/actions/workflows/ci.yml/badge.svg)](https://github.com/hypergonial/hikari-arc/actions/workflows/ci.yml)
```

### Comparing `hikari-arc-1.2.1/README.md` & `hikari_arc-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/__init__.py` & `hikari_arc-1.3.0/arc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 GitHub:
 https://github.com/hypergonial/hikari-arc
 Documentation:
 https://arc.hypergonial.com
 """
 
 from alluka import Client as Injector
+from alluka import OverridingContext as InjectorOverridingContext
 from alluka import inject
 
 from arc import abc, command, ext, utils
 
 from .abc import HookResult, Option, OptionType, with_concurrency_limit, with_hook, with_post_hook
 from .client import (
     GatewayClient,
@@ -24,16 +25,19 @@
     RESTContext,
     RESTPlugin,
 )
 from .command import (
     AttachmentParams,
     BoolParams,
     ChannelParams,
+    ColorParams,
+    ColourParams,
     FloatParams,
     IntParams,
+    MemberParams,
     MentionableParams,
     MessageCommand,
     RoleParams,
     SlashCommand,
     SlashGroup,
     SlashSubCommand,
     SlashSubGroup,
@@ -61,14 +65,15 @@
     GuildOnlyError,
     HookAbortError,
     InteractionResponseError,
     InvokerMissingPermissionsError,
     MaxConcurrencyReachedError,
     NoResponseIssuedError,
     NotOwnerError,
+    OptionConverterFailureError,
     ResponseAlreadyIssuedError,
     UnderCooldownError,
 )
 from .events import ArcEvent, CommandErrorEvent, StartedEvent, StoppingEvent
 from .extension import loader, unloader
 from .internal.about import __author__, __author_email__, __license__, __maintainer__, __url__, __version__
 from .locale import (
@@ -109,24 +114,27 @@
     "__maintainer__",
     "AutodeferMode",
     "inject",
     "Injector",
     "AutocompleteData",
     "Option",
     "Context",
-    "Context",
+    "InjectorOverridingContext",
     "BoolParams",
     "IntParams",
     "StrParams",
     "FloatParams",
     "UserParams",
     "ChannelParams",
     "RoleParams",
     "MentionableParams",
     "AttachmentParams",
+    "MemberParams",
+    "ColorParams",
+    "ColourParams",
     "SlashCommand",
     "SlashGroup",
     "SlashSubCommand",
     "SlashSubGroup",
     "MessageCommand",
     "UserCommand",
     "message_command",
@@ -154,14 +162,15 @@
     "NoResponseIssuedError",
     "ResponseAlreadyIssuedError",
     "ExtensionError",
     "ExtensionLoadError",
     "ExtensionUnloadError",
     "HookAbortError",
     "InteractionResponseError",
+    "OptionConverterFailureError",
     "PluginBase",
     "RESTPluginBase",
     "GatewayPluginBase",
     "loader",
     "unloader",
     "ArcEvent",
     "CommandErrorEvent",
```

### Comparing `hikari-arc-1.2.1/arc/__main__.py` & `hikari_arc-1.3.0/arc/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """CLI entry point for arc."""
+
 import os
 import platform
 import sys
 
 import hikari
 
 import arc
```

### Comparing `hikari-arc-1.2.1/arc/abc/__init__.py` & `hikari_arc-1.3.0/arc/abc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .command import CallableCommandBase, CallableCommandProto, CommandBase, CommandProto
 from .concurrency_limiting import ConcurrencyLimiterProto, HasConcurrencyLimiter, with_concurrency_limit
 from .error_handler import HasErrorHandler
 from .hookable import Hookable, HookResult, with_hook, with_post_hook
 from .limiter import LimiterProto
 from .option import (
     CommandOptionBase,
+    ConverterOption,
     Option,
     OptionBase,
     OptionParams,
     OptionType,
     OptionWithChoices,
     OptionWithChoicesParams,
 )
@@ -25,14 +26,15 @@
     "CommandProto",
     "CallableCommandProto",
     "CallableCommandBase",
     "Option",
     "OptionBase",
     "OptionType",
     "CommandOptionBase",
+    "ConverterOption",
     "OptionParams",
     "OptionWithChoices",
     "OptionWithChoicesParams",
     "Client",
     "PluginBase",
     "Hookable",
     "HookResult",
```

### Comparing `hikari-arc-1.2.1/arc/abc/client.py` & `hikari_arc-1.3.0/arc/abc/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,27 +18,30 @@
 from arc.abc.command import CallableCommandBase, _CommandSettings
 from arc.abc.plugin import PluginBase
 from arc.command.message import MessageCommand
 from arc.command.slash import SlashCommand, SlashGroup, SlashSubCommand, SlashSubGroup
 from arc.command.user import UserCommand
 from arc.context import AutodeferMode, Context
 from arc.errors import ExtensionLoadError, ExtensionUnloadError
+from arc.internal.deprecation import warn_deprecate
 from arc.internal.sync import _sync_commands
 from arc.internal.types import (
     AppT,
     BuilderT,
     CommandLocaleRequestT,
     CustomLocaleRequestT,
     ErrorHandlerCallbackT,
     HookT,
+    InjectionHookT,
     LifeCycleHookT,
     OptionLocaleRequestT,
     PostHookT,
     ResponseBuilderT,
 )
+from arc.internal.version import Version
 from arc.locale import CommandLocaleRequest, LocaleResponse, OptionLocaleRequest
 
 if t.TYPE_CHECKING:
     import typing_extensions as te
 
     from arc.abc.command import CommandBase
     from arc.abc.concurrency_limiting import ConcurrencyLimiterProto
@@ -94,18 +97,19 @@
         "_user_commands",
         "_injector",
         "_autosync",
         "_plugins",
         "_loaded_extensions",
         "_hooks",
         "_post_hooks",
+        "_injection_hooks",
         "_owner_ids",
         "_error_handler",
-        "_startup_hook",
-        "_shutdown_hook",
+        "_startup_hooks",
+        "_shutdown_hooks",
         "_provided_locales",
         "_command_locale_provider",
         "_option_locale_provider",
         "_custom_locale_provider",
         "_cmd_settings",
         "_concurrency_limiter",
         "_tasks",
@@ -145,22 +149,23 @@
         self._message_commands: dict[str, MessageCommand[te.Self]] = {}
         self._user_commands: dict[str, UserCommand[te.Self]] = {}
         self._injector: alluka.abc.Client = injector or alluka.Client()
         self._plugins: dict[str, PluginBase[te.Self]] = {}
         self._loaded_extensions: list[str] = []
         self._hooks: list[HookT[te.Self]] = []
         self._post_hooks: list[PostHookT[te.Self]] = []
+        self._injection_hooks: list[InjectionHookT[te.Self]] = []
         self._owner_ids: list[hikari.Snowflake] = []
         self._tasks: set[asyncio.Task[t.Any]] = set()
         self._started: asyncio.Event = asyncio.Event()
         self._application: hikari.Application | None = None
         self._error_handler: ErrorHandlerCallbackT[te.Self] | None = None
         self._concurrency_limiter: ConcurrencyLimiterProto[te.Self] | None = None
-        self._startup_hook: LifeCycleHookT[te.Self] | None = None
-        self._shutdown_hook: LifeCycleHookT[te.Self] | None = None
+        self._startup_hooks: list[LifeCycleHookT[te.Self] | None] = [None]
+        self._shutdown_hooks: list[LifeCycleHookT[te.Self] | None] = [None]
         self._command_locale_provider: CommandLocaleRequestT | None = None
         self._option_locale_provider: OptionLocaleRequestT | None = None
         self._custom_locale_provider: CustomLocaleRequestT | None = None
 
         self._injector.set_type_dependency(Client[t.Any], self)
         self._injector.set_type_dependency(Client, self)
         self._injector.set_type_dependency(type(self), self)
@@ -281,25 +286,38 @@
 
         logger.debug(f"Fetched application: '{self.application}'")
 
         if self._autosync:
             await _sync_commands(self)
 
         try:
-            if self._startup_hook:
-                await self._startup_hook(self)
+            for hook in self._startup_hooks:
+                if hook:
+                    try:
+                        await hook(self)
+                    except Exception as e:
+                        logger.error(f"Error in startup hook '{hook.__name__}': {e}")
+                        traceback.print_exc()
         finally:
             self._started.set()
 
     async def _on_shutdown(self) -> None:
         """Called when the client is shutting down.
         Reserved for internal shutdown logic.
         """
-        if self._shutdown_hook:
-            await self._shutdown_hook(self)
+        for hook in self._shutdown_hooks:
+            if hook:
+                try:
+                    await hook(self)
+                except Exception as e:
+                    logger.error(f"Error in shutdown hook '{hook.__name__}': {e}")
+                    traceback.print_exc()
+
+        for task in self._tasks:
+            task.cancel()
 
     async def _on_error(self, ctx: Context[te.Self], exception: Exception) -> None:
         if self._error_handler is not None:
             try:
                 return await self._error_handler(ctx, exception)
             except Exception as e:
                 exception = e
@@ -307,14 +325,24 @@
         print(f"Unhandled error in command '{ctx.command.name}' callback: {exception}", file=sys.stderr)
         traceback.print_exception(type(exception), exception, exception.__traceback__, file=sys.stderr)
         with suppress(Exception):
             # Try to respond to make autodefer less jarring when a command fails.
             if ctx.is_valid:
                 await ctx.respond("❌ Something went wrong. Please contact the bot developer.")
 
+    async def _create_overriding_ctx_for_command(self, ctx: Context[te.Self]) -> alluka.OverridingContext:
+        inj_ctx = alluka.OverridingContext.from_client(self.injector)
+
+        for hook in self._injection_hooks:
+            if inspect.iscoroutinefunction(hook):
+                await hook(ctx, inj_ctx)
+            else:
+                hook(ctx, inj_ctx)
+        return inj_ctx
+
     def _provide_command_locale(self, request: CommandLocaleRequest) -> LocaleResponse:
         """Provide a locale for a command."""
         if self._command_locale_provider is None:
             return LocaleResponse(name=request.command.name, description=getattr(request.command, "description", None))
 
         return self._command_locale_provider(request)
 
@@ -413,34 +441,32 @@
             return
 
         return await command._on_autocomplete(interaction)
 
     @t.overload
     def walk_commands(
         self, command_type: t.Literal[hikari.CommandType.USER], *, callable_only: bool = False
-    ) -> t.Iterator[UserCommand[te.Self]]:
-        ...
+    ) -> t.Iterator[UserCommand[te.Self]]: ...
 
     @t.overload
     def walk_commands(
         self, command_type: t.Literal[hikari.CommandType.MESSAGE], *, callable_only: bool = False
-    ) -> t.Iterator[MessageCommand[te.Self]]:
-        ...
+    ) -> t.Iterator[MessageCommand[te.Self]]: ...
 
     @t.overload
     def walk_commands(
         self, command_type: t.Literal[hikari.CommandType.SLASH], *, callable_only: t.Literal[False] = False
-    ) -> t.Iterator[SlashCommand[te.Self] | SlashSubCommand[te.Self] | SlashGroup[te.Self] | SlashSubGroup[te.Self]]:
-        ...
+    ) -> t.Iterator[
+        SlashCommand[te.Self] | SlashSubCommand[te.Self] | SlashGroup[te.Self] | SlashSubGroup[te.Self]
+    ]: ...
 
     @t.overload
     def walk_commands(
         self, command_type: t.Literal[hikari.CommandType.SLASH], *, callable_only: t.Literal[True] = True
-    ) -> t.Iterator[SlashCommand[te.Self] | SlashSubCommand[te.Self]]:
-        ...
+    ) -> t.Iterator[SlashCommand[te.Self] | SlashSubCommand[te.Self]]: ...
 
     def walk_commands(  # noqa: C901
         self, command_type: hikari.CommandType, *, callable_only: bool = False
     ) -> t.Iterator[t.Any]:
         """Iterate over all commands of a certain type added to this plugin.
 
         Parameters
@@ -503,20 +529,20 @@
                 yield command
 
         elif hikari.CommandType.USER is command_type:
             for command in self._user_commands.values():
                 yield command
 
     @t.overload
-    def include(self) -> t.Callable[[CallableCommandBase[te.Self, BuilderT]], CallableCommandBase[te.Self, BuilderT]]:
-        ...
+    def include(
+        self,
+    ) -> t.Callable[[CallableCommandBase[te.Self, BuilderT]], CallableCommandBase[te.Self, BuilderT]]: ...
 
     @t.overload
-    def include(self, command: CallableCommandBase[te.Self, BuilderT]) -> CallableCommandBase[te.Self, BuilderT]:
-        ...
+    def include(self, command: CallableCommandBase[te.Self, BuilderT]) -> CallableCommandBase[te.Self, BuilderT]: ...
 
     def include(
         self, command: CallableCommandBase[te.Self, BuilderT] | None = None
     ) -> (
         CallableCommandBase[te.Self, BuilderT]
         | t.Callable[[CallableCommandBase[te.Self, BuilderT]], CallableCommandBase[te.Self, BuilderT]]
     ):
@@ -699,20 +725,18 @@
         te.Self
             The client for chaining calls.
         """
         self._concurrency_limiter = limiter
         return self
 
     @t.overload
-    def add_hook(self, hook: HookT[te.Self]) -> te.Self:
-        ...
+    def add_hook(self, hook: HookT[te.Self]) -> te.Self: ...
 
     @t.overload
-    def add_hook(self) -> t.Callable[[HookT[te.Self]], HookT[te.Self]]:
-        ...
+    def add_hook(self) -> t.Callable[[HookT[te.Self]], HookT[te.Self]]: ...
 
     def add_hook(self, hook: HookT[te.Self] | None = None) -> te.Self | t.Callable[[HookT[te.Self]], HookT[te.Self]]:
         """Add a pre-execution hook to this client.
         This hook will be executed before **every command** that is added to this client.
 
         Parameters
         ----------
@@ -735,20 +759,18 @@
         def decorator(hook: HookT[te.Self]) -> HookT[te.Self]:
             self._hooks.append(hook)
             return hook
 
         return decorator
 
     @t.overload
-    def add_post_hook(self, hook: PostHookT[te.Self]) -> te.Self:
-        ...
+    def add_post_hook(self, hook: PostHookT[te.Self]) -> te.Self: ...
 
     @t.overload
-    def add_post_hook(self) -> t.Callable[[PostHookT[te.Self]], PostHookT[te.Self]]:
-        ...
+    def add_post_hook(self) -> t.Callable[[PostHookT[te.Self]], PostHookT[te.Self]]: ...
 
     def add_post_hook(
         self, hook: PostHookT[te.Self] | None = None
     ) -> te.Self | t.Callable[[PostHookT[te.Self]], PostHookT[te.Self]]:
         """Add a post-execution hook to this client.
         This hook will be executed after **every command** that is added to this client.
 
@@ -776,20 +798,84 @@
         def decorator(hook: PostHookT[te.Self]) -> PostHookT[te.Self]:
             self._post_hooks.append(hook)
             return hook
 
         return decorator
 
     @t.overload
-    def set_error_handler(self, handler: ErrorHandlerCallbackT[te.Self]) -> te.Self:
-        ...
+    def add_injection_hook(self, hook: InjectionHookT[te.Self]) -> te.Self: ...
+
+    @t.overload
+    def add_injection_hook(self) -> t.Callable[[InjectionHookT[te.Self]], InjectionHookT[te.Self]]: ...
+
+    def add_injection_hook(
+        self, hook: InjectionHookT[te.Self] | None = None
+    ) -> te.Self | t.Callable[[InjectionHookT[te.Self]], InjectionHookT[te.Self]]:
+        """Add an injection hook to this client.
+        This hook will be called when a command is called, and an OverridingContext is passed, allowing you to inject dependencies for the command call.
+
+        Parameters
+        ----------
+        hook : InjectionHookT[te.Self]
+            The hook to add.
+
+        Returns
+        -------
+        te.Self
+            The client for chaining calls.
+
+        Example
+        -------
+        ```py
+        @client.add_injection_hook
+        async def inject(ctx: arc.GatewayContext, inj_ctx: arc.InjectorOverridingContext) -> None:
+            foo: MyType = example_data[ctx.guild_id]
+            inj_ctx.set_type_dependency(MyType, foo)
+        ```
+
+        See Also
+        --------
+        - [`Client.set_type_dependency`][arc.client.Client.set_type_dependency]
+        """
+        if hook is not None:
+            self._injection_hooks.append(hook)
+            return self
+
+        def decorator(hook: InjectionHookT[te.Self]) -> InjectionHookT[te.Self]:
+            self._injection_hooks.append(hook)
+            return hook
+
+        return decorator
+
+    def remove_injection_hook(self, hook: InjectionHookT[te.Self]) -> te.Self:
+        """Remove an injection hook from this client.
+
+        Parameters
+        ----------
+        hook : InjectionHookT[te.Self]
+            The hook to remove.
+
+        Returns
+        -------
+        te.Self
+            The client for chaining calls.
+
+        Raises
+        ------
+        ValueError
+            If the hook is not registered with this client.
+        """
+        self._injection_hooks.remove(hook)
+        return self
+
+    @t.overload
+    def set_error_handler(self, handler: ErrorHandlerCallbackT[te.Self]) -> te.Self: ...
 
     @t.overload
-    def set_error_handler(self) -> t.Callable[[ErrorHandlerCallbackT[te.Self]], te.Self]:
-        ...
+    def set_error_handler(self) -> t.Callable[[ErrorHandlerCallbackT[te.Self]], te.Self]: ...
 
     def set_error_handler(
         self, handler: ErrorHandlerCallbackT[te.Self] | None = None
     ) -> te.Self | t.Callable[[ErrorHandlerCallbackT[te.Self]], te.Self]:
         """Decorator to set the error handler for this client.
 
         This will be called when a command callback raises an exception
@@ -830,28 +916,124 @@
 
         if handler is not None:
             return decorator(handler)
 
         return decorator
 
     @t.overload
-    def set_startup_hook(self, hook: LifeCycleHookT[te.Self]) -> te.Self:
-        ...
+    def add_startup_hook(self, hook: LifeCycleHookT[te.Self]) -> te.Self: ...
+
+    @t.overload
+    def add_startup_hook(self) -> t.Callable[[LifeCycleHookT[te.Self]], te.Self]: ...
+
+    def add_startup_hook(
+        self, hook: LifeCycleHookT[te.Self] | None = None
+    ) -> te.Self | t.Callable[[LifeCycleHookT[te.Self]], te.Self]:
+        """Decorator to add a startup hook for this client.
+
+        This will be called when the client starts up.
+
+        Parameters
+        ----------
+        hook : LifeCycleHookT[te.Self]
+            The startup hook to add.
+
+        Returns
+        -------
+        te.Self
+            The client for chaining calls.
+
+        Examples
+        --------
+        ```py
+        @client.add_startup_hook
+        async def startup_hook(client: arc.GatewayClient) -> None:
+            print("Client started up!")
+        ```
+
+        Or, as a function:
+
+        ```py
+        client.add_startup_hook(startup_hook)
+        ```
+        """
+
+        def decorator(handler: LifeCycleHookT[te.Self]) -> te.Self:
+            self._startup_hooks.append(handler)
+            return self
+
+        if hook is not None:
+            return decorator(hook)
+
+        return decorator
+
+    @t.overload
+    def add_shutdown_hook(self, hook: LifeCycleHookT[te.Self]) -> te.Self: ...
+
+    @t.overload
+    def add_shutdown_hook(self) -> t.Callable[[LifeCycleHookT[te.Self]], te.Self]: ...
+
+    def add_shutdown_hook(
+        self, hook: LifeCycleHookT[te.Self] | None = None
+    ) -> te.Self | t.Callable[[LifeCycleHookT[te.Self]], te.Self]:
+        """Decorator to add a shutdown hook for this client.
+
+        This will be called when the client shuts down.
+
+        Parameters
+        ----------
+        hook : LifeCycleHookT[te.Self]
+            The shutdown hook to add.
+
+        Returns
+        -------
+        te.Self
+            The client for chaining calls.
+
+        Examples
+        --------
+        ```py
+        @client.add_shutdown_hook
+        async def shutdown_hook(client: arc.GatewayClient) -> None:
+            print("Client shut down!")
+        ```
+
+        Or, as a function:
+
+        ```py
+        client.add_shutdown_hook(shutdown_hook)
+        ```
+        """
+
+        def decorator(handler: LifeCycleHookT[te.Self]) -> te.Self:
+            self._shutdown_hooks.append(handler)
+            return self
+
+        if hook is not None:
+            return decorator(hook)
+
+        return decorator
+
+    @t.overload
+    def set_startup_hook(self, hook: LifeCycleHookT[te.Self]) -> te.Self: ...
 
     @t.overload
-    def set_startup_hook(self) -> t.Callable[[LifeCycleHookT[te.Self]], te.Self]:
-        ...
+    def set_startup_hook(self) -> t.Callable[[LifeCycleHookT[te.Self]], te.Self]: ...
 
     def set_startup_hook(
         self, hook: LifeCycleHookT[te.Self] | None = None
     ) -> te.Self | t.Callable[[LifeCycleHookT[te.Self]], te.Self]:
         """Decorator to set the startup hook for this client.
 
         This will be called when the client starts up.
 
+        !!! warning "Deprecation Notice"
+            This method is deprecated and will be removed in version `2.0.0`.
+            Use [`Client.add_startup_hook`][arc.client.Client.add_startup_hook] instead.
+
         Parameters
         ----------
         hook : LifeCycleHookT[te.Self]
             The startup hook to set.
 
         Returns
         -------
@@ -868,39 +1050,42 @@
 
         Or, as a function:
 
         ```py
         client.set_startup_hook(startup_hook)
         ```
         """
+        warn_deprecate(what="set_startup_hook", when=Version(2, 0, 0), use_instead="add_startup_hook")
 
         def decorator(handler: LifeCycleHookT[te.Self]) -> te.Self:
-            self._startup_hook = handler
+            self._startup_hooks[0] = handler
             return self
 
         if hook is not None:
             return decorator(hook)
 
         return decorator
 
     @t.overload
-    def set_shutdown_hook(self, hook: LifeCycleHookT[te.Self]) -> te.Self:
-        ...
+    def set_shutdown_hook(self, hook: LifeCycleHookT[te.Self]) -> te.Self: ...
 
     @t.overload
-    def set_shutdown_hook(self) -> t.Callable[[LifeCycleHookT[te.Self]], te.Self]:
-        ...
+    def set_shutdown_hook(self) -> t.Callable[[LifeCycleHookT[te.Self]], te.Self]: ...
 
     def set_shutdown_hook(
         self, hook: LifeCycleHookT[te.Self] | None = None
     ) -> te.Self | t.Callable[[LifeCycleHookT[te.Self]], te.Self]:
         """Decorator to set the shutdown hook for this client.
 
         This will be called when the client shuts down.
 
+        !!! warning "Deprecation Notice"
+            This method is deprecated and will be removed in version `2.0.0`.
+            Use [`Client.add_shutdown_hook`][arc.client.Client.add_shutdown_hook] instead.
+
         Parameters
         ----------
         hook : LifeCycleHookT[te.Self]
             The shutdown hook to set.
 
         Returns
         -------
@@ -917,31 +1102,30 @@
 
         Or, as a function:
 
         ```py
         client.set_shutdown_hook(shutdown_hook)
         ```
         """
+        warn_deprecate(what="set_shutdown_hook", when=Version(2, 0, 0), use_instead="add_shutdown_hook")
 
         def decorator(handler: LifeCycleHookT[te.Self]) -> te.Self:
-            self._shutdown_hook = handler
+            self._shutdown_hooks[0] = handler
             return self
 
         if hook is not None:
             return decorator(hook)
 
         return decorator
 
     @t.overload
-    def set_command_locale_provider(self, provider: CommandLocaleRequestT) -> te.Self:
-        ...
+    def set_command_locale_provider(self, provider: CommandLocaleRequestT) -> te.Self: ...
 
     @t.overload
-    def set_command_locale_provider(self) -> t.Callable[[CommandLocaleRequestT], te.Self]:
-        ...
+    def set_command_locale_provider(self) -> t.Callable[[CommandLocaleRequestT], te.Self]: ...
 
     def set_command_locale_provider(
         self, provider: CommandLocaleRequestT | None = None
     ) -> te.Self | t.Callable[[CommandLocaleRequestT], te.Self]:
         """Decorator to set the command locale provider for this client.
 
         This will be called for each command for each locale.
@@ -977,20 +1161,18 @@
 
         if provider is not None:
             return decorator(provider)
 
         return decorator
 
     @t.overload
-    def set_option_locale_provider(self, provider: OptionLocaleRequestT) -> te.Self:
-        ...
+    def set_option_locale_provider(self, provider: OptionLocaleRequestT) -> te.Self: ...
 
     @t.overload
-    def set_option_locale_provider(self) -> t.Callable[[OptionLocaleRequestT], te.Self]:
-        ...
+    def set_option_locale_provider(self) -> t.Callable[[OptionLocaleRequestT], te.Self]: ...
 
     def set_option_locale_provider(
         self, provider: OptionLocaleRequestT | None = None
     ) -> te.Self | t.Callable[[OptionLocaleRequestT], te.Self]:
         """Decorator to set the option locale provider for this client.
 
         This will be called for each option of each command for each locale.
@@ -1026,20 +1208,18 @@
 
         if provider is not None:
             return decorator(provider)
 
         return decorator
 
     @t.overload
-    def set_custom_locale_provider(self, provider: CustomLocaleRequestT) -> te.Self:
-        ...
+    def set_custom_locale_provider(self, provider: CustomLocaleRequestT) -> te.Self: ...
 
     @t.overload
-    def set_custom_locale_provider(self) -> t.Callable[[CustomLocaleRequestT], te.Self]:
-        ...
+    def set_custom_locale_provider(self) -> t.Callable[[CustomLocaleRequestT], te.Self]: ...
 
     def set_custom_locale_provider(
         self, provider: CustomLocaleRequestT | None = None
     ) -> te.Self | t.Callable[[CustomLocaleRequestT], te.Self]:
         """Decorator to set the custom locale provider for this client.
 
         This will be called for each custom locale request performed via [`Context.loc()`][arc.context.base.Context.loc].
@@ -1281,20 +1461,18 @@
         - [`Client.inject_dependencies`][arc.client.Client.inject_dependencies]
             A decorator to inject dependencies into arbitrary functions.
         """
         self._injector.set_type_dependency(type_, instance)
         return self
 
     @t.overload
-    def get_type_dependency(self, type_: type[T]) -> T:
-        ...
+    def get_type_dependency(self, type_: type[T]) -> T: ...
 
     @t.overload
-    def get_type_dependency(self, type_: type[T], *, default: DefaultT) -> T | DefaultT:
-        ...
+    def get_type_dependency(self, type_: type[T], *, default: DefaultT) -> T | DefaultT: ...
 
     def get_type_dependency(
         self, type_: type[T], *, default: DefaultT | hikari.UndefinedType = hikari.UNDEFINED
     ) -> T | DefaultT:
         """Get a type dependency for this client.
 
         Parameters
@@ -1312,28 +1490,23 @@
 
         Raises
         ------
         KeyError
             If the dependency does not exist and `default` was not provided.
         """
         if default is hikari.UNDEFINED:
-            value = self._injector.get_type_dependency(type_)
-            if isinstance(value, alluka.abc.Undefined):
-                raise KeyError(f"Could not resolve dependency of type {type_}.")
-            return value
+            return self._injector.get_type_dependency(type_)
         else:
             return self._injector.get_type_dependency(type_, default=default)
 
     @t.overload
-    def inject_dependencies(self, func: t.Callable[P, T]) -> t.Callable[P, T]:
-        ...
+    def inject_dependencies(self, func: t.Callable[P, T]) -> t.Callable[P, T]: ...
 
     @t.overload
-    def inject_dependencies(self) -> t.Callable[[t.Callable[P, T]], t.Callable[P, T]]:
-        ...
+    def inject_dependencies(self) -> t.Callable[[t.Callable[P, T]], t.Callable[P, T]]: ...
 
     def inject_dependencies(
         self, func: t.Callable[P, T] | None = None
     ) -> t.Callable[P, T] | t.Callable[[t.Callable[P, T]], t.Callable[P, T]]:
         """Decorator to inject dependencies into the decorated function.
 
         !!! note
```

### Comparing `hikari-arc-1.2.1/arc/abc/command.py` & `hikari_arc-1.3.0/arc/abc/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -357,15 +357,15 @@
         guild: hikari.SnowflakeishOr[hikari.PartialGuild] | hikari.UndefinedType = hikari.UNDEFINED,
     ) -> None:
         self._instances[hikari.Snowflake(guild) if guild else None] = instance
 
     async def _handle_exception(self, ctx: Context[ClientT], exc: Exception) -> None:
         try:
             if self.error_handler is not None:
-                await self.error_handler(ctx, exc)
+                await ctx._injection_ctx.call_with_async_di(self.error_handler, ctx, exc)
             else:
                 raise exc
         except Exception as exc:
             if self.plugin:
                 await self.plugin._handle_exception(ctx, exc)
             else:
                 await self.client._on_error(ctx, exc)
@@ -398,20 +398,20 @@
 
         if self._client:
             return self._client._concurrency_limiter
 
         return None
 
     def _resolve_hooks(self) -> list[HookT[ClientT]]:
-        plugin_hooks = self.plugin._resolve_hooks() if self.plugin else []
-        return self.client._hooks + plugin_hooks + self._hooks
+        upstream_hooks = self.plugin._resolve_hooks() if self.plugin else self.client._hooks
+        return upstream_hooks + self._hooks
 
     def _resolve_post_hooks(self) -> list[PostHookT[ClientT]]:
-        plugin_hooks = self.plugin._resolve_post_hooks() if self.plugin else []
-        return self.client._post_hooks + plugin_hooks + self._post_hooks
+        upstream_hooks = self.plugin._resolve_post_hooks() if self.plugin else self.client._post_hooks
+        return upstream_hooks + self._post_hooks
 
     async def publish(self, guild: hikari.SnowflakeishOr[hikari.PartialGuild] | None = None) -> hikari.PartialCommand:
         """Publish this command to the given guild, or globally if no guild is provided.
 
         Parameters
         ----------
         guild : hikari.Snowflakeish | None
@@ -545,18 +545,18 @@
         bool
             Whether the command should be aborted.
         """
         aborted = False
         try:
             hooks = command._resolve_hooks()
             for hook in hooks:
-                res = hook(ctx)
-
-                if inspect.isawaitable(res):
-                    res = await res
+                if inspect.iscoroutinefunction(hook):
+                    res = await ctx._injection_ctx.call_with_async_di(hook, ctx)
+                else:
+                    res = ctx._injection_ctx.call_with_di(hook, ctx)
 
                 res = t.cast(HookResult | None, res)
 
                 if res and res._abort:
                     aborted = True
         except Exception as e:
             aborted = True
@@ -566,44 +566,47 @@
 
     async def _handle_post_hooks(self, command: CallableCommandProto[ClientT], ctx: Context[ClientT]) -> None:
         """Handle all post-execution hooks for a command, and release the concurrency limiter if applicable."""
         try:
             post_hooks = command._resolve_post_hooks()
             for hook in post_hooks:
                 if inspect.iscoroutinefunction(hook):
-                    await hook(ctx)
+                    await ctx._injection_ctx.call_with_async_di(hook, ctx)
                 else:
-                    hook(ctx)
+                    ctx._injection_ctx.call_with_di(hook, ctx)
         except Exception as e:
             await command._handle_exception(ctx, e)
         finally:
             if (limiter := command._resolve_concurrency_limiter()) is not None:
                 limiter.release(ctx)
 
     async def _handle_callback(
         self, command: CallableCommandProto[ClientT], ctx: Context[ClientT], *args: t.Any, **kwargs: t.Any
     ) -> None:
         """Handle the callback of a command. Invoke all hooks and the callback, and handle any exceptions."""
         # If hook aborted, stop invocation
 
+        injection_ctx = await self.client._create_overriding_ctx_for_command(ctx)
+        ctx._injection_ctx = injection_ctx
+
         max_concurrency = command._resolve_concurrency_limiter()
 
         if max_concurrency is not None and max_concurrency.is_exhausted(ctx):
             return await command._handle_exception(
                 ctx, MaxConcurrencyReachedError(max_concurrency, max_concurrency.limit)
             )
 
         try:
             if max_concurrency is not None:
                 await max_concurrency.acquire(ctx)
 
             if await self._handle_pre_hooks(command, ctx):
                 return
 
-            await self.client.injector.call_with_async_di(command.callback, ctx, *args, **kwargs)
+            await injection_ctx.call_with_async_di(command.callback, ctx, *args, **kwargs)
 
         except Exception as e:
             ctx._has_command_failed = True
             await command._handle_exception(ctx, e)
         finally:
             # This also releases the concurrency limiter
             await self._handle_post_hooks(command, ctx)
```

### Comparing `hikari-arc-1.2.1/arc/abc/concurrency_limiting.py` & `hikari_arc-1.3.0/arc/abc/concurrency_limiting.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/abc/error_handler.py` & `hikari_arc-1.3.0/arc/abc/error_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,18 @@
     @abc.abstractmethod
     def error_handler(self, callback: ErrorHandlerCallbackT[ClientT] | None) -> None:
         """Set the error handler for this object."""
 
     @t.overload
     def set_error_handler(
         self, callback: None = ...
-    ) -> t.Callable[[ErrorHandlerCallbackT[ClientT]], ErrorHandlerCallbackT[ClientT]]:
-        ...
+    ) -> t.Callable[[ErrorHandlerCallbackT[ClientT]], ErrorHandlerCallbackT[ClientT]]: ...
 
     @t.overload
-    def set_error_handler(self, callback: ErrorHandlerCallbackT[ClientT]) -> ErrorHandlerCallbackT[ClientT]:
-        ...
+    def set_error_handler(self, callback: ErrorHandlerCallbackT[ClientT]) -> ErrorHandlerCallbackT[ClientT]: ...
 
     def set_error_handler(
         self, callback: ErrorHandlerCallbackT[ClientT] | None = None
     ) -> ErrorHandlerCallbackT[ClientT] | t.Callable[[ErrorHandlerCallbackT[ClientT]], ErrorHandlerCallbackT[ClientT]]:
         """Decorator to set an error handler for this object. This can be added to commands, groups, or plugins.
 
         This function will be called when an exception is raised during the invocation of a command.
```

### Comparing `hikari-arc-1.2.1/arc/abc/hookable.py` & `hikari_arc-1.3.0/arc/abc/hookable.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/abc/limiter.py` & `hikari_arc-1.3.0/arc/abc/limiter.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/abc/option.py` & `hikari_arc-1.3.0/arc/abc/option.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import abc
 import enum
 import typing as t
-from typing import Any
 
 import attr
 import hikari
 
 from arc.internal.types import AutocompleteCallbackT, ChoiceT, ClientT, ParamsT
 from arc.locale import OptionLocaleRequest
 
@@ -20,18 +19,20 @@
 __all__ = (
     "Option",
     "OptionParams",
     "OptionWithChoices",
     "OptionWithChoicesParams",
     "OptionBase",
     "CommandOptionBase",
+    "ConverterOption",
     "OptionType",
 )
 
 T = t.TypeVar("T")
+OriginT = t.TypeVar("OriginT")
 
 Option = t.Annotated
 """Alias for typing.Annotated.
 
 Examples
 --------
 ```py
@@ -45,16 +46,17 @@
 ```
 """
 
 
 class OptionType(enum.IntEnum):
     """The type of a command option.
 
-    This is practically identical to `hikari.OptionType` at the moment.
-    It may however be used in the future to define custom option types.
+    This includes all hikari option types along with some custom ones.
+
+    Custom arc-specific options start with 10k.
     """
 
     SUB_COMMAND = 1
     """Denotes a command option where the value will be a sub command."""
 
     SUB_COMMAND_GROUP = 2
     """Denotes a command option where the value will be a sub command group."""
@@ -88,25 +90,36 @@
 
     This is range limited between -2^53 and 2^53.
     """
 
     ATTACHMENT = 11
     """Denotes a command option where the value will be an attachment."""
 
+    # Custom optiontypes are 10k+
+
+    MEMBER = 10001
+    """Denotes a command option where the value will be resolved to a member."""
+
+    COLOR = 10002
+    """Denotes a command option where the value will be a color."""
+
     @classmethod
     def from_hikari(cls, option_type: hikari.OptionType) -> OptionType:
         """Convert a hikari.OptionType to an OptionType."""
         return cls(option_type.value)
 
     def to_hikari(self) -> hikari.OptionType:
         """Convert an OptionType to a hikari.OptionType."""
-        # TODO: Map custom option types to their respective hikari.OptionType
-        return hikari.OptionType(self.value)
+        if self.value < 10000:
+            return hikari.OptionType(self.value)
 
-    # TODO: When adding custom convertible option types, add them with an offset of 1000 or so
+        if self is OptionType.MEMBER:
+            return hikari.OptionType.USER
+        else:
+            return hikari.OptionType.STRING
 
 
 class OptionParams(t.Generic[T]):
     """The base class for all option parameters objects.
 
     Parameters
     ----------
@@ -269,36 +282,52 @@
 @attr.define(slots=True, kw_only=True)
 class CommandOptionBase(OptionBase[T], t.Generic[T, ClientT, ParamsT]):
     """An abstract base class for all slash command options. This does not include subcommands."""
 
     is_required: bool = True
     """Whether the option is required."""
 
+    arg_name: str
+    """The name of the parameter this option represents.
+    This is going to be the same as `name` unless `name` was overriden.
+    """
+
     @classmethod
     @abc.abstractmethod
-    def _from_params(cls, *, name: str, is_required: bool, params: ParamsT, **kwargs: t.Any) -> te.Self:
+    def _from_params(cls, *, name: str, arg_name: str, is_required: bool, params: ParamsT, **kwargs: t.Any) -> te.Self:
         """Construct a new Option instance from the given parameters object.
 
         Parameters
         ----------
         name : str
             The name of the option
+        arg_name : str
+            The name of the parameter this option represents
         is_required : bool
             Whether the option is required
         params : ParamsT
             The parameters for the option
         kwargs : dict[str, Any]
             Any additional keyword arguments to pass to the constructor
         """
 
-    def _to_dict(self) -> dict[str, Any]:
+    def _to_dict(self) -> dict[str, t.Any]:
         return {**super()._to_dict(), "is_required": self.is_required}
 
 
 @attr.define(slots=True, kw_only=True)
+class ConverterOption(CommandOptionBase[T, ClientT, ParamsT], t.Generic[T, ClientT, ParamsT, OriginT]):
+    """An option with a built-in converter."""
+
+    @abc.abstractmethod
+    def _convert_value(self, value: OriginT) -> T:
+        """Convert the value to the desired type."""
+
+
+@attr.define(slots=True, kw_only=True)
 class OptionWithChoices(CommandOptionBase[ChoiceT, ClientT, ParamsT]):
     """An option that can have choices or be autocompleted."""
 
     choices: t.Sequence[ChoiceT | hikari.CommandChoice] | t.Mapping[str, ChoiceT] | None = None
     """The choices for the option."""
 
     autocomplete_with: AutocompleteCallbackT[ClientT, ChoiceT] | None = None
```

### Comparing `hikari-arc-1.2.1/arc/abc/plugin.py` & `hikari_arc-1.3.0/arc/abc/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     def default_enabled_guilds(self) -> t.Sequence[hikari.Snowflake] | hikari.UndefinedType:
         """The default guilds to enable commands in."""
         return self._default_enabled_guilds
 
     async def _handle_exception(self, ctx: Context[ClientT], exc: Exception) -> None:
         try:
             if self.error_handler is not None:
-                await self.error_handler(ctx, exc)
+                await ctx._injection_ctx.call_with_async_di(self.error_handler, ctx, exc)
             else:
                 raise exc
         except Exception as exc:
             await self.client._on_error(ctx, exc)
 
     def _resolve_settings(self) -> _CommandSettings:
         settings = self._client._cmd_settings if self._client is not None else _CommandSettings.default()
@@ -205,20 +205,20 @@
             self._user_commands[command.name] = command
         elif isinstance(command, MessageCommand):
             self._message_commands[command.name] = command
         else:
             raise TypeError(f"Unknown command type '{type(command).__name__}'.")
 
     @t.overload
-    def include(self) -> t.Callable[[CallableCommandBase[ClientT, BuilderT]], CallableCommandBase[ClientT, BuilderT]]:
-        ...
+    def include(
+        self,
+    ) -> t.Callable[[CallableCommandBase[ClientT, BuilderT]], CallableCommandBase[ClientT, BuilderT]]: ...
 
     @t.overload
-    def include(self, command: CallableCommandBase[ClientT, BuilderT]) -> CallableCommandBase[ClientT, BuilderT]:
-        ...
+    def include(self, command: CallableCommandBase[ClientT, BuilderT]) -> CallableCommandBase[ClientT, BuilderT]: ...
 
     def include(
         self, command: CallableCommandBase[ClientT, BuilderT] | None = None
     ) -> (
         CallableCommandBase[ClientT, BuilderT]
         | t.Callable[[CallableCommandBase[ClientT, BuilderT]], CallableCommandBase[ClientT, BuilderT]]
     ):
@@ -319,20 +319,18 @@
             description_localizations=description_localizations or {},
             is_nsfw=is_nsfw,
         )
         group._plugin_include_hook(self)
         return group
 
     @t.overload
-    def inject_dependencies(self, func: t.Callable[P, T]) -> t.Callable[P, T]:
-        ...
+    def inject_dependencies(self, func: t.Callable[P, T]) -> t.Callable[P, T]: ...
 
     @t.overload
-    def inject_dependencies(self) -> t.Callable[[t.Callable[P, T]], t.Callable[P, T]]:
-        ...
+    def inject_dependencies(self) -> t.Callable[[t.Callable[P, T]], t.Callable[P, T]]: ...
 
     def inject_dependencies(
         self, func: t.Callable[P, T] | None = None
     ) -> t.Callable[P, T] | t.Callable[[t.Callable[P, T]], t.Callable[P, T]]:
         """First order decorator to inject dependencies into the decorated function.
 
         !!! warning
@@ -400,34 +398,32 @@
             return decorator(func)
 
         return decorator
 
     @t.overload
     def walk_commands(
         self, command_type: t.Literal[hikari.CommandType.USER], *, callable_only: bool = False
-    ) -> t.Iterator[UserCommand[ClientT]]:
-        ...
+    ) -> t.Iterator[UserCommand[ClientT]]: ...
 
     @t.overload
     def walk_commands(
         self, command_type: t.Literal[hikari.CommandType.MESSAGE], *, callable_only: bool = False
-    ) -> t.Iterator[MessageCommand[ClientT]]:
-        ...
+    ) -> t.Iterator[MessageCommand[ClientT]]: ...
 
     @t.overload
     def walk_commands(
         self, command_type: t.Literal[hikari.CommandType.SLASH], *, callable_only: t.Literal[False]
-    ) -> t.Iterator[SlashCommand[ClientT] | SlashSubCommand[ClientT] | SlashGroup[ClientT] | SlashSubGroup[ClientT]]:
-        ...
+    ) -> t.Iterator[
+        SlashCommand[ClientT] | SlashSubCommand[ClientT] | SlashGroup[ClientT] | SlashSubGroup[ClientT]
+    ]: ...
 
     @t.overload
     def walk_commands(
         self, command_type: t.Literal[hikari.CommandType.SLASH], *, callable_only: t.Literal[True]
-    ) -> t.Iterator[SlashCommand[ClientT] | SlashSubCommand[ClientT]]:
-        ...
+    ) -> t.Iterator[SlashCommand[ClientT] | SlashSubCommand[ClientT]]: ...
 
     def walk_commands(  # noqa: C901
         self, command_type: hikari.CommandType, *, callable_only: bool = False
     ) -> t.Iterator[t.Any]:
         """Iterate over all commands of a certain type added to this plugin.
 
         Parameters
```

### Comparing `hikari-arc-1.2.1/arc/client.py` & `hikari_arc-1.3.0/arc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 from arc.plugin import GatewayPluginBase, RESTPluginBase
 
 if t.TYPE_CHECKING:
     import alluka
     import typing_extensions as te
 
     from arc import AutodeferMode
-
-    from .internal.types import EventCallbackT, EventT, ResponseBuilderT
+    from arc.internal.types import EventCallbackT, EventT, ResponseBuilderT
 
 __all__ = (
     "GatewayClientBase",
     "RESTClientBase",
     "GatewayClient",
     "RESTClient",
     "GatewayContext",
```

### Comparing `hikari-arc-1.2.1/arc/command/__init__.py` & `hikari_arc-1.3.0/arc/command/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,24 @@
 from .option import (
     AttachmentOption,
     AttachmentParams,
     BoolOption,
     BoolParams,
     ChannelOption,
     ChannelParams,
+    ColorOption,
+    ColorParams,
+    ColourOption,
+    ColourParams,
     FloatOption,
     FloatParams,
     IntOption,
     IntParams,
+    MemberOption,
+    MemberParams,
     MentionableOption,
     MentionableParams,
     RoleOption,
     RoleParams,
     StrOption,
     StrParams,
     UserOption,
@@ -52,14 +58,20 @@
     "ChannelParams",
     "RoleOption",
     "RoleParams",
     "MentionableOption",
     "MentionableParams",
     "AttachmentOption",
     "AttachmentParams",
+    "MemberOption",
+    "MemberParams",
+    "ColorOption",
+    "ColorParams",
+    "ColourOption",
+    "ColourParams",
     "UserCommand",
     "user_command",
     "MessageCommand",
     "message_command",
 )
 
 # MIT License
```

### Comparing `hikari-arc-1.2.1/arc/command/message.py` & `hikari_arc-1.3.0/arc/command/message.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/command/option/__init__.py` & `hikari_arc-1.3.0/arc/command/option/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .attachment import AttachmentOption, AttachmentParams
 from .bool import BoolOption, BoolParams
 from .channel import ChannelOption, ChannelParams
+from .custom import ColorOption, ColorParams, ColourOption, ColourParams, MemberOption, MemberParams
 from .float import FloatOption, FloatParams
 from .int import IntOption, IntParams
 from .mentionable import MentionableOption, MentionableParams
 from .role import RoleOption, RoleParams
 from .str import StrOption, StrParams
 from .user import UserOption, UserParams
 
@@ -23,14 +24,20 @@
     "ChannelParams",
     "RoleOption",
     "RoleParams",
     "MentionableOption",
     "MentionableParams",
     "AttachmentOption",
     "AttachmentParams",
+    "MemberOption",
+    "MemberParams",
+    "ColorOption",
+    "ColorParams",
+    "ColourOption",
+    "ColourParams",
 )
 
 # MIT License
 #
 # Copyright (c) 2023-present hypergonial
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hikari-arc-1.2.1/arc/command/option/attachment.py` & `hikari_arc-1.3.0/arc/command/option/attachment.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,17 +48,20 @@
     """
 
     @property
     def option_type(self) -> OptionType:
         return OptionType.ATTACHMENT
 
     @classmethod
-    def _from_params(cls, *, name: str, is_required: bool, params: AttachmentParams, **kwargs: t.Any) -> te.Self:
+    def _from_params(
+        cls, *, name: str, arg_name: str, is_required: bool, params: AttachmentParams, **kwargs: t.Any
+    ) -> te.Self:
         return cls(
             name=name,
+            arg_name=arg_name,
             description=params.description,
             is_required=is_required,
             name_localizations=params.name_localizations,
             description_localizations=params.description_localizations,
             **kwargs,
         )
```

### Comparing `hikari-arc-1.2.1/arc/command/option/bool.py` & `hikari_arc-1.3.0/arc/command/option/bool.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,17 +47,20 @@
     """
 
     @property
     def option_type(self) -> OptionType:
         return OptionType.BOOLEAN
 
     @classmethod
-    def _from_params(cls, *, name: str, is_required: bool, params: BoolParams, **kwargs: t.Any) -> te.Self:
+    def _from_params(
+        cls, *, name: str, arg_name: str, is_required: bool, params: BoolParams, **kwargs: t.Any
+    ) -> te.Self:
         return cls(
             name=name,
+            arg_name=arg_name,
             description=params.description,
             is_required=is_required,
             name_localizations=params.name_localizations,
             description_localizations=params.description_localizations,
             **kwargs,
         )
```

### Comparing `hikari-arc-1.2.1/arc/command/option/channel.py` & `hikari_arc-1.3.0/arc/command/option/channel.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,18 +59,21 @@
     """The channel types that the option can be."""
 
     @property
     def option_type(self) -> OptionType:
         return OptionType.CHANNEL
 
     @classmethod
-    def _from_params(cls, *, name: str, is_required: bool, params: ChannelParams, **kwargs: t.Any) -> te.Self:
+    def _from_params(
+        cls, *, name: str, arg_name: str, is_required: bool, params: ChannelParams, **kwargs: t.Any
+    ) -> te.Self:
         channel_types = kwargs.pop("channel_types")
         return cls(
             name=name,
+            arg_name=arg_name,
             description=params.description,
             is_required=is_required,
             name_localizations=params.name_localizations,
             description_localizations=params.description_localizations,
             channel_types=channel_types,
             **kwargs,
         )
```

### Comparing `hikari-arc-1.2.1/arc/command/option/float.py` & `hikari_arc-1.3.0/arc/command/option/float.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,20 @@
     """The maximum value of the option."""
 
     @property
     def option_type(self) -> OptionType:
         return OptionType.FLOAT
 
     @classmethod
-    def _from_params(cls, *, name: str, is_required: bool, params: FloatParams[ClientT], **kwargs: t.Any) -> te.Self:
+    def _from_params(
+        cls, *, name: str, arg_name: str, is_required: bool, params: FloatParams[ClientT], **kwargs: t.Any
+    ) -> te.Self:
         return cls(
             name=name,
+            arg_name=arg_name,
             description=params.description,
             is_required=is_required,
             min=params.min,
             max=params.max,
             choices=params.choices,
             autocomplete_with=params.autocomplete_with,
             name_localizations=params.name_localizations,
```

### Comparing `hikari-arc-1.2.1/arc/command/option/int.py` & `hikari_arc-1.3.0/arc/command/option/int.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,20 @@
     """The maximum value of the option."""
 
     @property
     def option_type(self) -> OptionType:
         return OptionType.INTEGER
 
     @classmethod
-    def _from_params(cls, *, name: str, is_required: bool, params: IntParams[ClientT], **kwargs: t.Any) -> te.Self:
+    def _from_params(
+        cls, *, name: str, arg_name: str, is_required: bool, params: IntParams[ClientT], **kwargs: t.Any
+    ) -> te.Self:
         return cls(
             name=name,
+            arg_name=arg_name,
             description=params.description,
             is_required=is_required,
             min=params.min,
             max=params.max,
             choices=params.choices,
             autocomplete_with=params.autocomplete_with,
             name_localizations=params.name_localizations,
```

### Comparing `hikari-arc-1.2.1/arc/command/option/mentionable.py` & `hikari_arc-1.3.0/arc/command/option/mentionable.py`

 * *Files 11% similar despite different names*

```diff
@@ -49,17 +49,20 @@
     """
 
     @property
     def option_type(self) -> OptionType:
         return OptionType.MENTIONABLE
 
     @classmethod
-    def _from_params(cls, *, name: str, is_required: bool, params: MentionableParams, **kwargs: t.Any) -> te.Self:
+    def _from_params(
+        cls, *, name: str, arg_name: str, is_required: bool, params: MentionableParams, **kwargs: t.Any
+    ) -> te.Self:
         return cls(
             name=name,
+            arg_name=arg_name,
             description=params.description,
             is_required=is_required,
             name_localizations=params.name_localizations,
             description_localizations=params.description_localizations,
             **kwargs,
         )
```

### Comparing `hikari-arc-1.2.1/arc/command/option/role.py` & `hikari_arc-1.3.0/arc/command/option/role.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,17 +48,20 @@
     """
 
     @property
     def option_type(self) -> OptionType:
         return OptionType.ROLE
 
     @classmethod
-    def _from_params(cls, *, name: str, is_required: bool, params: RoleParams, **kwargs: t.Any) -> te.Self:
+    def _from_params(
+        cls, *, name: str, arg_name: str, is_required: bool, params: RoleParams, **kwargs: t.Any
+    ) -> te.Self:
         return cls(
             name=name,
+            arg_name=arg_name,
             description=params.description,
             is_required=is_required,
             name_localizations=params.name_localizations,
             description_localizations=params.description_localizations,
             **kwargs,
         )
```

### Comparing `hikari-arc-1.2.1/arc/command/option/str.py` & `hikari_arc-1.3.0/arc/command/option/str.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,20 @@
     """The maximum length of the option."""
 
     @property
     def option_type(self) -> OptionType:
         return OptionType.STRING
 
     @classmethod
-    def _from_params(cls, *, name: str, is_required: bool, params: StrParams[ClientT], **kwargs: t.Any) -> te.Self:
+    def _from_params(
+        cls, *, name: str, arg_name: str, is_required: bool, params: StrParams[ClientT], **kwargs: t.Any
+    ) -> te.Self:
         return cls(
             name=name,
+            arg_name=arg_name,
             description=params.description,
             is_required=is_required,
             min_length=params.min_length,
             max_length=params.max_length,
             choices=params.choices,
             autocomplete_with=params.autocomplete_with,
             name_localizations=params.name_localizations,
```

### Comparing `hikari-arc-1.2.1/arc/command/option/user.py` & `hikari_arc-1.3.0/arc/command/option/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,20 @@
     """
 
     @property
     def option_type(self) -> OptionType:
         return OptionType.USER
 
     @classmethod
-    def _from_params(cls, *, name: str, is_required: bool, params: UserParams, **kwargs: t.Any) -> te.Self:
+    def _from_params(
+        cls, *, name: str, arg_name: str, is_required: bool, params: UserParams, **kwargs: t.Any
+    ) -> te.Self:
         return cls(
             name=name,
+            arg_name=arg_name,
             description=params.description,
             is_required=is_required,
             name_localizations=params.name_localizations,
             description_localizations=params.description_localizations,
             **kwargs,
         )
```

### Comparing `hikari-arc-1.2.1/arc/command/slash.py` & `hikari_arc-1.3.0/arc/command/slash.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,20 @@
     "SlashSubGroup",
     "slash_command",
     "slash_subcommand",
 )
 
 
 def _choices_to_builders(
-    choices: t.Sequence[hikari.api.AutocompleteChoiceBuilder] | t.Sequence[t.Any],
+    choices: t.Sequence[hikari.api.AutocompleteChoiceBuilder] | t.Sequence[t.Any] | t.Mapping[str, t.Any],
 ) -> t.Sequence[hikari.api.AutocompleteChoiceBuilder]:
     """Convert a sequence of choices to a sequence of choice builders."""
+    if isinstance(choices, t.Mapping):
+        return [hikari.impl.AutocompleteChoiceBuilder(str(k), v) for k, v in choices.items()]
+
     return [
         (
             hikari.impl.AutocompleteChoiceBuilder(str(e), e)
             if not isinstance(e, hikari.api.AutocompleteChoiceBuilder)
             else e
         )
         for e in choices
@@ -399,20 +402,18 @@
         self.name_localizations: t.Mapping[hikari.Locale, str] = name_locales
         self.description_localizations: t.Mapping[hikari.Locale, str] = desc_locales
 
         for sub in self.children.values():
             sub._request_option_locale(self._client, self)
 
     @t.overload
-    def include(self) -> t.Callable[[SlashSubCommand[ClientT]], SlashSubCommand[ClientT]]:
-        ...
+    def include(self) -> t.Callable[[SlashSubCommand[ClientT]], SlashSubCommand[ClientT]]: ...
 
     @t.overload
-    def include(self, command: SlashSubCommand[ClientT]) -> SlashSubCommand[ClientT]:
-        ...
+    def include(self, command: SlashSubCommand[ClientT]) -> SlashSubCommand[ClientT]: ...
 
     def include(
         self, command: SlashSubCommand[ClientT] | None = None
     ) -> SlashSubCommand[ClientT] | t.Callable[[SlashSubCommand[ClientT]], SlashSubCommand[ClientT]]:
         """Decorator to add a subcommand to this group."""
 
         def decorator(command: SlashSubCommand[ClientT]) -> SlashSubCommand[ClientT]:
@@ -536,34 +537,32 @@
     def _resolve_concurrency_limiter(self) -> ConcurrencyLimiterProto[ClientT] | None:
         assert self._parent is not None
         return self._parent._resolve_concurrency_limiter()
 
     async def _handle_exception(self, ctx: Context[ClientT], exc: Exception) -> None:
         try:
             if self.error_handler:
-                await self.error_handler(ctx, exc)
+                await ctx._injection_ctx.call_with_async_di(self.error_handler, ctx, exc)
             else:
                 raise exc
-        except Exception as e:
+        except Exception as exc:
             assert self._parent is not None
-            await self._parent._handle_exception(ctx, e)
+            await ctx._injection_ctx.call_with_async_di(self._parent._handle_exception, ctx, exc)
 
     def _request_option_locale(self, client: Client[t.Any], command: CommandProto) -> None:
         super()._request_option_locale(client, command)
 
         for subcommand in self.children.values():
             subcommand._request_option_locale(client, command)
 
     @t.overload
-    def include(self) -> t.Callable[[SlashSubCommand[ClientT]], SlashSubCommand[ClientT]]:
-        ...
+    def include(self) -> t.Callable[[SlashSubCommand[ClientT]], SlashSubCommand[ClientT]]: ...
 
     @t.overload
-    def include(self, command: SlashSubCommand[ClientT]) -> SlashSubCommand[ClientT]:
-        ...
+    def include(self, command: SlashSubCommand[ClientT]) -> SlashSubCommand[ClientT]: ...
 
     def include(
         self, command: SlashSubCommand[ClientT] | None = None
     ) -> SlashSubCommand[ClientT] | t.Callable[[SlashSubCommand[ClientT]], SlashSubCommand[ClientT]]:
         """First-order decorator to add a subcommand to this group."""
 
         def decorator(command: SlashSubCommand[ClientT]) -> SlashSubCommand[ClientT]:
@@ -696,15 +695,15 @@
         try:
             if self.error_handler:
                 await self.error_handler(ctx, exc)
             else:
                 raise exc
         except Exception as e:
             assert self._parent is not None
-            await self._parent._handle_exception(ctx, e)
+            await self._handle_exception(ctx, e)
 
     def _request_option_locale(self, client: Client[t.Any], command: CommandProto) -> None:
         super()._request_option_locale(client, command)
 
         for option in self.options.values():
             option._request_option_locale(client, command)
```

### Comparing `hikari-arc-1.2.1/arc/command/user.py` & `hikari_arc-1.3.0/arc/command/user.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/context/__init__.py` & `hikari_arc-1.3.0/arc/context/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/context/autocomplete.py` & `hikari_arc-1.3.0/arc/context/autocomplete.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/context/base.py` & `hikari_arc-1.3.0/arc/context/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 import datetime
 import enum
 import logging
 import typing as t
 from contextlib import suppress
 
+import alluka
 import attr
 import hikari
 
 from arc.abc.option import OptionType  # noqa: TCH001 Needed for tests
 from arc.errors import NoResponseIssuedError, ResponseAlreadyIssuedError
 from arc.internal.options import OPTIONTYPE_TO_TYPE, resolve_snowflake_value
 from arc.internal.types import ClientT, ResponseBuilderT
@@ -19,14 +20,17 @@
 if t.TYPE_CHECKING:
     from arc.abc.command import CallableCommandProto
 
 __all__ = ("Context", "InteractionResponse", "AutodeferMode")
 
 logger = logging.getLogger(__name__)
 
+T = t.TypeVar("T")
+DefaultT = t.TypeVar("DefaultT")
+
 
 @t.final
 class AutodeferMode(enum.IntEnum):
     """An enum representing autodefer configuration."""
 
     OFF = 0
     """Do not autodefer."""
@@ -250,21 +254,23 @@
         "_resp_builder",
         "_issued_response",
         "_response_lock",
         "_autodefer_task",
         "_created_at",
         "_has_command_failed",
         "_options",
+        "_injection_ctx",
     )
 
     def __init__(
         self, client: ClientT, command: CallableCommandProto[ClientT], interaction: hikari.CommandInteraction
     ) -> None:
         self._client = client
         self._command = command
+        self._injection_ctx = alluka.OverridingContext.from_client(client.injector)
         self._interaction: hikari.CommandInteraction = interaction
         self._options: t.Sequence[hikari.CommandInteractionOption] | None = None
         self._responses: t.MutableSequence[InteractionResponse] = []
         self._resp_builder: asyncio.Future[ResponseBuilderT] = asyncio.Future()
         self._issued_response: bool = False
         self._response_lock: asyncio.Lock = asyncio.Lock()
         self._created_at = datetime.datetime.now()
@@ -409,48 +415,47 @@
         return self._interaction.get_guild()
 
     def get_channel(self) -> hikari.TextableGuildChannel | None:
         """Gets the channel this context represents, None if in a DM. Requires application cache."""
         return self._interaction.get_channel()
 
     @t.overload
-    def get_option(self, name: str, opt_type: t.Literal[OptionType.ATTACHMENT]) -> hikari.Attachment | None:
-        ...
+    def get_option(self, name: str, opt_type: t.Literal[OptionType.COLOR]) -> hikari.Color | None: ...
+
+    @t.overload
+    def get_option(self, name: str, opt_type: t.Literal[OptionType.MEMBER]) -> hikari.Member | None: ...
 
     @t.overload
-    def get_option(self, name: str, opt_type: t.Literal[OptionType.MENTIONABLE]) -> hikari.User | hikari.Role | None:
-        ...
+    def get_option(self, name: str, opt_type: t.Literal[OptionType.ATTACHMENT]) -> hikari.Attachment | None: ...
 
     @t.overload
-    def get_option(self, name: str, opt_type: t.Literal[OptionType.USER]) -> hikari.User | None:
-        ...
+    def get_option(
+        self, name: str, opt_type: t.Literal[OptionType.MENTIONABLE]
+    ) -> hikari.User | hikari.Role | None: ...
 
     @t.overload
-    def get_option(self, name: str, opt_type: t.Literal[OptionType.ROLE]) -> hikari.Role | None:
-        ...
+    def get_option(self, name: str, opt_type: t.Literal[OptionType.USER]) -> hikari.User | None: ...
 
     @t.overload
-    def get_option(self, name: str, opt_type: t.Literal[OptionType.CHANNEL]) -> hikari.PartialChannel | None:
-        ...
+    def get_option(self, name: str, opt_type: t.Literal[OptionType.ROLE]) -> hikari.Role | None: ...
 
     @t.overload
-    def get_option(self, name: str, opt_type: t.Literal[OptionType.STRING]) -> str | None:
-        ...
+    def get_option(self, name: str, opt_type: t.Literal[OptionType.CHANNEL]) -> hikari.PartialChannel | None: ...
 
     @t.overload
-    def get_option(self, name: str, opt_type: t.Literal[OptionType.BOOLEAN]) -> bool | None:
-        ...
+    def get_option(self, name: str, opt_type: t.Literal[OptionType.STRING]) -> str | None: ...
 
     @t.overload
-    def get_option(self, name: str, opt_type: t.Literal[OptionType.FLOAT]) -> float | None:
-        ...
+    def get_option(self, name: str, opt_type: t.Literal[OptionType.BOOLEAN]) -> bool | None: ...
 
     @t.overload
-    def get_option(self, name: str, opt_type: t.Literal[OptionType.INTEGER]) -> int | None:
-        ...
+    def get_option(self, name: str, opt_type: t.Literal[OptionType.FLOAT]) -> float | None: ...
+
+    @t.overload
+    def get_option(self, name: str, opt_type: t.Literal[OptionType.INTEGER]) -> int | None: ...
 
     def get_option(self, name: str, opt_type: OptionType) -> t.Any | None:
         """Get the value of an option by name.
 
         Parameters
         ----------
         name : str
@@ -526,14 +531,48 @@
 
         if locale not in self._client._provided_locales:
             locale = hikari.Locale.EN_US
 
         request = CustomLocaleRequest(self.command, locale, self, key)
         return self._client._custom_locale_provider(request).format(**kwargs)
 
+    @t.overload
+    def get_type_dependency(self, type_: type[T]) -> T: ...
+
+    @t.overload
+    def get_type_dependency(self, type_: type[T], *, default: DefaultT) -> T | DefaultT: ...
+
+    def get_type_dependency(
+        self, type_: type[T], *, default: DefaultT | hikari.UndefinedType = hikari.UNDEFINED
+    ) -> T | DefaultT:
+        """Get a type dependency for the current context.
+
+        Parameters
+        ----------
+        type_ : type[T]
+            The type of the dependency.
+        default : DefaultT
+            The default value to return if the dependency does not exist.
+            If not provided, this will raise an exception if the dependency does not exist.
+
+        Returns
+        -------
+        T | DefaultT
+            The instance of the dependency, if it exists, otherwise `default`.
+
+        Raises
+        ------
+        KeyError
+            If the dependency does not exist and `default` was not provided.
+        """
+        if default is hikari.UNDEFINED:
+            return self._injection_ctx.get_type_dependency(type_)
+        else:
+            return self._injection_ctx.get_type_dependency(type_, default=default)
+
     async def get_last_response(self) -> InteractionResponse:
         """Get the last response issued to the interaction this context is proxying.
 
         Returns
         -------
         InteractionResponse
             The response object.
@@ -648,22 +687,20 @@
                 self._issued_response = True
                 response = await self._create_response()
             if delete_after:
                 response.delete_after(delete_after)
             return response
 
     @t.overload
-    async def respond_with_builder(self, builder: hikari.api.InteractionModalBuilder) -> None:
-        ...
+    async def respond_with_builder(self, builder: hikari.api.InteractionModalBuilder) -> None: ...
 
     @t.overload
     async def respond_with_builder(
         self, builder: hikari.api.InteractionMessageBuilder | hikari.api.InteractionDeferredBuilder
-    ) -> InteractionResponse:
-        ...
+    ) -> InteractionResponse: ...
 
     async def respond_with_builder(self, builder: ResponseBuilderT) -> InteractionResponse | None:
         """Respond to the interaction with a builder. This method will try to turn the builder into a valid
         response or followup, depending on the builder type and interaction state.
 
         Parameters
         ----------
```

### Comparing `hikari-arc-1.2.1/arc/errors.py` & `hikari_arc-1.3.0/arc/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing as t
 
 if t.TYPE_CHECKING:
     import hikari
 
     from arc.abc.concurrency_limiting import ConcurrencyLimiterProto
     from arc.abc.limiter import LimiterProto
+    from arc.abc.option import ConverterOption
 
 
 class ArcError(Exception):
     """Base exception for all Arc errors."""
 
 
 class AutocompleteError(ArcError):
@@ -158,14 +159,31 @@
     """
 
     def __init__(self, guild_id: hikari.Snowflake, *args: t.Any) -> None:
         self.guild_id = guild_id
         super().__init__(*args)
 
 
+class OptionConverterFailureError(ArcError):
+    """Raised when an option converter fails to convert a value.
+
+    Attributes
+    ----------
+    option : arc.abc.option.ConverterOption
+        The option that failed to convert the value.
+    value : t.Any
+        The value that failed to be converted.
+    """
+
+    def __init__(self, option: ConverterOption[t.Any, t.Any, t.Any, t.Any], value: t.Any, *args: t.Any) -> None:
+        self.option = option
+        self.value = value
+        super().__init__(*args)
+
+
 # MIT License
 #
 # Copyright (c) 2023-present hypergonial
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
```

### Comparing `hikari-arc-1.2.1/arc/events.py` & `hikari_arc-1.3.0/arc/events.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/extension.py` & `hikari_arc-1.3.0/arc/extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,19 @@
 import typing as t
 
 if t.TYPE_CHECKING:
     from arc.internal.types import ClientT
 
 
 @t.overload
-def loader() -> t.Callable[[t.Callable[[ClientT], None]], t.Callable[[ClientT], None]]:
-    ...
+def loader() -> t.Callable[[t.Callable[[ClientT], None]], t.Callable[[ClientT], None]]: ...
 
 
 @t.overload
-def loader(callback: t.Callable[[ClientT], None]) -> t.Callable[[ClientT], None]:
-    ...
+def loader(callback: t.Callable[[ClientT], None]) -> t.Callable[[ClientT], None]: ...
 
 
 def loader(
     callback: t.Callable[[ClientT], None] | None = None,
 ) -> t.Callable[[ClientT], None] | t.Callable[[t.Callable[[ClientT], None]], t.Callable[[ClientT], None]]:
     """Decorator to set the load callback for this module.
 
@@ -47,21 +45,19 @@
     if callback is not None:
         return decorator(callback)
 
     return decorator
 
 
 @t.overload
-def unloader() -> t.Callable[[t.Callable[[ClientT], None]], t.Callable[[ClientT], None]]:
-    ...
+def unloader() -> t.Callable[[t.Callable[[ClientT], None]], t.Callable[[ClientT], None]]: ...
 
 
 @t.overload
-def unloader(callback: t.Callable[[ClientT], None]) -> t.Callable[[ClientT], None]:
-    ...
+def unloader(callback: t.Callable[[ClientT], None]) -> t.Callable[[ClientT], None]: ...
 
 
 def unloader(
     callback: t.Callable[[ClientT], None] | None = None,
 ) -> t.Callable[[ClientT], None] | t.Callable[[t.Callable[[ClientT], None]], t.Callable[[ClientT], None]]:
     """Decorator to set the unload callback for this module.
```

### Comparing `hikari-arc-1.2.1/arc/internal/__init__.py` & `hikari_arc-1.3.0/arc/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/internal/about.py` & `hikari_arc-1.3.0/arc/internal/about.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
 __author__: t.Final[str] = "hypergonial"
 __author_email__: t.Final[str] = "git@hypergonial.com"
 __maintainer__: t.Final[str] = "hypergonial"
 __license__: t.Final[str] = "MIT"
 __url__: t.Final[str] = "https://github.com/hypergonial/hikari-arc"
-__version__: t.Final[str] = "1.2.1"
+__version__: t.Final[str] = "1.3.0"
 
 # MIT License
 #
 # Copyright (c) 2023-present hypergonial
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
```

### Comparing `hikari-arc-1.2.1/arc/internal/deprecation.py` & `hikari_arc-1.3.0/arc/internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/internal/options.py` & `hikari_arc-1.3.0/arc/internal/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import typing as t
 
 import hikari
 
-from arc.abc.option import OptionType
+from arc.abc.option import ConverterOption, OptionType
 
 if t.TYPE_CHECKING:
     from arc.abc.option import CommandOptionBase
     from arc.internal.types import ClientT
 
 
 OPTIONTYPE_TO_TYPE: dict[OptionType, type[t.Any]] = {
@@ -17,14 +17,16 @@
     OptionType.BOOLEAN: bool,
     OptionType.USER: hikari.PartialUser,
     OptionType.CHANNEL: hikari.PartialChannel,
     OptionType.ROLE: hikari.Role,
     OptionType.MENTIONABLE: hikari.Unique,
     OptionType.FLOAT: float,
     OptionType.ATTACHMENT: hikari.Attachment,
+    OptionType.COLOR: hikari.Color,
+    OptionType.MEMBER: hikari.Member,
 }
 """Used for runtime type checking in Context.get_option, not much else at the moment."""
 
 
 def resolve_snowflake_value(
     value: hikari.Snowflake, opt_type: hikari.OptionType | int, resolved: hikari.ResolvedOptionData
 ) -> t.Any:
@@ -85,22 +87,25 @@
     Returns
     -------
     dict[str, Any]
         The resolved options as kwargs, ready to be passed to the callback.
     """
     option_kwargs: dict[str, t.Any] = {}
 
-    for arg_name, opt in local_options.items():
+    for opt in local_options.values():
         inter_opt = next((o for o in incoming_options if o.name == opt.name), None)
 
         if inter_opt is None:
             continue
 
         if isinstance(inter_opt.value, hikari.Snowflake) and resolved:
-            option_kwargs[arg_name] = resolve_snowflake_value(inter_opt.value, inter_opt.type, resolved)
+            option_kwargs[opt.arg_name] = resolve_snowflake_value(inter_opt.value, inter_opt.type, resolved)
 
         elif isinstance(inter_opt.value, hikari.Snowflake):
             raise ValueError(f"Missing resolved option data for '{inter_opt.name}'.")
         else:
-            option_kwargs[arg_name] = inter_opt.value
+            option_kwargs[opt.arg_name] = inter_opt.value
+
+        if isinstance(opt, ConverterOption):
+            option_kwargs[opt.arg_name] = opt._convert_value(option_kwargs[opt.arg_name])  # pyright: ignore
 
     return option_kwargs
```

### Comparing `hikari-arc-1.2.1/arc/internal/sigparse.py` & `hikari_arc-1.3.0/arc/internal/sigparse.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,22 @@
 from arc.command.option import (
     AttachmentOption,
     AttachmentParams,
     BoolOption,
     BoolParams,
     ChannelOption,
     ChannelParams,
+    ColorOption,
+    ColorParams,
     FloatOption,
     FloatParams,
     IntOption,
     IntParams,
+    MemberOption,
+    MemberParams,
     MentionableOption,
     MentionableParams,
     RoleOption,
     RoleParams,
     StrOption,
     StrParams,
     UserOption,
@@ -42,27 +46,32 @@
 TYPE_TO_OPTION_MAPPING: dict[type[t.Any], type[CommandOptionBase[t.Any, t.Any, t.Any]]] = {
     bool: BoolOption,
     int: IntOption,
     str: StrOption,
     float: FloatOption,
     hikari.Role: RoleOption,
     hikari.Attachment: AttachmentOption,
+    hikari.Member: MemberOption,
+    hikari.InteractionMember: MemberOption,
+    hikari.Color: ColorOption,
     hikari.User: UserOption,
 }
 
 OPT_TO_PARAMS_MAPPING: dict[type[CommandOptionBase[t.Any, t.Any, t.Any]], type[t.Any]] = {
     BoolOption: BoolParams,
     IntOption: IntParams,
     StrOption: StrParams,
     FloatOption: FloatParams,
     UserOption: UserParams,
     ChannelOption: ChannelParams,
     MentionableOption: MentionableParams,
     RoleOption: RoleParams,
     AttachmentOption: AttachmentParams,
+    MemberOption: MemberParams,
+    ColorOption: ColorParams,
 }
 
 BASE_CHANNEL_TYPE_MAP: dict[type[hikari.PartialChannel], hikari.ChannelType] = {
     hikari.GuildTextChannel: hikari.ChannelType.GUILD_TEXT,
     hikari.DMChannel: hikari.ChannelType.DM,
     hikari.GuildVoiceChannel: hikari.ChannelType.GUILD_VOICE,
     hikari.GroupDMChannel: hikari.ChannelType.GROUP_DM,
@@ -301,32 +310,37 @@
             raise TypeError(
                 f"Expected params object to be of type '{OPT_TO_PARAMS_MAPPING[opt_type].__name__}', got '{type(params).__name__}'"
             )
 
         # If it's a union of channel types, we need to parse all channel types
         if union is not None and any(arg in CHANNEL_TYPES_MAPPING for arg in t.get_args(union)):
             channel_types = _parse_channel_union_type_hint(union)
-            options[arg_name] = ChannelOption._from_params(
-                name=params.name or arg_name, is_required=not is_optional, params=params, channel_types=channel_types
+            options[params.name or arg_name] = ChannelOption._from_params(
+                name=params.name or arg_name,
+                arg_name=arg_name,
+                is_required=not is_optional,
+                params=params,
+                channel_types=channel_types,
             )
             continue
 
         # If it's a single channel type, just pass the channel type
         elif type_ in CHANNEL_TYPES_MAPPING:
-            options[arg_name] = ChannelOption._from_params(
+            options[params.name or arg_name] = ChannelOption._from_params(
                 name=params.name or arg_name,
+                arg_name=arg_name,
                 is_required=not is_optional,
                 params=params,
                 channel_types=_channels_to_channel_types([type_]),
             )
             continue
 
         # Otherwise just build the option
-        options[arg_name] = opt_type._from_params(
-            name=params.name or arg_name, is_required=not is_optional, params=params
+        options[params.name or arg_name] = opt_type._from_params(
+            name=params.name or arg_name, arg_name=arg_name, is_required=not is_optional, params=params
         )
 
     return options
 
 
 def _hint_to_event(hint: t.Any) -> type[hikari.Event] | None:
     """Convert a type hint to an event type."""
```

### Comparing `hikari-arc-1.2.1/arc/internal/sync.py` & `hikari_arc-1.3.0/arc/internal/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,17 @@
 
     Returns
     -------
     dict[hikari.Snowflake | None, dict[hikari.CommandType, dict[str, CommandBase[t.Any, t.Any]]]]
         A mapping of guilds to command types to command names to commands that should be registered.
     """
     # The big daddy of all mappings
-    mapping: dict[
-        hikari.Snowflake | None, dict[hikari.CommandType, dict[str, CommandBase[t.Any, t.Any]]]
-    ] = defaultdict(lambda: defaultdict(lambda: defaultdict(dict)))  # type: ignore
+    mapping: dict[hikari.Snowflake | None, dict[hikari.CommandType, dict[str, CommandBase[t.Any, t.Any]]]] = (
+        defaultdict(lambda: defaultdict(lambda: defaultdict(dict)))  # type: ignore
+    )
 
     for command in itertools.chain(
         client._slash_commands.values(), client._message_commands.values(), client._user_commands.values()
     ):
         guild_ids = (
             command.guilds
             or (command.plugin.default_enabled_guilds if command.plugin else None)
```

### Comparing `hikari-arc-1.2.1/arc/internal/types.py` & `hikari_arc-1.3.0/arc/internal/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import typing as t
 
 if t.TYPE_CHECKING:
+    import alluka
     import hikari
 
     from arc.abc import Client, Hookable, HookResult, OptionParams
     from arc.abc.concurrency_limiting import HasConcurrencyLimiter
     from arc.client import GatewayClientBase, RESTClientBase
     from arc.command import SlashCommand, SlashGroup
     from arc.context import AutocompleteData, Context
@@ -30,20 +31,21 @@
 # Type aliases
 EventCallbackT: t.TypeAlias = "t.Callable[[EventT], t.Awaitable[None]]"
 ErrorHandlerCallbackT: t.TypeAlias = "t.Callable[[Context[ClientT], Exception], t.Awaitable[None]]"
 SlashCommandLike: t.TypeAlias = "SlashCommand[ClientT] | SlashGroup[ClientT]"
 CommandCallbackT: t.TypeAlias = "t.Callable[t.Concatenate[Context[ClientT], ...], t.Awaitable[None]]"
 MessageCommandCallbackT: t.TypeAlias = "t.Callable[[Context[ClientT], hikari.Message], t.Awaitable[None]]"
 UserCommandCallbackT: t.TypeAlias = "t.Callable[[Context[ClientT], hikari.User], t.Awaitable[None]]"
-AutocompleteCallbackT: t.TypeAlias = "t.Callable[[AutocompleteData[ClientT, ChoiceT]], t.Awaitable[t.Sequence[ChoiceT]]] | t.Callable[[AutocompleteData[ClientT, ChoiceT]], t.Awaitable[t.Sequence[hikari.api.AutocompleteChoiceBuilder]]]"
+AutocompleteCallbackT: t.TypeAlias = "t.Callable[[AutocompleteData[ClientT, ChoiceT]], t.Awaitable[t.Sequence[ChoiceT]]] | t.Callable[[AutocompleteData[ClientT, ChoiceT]], t.Awaitable[t.Mapping[str, ChoiceT]]] | t.Callable[[AutocompleteData[ClientT, ChoiceT]], t.Awaitable[t.Sequence[hikari.api.AutocompleteChoiceBuilder]]]"
 ResponseBuilderT: t.TypeAlias = (
     "hikari.api.InteractionMessageBuilder | hikari.api.InteractionDeferredBuilder | hikari.api.InteractionModalBuilder"
 )
 HookT: t.TypeAlias = "t.Callable[[Context[ClientT]], t.Awaitable[HookResult]] | t.Callable[[Context[ClientT]], HookResult] | t.Callable[[Context[ClientT]], None] | t.Callable[[Context[ClientT]], t.Awaitable[None]]"
 PostHookT: t.TypeAlias = "t.Callable[[Context[ClientT]], None] | t.Callable[[Context[ClientT]], t.Awaitable[None]]"
+InjectionHookT: t.TypeAlias = "t.Callable[[Context[ClientT], alluka.OverridingContext], None] | t.Callable[[Context[ClientT], alluka.OverridingContext], t.Awaitable[None]]"
 LifeCycleHookT: t.TypeAlias = "t.Callable[[ClientT], t.Awaitable[None]]"
 CommandLocaleRequestT: t.TypeAlias = "t.Callable[[CommandLocaleRequest], LocaleResponse]"
 OptionLocaleRequestT: t.TypeAlias = "t.Callable[[OptionLocaleRequest], LocaleResponse]"
 CustomLocaleRequestT: t.TypeAlias = "t.Callable[[CustomLocaleRequest], str]"
 
 # MIT License
 #
```

### Comparing `hikari-arc-1.2.1/arc/internal/version.py` & `hikari_arc-1.3.0/arc/internal/version.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/locale.py` & `hikari_arc-1.3.0/arc/locale.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/plugin.py` & `hikari_arc-1.3.0/arc/plugin.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/utils/__init__.py` & `hikari_arc-1.3.0/arc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/utils/concurrency_limiter.py` & `hikari_arc-1.3.0/arc/utils/concurrency_limiter.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
     async def acquire(self, item: KeyT) -> None:
         """Acquire a concurrency slot for an item.
 
         This will block until a slot is available.
         """
         key = self._get_key(item)
-        bucket = self._buckets.setdefault(key, _Bucket.for_limiter(key, self))
+        bucket = self._buckets.setdefault(key, _Bucket.for_limiter(key, self))  # pyright: ignore reportUnknowMemberType
         await bucket.semaphore.acquire()
 
     def release(self, item: KeyT) -> None:
         """Release a concurrency slot for an item."""
         key = self._get_key(item)
         bucket = self._buckets.get(key)
         if bucket is None:
```

### Comparing `hikari-arc-1.2.1/arc/utils/hooks/__init__.py` & `hikari_arc-1.3.0/arc/utils/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/utils/hooks/basic.py` & `hikari_arc-1.3.0/arc/utils/hooks/basic.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/utils/hooks/limiters.py` & `hikari_arc-1.3.0/arc/utils/hooks/limiters.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/utils/loops.py` & `hikari_arc-1.3.0/arc/utils/loops.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/arc/utils/ratelimiter.py` & `hikari_arc-1.3.0/arc/utils/ratelimiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         RateLimiterExhaustedError
             If the ratelimiter is ratelimited and wait is False.
         """
         event = asyncio.Event()
 
         key = self.get_key(item)
         # Get existing or insert new bucket
-        bucket = self._buckets.setdefault(key, _Bucket.for_limiter(key, self))
+        bucket = self._buckets.setdefault(key, _Bucket.for_limiter(key, self))  # pyright: ignore reportUnknowMemberType
 
         if bucket.is_exhausted and not wait:
             raise RateLimiterExhaustedError(
                 self,
                 bucket.reset_at - time.monotonic(),
                 f"Ratelimited for {bucket.reset_at - time.monotonic()} seconds.",
             )
```

### Comparing `hikari-arc-1.2.1/hikari_arc.egg-info/PKG-INFO` & `hikari_arc-1.3.0/hikari_arc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-arc
-Version: 1.2.1
+Version: 1.3.0
 Summary: A command handler for hikari with a focus on type-safety and correctness.
 Home-page: https://github.com/hypergonial/hikari-arc
 Author: hypergonial
 Author-email: git@hypergonial.com
 Maintainer: hypergonial
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,37 +20,37 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10.0,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hikari>=2.0.0.dev122
-Requires-Dist: alluka>=0.1.4
+Requires-Dist: alluka<0.4,>=0.3.0
 Requires-Dist: attrs>=23.1
 Requires-Dist: colorama; sys_platform == "win32"
 Provides-Extra: docs
-Requires-Dist: mkdocs-material[imaging]~=9.5.7; extra == "docs"
-Requires-Dist: mkdocs~=1.5.3; extra == "docs"
-Requires-Dist: mkdocstrings-python~=1.8.0; extra == "docs"
-Requires-Dist: black~=24.1.1; extra == "docs"
+Requires-Dist: mkdocs-material[imaging]~=9.5.21; extra == "docs"
+Requires-Dist: mkdocs~=1.6.0; extra == "docs"
+Requires-Dist: mkdocstrings-python~=1.10.0; extra == "docs"
+Requires-Dist: black~=24.4.2; extra == "docs"
 Requires-Dist: griffe-inherited-docstrings~=1.0.0; extra == "docs"
-Requires-Dist: mkdocs-glightbox~=0.3.7; extra == "docs"
+Requires-Dist: mkdocs-glightbox~=0.4.0; extra == "docs"
 Provides-Extra: dev
-Requires-Dist: ruff==0.1.14; extra == "dev"
-Requires-Dist: pyright==1.1.350; extra == "dev"
-Requires-Dist: nox==2023.4.22; extra == "dev"
-Requires-Dist: typing_extensions==4.9.0; extra == "dev"
-Requires-Dist: pytest==7.4.4; extra == "dev"
-Requires-Dist: pytest-asyncio==0.23.4; extra == "dev"
-Requires-Dist: slotscheck==0.17.1; extra == "dev"
+Requires-Dist: ruff==0.4.4; extra == "dev"
+Requires-Dist: pyright==1.1.362; extra == "dev"
+Requires-Dist: nox==2024.4.15; extra == "dev"
+Requires-Dist: typing_extensions==4.11.0; extra == "dev"
+Requires-Dist: pytest==8.2.0; extra == "dev"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "dev"
+Requires-Dist: slotscheck==0.19.0; extra == "dev"
 Provides-Extra: rest
 Requires-Dist: hikari[server]>=2.0.0.dev122; extra == "rest"
 Provides-Extra: cron
-Requires-Dist: croniter==2.0.1; extra == "cron"
-Requires-Dist: types-croniter==2.0.0.20240106; extra == "cron"
+Requires-Dist: croniter==2.0.5; extra == "cron"
+Requires-Dist: types-croniter==2.0.0.20240423; extra == "cron"
 
 # hikari-arc
 
 <div align="center">
 
 [![PyPI](https://img.shields.io/pypi/v/hikari-arc)](https://pypi.org/project/hikari-arc)
 [![CI](https://github.com/hypergonial/hikari-arc/actions/workflows/ci.yml/badge.svg)](https://github.com/hypergonial/hikari-arc/actions/workflows/ci.yml)
```

### Comparing `hikari-arc-1.2.1/pyproject.toml` & `hikari_arc-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 [tool.ruff]
-exclude = ["docs", "build"]
+exclude = ["examples", "docs", "build"]
+line-length = 120
+target-version = "py310"
+
+[tool.ruff.lint]
 select = [
     "E",
     "F",
     "I",
     "TCH",
     "C",
     "N",
@@ -17,26 +21,24 @@
     "Q",
     "RSE",
     "SIM",
     "RUF",
 ]
 ignore = ["F405", "F403", "E501", "D205"]
 fixable = ["I", "TCH", "D"]
-line-length = 120
-target-version = "py310"
-
-[tool.ruff.format]
-skip-magic-trailing-comma = true
 
 [tool.ruff.lint.isort]
 split-on-trailing-comma = false
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
+[tool.ruff.format]
+skip-magic-trailing-comma = true
+
 [tool.slotscheck]
 strict-imports = true
 require-superclass = false
 require-subclass = true
 exclude-classes = ":.*(Exception|Error|Proto|AutocompleteData)"
 
 [tool.mypy]
```

### Comparing `hikari-arc-1.2.1/setup.py` & `hikari_arc-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/tests/test_client.py` & `hikari_arc-1.3.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/tests/test_context_command.py` & `hikari_arc-1.3.0/tests/test_context_command.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/tests/test_di.py` & `hikari_arc-1.3.0/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/tests/test_inheritance.py` & `hikari_arc-1.3.0/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/tests/test_options.py` & `hikari_arc-1.3.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `hikari-arc-1.2.1/tests/test_sigparse.py` & `hikari_arc-1.3.0/tests/test_sigparse.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 
 import arc
 from arc.internal.sigparse import BASE_CHANNEL_TYPE_MAP, CHANNEL_TYPES_MAPPING, parse_command_signature
 
 
 async def correct_command(
     ctx: arc.GatewayContext,
-    a: arc.Option[int, arc.IntParams(description="foo", min=10)],
-    b: arc.Option[str, arc.StrParams(description="bar", min_length=100)],
-    c: arc.Option[float | None, arc.FloatParams(description="baz", max=50.0)],
-    d: arc.Option[hikari.GuildTextChannel | hikari.GuildNewsChannel | None, arc.ChannelParams(description="qux")],
-    e: arc.Option[hikari.GuildChannel | None, arc.ChannelParams(description="quux")],
-    f: arc.Option[hikari.Role | hikari.User | None, arc.MentionableParams(description="quuz")] = None,
-    g: arc.Option[hikari.Attachment | None, arc.AttachmentParams(description="among us")] = None,
-    h: arc.Option[bool, arc.BoolParams(description="among us")] = False,
-    i: arc.Option[str, arc.StrParams(description="foo")] = "among us",
+    a: arc.Option[int, arc.IntParams("foo", min=10)],
+    b: arc.Option[str, arc.StrParams("bar", min_length=100)],
+    c: arc.Option[float | None, arc.FloatParams("baz", max=50.0)],
+    d: arc.Option[hikari.GuildTextChannel | hikari.GuildNewsChannel | None, arc.ChannelParams("qux")],
+    e: arc.Option[hikari.GuildChannel | None, arc.ChannelParams("quux")],
+    f: arc.Option[hikari.Role | hikari.User | None, arc.MentionableParams("quuz")] = None,
+    g: arc.Option[hikari.Attachment | None, arc.AttachmentParams("among us")] = None,
+    h: arc.Option[bool, arc.BoolParams("among us")] = False,
+    i: arc.Option[str, arc.StrParams("foo")] = "among us",
+    j: arc.Option[hikari.Member | None, arc.MemberParams("among us")] = None,
+    k: arc.Option[hikari.Color, arc.ColorParams("foo", name="color")] = hikari.Color(0x000000),
 ) -> None:
     pass
 
 
 def test_correct_command() -> None:
     options = parse_command_signature(correct_command)
-    assert len(options) == 9
+    assert len(options) == 11
 
     assert isinstance(options["a"], arc.command.IntOption)
     assert options["a"].name == "a"
     assert options["a"].description == "foo"
     assert options["a"].is_required
     assert options["a"].min == 10
     assert options["a"].max is None
@@ -87,14 +89,25 @@
     assert not options["h"].is_required
 
     assert isinstance(options["i"], arc.command.StrOption)
     assert options["i"].name == "i"
     assert options["i"].description == "foo"
     assert not options["i"].is_required
 
+    assert isinstance(options["j"], arc.command.MemberOption)
+    assert options["j"].name == "j"
+    assert options["j"].description == "among us"
+    assert not options["j"].is_required
+
+    assert isinstance(options["color"], arc.command.ColorOption)
+    assert options["color"].name == "color"
+    assert options["color"].arg_name == "k"
+    assert options["color"].description == "foo"
+    assert not options["color"].is_required
+
 
 async def wrong_params_type(
     ctx: arc.GatewayContext,
     a: arc.Option[int, arc.IntParams(description="foo", min=10)],
     b: arc.Option[str, arc.IntParams(description="bar", max=50)],
 ) -> None:
     pass
@@ -139,20 +152,20 @@
     assert isinstance(options["a"], arc.command.IntOption)
     assert options["a"].name == "a"
     assert options["a"].description == "foo"
     assert options["a"].is_required
     assert options["a"].min == 10
     assert options["a"].max is None
 
-    assert isinstance(options["c"], arc.command.StrOption)
-    assert options["c"].name == "b"
-    assert options["c"].description == "bar"
-    assert options["c"].is_required
-    assert options["c"].min_length == 100
-    assert options["c"].max_length is None
+    assert isinstance(options["b"], arc.command.StrOption)
+    assert options["b"].name == "b"
+    assert options["b"].description == "bar"
+    assert options["b"].is_required
+    assert options["b"].min_length == 100
+    assert options["b"].max_length is None
 
 
 def test_ensure_parse_channel_types_has_every_channel_class() -> None:
     for _, attribute in inspect.getmembers(
         hikari, lambda a: isinstance(a, type) and issubclass(a, hikari.PartialChannel)
     ):
         result = CHANNEL_TYPES_MAPPING.get(attribute)
```

### Comparing `hikari-arc-1.2.1/tests/test_slash.py` & `hikari_arc-1.3.0/tests/test_slash.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 client = arc.GatewayClient(bot)
 
 
 @client.include()
 @arc.slash_command("test", default_permissions=hikari.Permissions.ADMINISTRATOR)
 async def my_command(
     ctx: arc.GatewayContext,
-    a: arc.Option[int, arc.IntParams(description="foo", min=10)],
-    b: arc.Option[str, arc.StrParams(description="bar", min_length=100)],
-    c: arc.Option[float | None, arc.FloatParams(description="baz", max=50.0)],
-    d: arc.Option[hikari.GuildTextChannel | hikari.GuildNewsChannel | None, arc.ChannelParams(description="qux")],
-    e: arc.Option[hikari.GuildChannel | None, arc.ChannelParams(description="quux")],
-    f: arc.Option[hikari.Role | hikari.User, arc.MentionableParams(description="quuz")],
-    g: arc.Option[hikari.Attachment | None, arc.AttachmentParams(description="among us")],
+    a: arc.Option[int, arc.IntParams("foo", min=10)],
+    b: arc.Option[str, arc.StrParams("bar", min_length=100)],
+    c: arc.Option[float | None, arc.FloatParams("baz", max=50.0)],
+    d: arc.Option[hikari.GuildTextChannel | hikari.GuildNewsChannel | None, arc.ChannelParams("qux")],
+    e: arc.Option[hikari.GuildChannel | None, arc.ChannelParams("quux")],
+    f: arc.Option[hikari.Role | hikari.User, arc.MentionableParams("quuz")],
+    g: arc.Option[hikari.Attachment | None, arc.AttachmentParams(name="last", description="among us")],
 ) -> None:
     pass
 
 
 group = client.include_slash_group(
     "my_group", "My group description", default_permissions=hikari.Permissions.ADMINISTRATOR
 )
@@ -28,26 +28,26 @@
 subgroup = group.include_subgroup("my_subgroup", "My subgroup description")
 
 
 @group.include
 @arc.slash_subcommand("test_subcommand", "My subcommand description")
 async def my_subcommand(
     ctx: arc.GatewayContext,
-    a: arc.Option[int, arc.IntParams(description="foo", min=10)],
-    b: arc.Option[str, arc.StrParams(description="bar", min_length=100)],
+    a: arc.Option[int, arc.IntParams("foo", min=10)],
+    b: arc.Option[str, arc.StrParams("bar", min_length=100)],
 ) -> None:
     pass
 
 
 @subgroup.include()
 @arc.slash_subcommand("test_subsubcommand", "My subsubcommand description")
 async def my_subsubcommand(
     ctx: arc.GatewayContext,
-    a: arc.Option[int, arc.IntParams(description="foo", min=10)],
-    b: arc.Option[str, arc.StrParams(description="bar", min_length=100)],
+    a: arc.Option[int, arc.IntParams("foo", min=10)],
+    b: arc.Option[str, arc.StrParams("bar", min_length=100)],
 ) -> None:
     pass
 
 
 def test_my_command() -> None:
     assert len(client._slash_commands) == 2
 
@@ -112,18 +112,19 @@
     }
 
     assert isinstance(options["f"], arc.command.MentionableOption)
     assert options["f"].name == "f"
     assert options["f"].description == "quuz"
     assert options["f"].is_required
 
-    assert isinstance(options["g"], arc.command.AttachmentOption)
-    assert options["g"].name == "g"
-    assert options["g"].description == "among us"
-    assert not options["g"].is_required
+    assert isinstance(options["last"], arc.command.AttachmentOption)
+    assert options["last"].name == "last"
+    assert options["last"].arg_name == "g"
+    assert options["last"].description == "among us"
+    assert not options["last"].is_required
 
 
 def test_my_group() -> None:
     group = client._slash_commands["my_group"]
     assert isinstance(group, arc.SlashGroup)
 
     assert len(group.children) == 2
```

