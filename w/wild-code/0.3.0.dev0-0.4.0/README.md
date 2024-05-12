# Comparing `tmp/wild_code-0.3.0.dev0.tar.gz` & `tmp/wild_code-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wild_code-0.3.0.dev0.tar", last modified: Thu May  9 22:33:09 2024, max compression
+gzip compressed data, was "wild_code-0.4.0.tar", last modified: Sun May 12 00:36:31 2024, max compression
```

## Comparing `wild_code-0.3.0.dev0.tar` & `wild_code-0.4.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:32.705349 wild_code-0.3.0.dev0/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3286 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.dockerignore
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.925358 wild_code-0.3.0.dev0/.github/
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.924756 wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1411 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/buggy_contract.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/buggy_test.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/model_eval_request.yml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.gitignore
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/.pre-commit-config.yaml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/CITATION.cff
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      542 2024-05-09 21:30:14.000000 wild_code-0.3.0.dev0/Dockerfile
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/LICENSE
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/MANIFEST.in
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10697 2024-05-09 22:30:32.701093 wild_code-0.3.0.dev0/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9579 2024-05-09 21:16:41.000000 wild_code-0.3.0.dev0/README.md
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/pyproject.toml
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      639 2024-05-09 22:24:07.000000 wild_code-0.3.0.dev0/release.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      155 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1334 2024-05-09 21:29:07.000000 wild_code-0.3.0.dev0/run.sh
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1237 2024-05-09 22:30:32.722612 wild_code-0.3.0.dev0/setup.cfg
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.930281 wild_code-0.3.0.dev0/tests/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/tests/requirements.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/tests/test_legacy_sanitizer.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/tests/test_treesitter_sanitizer.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:32.682162 wild_code-0.3.0.dev0/wild_code.egg-info/
--rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10697 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/PKG-INFO
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/SOURCES.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/dependency_links.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/entry_points.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      264 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/requires.txt
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wild_code.egg-info/top_level.txt
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.959927 wild_code-0.3.0.dev0/wildcode/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      424 2024-05-09 22:30:31.000000 wild_code-0.3.0.dev0/wildcode/_version.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.948951 wild_code-0.3.0.dev0/wildcode/data/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      163 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/data/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/data/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1670 2024-05-09 17:42:50.000000 wild_code-0.3.0.dev0/wildcode/data/wildcodebench.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.954317 wild_code-0.3.0.dev0/wildcode/eval/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7214 2024-05-09 18:37:38.000000 wild_code-0.3.0.dev0/wildcode/eval/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/eval/_special_oracle.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5654 2024-05-09 20:59:10.000000 wild_code-0.3.0.dev0/wildcode/eval/utils.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8293 2024-05-09 21:19:35.000000 wild_code-0.3.0.dev0/wildcode/evaluate.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.968590 wild_code-0.3.0.dev0/wildcode/gen/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/gen/__init__.py
-drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-09 22:30:31.968039 wild_code-0.3.0.dev0/wildcode/gen/util/
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1663 2024-05-08 23:14:51.000000 wild_code-0.3.0.dev0/wildcode/gen/util/__init__.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/gen/util/anthropic_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/gen/util/openai_request.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5554 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/generate.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2314 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/inspect.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5724 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/lecacy_sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    14089 2024-05-09 02:01:13.000000 wild_code-0.3.0.dev0/wildcode/model.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7995 2024-05-09 20:59:00.000000 wild_code-0.3.0.dev0/wildcode/sanitize.py
--rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3466 2024-05-07 17:11:36.000000 wild_code-0.3.0.dev0/wildcode/syncheck.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:53.208150 wild_code-0.4.0/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3206 2024-05-11 18:05:22.000000 wild_code-0.4.0/.dockerignore
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.409448 wild_code-0.4.0/.github/
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.408497 wild_code-0.4.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1407 2024-05-10 14:48:48.000000 wild_code-0.4.0/.github/ISSUE_TEMPLATE/buggy_contract.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1461 2024-05-07 17:11:36.000000 wild_code-0.4.0/.github/ISSUE_TEMPLATE/buggy_test.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       27 2024-05-07 17:11:36.000000 wild_code-0.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2177 2024-05-07 17:11:36.000000 wild_code-0.4.0/.github/ISSUE_TEMPLATE/model_eval_request.yml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3237 2024-05-07 17:11:36.000000 wild_code-0.4.0/.gitignore
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      458 2024-05-07 17:11:36.000000 wild_code-0.4.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      413 2024-05-07 17:11:36.000000 wild_code-0.4.0/CITATION.cff
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      757 2024-05-11 23:30:52.000000 wild_code-0.4.0/Dockerfile
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    11438 2024-05-07 17:11:36.000000 wild_code-0.4.0/LICENSE
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)       39 2024-05-07 17:11:36.000000 wild_code-0.4.0/MANIFEST.in
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10797 2024-05-12 00:33:53.201888 wild_code-0.4.0/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     9684 2024-05-11 23:45:13.000000 wild_code-0.4.0/README.md
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      246 2024-05-07 17:11:36.000000 wild_code-0.4.0/pyproject.toml
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      592 2024-05-11 23:46:21.000000 wild_code-0.4.0/release.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      155 2024-05-11 23:46:56.000000 wild_code-0.4.0/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1348 2024-05-11 20:16:24.000000 wild_code-0.4.0/run.sh
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1237 2024-05-12 00:33:53.224755 wild_code-0.4.0/setup.cfg
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.414260 wild_code-0.4.0/tests/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        7 2024-05-07 17:11:36.000000 wild_code-0.4.0/tests/requirements.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      854 2024-05-07 17:11:36.000000 wild_code-0.4.0/tests/test_legacy_sanitizer.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3964 2024-05-07 17:11:36.000000 wild_code-0.4.0/tests/test_treesitter_sanitizer.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:53.178377 wild_code-0.4.0/wild_code.egg-info/
+-rw-r--r--   0 zhuoyt    (1001) zhuoyt    (1001)    10797 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/PKG-INFO
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1095 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        1 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      288 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/entry_points.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      264 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/requires.txt
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)        9 2024-05-12 00:33:52.000000 wild_code-0.4.0/wild_code.egg-info/top_level.txt
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.443536 wild_code-0.4.0/wildcode/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      120 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      411 2024-05-12 00:33:52.000000 wild_code-0.4.0/wildcode/_version.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.432472 wild_code-0.4.0/wildcode/data/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      159 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/data/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     6076 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/data/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1612 2024-05-10 15:13:52.000000 wild_code-0.4.0/wildcode/data/wildcodebench.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.437948 wild_code-0.4.0/wildcode/eval/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7214 2024-05-11 17:29:07.000000 wild_code-0.4.0/wildcode/eval/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      377 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/eval/_special_oracle.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5715 2024-05-11 17:28:58.000000 wild_code-0.4.0/wildcode/eval/utils.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     8279 2024-05-10 22:27:09.000000 wild_code-0.4.0/wildcode/evaluate.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.452117 wild_code-0.4.0/wildcode/gen/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)      753 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/gen/__init__.py
+drwxrwxr-x   0 zhuoyt    (1001) zhuoyt    (1001)        0 2024-05-12 00:33:52.451450 wild_code-0.4.0/wildcode/gen/util/
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2159 2024-05-11 17:28:48.000000 wild_code-0.4.0/wildcode/gen/util/__init__.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1439 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/gen/util/anthropic_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     1813 2024-05-07 17:11:36.000000 wild_code-0.4.0/wildcode/gen/util/openai_request.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5550 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/generate.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     2310 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/inspect.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     5720 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/lecacy_sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)    14089 2024-05-09 02:01:13.000000 wild_code-0.4.0/wildcode/model.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     7991 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/sanitize.py
+-rw-rw-r--   0 zhuoyt    (1001) zhuoyt    (1001)     3462 2024-05-10 14:48:48.000000 wild_code-0.4.0/wildcode/syncheck.py
```

### Comparing `wild_code-0.3.0.dev0/.dockerignore` & `wild_code-0.4.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -158,17 +158,16 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #  nuclear option because steven uses PyCharm.
 .idea/
 
 # VSCode
 .vscode/
