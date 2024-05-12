# Comparing `tmp/vnerrant-1.0.1rc1.tar.gz` & `tmp/vnerrant-1.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnerrant-1.0.1rc1.tar", last modified: Sun Apr 28 07:09:41 2024, max compression
+gzip compressed data, was "vnerrant-1.0.1rc2.tar", last modified: Sun May 12 17:53:45 2024, max compression
```

## Comparing `vnerrant-1.0.1rc1.tar` & `vnerrant-1.0.1rc2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.127676 vnerrant-1.0.1rc1/
--rw-r--r--   0 manred1997   (501) staff       (20)      101 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/MANIFEST.in
--rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-04-28 07:09:41.127067 vnerrant-1.0.1rc1/PKG-INFO
--rw-r--r--   0 manred1997   (501) staff       (20)     9342 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/README.md
--rw-r--r--   0 manred1997   (501) staff       (20)       38 2024-04-28 07:09:41.127716 vnerrant-1.0.1rc1/setup.cfg
--rw-r--r--   0 manred1997   (501) staff       (20)     1527 2024-04-28 07:09:29.000000 vnerrant-1.0.1rc1/setup.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.111078 vnerrant-1.0.1rc1/tests/
--rw-r--r--   0 manred1997   (501) staff       (20)     6916 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc1/tests/test_vnerrant.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.112774 vnerrant-1.0.1rc1/vnerrant/
--rw-r--r--   0 manred1997   (501) staff       (20)     1079 2024-04-28 07:09:25.000000 vnerrant-1.0.1rc1/vnerrant/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    11910 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc1/vnerrant/annotator.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.114196 vnerrant-1.0.1rc1/vnerrant/cli/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/cli/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10307 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/cli/convert.py
--rw-r--r--   0 manred1997   (501) staff       (20)     4512 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/cli/evaluate.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.116223 vnerrant-1.0.1rc1/vnerrant/components/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     9008 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/alignment.py
--rw-r--r--   0 manred1997   (501) staff       (20)      479 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/classifier.py
--rw-r--r--   0 manred1997   (501) staff       (20)     6382 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/converter.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.118517 vnerrant-1.0.1rc1/vnerrant/components/en/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    31652 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/en/classifier.py
--rw-r--r--   0 manred1997   (501) staff       (20)     3082 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/constants.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1886 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/en/explainer.py
--rw-r--r--   0 manred1997   (501) staff       (20)    12286 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/lancaster.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10931 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/en/merger.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.119985 vnerrant-1.0.1rc1/vnerrant/components/en/resources/
--rw-r--r--   0 manred1997   (501) staff       (20)     1035 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/resources/README.md
--rw-r--r--   0 manred1997   (501) staff       (20)      394 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/resources/en-ptb_map
--rw-r--r--   0 manred1997   (501) staff       (20)  1839291 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/resources/en_GB-large.txt
--rw-r--r--   0 manred1997   (501) staff       (20)     1595 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/en/utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)     9042 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/evaluater.py
--rw-r--r--   0 manred1997   (501) staff       (20)      200 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/explainer.py
--rw-r--r--   0 manred1997   (501) staff       (20)     3188 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/components/merger.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2510 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/components/tokenizer.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.123707 vnerrant-1.0.1rc1/vnerrant/config/
--rw-r--r--   0 manred1997   (501) staff       (20)     2187 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/config/errant_verbose.json
--rw-r--r--   0 manred1997   (501) staff       (20)      532 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/config/mapping_type_error.yaml
--rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/config.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1981 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/constants.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.124123 vnerrant-1.0.1rc1/vnerrant/metrics/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/metrics/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2567 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/metrics/criteria.py
--rw-r--r--   0 manred1997   (501) staff       (20)      389 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/metrics/stats.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.124556 vnerrant-1.0.1rc1/vnerrant/model/
--rw-r--r--   0 manred1997   (501) staff       (20)       52 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc1/vnerrant/model/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10929 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc1/vnerrant/model/edit.py
--rw-r--r--   0 manred1997   (501) staff       (20)      556 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/run_cli.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.126653 vnerrant-1.0.1rc1/vnerrant/utils/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/utils/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     6734 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc1/vnerrant/utils/edit_utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)      647 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/utils/helper.py
--rw-r--r--   0 manred1997   (501) staff       (20)     4516 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/utils/pretty_results.py
--rw-r--r--   0 manred1997   (501) staff       (20)     7720 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc1/vnerrant/utils/string_utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1181 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc1/vnerrant/utils/utils.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-04-28 07:09:41.126838 vnerrant-1.0.1rc1/vnerrant.egg-info/
--rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/PKG-INFO
--rw-r--r--   0 manred1997   (501) staff       (20)     1446 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/SOURCES.txt
--rw-r--r--   0 manred1997   (501) staff       (20)        1 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/dependency_links.txt
--rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/entry_points.txt
--rw-r--r--   0 manred1997   (501) staff       (20)       26 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/requires.txt
--rw-r--r--   0 manred1997   (501) staff       (20)        9 2024-04-28 07:09:41.000000 vnerrant-1.0.1rc1/vnerrant.egg-info/top_level.txt
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.751693 vnerrant-1.0.1rc2/
+-rw-r--r--   0 manred1997   (501) staff       (20)      101 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/MANIFEST.in
+-rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-12 17:53:45.751454 vnerrant-1.0.1rc2/PKG-INFO
+-rw-r--r--   0 manred1997   (501) staff       (20)     9342 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc2/README.md
+-rw-r--r--   0 manred1997   (501) staff       (20)       38 2024-05-12 17:53:45.751737 vnerrant-1.0.1rc2/setup.cfg
+-rw-r--r--   0 manred1997   (501) staff       (20)     1527 2024-05-12 17:48:59.000000 vnerrant-1.0.1rc2/setup.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.734979 vnerrant-1.0.1rc2/tests/
+-rw-r--r--   0 manred1997   (501) staff       (20)     6916 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc2/tests/test_vnerrant.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.736661 vnerrant-1.0.1rc2/vnerrant/
+-rw-r--r--   0 manred1997   (501) staff       (20)     1079 2024-05-12 17:49:03.000000 vnerrant-1.0.1rc2/vnerrant/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    11976 2024-05-12 17:47:49.000000 vnerrant-1.0.1rc2/vnerrant/annotator.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.738174 vnerrant-1.0.1rc2/vnerrant/cli/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/cli/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10307 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/cli/convert.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     4512 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/cli/evaluate.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.740427 vnerrant-1.0.1rc2/vnerrant/components/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     9008 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/alignment.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      479 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/classifier.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     6382 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc2/vnerrant/components/converter.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.742380 vnerrant-1.0.1rc2/vnerrant/components/en/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/en/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    31652 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc2/vnerrant/components/en/classifier.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     3082 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/en/constants.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1886 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc2/vnerrant/components/en/explainer.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    12286 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/en/lancaster.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10931 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc2/vnerrant/components/en/merger.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.744195 vnerrant-1.0.1rc2/vnerrant/components/en/resources/
+-rw-r--r--   0 manred1997   (501) staff       (20)     1035 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/en/resources/README.md
+-rw-r--r--   0 manred1997   (501) staff       (20)      394 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/en/resources/en-ptb_map
+-rw-r--r--   0 manred1997   (501) staff       (20)  1839291 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/en/resources/en_GB-large.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)     1595 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/en/utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     9042 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/evaluater.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      200 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc2/vnerrant/components/explainer.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     3188 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc2/vnerrant/components/merger.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2510 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/components/tokenizer.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.748116 vnerrant-1.0.1rc2/vnerrant/config/
+-rw-r--r--   0 manred1997   (501) staff       (20)     2187 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc2/vnerrant/config/errant_verbose.json
+-rw-r--r--   0 manred1997   (501) staff       (20)      532 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/config/mapping_type_error.yaml
+-rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/config.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1981 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc2/vnerrant/constants.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.748509 vnerrant-1.0.1rc2/vnerrant/metrics/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/metrics/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2567 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/metrics/criteria.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      389 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/metrics/stats.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.748946 vnerrant-1.0.1rc2/vnerrant/model/
+-rw-r--r--   0 manred1997   (501) staff       (20)       52 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc2/vnerrant/model/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10929 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc2/vnerrant/model/edit.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      556 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/run_cli.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.751042 vnerrant-1.0.1rc2/vnerrant/utils/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/utils/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     7281 2024-05-12 17:47:44.000000 vnerrant-1.0.1rc2/vnerrant/utils/edit_utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      647 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/utils/helper.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     4516 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/utils/pretty_results.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     7720 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc2/vnerrant/utils/string_utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1181 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc2/vnerrant/utils/utils.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 17:53:45.751229 vnerrant-1.0.1rc2/vnerrant.egg-info/
+-rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-12 17:53:45.000000 vnerrant-1.0.1rc2/vnerrant.egg-info/PKG-INFO
+-rw-r--r--   0 manred1997   (501) staff       (20)     1446 2024-05-12 17:53:45.000000 vnerrant-1.0.1rc2/vnerrant.egg-info/SOURCES.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)        1 2024-05-12 17:53:45.000000 vnerrant-1.0.1rc2/vnerrant.egg-info/dependency_links.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-05-12 17:53:45.000000 vnerrant-1.0.1rc2/vnerrant.egg-info/entry_points.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)       26 2024-05-12 17:53:45.000000 vnerrant-1.0.1rc2/vnerrant.egg-info/requires.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)        9 2024-05-12 17:53:45.000000 vnerrant-1.0.1rc2/vnerrant.egg-info/top_level.txt
```

### Comparing `vnerrant-1.0.1rc1/PKG-INFO` & `vnerrant-1.0.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnerrant
-Version: 1.0.1rc1
+Version: 1.0.1rc2
 Summary: The ERRor ANnotation Toolkit (ERRANT).         Automatically extract and classify edits in parallel sentences.
 License: MIT
 Keywords: automatic annotation,grammatical errors,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnerrant-1.0.1rc1/README.md` & `vnerrant-1.0.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/setup.py` & `vnerrant-1.0.1rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Readme text for long description
 with open(base_dir / "README.md") as f:
     readme = f.read()
 
 setup(
     name="vnerrant",
-    version="1.0.1rc1",
+    version="1.0.1rc2",
     license="MIT",
     description="The ERRor ANnotation Toolkit (ERRANT). \
         Automatically extract and classify edits in parallel sentences.",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords=[
         "automatic annotation",
```

### Comparing `vnerrant-1.0.1rc1/tests/test_vnerrant.py` & `vnerrant-1.0.1rc2/tests/test_vnerrant.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/__init__.py` & `vnerrant-1.0.1rc2/vnerrant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any
 
 import spacy
 
 from vnerrant.annotator import Annotator
 from vnerrant.utils.utils import get_spacy_models_for_language
 
-__version__ = "v1.0.1rc1"
+__version__ = "v1.0.1rc2"
 
 
 def load(
     lang: str = "en",
     model_name: str = "en_core_web_sm",
     nlp: Any = None,
 ) -> Annotator:
```

### Comparing `vnerrant-1.0.1rc1/vnerrant/annotator.py` & `vnerrant-1.0.1rc2/vnerrant/annotator.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,14 +285,15 @@
             if edit.original.text == edit.corrected.text:
                 continue
 
             space_edits.append(edit_utils.process_space_edit(edit))
 
         edit_utils.merge_edit_collection_with_space_edits(edit_collection, space_edits)
         edit_utils.update_operator(edit_collection.edits)
+        edit_utils.update_replace_operator(edit_collection.edits)
 
     def import_edit(
         self,
         orig: Doc,
         cor: Doc,
         edit: list,
         min: bool = True,
```

### Comparing `vnerrant-1.0.1rc1/vnerrant/cli/convert.py` & `vnerrant-1.0.1rc2/vnerrant/cli/convert.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/cli/evaluate.py` & `vnerrant-1.0.1rc2/vnerrant/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/alignment.py` & `vnerrant-1.0.1rc2/vnerrant/components/alignment.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/converter.py` & `vnerrant-1.0.1rc2/vnerrant/components/converter.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/en/classifier.py` & `vnerrant-1.0.1rc2/vnerrant/components/en/classifier.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/en/constants.py` & `vnerrant-1.0.1rc2/vnerrant/components/en/constants.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/en/explainer.py` & `vnerrant-1.0.1rc2/vnerrant/components/en/explainer.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/en/lancaster.py` & `vnerrant-1.0.1rc2/vnerrant/components/en/lancaster.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/en/merger.py` & `vnerrant-1.0.1rc2/vnerrant/components/en/merger.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/en/resources/README.md` & `vnerrant-1.0.1rc2/vnerrant/components/en/resources/README.md`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/en/resources/en_GB-large.txt` & `vnerrant-1.0.1rc2/vnerrant/components/en/resources/en_GB-large.txt`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/en/utils.py` & `vnerrant-1.0.1rc2/vnerrant/components/en/utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/evaluater.py` & `vnerrant-1.0.1rc2/vnerrant/components/evaluater.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/merger.py` & `vnerrant-1.0.1rc2/vnerrant/components/merger.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/components/tokenizer.py` & `vnerrant-1.0.1rc2/vnerrant/components/tokenizer.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/config/errant_verbose.json` & `vnerrant-1.0.1rc2/vnerrant/config/errant_verbose.json`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/config/mapping_type_error.yaml` & `vnerrant-1.0.1rc2/vnerrant/config/mapping_type_error.yaml`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/constants.py` & `vnerrant-1.0.1rc2/vnerrant/constants.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/metrics/criteria.py` & `vnerrant-1.0.1rc2/vnerrant/metrics/criteria.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/model/edit.py` & `vnerrant-1.0.1rc2/vnerrant/model/edit.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/run_cli.py` & `vnerrant-1.0.1rc2/vnerrant/run_cli.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/utils/edit_utils.py` & `vnerrant-1.0.1rc2/vnerrant/utils/edit_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,14 +124,26 @@
         if orig_text and cor_text:
             edit.edit_type = "R" + edit.edit_type[1:]
         elif not orig_text and cor_text:
             edit.edit_type = "M" + edit.edit_type[1:]
         else:
             edit.edit_type = "U" + edit.edit_type[1:]
 
+def update_replace_operator(edits: List[Edit]):
+    """
+    Update the replace operator of the edits.
+    Args:
+        edits (list[Edit]): A list of Edit objects to be updated.
+    """
+    for edit in edits:
+        if edit.edit_type[0] == "R":
+            edit.original.text = edit.original.text.strip()
+            edit.original.end_char = edit.original.start_char + len(edit.original.text)
+            edit.corrected.text = edit.corrected.text.strip()
+            edit.corrected.end_char = edit.corrected.start_char + len(edit.corrected.text)
 
 def process_space_edit(edit: Edit) -> Edit:
     """
     Process the space edit.
     Args:
         edit (Edit): An Edit object to be processed.
```

### Comparing `vnerrant-1.0.1rc1/vnerrant/utils/helper.py` & `vnerrant-1.0.1rc2/vnerrant/utils/helper.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/utils/pretty_results.py` & `vnerrant-1.0.1rc2/vnerrant/utils/pretty_results.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/utils/string_utils.py` & `vnerrant-1.0.1rc2/vnerrant/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant/utils/utils.py` & `vnerrant-1.0.1rc2/vnerrant/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc1/vnerrant.egg-info/PKG-INFO` & `vnerrant-1.0.1rc2/vnerrant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnerrant
-Version: 1.0.1rc1
+Version: 1.0.1rc2
 Summary: The ERRor ANnotation Toolkit (ERRANT).         Automatically extract and classify edits in parallel sentences.
 License: MIT
 Keywords: automatic annotation,grammatical errors,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnerrant-1.0.1rc1/vnerrant.egg-info/SOURCES.txt` & `vnerrant-1.0.1rc2/vnerrant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

