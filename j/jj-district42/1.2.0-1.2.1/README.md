# Comparing `tmp/jj-district42-1.2.0.tar.gz` & `tmp/jj_district42-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj-district42-1.2.0.tar", last modified: Fri Mar 22 14:26:43 2024, max compression
+gzip compressed data, was "jj_district42-1.2.1.tar", last modified: Sun May 12 14:00:58 2024, max compression
```

## Comparing `jj-district42-1.2.0.tar` & `jj_district42-1.2.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.219945 jj-district42-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-22 14:26:35.000000 jj-district42-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-22 14:26:43.219945 jj-district42-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-22 14:26:35.000000 jj-district42-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.207945 jj-district42-1.2.0/jj_district42/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.211945 jj-district42-1.2.0/jj_district42/history_request/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/history_request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/history_request/_history_request_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/history_request/_history_request_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/history_request/_history_request_substitutor.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/history_request/_history_request_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.211945 jj-district42-1.2.0/jj_district42/history_response/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/history_response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/history_response/_history_response_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/history_response/_history_response_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/history_response/_history_response_substitutor.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/history_response/_history_response_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.211945 jj-district42-1.2.0/jj_district42/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.211945 jj-district42-1.2.0/jj_district42/types/header_list/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/types/header_list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.211945 jj-district42-1.2.0/jj_district42/types/istr/
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/types/istr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.211945 jj-district42-1.2.0/jj_district42/types/param_list/
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/types/param_list/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.211945 jj-district42-1.2.0/jj_district42/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-22 14:26:35.000000 jj-district42-1.2.0/jj_district42/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.219945 jj-district42-1.2.0/jj_district42.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-03-22 14:26:43.000000 jj-district42-1.2.0/jj_district42.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-03-22 14:26:43.000000 jj-district42-1.2.0/jj_district42.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 14:26:43.000000 jj-district42-1.2.0/jj_district42.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-22 14:26:43.000000 jj-district42-1.2.0/jj_district42.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-22 14:26:43.000000 jj-district42-1.2.0/jj_district42.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-22 14:26:43.219945 jj-district42-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-03-22 14:26:35.000000 jj-district42-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.207945 jj-district42-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.215945 jj-district42-1.2.0/tests/history_request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_request/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_request/test_history_request_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_request/test_history_request_representor.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_request/test_history_request_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_request/test_history_request_substitutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_request/test_history_request_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_request/test_history_request_validator_headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_request/test_history_request_validator_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.215945 jj-district42-1.2.0/tests/history_response/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_response/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_response/test_history_response_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_response/test_history_response_representor.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_response/test_history_response_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_response/test_history_response_substitutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_response/test_history_response_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/history_response/test_history_response_validator_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.215945 jj-district42-1.2.0/tests/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.215945 jj-district42-1.2.0/tests/types/header_list/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/header_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/header_list/test_header_list_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/header_list/test_header_list_representor.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/header_list/test_header_list_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/header_list/test_header_list_substitutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/header_list/test_header_list_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.219945 jj-district42-1.2.0/tests/types/istr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/istr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/istr/test_istr_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/istr/test_istr_representor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/istr/test_istr_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/istr/test_istr_substitutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/istr/test_istr_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.219945 jj-district42-1.2.0/tests/types/param_list/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/param_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/param_list/test_param_list_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/param_list/test_param_list_representor.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/param_list/test_param_list_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/param_list/test_param_list_substitutor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/types/param_list/test_param_list_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:43.219945 jj-district42-1.2.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-22 14:26:35.000000 jj-district42-1.2.0/tests/utils/test_contains.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:58.004040 jj_district42-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 14:00:50.000000 jj_district42-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-12 14:00:58.004040 jj_district42-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-12 14:00:50.000000 jj_district42-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:57.996040 jj_district42-1.2.1/jj_district42/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:57.996040 jj_district42-1.2.1/jj_district42/history_request/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/history_request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/history_request/_history_request_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/history_request/_history_request_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/history_request/_history_request_substitutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/history_request/_history_request_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:57.996040 jj_district42-1.2.1/jj_district42/history_response/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/history_response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/history_response/_history_response_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/history_response/_history_response_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/history_response/_history_response_substitutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/history_response/_history_response_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:57.996040 jj_district42-1.2.1/jj_district42/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:57.996040 jj_district42-1.2.1/jj_district42/types/header_list/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/types/header_list/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:57.996040 jj_district42-1.2.1/jj_district42/types/istr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/types/istr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:57.996040 jj_district42-1.2.1/jj_district42/types/param_list/
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/types/param_list/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:57.996040 jj_district42-1.2.1/jj_district42/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-12 14:00:50.000000 jj_district42-1.2.1/jj_district42/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:58.004040 jj_district42-1.2.1/jj_district42.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-12 14:00:57.000000 jj_district42-1.2.1/jj_district42.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-12 14:00:57.000000 jj_district42-1.2.1/jj_district42.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:00:57.000000 jj_district42-1.2.1/jj_district42.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-12 14:00:57.000000 jj_district42-1.2.1/jj_district42.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-12 14:00:57.000000 jj_district42-1.2.1/jj_district42.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-12 14:00:58.004040 jj_district42-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-12 14:00:50.000000 jj_district42-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:57.992040 jj_district42-1.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:58.000040 jj_district42-1.2.1/tests/history_request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_request/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_request/test_history_request_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_request/test_history_request_representor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_request/test_history_request_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_request/test_history_request_substitutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_request/test_history_request_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_request/test_history_request_validator_headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_request/test_history_request_validator_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:58.000040 jj_district42-1.2.1/tests/history_response/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_response/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_response/test_history_response_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_response/test_history_response_representor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_response/test_history_response_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_response/test_history_response_substitutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_response/test_history_response_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/history_response/test_history_response_validator_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:58.000040 jj_district42-1.2.1/tests/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:58.000040 jj_district42-1.2.1/tests/types/header_list/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/header_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/header_list/test_header_list_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/header_list/test_header_list_representor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/header_list/test_header_list_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/header_list/test_header_list_substitutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/header_list/test_header_list_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:58.004040 jj_district42-1.2.1/tests/types/istr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/istr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/istr/test_istr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/istr/test_istr_representor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/istr/test_istr_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/istr/test_istr_substitutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/istr/test_istr_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:58.004040 jj_district42-1.2.1/tests/types/param_list/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/param_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/param_list/test_param_list_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/param_list/test_param_list_representor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/param_list/test_param_list_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/param_list/test_param_list_substitutor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/types/param_list/test_param_list_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:58.004040 jj_district42-1.2.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-12 14:00:50.000000 jj_district42-1.2.1/tests/utils/test_contains.py
```

### Comparing `jj-district42-1.2.0/LICENSE` & `jj_district42-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/PKG-INFO` & `jj_district42-1.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: jj-district42
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://github.com/jj-mock/jj-district42
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
-Project-URL: Docs, https://jj.vedro.io/docs/integrations/d42
+Project-URL: Docs, https://jj-mock.io/docs/integrations/d42
 Project-URL: GitHub, https://github.com/jj-mock/jj-district42
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `jj-district42-1.2.0/README.md` & `jj_district42-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/__init__.py` & `jj_district42-1.2.1/jj_district42/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/history_request/__init__.py` & `jj_district42-1.2.1/jj_district42/history_request/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/history_request/_history_request_generator.py` & `jj_district42-1.2.1/jj_district42/history_request/_history_request_generator.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/history_request/_history_request_schema.py` & `jj_district42-1.2.1/jj_district42/history_request/_history_request_schema.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/history_request/_history_request_substitutor.py` & `jj_district42-1.2.1/jj_district42/history_request/_history_request_substitutor.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/history_request/_history_request_validator.py` & `jj_district42-1.2.1/jj_district42/history_request/_history_request_validator.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/history_response/__init__.py` & `jj_district42-1.2.1/jj_district42/history_response/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/history_response/_history_response_generator.py` & `jj_district42-1.2.1/jj_district42/history_response/_history_response_generator.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/history_response/_history_response_schema.py` & `jj_district42-1.2.1/jj_district42/history_response/_history_response_schema.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/history_response/_history_response_substitutor.py` & `jj_district42-1.2.1/jj_district42/history_response/_history_response_substitutor.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/history_response/_history_response_validator.py` & `jj_district42-1.2.1/jj_district42/history_response/_history_response_validator.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/types/header_list/__init__.py` & `jj_district42-1.2.1/jj_district42/types/header_list/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/types/istr/__init__.py` & `jj_district42-1.2.1/jj_district42/types/istr/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/types/param_list/__init__.py` & `jj_district42-1.2.1/jj_district42/types/param_list/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42/utils/__init__.py` & `jj_district42-1.2.1/jj_district42/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/jj_district42.egg-info/PKG-INFO` & `jj_district42-1.2.1/jj_district42.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: jj-district42
-Version: 1.2.0
+Version: 1.2.1
 Home-page: https://github.com/jj-mock/jj-district42
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
-Project-URL: Docs, https://jj.vedro.io/docs/integrations/d42
+Project-URL: Docs, https://jj-mock.io/docs/integrations/d42
 Project-URL: GitHub, https://github.com/jj-mock/jj-district42
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `jj-district42-1.2.0/jj_district42.egg-info/SOURCES.txt` & `jj_district42-1.2.1/jj_district42.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/setup.cfg` & `jj_district42-1.2.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.0
+current_version = 1.2.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `jj-district42-1.2.0/setup.py` & `jj_district42-1.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="jj-district42",
-    version="1.2.0",
+    version="1.2.1",
     description="",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
     url="https://github.com/jj-mock/jj-district42",
     project_urls={
-        "Docs": "https://jj.vedro.io/docs/integrations/d42",
+        "Docs": "https://jj-mock.io/docs/integrations/d42",
         "GitHub": "https://github.com/jj-mock/jj-district42",
     },
     license="Apache-2.0",
     packages=find_packages(exclude=("tests",)),
     package_data={"jj_district42": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
```