-EvalPlus/
+OpenPlus/
 backup/
 passrate.p*
 min_cov_dir/
-HumanEvalPlus*.jsonl
-HumanEvalPlus*.gz
-MbppPlus*.jsonl
-MbppPlus*.gz
 wildcode/_version.py
-*mbpp.json
+*.jsonl
+inspect/
+*.zip
+*.json
```

### Comparing `wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/buggy_contract.yml` & `wild_code-0.4.0/.github/ISSUE_TEMPLATE/buggy_contract.yml`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
       placeholder: WildCodeBench/[??]
     validations:
       required: true
   - type: textarea
     id: original
     attributes:
       label: "The original wrong contract"
-      description: You can run `python -c "from wildcode.data import get_wild_code_bench print(get_wild_code_bench['WildCodeBench/❓']['contract'])"`
+      description: You can run `python -c "from wildcode.data import get_wildcodebench print(get_wildcodebench['WildCodeBench/❓']['contract'])"`
       render: python
     validations:
       required: true
   - type: textarea
     id: new
     attributes:
       label: "Your proposed new contract"
```

### Comparing `wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/buggy_test.yml` & `wild_code-0.4.0/.github/ISSUE_TEMPLATE/buggy_test.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/.github/ISSUE_TEMPLATE/model_eval_request.yml` & `wild_code-0.4.0/.github/ISSUE_TEMPLATE/model_eval_request.yml`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/.gitignore` & `wild_code-0.4.0/.dockerignore`

 * *Files 2% similar despite different names*

```diff
@@ -158,16 +158,12 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #  nuclear option because steven uses PyCharm.
 .idea/
 
 # VSCode
 .vscode/
-OpenPlus/
 backup/
 passrate.p*
 min_cov_dir/
 wildcode/_version.py
-*.jsonl
 inspect/
-*.zip
-*.json
```

### Comparing `wild_code-0.3.0.dev0/Dockerfile` & `wild_code-0.4.0/Dockerfile`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # Better use newer Python as generated code can use new features
 FROM python:3.10-slim
 
-# install git
-RUN apt-get update && apt-get install -y git && apt-get -y install g++
+# install git, g++ and python3-tk
+RUN apt-get update && apt-get install -y git g++ python3-tk zip unzip procps
 
 # upgrade to latest pip
 RUN pip install --upgrade pip
 
+# Add a new user "wildcodeuser"
+RUN adduser --disabled-password --gecos "" wildcodeuser
+
 COPY . /wildcode
 
-RUN cd /wildcode && pip install . && pip install -r https://raw.githubusercontent.com/bigcode-project/open-eval/main/requirements.txt
+RUN cd /wildcode && pip install . && pip install -r https://raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/requirements.txt
 
 # Pre-install the dataset
-RUN python3 -c "from wildcode.data import get_wild_code_bench;"
+RUN python3 -c "from wildcode.data import get_wildcodebench; get_wildcodebench()"
+
+RUN chown -R wildcodeuser:wildcodeuser /wildcode
+USER wildcodeuser
 
 WORKDIR /wildcode
 
-ENTRYPOINT ["python3", "-m", "wildcode.evaluate"]
+ENTRYPOINT ["python3", "-m", "wildcode.evaluate"]
```

### Comparing `wild_code-0.3.0.dev0/LICENSE` & `wild_code-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/PKG-INFO` & `wild_code-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.3.0.dev0
+Version: 0.4.0
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -119,38 +119,38 @@
 </details>
 
 ### Code Generation
 
 To generate code samples from a model, you can use the following command:
 
 ```shell
-wildcode.generate --model [model_name] --dataset wildcodebench --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
+wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
 ```
 The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
 * `entry_point` is the name of the function
 * `prompt` is the function signature with docstring
 * `instruction` is the instruction for the task completion
-+ `canonical_solution` is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
++ `canonical_solution` is the ground-truth implementation
 + `test` is the `unittest` test case
 
 </div>
 </details>
 
 > [!Note]
 >
 > **Expected Schema of `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`**
 >
-> 1. `task_id`: Task ID, which are the keys of `get_[human_eval|mbpp]_plus()`
+> 1. `task_id`: Task ID, which are the keys of `get_wildcodebench()`
 > 2. `solution` (optional): Self-contained solution (usually including the prompt)
->    * Example: `{"task_id": "HumanEval/?", "solution": "def f():\n    return 1"}`
+>    * Example: `{"task_id": "WildCodeBench/?", "solution": "def f():\n    return 1"}`
 
 ### Code Post-processing
 
 LLM-generated text may not be compilable code for including natural language lines or incomplete extra code.
 We provide a tool namely `wildcode.sanitize` to clean up the code:
 
 ```shell
@@ -181,23 +181,26 @@
 
 
 ### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
-docker run -v $(pwd):/app terryzho/wildcode:latest --dataset [wildcodebench] --samples samples.jsonl
+# mount the current directory to the container
+docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl
+# ...Or locally ⚠️
+wildcode.evaluate --dataset wildcodebench --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
 
 ```shell
