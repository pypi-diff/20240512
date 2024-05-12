# Comparing `tmp/py_alpaca_api-0.2.0.tar.gz` & `tmp/py_alpaca_api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.2.0.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.2.1.tar", max compression
```

## Comparing `py_alpaca_api-0.2.0.tar` & `py_alpaca_api-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.2.0/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0    14783 2024-05-11 04:26:53.113563 py_alpaca_api-0.2.0/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0     2225 2024-05-11 03:07:09.065209 py_alpaca_api-0.2.0/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0      453 2024-05-11 04:53:54.523003 py_alpaca_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 py_alpaca_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 00:31:44.448417 py_alpaca_api-0.2.1/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0    20957 2024-05-11 19:30:48.419299 py_alpaca_api-0.2.1/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0    10930 2024-05-11 13:09:02.198804 py_alpaca_api-0.2.1/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0      637 2024-05-11 19:39:17.689124 py_alpaca_api-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 py_alpaca_api-0.2.1/PKG-INFO
```