### Comparing `jj-district42-1.2.0/tests/history_request/_utils.py` & `jj_district42-1.2.1/tests/history_request/_utils.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_request/test_history_request_representor.py` & `jj_district42-1.2.1/tests/history_request/test_history_request_representor.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_request/test_history_request_schema.py` & `jj_district42-1.2.1/tests/history_request/test_history_request_schema.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_request/test_history_request_substitutor.py` & `jj_district42-1.2.1/tests/history_request/test_history_request_substitutor.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_request/test_history_request_validator.py` & `jj_district42-1.2.1/tests/history_request/test_history_request_validator.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_request/test_history_request_validator_headers.py` & `jj_district42-1.2.1/tests/history_request/test_history_request_validator_headers.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_request/test_history_request_validator_params.py` & `jj_district42-1.2.1/tests/history_request/test_history_request_validator_params.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_response/_utils.py` & `jj_district42-1.2.1/tests/history_response/_utils.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_response/test_history_response_representor.py` & `jj_district42-1.2.1/tests/history_response/test_history_response_representor.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_response/test_history_response_schema.py` & `jj_district42-1.2.1/tests/history_response/test_history_response_schema.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_response/test_history_response_substitutor.py` & `jj_district42-1.2.1/tests/history_response/test_history_response_substitutor.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_response/test_history_response_validator.py` & `jj_district42-1.2.1/tests/history_response/test_history_response_validator.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/history_response/test_history_response_validator_headers.py` & `jj_district42-1.2.1/tests/history_response/test_history_response_validator_headers.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/types/header_list/test_header_list_substitutor.py` & `jj_district42-1.2.1/tests/types/header_list/test_header_list_substitutor.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/types/header_list/test_header_list_validator.py` & `jj_district42-1.2.1/tests/types/header_list/test_header_list_validator.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/types/istr/test_istr_representor.py` & `jj_district42-1.2.1/tests/types/istr/test_istr_representor.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/types/istr/test_istr_schema.py` & `jj_district42-1.2.1/tests/types/istr/test_istr_schema.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/types/istr/test_istr_substitutor.py` & `jj_district42-1.2.1/tests/types/istr/test_istr_substitutor.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/types/istr/test_istr_validator.py` & `jj_district42-1.2.1/tests/types/istr/test_istr_validator.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/types/param_list/test_param_list_substitutor.py` & `jj_district42-1.2.1/tests/types/param_list/test_param_list_substitutor.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/types/param_list/test_param_list_validator.py` & `jj_district42-1.2.1/tests/types/param_list/test_param_list_validator.py`

 * *Files identical despite different names*

### Comparing `jj-district42-1.2.0/tests/utils/test_contains.py` & `jj_district42-1.2.1/tests/utils/test_contains.py`

 * *Files identical despite different names*