-pip install -r requirements-wildcodebench.txt
+pip install -r https://raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/requirements.txt
 ```
 
 Then, run the evaluation:
 
 ```shell
 wildcode.evaluate --dataset [wildcodebench] --samples samples.jsonl
 ```
@@ -222,23 +225,22 @@
 
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Asserting the groundtruth...
 Expected outputs computed in 1200.0 seconds
 Reading samples...
-1047it [00:00, 1901.64it/s]
+1140it [00:00, 1901.64it/s]
 Evaluating samples...
-100%|██████████████████████████████████████████| 1047/1047 [19:53<00:00, 6.75it/s]
-Base
-{'pass@1': 0.548}
+100%|██████████████████████████████████████████| 1140/1140 [19:53<00:00, 6.75it/s]
+wildcodebench
+{'pass@1': 0.568}
 ```
 
-- `Base` is the `pass@k` for the original HumanEval
-- The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
+- The "k" includes `[1, 5, 10]` where k values `<=` the sample size will be used
 - A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
 
 <details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
 <div>
 
 If you do greedy decoding where there is only one sample for each task, the evaluation should take just a few seconds.
 When running 1 sample x 964 tasks x all tests, it can take around ??-?? minutes by using `--parallel 64` and `--test-details`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.3.0.dev0 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.4.0 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
