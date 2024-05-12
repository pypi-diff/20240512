# Comparing `tmp/poetry_moment-0.0.4.tar.gz` & `tmp/poetry_moment-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_moment-0.0.4.tar", max compression
+gzip compressed data, was "poetry_moment-0.0.5.tar", max compression
```

## Comparing `poetry_moment-0.0.4.tar` & `poetry_moment-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1383 2024-05-11 12:52:21.979244 poetry_moment-0.0.4/poetry_moment/__init__.py
--rw-r--r--   0        0        0     2127 2024-05-11 12:26:28.391307 poetry_moment-0.0.4/poetry_moment/core.py
--rw-r--r--   0        0        0      354 2024-05-11 12:52:55.829127 poetry_moment-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      189 2024-05-10 13:02:56.918283 poetry_moment-0.0.4/README.md
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 poetry_moment-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1383 2024-05-11 12:52:21.979244 poetry_moment-0.0.5/poetry_moment/__init__.py
+-rw-r--r--   0        0        0     2127 2024-05-11 13:26:19.714880 poetry_moment-0.0.5/poetry_moment/core.py
+-rw-r--r--   0        0        0      372 2024-05-11 15:34:50.660713 poetry_moment-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      189 2024-05-10 13:02:56.918283 poetry_moment-0.0.5/README.md
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 poetry_moment-0.0.5/PKG-INFO
```

### Comparing `poetry_moment-0.0.4/poetry_moment/__init__.py` & `poetry_moment-0.0.5/poetry_moment/__init__.py`

 * *Files identical despite different names*

### Comparing `poetry_moment-0.0.4/poetry_moment/core.py` & `poetry_moment-0.0.5/poetry_moment/core.py`

 * *Files identical despite different names*