@@ -57,67 +57,67 @@
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
 ### Code Generation To generate code samples from a model, you can use the
 following command: ```shell wildcode.generate --model [model_name] --dataset
-wildcodebench --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] -
--resume --backend [vllm|hf|openai] ``` The generated code samples will be
+[wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples]
+--resume --backend [vllm|hf|openai] ``` The generated code samples will be
 stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-
 [n_samples].jsonl`. ð¤ Structure of `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
-is the ground-truth implementation (re-implemented to fix bugs in HumanEval) +
-`test` is the `unittest` test case
+is the ground-truth implementation + `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
 [temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
-`get_[human_eval|mbpp]_plus()` > 2. `solution` (optional): Self-contained
-solution (usually including the prompt) > * Example: `{"task_id": "HumanEval/
-?", "solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated
-text may not be compilable code for including natural language lines or
-incomplete extra code. We provide a tool namely `wildcode.sanitize` to clean up
-the code: ```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize
---samples samples.jsonl # Sanitized code will be produced to `samples-
-sanitized.jsonl` # ð¡ If you are storing codes in directories:
-wildcode.sanitize --samples /path/to/vicuna-[??]b_temp_[??] # Sanitized code
-will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ð
-Checking the compilability of post-processed code:: click to expand ::
+`get_wildcodebench()` > 2. `solution` (optional): Self-contained solution
+(usually including the prompt) > * Example: `{"task_id": "WildCodeBench/?",
+"solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated text
+may not be compilable code for including natural language lines or incomplete
+extra code. We provide a tool namely `wildcode.sanitize` to clean up the code:
+```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize --samples
+samples.jsonl # Sanitized code will be produced to `samples-sanitized.jsonl` #
+ð¡ If you are storing codes in directories: wildcode.sanitize --samples /
+path/to/vicuna-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/
+vicuna-[??]b_temp_[??]-sanitized` ``` ð Checking the compilability of post-
+processed code:: click to expand ::
 To double-check the post-processing results, you can use `wildcode.syncheck` to
 check the code validity before and after sanitization, which will print
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
 ### Code Evaluation You are strongly recommended to use a sandbox such as
-[docker](https://docs.docker.com/get-docker/): ```shell docker run -v $(pwd):/
-app terryzho/wildcode:latest --dataset [wildcodebench] --samples samples.jsonl
-``` ...Or if you want to try it locally regardless of the risks â ï¸: First,
-install the dependencies for WildCodeBench: ```shell pip install -
-r requirements-wildcodebench.txt ``` Then, run the evaluation: ```shell
-wildcode.evaluate --dataset [wildcodebench] --samples samples.jsonl ``` >
-[!Tip] > > Do you use a very slow machine? > > LLM solutions are regarded as
-**failed** on timeout (and OOM etc.). > Specifically, we set the dynamic
-timeout based on the ground-truth solution's runtime. > > Additionally, you are
-**NOT** encouraged to make your test-bed over stressed while running
-evaluation. > For example, using `--parallel 64` on a 4-core machine or doing
-something else during evaluation are bad ideas... â¨ï¸ More command-line
-flags :: click to expand ::
+[docker](https://docs.docker.com/get-docker/): ```shell # mount the current
+directory to the container docker run -v $(pwd) terryzho/wildcode:latest --
+dataset wildcodebench --samples samples.jsonl # ...Or locally â ï¸
+wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ``` ...Or if
+you want to try it locally regardless of the risks â ï¸: First, install the
+dependencies for WildCodeBench: ```shell pip install -r https://
+raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/
+requirements.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
+dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
+very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
+OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
+solution's runtime. > > Additionally, you are **NOT** encouraged to make your
+test-bed over stressed while running evaluation. > For example, using `--
+parallel 64` on a 4-core machine or doing something else during evaluation are
+bad ideas... â¨ï¸ More command-line flags :: click to expand ::
 * `--parallel`: by default half of the cores
 The output should be like (below is GPT-4 greedy decoding example): ```
 Asserting the groundtruth... Expected outputs computed in 1200.0 seconds
-Reading samples... 1047it [00:00, 1901.64it/s] Evaluating samples...
+Reading samples... 1140it [00:00, 1901.64it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
-1047/1047 [19:53<00:00, 6.75it/s] Base {'pass@1': 0.548} ``` - `Base` is the
-`pass@k` for the original HumanEval - The "k" includes `[1, 10, 100]` where k
-values `<=` the sample size will be used - A cache file named like
-`samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
-ð¤ How long it would take? :: click to expand ::
+1140/1140 [19:53<00:00, 6.75it/s] wildcodebench {'pass@1': 0.568} ``` - The "k"
+includes `[1, 5, 10]` where k values `<=` the sample size will be used - A
+cache file named like `samples_eval_results.jsonl` will be cached. Remove it to
+re-run the evaluation ð¤ How long it would take? :: click to expand ::
 If you do greedy decoding where there is only one sample for each task, the
 evaluation should take just a few seconds. When running 1 sample x 964 tasks x
 all tests, it can take around ??-?? minutes by using `--parallel 64` and `--
 test-details`. Here are some tips to speed up the evaluation: * Use `--parallel
 $(nproc)` * Use our pre-evaluated results (see [LLM-generated code](#-LLM-
 generated-code))
 ## Failure Inspection You can inspect the failed samples by using the following
```

### Comparing `wild_code-0.3.0.dev0/README.md` & `wild_code-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -85,38 +85,38 @@
 </details>
 
 ### Code Generation
 
 To generate code samples from a model, you can use the following command:
 
 ```shell
-wildcode.generate --model [model_name] --dataset wildcodebench --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
+wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
 ```
 The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
 * `entry_point` is the name of the function
 * `prompt` is the function signature with docstring
 * `instruction` is the instruction for the task completion
-+ `canonical_solution` is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
++ `canonical_solution` is the ground-truth implementation
 + `test` is the `unittest` test case
 
 </div>
 </details>
 
 > [!Note]
 >
 > **Expected Schema of `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`**
 >
-> 1. `task_id`: Task ID, which are the keys of `get_[human_eval|mbpp]_plus()`
+> 1. `task_id`: Task ID, which are the keys of `get_wildcodebench()`
 > 2. `solution` (optional): Self-contained solution (usually including the prompt)
->    * Example: `{"task_id": "HumanEval/?", "solution": "def f():\n    return 1"}`
+>    * Example: `{"task_id": "WildCodeBench/?", "solution": "def f():\n    return 1"}`
 
 ### Code Post-processing
 
 LLM-generated text may not be compilable code for including natural language lines or incomplete extra code.
 We provide a tool namely `wildcode.sanitize` to clean up the code:
 
 ```shell
@@ -147,23 +147,26 @@
 
 
 ### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
-docker run -v $(pwd):/app terryzho/wildcode:latest --dataset [wildcodebench] --samples samples.jsonl
+# mount the current directory to the container
+docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl
+# ...Or locally ⚠️
+wildcode.evaluate --dataset wildcodebench --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
 
 ```shell
-pip install -r requirements-wildcodebench.txt
+pip install -r https://raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/requirements.txt
 ```
 
 Then, run the evaluation:
 
 ```shell
 wildcode.evaluate --dataset [wildcodebench] --samples samples.jsonl
 ```
@@ -188,23 +191,22 @@
 
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Asserting the groundtruth...
 Expected outputs computed in 1200.0 seconds
 Reading samples...
-1047it [00:00, 1901.64it/s]
+1140it [00:00, 1901.64it/s]
 Evaluating samples...
-100%|██████████████████████████████████████████| 1047/1047 [19:53<00:00, 6.75it/s]
-Base
-{'pass@1': 0.548}
+100%|██████████████████████████████████████████| 1140/1140 [19:53<00:00, 6.75it/s]
+wildcodebench
+{'pass@1': 0.568}
 ```
 
-- `Base` is the `pass@k` for the original HumanEval
-- The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
+- The "k" includes `[1, 5, 10]` where k values `<=` the sample size will be used
 - A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
 
 <details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
 <div>
 
 If you do greedy decoding where there is only one sample for each task, the evaluation should take just a few seconds.
 When running 1 sample x 964 tasks x all tests, it can take around ??-?? minutes by using `--parallel 64` and `--test-details`.
```

#### html2text {}

```diff
@@ -42,67 +42,67 @@
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
 ### Code Generation To generate code samples from a model, you can use the
 following command: ```shell wildcode.generate --model [model_name] --dataset
-wildcodebench --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] -
--resume --backend [vllm|hf|openai] ``` The generated code samples will be
+[wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples]
+--resume --backend [vllm|hf|openai] ``` The generated code samples will be
 stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-
 [n_samples].jsonl`. ð¤ Structure of `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
-is the ground-truth implementation (re-implemented to fix bugs in HumanEval) +
-`test` is the `unittest` test case
+is the ground-truth implementation + `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
 [temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
-`get_[human_eval|mbpp]_plus()` > 2. `solution` (optional): Self-contained
-solution (usually including the prompt) > * Example: `{"task_id": "HumanEval/
-?", "solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated
-text may not be compilable code for including natural language lines or
-incomplete extra code. We provide a tool namely `wildcode.sanitize` to clean up
-the code: ```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize
---samples samples.jsonl # Sanitized code will be produced to `samples-
-sanitized.jsonl` # ð¡ If you are storing codes in directories:
-wildcode.sanitize --samples /path/to/vicuna-[??]b_temp_[??] # Sanitized code
-will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ð
-Checking the compilability of post-processed code:: click to expand ::
+`get_wildcodebench()` > 2. `solution` (optional): Self-contained solution
+(usually including the prompt) > * Example: `{"task_id": "WildCodeBench/?",
+"solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated text
+may not be compilable code for including natural language lines or incomplete
+extra code. We provide a tool namely `wildcode.sanitize` to clean up the code:
+```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize --samples
+samples.jsonl # Sanitized code will be produced to `samples-sanitized.jsonl` #
+ð¡ If you are storing codes in directories: wildcode.sanitize --samples /
+path/to/vicuna-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/
+vicuna-[??]b_temp_[??]-sanitized` ``` ð Checking the compilability of post-
+processed code:: click to expand ::
 To double-check the post-processing results, you can use `wildcode.syncheck` to
 check the code validity before and after sanitization, which will print
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
 ### Code Evaluation You are strongly recommended to use a sandbox such as
-[docker](https://docs.docker.com/get-docker/): ```shell docker run -v $(pwd):/
-app terryzho/wildcode:latest --dataset [wildcodebench] --samples samples.jsonl
-``` ...Or if you want to try it locally regardless of the risks â ï¸: First,
-install the dependencies for WildCodeBench: ```shell pip install -
-r requirements-wildcodebench.txt ``` Then, run the evaluation: ```shell
-wildcode.evaluate --dataset [wildcodebench] --samples samples.jsonl ``` >
-[!Tip] > > Do you use a very slow machine? > > LLM solutions are regarded as
-**failed** on timeout (and OOM etc.). > Specifically, we set the dynamic
-timeout based on the ground-truth solution's runtime. > > Additionally, you are
-**NOT** encouraged to make your test-bed over stressed while running
-evaluation. > For example, using `--parallel 64` on a 4-core machine or doing
-something else during evaluation are bad ideas... â¨ï¸ More command-line
-flags :: click to expand ::
+[docker](https://docs.docker.com/get-docker/): ```shell # mount the current
+directory to the container docker run -v $(pwd) terryzho/wildcode:latest --
+dataset wildcodebench --samples samples.jsonl # ...Or locally â ï¸
+wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ``` ...Or if
+you want to try it locally regardless of the risks â ï¸: First, install the
+dependencies for WildCodeBench: ```shell pip install -r https://
+raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/
+requirements.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
+dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
+very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
+OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
+solution's runtime. > > Additionally, you are **NOT** encouraged to make your
+test-bed over stressed while running evaluation. > For example, using `--
+parallel 64` on a 4-core machine or doing something else during evaluation are
+bad ideas... â¨ï¸ More command-line flags :: click to expand ::
 * `--parallel`: by default half of the cores
 The output should be like (below is GPT-4 greedy decoding example): ```
 Asserting the groundtruth... Expected outputs computed in 1200.0 seconds
-Reading samples... 1047it [00:00, 1901.64it/s] Evaluating samples...
+Reading samples... 1140it [00:00, 1901.64it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
-1047/1047 [19:53<00:00, 6.75it/s] Base {'pass@1': 0.548} ``` - `Base` is the
-`pass@k` for the original HumanEval - The "k" includes `[1, 10, 100]` where k
-values `<=` the sample size will be used - A cache file named like
-`samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
-ð¤ How long it would take? :: click to expand ::
+1140/1140 [19:53<00:00, 6.75it/s] wildcodebench {'pass@1': 0.568} ``` - The "k"
+includes `[1, 5, 10]` where k values `<=` the sample size will be used - A
+cache file named like `samples_eval_results.jsonl` will be cached. Remove it to
+re-run the evaluation ð¤ How long it would take? :: click to expand ::
 If you do greedy decoding where there is only one sample for each task, the
 evaluation should take just a few seconds. When running 1 sample x 964 tasks x
 all tests, it can take around ??-?? minutes by using `--parallel 64` and `--
 test-details`. Here are some tips to speed up the evaluation: * Use `--parallel
 $(nproc)` * Use our pre-evaluated results (see [LLM-generated code](#-LLM-
 generated-code))
 ## Failure Inspection You can inspect the failed samples by using the following
```

### Comparing `wild_code-0.3.0.dev0/release.sh` & `wild_code-0.4.0/release.sh`

 * *Files 14% similar despite different names*

```diff
@@ -18,20 +18,19 @@
   exit 1
 fi
 
 export PYTHONPATH=$PWD pytest tests
 
 git tag $version
 
-# # docker build
-# docker build . -t terryzho/wildcode:$version
-# docker tag terryzho/wildcode:$version terryzho/wildcode:latest
-# docker push terryzho/wildcode:$version
-# docker push terryzho/wildcode:latest
+# docker build
+docker build . -t terryzho/wildcode:$version
+docker tag terryzho/wildcode:$version terryzho/wildcode:latest
+docker push terryzho/wildcode:$version
+docker push terryzho/wildcode:latest
 
 rm -rf dist
 python3 -m build
-python3 -m twine upload --skip-existing --verbose dist/*
+python3 -m twine upload dist/*
 
-# git push
 git push
 git push --tags
```

### Comparing `wild_code-0.3.0.dev0/run.sh` & `wild_code-0.4.0/run.sh`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #Qwen/CodeQwen1.5-7B-Chat
 #gpt-3.5-turbo-0125
 #deepseek-ai/deepseek-coder-33b-instruct
 #bigcode/starcoder2-15b-instruct-v0.1
 #bigcode/starcoder2-15b
 #gpt-4-turbo-2024-04-09
-BS=10
+BS=5
 DATASET=wildcodebench
 # MODELS=(Qwen/CodeQwen1.5-7B-Chat)
 # BACKEND=vllm
-MODELS=(gpt-3.5-turbo-0125)
+MODELS=(gpt-4-turbo-2024-04-09)
 BACKEND=openai
 TEMPS=(0)
 N_SAMPLESES=(1)
 
 for MODEL in ${MODELS[@]}; do
   for TEMP in ${TEMPS[@]}; do
     for N_SAMPLES in ${N_SAMPLESES[@]}; do
@@ -32,11 +32,11 @@
         MODEL=$ORG--$MODEL
       fi
 
       SAMPLE_FILE=$MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES.jsonl
       python -m wildcode.sanitize --samples $SAMPLE_FILE
       rm -rf $MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES-sanitized_eval_results.json
       python -m wildcode.evaluate --dataset $DATASET --samples $MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES-sanitized.jsonl
-      # python -m wildcode.inspect --dataset $DATASET --eval-results $MODEL-$DATASET-$TEMP-$N_SAMPLES-sanitized_eval_results.json --in-place
+      # python -m wildcode.inspect --dataset $DATASET --eval-results $MODEL--$DATASET--$BACKEND-$TEMP-$N_SAMPLES-sanitized_eval_results.json --in-place
     done
   done
 done
```

### Comparing `wild_code-0.3.0.dev0/setup.cfg` & `wild_code-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/tests/test_legacy_sanitizer.py` & `wild_code-0.4.0/tests/test_legacy_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/tests/test_treesitter_sanitizer.py` & `wild_code-0.4.0/tests/test_treesitter_sanitizer.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/wild_code.egg-info/PKG-INFO` & `wild_code-0.4.0/wild_code.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-code
-Version: 0.3.0.dev0
+Version: 0.4.0
 Summary: "WildCode: A minimal viable package to evaluate code generation with realistic constraints in the wild"
 Home-page: https://github.com/bigcode-project/wild-code
 License: Apache-2.0
 Platform: any
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -119,38 +119,38 @@
 </details>
 
 ### Code Generation
 
 To generate code samples from a model, you can use the following command:
 
 ```shell
-wildcode.generate --model [model_name] --dataset wildcodebench --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
+wildcode.generate --model [model_name] --dataset [wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] --resume --backend [vllm|hf|openai]
 ```
 The generated code samples will be stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`.
 
 <details><summary>🤔 Structure of `problem`? <i>:: click to expand ::</i></summary>
 <div>
 
 * `task_id` is the identifier string for the task
 * `entry_point` is the name of the function
 * `prompt` is the function signature with docstring
 * `instruction` is the instruction for the task completion
-+ `canonical_solution` is the ground-truth implementation (re-implemented to fix bugs in HumanEval)
++ `canonical_solution` is the ground-truth implementation
 + `test` is the `unittest` test case
 
 </div>
 </details>
 
 > [!Note]
 >
 > **Expected Schema of `[model_name]--wildcodebench--[backend]-[temp]-[n_samples].jsonl`**
 >
-> 1. `task_id`: Task ID, which are the keys of `get_[human_eval|mbpp]_plus()`
+> 1. `task_id`: Task ID, which are the keys of `get_wildcodebench()`
 > 2. `solution` (optional): Self-contained solution (usually including the prompt)
->    * Example: `{"task_id": "HumanEval/?", "solution": "def f():\n    return 1"}`
+>    * Example: `{"task_id": "WildCodeBench/?", "solution": "def f():\n    return 1"}`
 
 ### Code Post-processing
 
 LLM-generated text may not be compilable code for including natural language lines or incomplete extra code.
 We provide a tool namely `wildcode.sanitize` to clean up the code:
 
 ```shell
@@ -181,23 +181,26 @@
 
 
 ### Code Evaluation
 
 You are strongly recommended to use a sandbox such as [docker](https://docs.docker.com/get-docker/):
 
 ```shell
-docker run -v $(pwd):/app terryzho/wildcode:latest --dataset [wildcodebench] --samples samples.jsonl
+# mount the current directory to the container
+docker run -v $(pwd) terryzho/wildcode:latest --dataset wildcodebench --samples samples.jsonl
+# ...Or locally ⚠️
+wildcode.evaluate --dataset wildcodebench --samples samples.jsonl
 ```
 
 ...Or if you want to try it locally regardless of the risks ⚠️:
 
 First, install the dependencies for WildCodeBench:
 
 ```shell
-pip install -r requirements-wildcodebench.txt
+pip install -r https://raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/requirements.txt
 ```
 
 Then, run the evaluation:
 
 ```shell
 wildcode.evaluate --dataset [wildcodebench] --samples samples.jsonl
 ```
@@ -222,23 +225,22 @@
 
 The output should be like (below is GPT-4 greedy decoding example):
 
 ```
 Asserting the groundtruth...
 Expected outputs computed in 1200.0 seconds
 Reading samples...
-1047it [00:00, 1901.64it/s]
+1140it [00:00, 1901.64it/s]
 Evaluating samples...
-100%|██████████████████████████████████████████| 1047/1047 [19:53<00:00, 6.75it/s]
-Base
-{'pass@1': 0.548}
+100%|██████████████████████████████████████████| 1140/1140 [19:53<00:00, 6.75it/s]
+wildcodebench
+{'pass@1': 0.568}
 ```
 
-- `Base` is the `pass@k` for the original HumanEval
-- The "k" includes `[1, 10, 100]` where k values `<=` the sample size will be used
+- The "k" includes `[1, 5, 10]` where k values `<=` the sample size will be used
 - A cache file named like `samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
 
 <details><summary>🤔 How long it would take? <i>:: click to expand ::</i></summary>
 <div>
 
 If you do greedy decoding where there is only one sample for each task, the evaluation should take just a few seconds.
 When running 1 sample x 964 tasks x all tests, it can take around ??-?? minutes by using `--parallel 64` and `--test-details`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wild-code Version: 0.3.0.dev0 Summary: "WildCode: A
+Metadata-Version: 2.1 Name: wild-code Version: 0.4.0 Summary: "WildCode: A
 minimal viable package to evaluate code generation with realistic constraints
 in the wild" Home-page: https://github.com/bigcode-project/wild-code License:
 Apache-2.0 Platform: any Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: Apache Software License Requires-Python: >=3.8 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: wget>=3.2 Requires-
 Dist: tempdir>=0.7.1 Requires-Dist: multipledispatch>=0.6.0 Requires-Dist:
@@ -57,67 +57,67 @@
 ```shell pip install "git+https://github.com/bigcode-project/wild-code.git" --
 upgrade ```
 â¬ Using WildCode as a local repo? :: click to expand ::
 ```shell git clone https://github.com/bigcode-project/wild-code.git cd wild-
 code export PYTHONPATH=$PYTHONPATH:$(pwd) pip install -e . ```
 ### Code Generation To generate code samples from a model, you can use the
 following command: ```shell wildcode.generate --model [model_name] --dataset
-wildcodebench --greedy --bs [bs] --temperature [temp] --n_samples [n_samples] -
--resume --backend [vllm|hf|openai] ``` The generated code samples will be
+[wildcodebench] --greedy --bs [bs] --temperature [temp] --n_samples [n_samples]
+--resume --backend [vllm|hf|openai] ``` The generated code samples will be
 stored in a file named `[model_name]--wildcodebench--[backend]-[temp]-
 [n_samples].jsonl`. ð¤ Structure of `problem`? :: click to expand ::
 * `task_id` is the identifier string for the task * `entry_point` is the name
 of the function * `prompt` is the function signature with docstring *
 `instruction` is the instruction for the task completion + `canonical_solution`
-is the ground-truth implementation (re-implemented to fix bugs in HumanEval) +
-`test` is the `unittest` test case
+is the ground-truth implementation + `test` is the `unittest` test case
 > [!Note] > > **Expected Schema of `[model_name]--wildcodebench--[backend]-
 [temp]-[n_samples].jsonl`** > > 1. `task_id`: Task ID, which are the keys of
-`get_[human_eval|mbpp]_plus()` > 2. `solution` (optional): Self-contained
-solution (usually including the prompt) > * Example: `{"task_id": "HumanEval/
-?", "solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated
-text may not be compilable code for including natural language lines or
-incomplete extra code. We provide a tool namely `wildcode.sanitize` to clean up
-the code: ```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize
---samples samples.jsonl # Sanitized code will be produced to `samples-
-sanitized.jsonl` # ð¡ If you are storing codes in directories:
-wildcode.sanitize --samples /path/to/vicuna-[??]b_temp_[??] # Sanitized code
-will be produced to `/path/to/vicuna-[??]b_temp_[??]-sanitized` ``` ð
-Checking the compilability of post-processed code:: click to expand ::
+`get_wildcodebench()` > 2. `solution` (optional): Self-contained solution
+(usually including the prompt) > * Example: `{"task_id": "WildCodeBench/?",
+"solution": "def f():\n return 1"}` ### Code Post-processing LLM-generated text
+may not be compilable code for including natural language lines or incomplete
+extra code. We provide a tool namely `wildcode.sanitize` to clean up the code:
+```shell # ð¡ If you are storing codes in jsonl: wildcode.sanitize --samples
+samples.jsonl # Sanitized code will be produced to `samples-sanitized.jsonl` #
+ð¡ If you are storing codes in directories: wildcode.sanitize --samples /
+path/to/vicuna-[??]b_temp_[??] # Sanitized code will be produced to `/path/to/
+vicuna-[??]b_temp_[??]-sanitized` ``` ð Checking the compilability of post-
+processed code:: click to expand ::
 To double-check the post-processing results, you can use `wildcode.syncheck` to
 check the code validity before and after sanitization, which will print
 erroneous code snippets and why they are wrong: ```shell # ð¡ If you are
 storing codes in jsonl: wildcode.syncheck --samples samples.jsonl --dataset
 [wildcodebench] # ð¡ If you are storing codes in directories:
 wildcode.syncheck --samples /path/to/vicuna-[??]b_temp_[??] --dataset
 [wildcodebench] ```
 ### Code Evaluation You are strongly recommended to use a sandbox such as
-[docker](https://docs.docker.com/get-docker/): ```shell docker run -v $(pwd):/
-app terryzho/wildcode:latest --dataset [wildcodebench] --samples samples.jsonl
-``` ...Or if you want to try it locally regardless of the risks â ï¸: First,
-install the dependencies for WildCodeBench: ```shell pip install -
-r requirements-wildcodebench.txt ``` Then, run the evaluation: ```shell
-wildcode.evaluate --dataset [wildcodebench] --samples samples.jsonl ``` >
-[!Tip] > > Do you use a very slow machine? > > LLM solutions are regarded as
-**failed** on timeout (and OOM etc.). > Specifically, we set the dynamic
-timeout based on the ground-truth solution's runtime. > > Additionally, you are
-**NOT** encouraged to make your test-bed over stressed while running
-evaluation. > For example, using `--parallel 64` on a 4-core machine or doing
-something else during evaluation are bad ideas... â¨ï¸ More command-line
-flags :: click to expand ::
+[docker](https://docs.docker.com/get-docker/): ```shell # mount the current
+directory to the container docker run -v $(pwd) terryzho/wildcode:latest --
+dataset wildcodebench --samples samples.jsonl # ...Or locally â ï¸
+wildcode.evaluate --dataset wildcodebench --samples samples.jsonl ``` ...Or if
+you want to try it locally regardless of the risks â ï¸: First, install the
+dependencies for WildCodeBench: ```shell pip install -r https://
+raw.githubusercontent.com/bigcode-project/wildcodebench-annotation/main/
+requirements.txt ``` Then, run the evaluation: ```shell wildcode.evaluate --
+dataset [wildcodebench] --samples samples.jsonl ``` > [!Tip] > > Do you use a
+very slow machine? > > LLM solutions are regarded as **failed** on timeout (and
+OOM etc.). > Specifically, we set the dynamic timeout based on the ground-truth
+solution's runtime. > > Additionally, you are **NOT** encouraged to make your
+test-bed over stressed while running evaluation. > For example, using `--
+parallel 64` on a 4-core machine or doing something else during evaluation are
+bad ideas... â¨ï¸ More command-line flags :: click to expand ::
 * `--parallel`: by default half of the cores
 The output should be like (below is GPT-4 greedy decoding example): ```
 Asserting the groundtruth... Expected outputs computed in 1200.0 seconds
-Reading samples... 1047it [00:00, 1901.64it/s] Evaluating samples...
+Reading samples... 1140it [00:00, 1901.64it/s] Evaluating samples...
 100%|ââââââââââââââââââââââââââââââââââââââââââ|
-1047/1047 [19:53<00:00, 6.75it/s] Base {'pass@1': 0.548} ``` - `Base` is the
-`pass@k` for the original HumanEval - The "k" includes `[1, 10, 100]` where k
-values `<=` the sample size will be used - A cache file named like
-`samples_eval_results.jsonl` will be cached. Remove it to re-run the evaluation
-ð¤ How long it would take? :: click to expand ::
+1140/1140 [19:53<00:00, 6.75it/s] wildcodebench {'pass@1': 0.568} ``` - The "k"
+includes `[1, 5, 10]` where k values `<=` the sample size will be used - A
+cache file named like `samples_eval_results.jsonl` will be cached. Remove it to
+re-run the evaluation ð¤ How long it would take? :: click to expand ::
 If you do greedy decoding where there is only one sample for each task, the
 evaluation should take just a few seconds. When running 1 sample x 964 tasks x
 all tests, it can take around ??-?? minutes by using `--parallel 64` and `--
 test-details`. Here are some tips to speed up the evaluation: * Use `--parallel
 $(nproc)` * Use our pre-evaluated results (see [LLM-generated code](#-LLM-
 generated-code))
 ## Failure Inspection You can inspect the failed samples by using the following
```

### Comparing `wild_code-0.3.0.dev0/wild_code.egg-info/SOURCES.txt` & `wild_code-0.4.0/wild_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/wildcode/data/utils.py` & `wild_code-0.4.0/wildcode/data/utils.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/wildcode/eval/__init__.py` & `wild_code-0.4.0/wildcode/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/wildcode/eval/utils.py` & `wild_code-0.4.0/wildcode/eval/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,7 +174,10 @@
 
     faulthandler.disable()
 
     import builtins
 
     builtins.exit = None
     builtins.quit = None
+
+    import matplotlib.pyplot as plt
+    plt.close('all')
```

### Comparing `wild_code-0.3.0.dev0/wildcode/evaluate.py` & `wild_code-0.4.0/wildcode/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from warnings import warn
 
 import numpy as np
 from termcolor import cprint
 from tqdm import tqdm
 
 from wildcode.data import (
-    get_wild_code_bench,
-    get_wild_code_bench_hash,
+    get_wildcodebench,
+    get_wildcodebench_hash,
     load_solutions,
 )
 from wildcode.data.utils import CACHE_DIR
 from wildcode.eval import (
     PASS,
     compatible_eval_result,
     estimate_pass_at_k,
@@ -48,15 +48,15 @@
     print("\nAsserting the groundtruth...")
     tbegin = time.time()
     expected_time = {}
     for task_id, problem in tqdm(problems.items()):
         expected_time[task_id] = trusted_exec(
             problem["prompt"] + "\n" + problem["clean_canonical_solution"],
             problem["test"],
-            problem["entry_point"],
+            problem["task_id"],
         )
     print(f"Expected outputs computed in {time.time() - tbegin:.2f}s")
     
     with open(cache_file, "wb") as f:
         pickle.dump(expected_time, f)
 
     return expected_time
@@ -107,16 +107,16 @@
         print(f"Load from previous results from {result_path}")
         with open(result_path, "r") as f:
             results = json.load(f)
 
         results = compatible_eval_result(results)
     else:
         if flags.dataset == "wildcodebench":
-            problems = get_wild_code_bench()
-            dataset_hash = get_wild_code_bench_hash()       
+            problems = get_wildcodebench()
+            dataset_hash = get_wildcodebench_hash()       
             expected_time = get_groundtruth(problems, dataset_hash, flags.check_gt_only)
         
         if flags.check_gt_only:
             return
         
         results = {
             "date": datetime.now().strftime("%Y-%m-%d %H:%M"),
@@ -203,15 +203,15 @@
         bc = sum([r["status"] == PASS for r in res])
         base_correct.append(bc)
 
     base_correct = np.array(base_correct)
 
     pass_at_k = {
         f"pass@{k}": estimate_pass_at_k(total, base_correct, k).mean()
-        for k in [1, 10, 100]
+        for k in [1, 5, 10]
         if total.min() >= k
     }
     cprint(f"{flags.dataset}", "green")
     for k, v in pass_at_k.items():
         cprint(f"{k}:\t{v:.3f}", "green")
 
     # save results
```

### Comparing `wild_code-0.3.0.dev0/wildcode/gen/__init__.py` & `wild_code-0.4.0/wildcode/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/wildcode/gen/util/anthropic_request.py` & `wild_code-0.4.0/wildcode/gen/util/anthropic_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/wildcode/gen/util/openai_request.py` & `wild_code-0.4.0/wildcode/gen/util/openai_request.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/wildcode/generate.py` & `wild_code-0.4.0/wildcode/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,17 @@
         TextColumn(f"{dataset} •" + "[progress.percentage]{task.percentage:>3.0f}%"),
         BarColumn(),
         MofNCompleteColumn(),
         TextColumn("•"),
         TimeElapsedColumn(),
     ) as p:
         if dataset == "wildcodebench":
-            from wildcode.data import get_wild_code_bench, write_jsonl
+            from wildcode.data import get_wildcodebench, write_jsonl
 
-            dataset = get_wild_code_bench()
+            dataset = get_wildcodebench()
 
         # create save_path if it doesn't exist, e.g., a/b.jsonl
         dirname = os.path.dirname(save_path)
         if not os.path.exists(dirname) and dirname != "":
             os.makedirs(dirname)
         for task_id, task in p.track(dataset.items()):
             if id_range is not None:
```

### Comparing `wild_code-0.3.0.dev0/wildcode/inspect.py` & `wild_code-0.4.0/wildcode/inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from wildcode.data import get_wild_code_bench
+from wildcode.data import get_wildcodebench
 import sys
 import os
 import shutil
 import json
 import argparse
 
 def inspection(args):
@@ -17,15 +17,15 @@
     """
     path = os.path.join("inspect", args.eval_results.split("/")[-1].replace(".json", ""))
     if args.in_place:
         shutil.rmtree(path, ignore_errors=True)
     if not os.path.exists(path):
         os.makedirs(path)
     if args.dataset == "wildcodebench":
-        problems = get_wild_code_bench()
+        problems = get_wildcodebench()
 
     eval_results = json.load(open(args.eval_results, "r"))
     for task_id, results in eval_results["eval"].items():
         if all(result["status"] == "pass" for result in results):
             continue
         task_path = os.path.join(path, task_id)
         if not os.path.exists(task_path):
```

### Comparing `wild_code-0.3.0.dev0/wildcode/lecacy_sanitize.py` & `wild_code-0.4.0/wildcode/lecacy_sanitize.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pathlib
 import re
 from typing import List, Optional
 
 from tqdm import tqdm
 
 from wildcode.data import (
-    get_wild_code_bench,
+    get_wildcodebench,
     load_solutions,
     write_directory,
     write_jsonl,
 )
 from wildcode.syncheck import syntax_check
 
 
@@ -120,15 +120,15 @@
     eofs: List[str] = [],
     inplace: bool = False,
     rm_prefix_lines: str = None,
     debug_task: str = None,
 ):
     # task_id -> entry_point
     entry_point = {}
-    dataset = {**get_wild_code_bench()}
+    dataset = {**get_wildcodebench()}
 
     for task_id, problem in dataset.items():
         entry_point[task_id] = problem["entry_point"]
 
     # make a new folder with "-sanitized" suffix
     is_folder = os.path.isdir(samples)
     target_path = pathlib.Path(samples)
```

### Comparing `wild_code-0.3.0.dev0/wildcode/model.py` & `wild_code-0.4.0/wildcode/model.py`

 * *Files identical despite different names*

### Comparing `wild_code-0.3.0.dev0/wildcode/sanitize.py` & `wild_code-0.4.0/wildcode/sanitize.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Dict, Generator, List, Optional, Set, Tuple
 
 from tqdm import tqdm
 from tree_sitter import Node
 from tree_sitter_languages import get_parser
 
 from wildcode.data import (
-    get_wild_code_bench,
+    get_wildcodebench,
     load_solutions,
     write_directory,
     write_jsonl,
 )
 from wildcode.syncheck import syntax_check
 
 CLASS_TYPE = "class_definition"
@@ -181,15 +181,15 @@
 
 def script(
     samples: str, inplace: bool = False, debug_task: str = None
 ):
     # task_id -> entry_point
     entry_point = {}
     # merge two datasets
-    dataset = {**get_wild_code_bench()}
+    dataset = {**get_wildcodebench()}
 
     for task_id, problem in dataset.items():
         entry_point[task_id] = problem["entry_point"]
 
     # make a new folder with "-sanitized" suffix
     is_folder = os.path.isdir(samples)
     target_path = pathlib.Path(samples)
```

### Comparing `wild_code-0.3.0.dev0/wildcode/syncheck.py` & `wild_code-0.4.0/wildcode/syncheck.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 def script(
     samples: str, dataset: str, nsample_check: int = None, verbose: bool = False
 ):
     # List[Dict{"task_id", "solution"}]
     solutions = load_solutions(samples)
 
     if dataset == "wildcodebench":
-        from wildcode.data import get_wild_code_bench
+        from wildcode.data import get_wildcodebench
 
-        dataset = get_wild_code_bench()
+        dataset = get_wildcodebench()
         dataset_name = "WildCodeBench"
 
     print(colored(f"Dataset: {dataset_name}", "blue"))
 
     id2solutions = {}
     for solution in solutions:
         task_id = solution["task_id"]
```

