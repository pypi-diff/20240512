# Comparing `tmp/apicat-0.0.4.tar.gz` & `tmp/apicat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicat-0.0.4.tar", max compression
+gzip compressed data, was "apicat-0.0.5.tar", max compression
```

## Comparing `apicat-0.0.4.tar` & `apicat-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      924 2024-05-11 12:53:55.687247 apicat-0.0.4/apicat/__init__.py
--rw-r--r--   0        0        0      519 2024-05-11 12:54:32.274728 apicat-0.0.4/apicat/config.py
--rw-r--r--   0        0        0      578 2024-05-10 12:53:29.917401 apicat-0.0.4/apicat/core.py
--rw-r--r--   0        0        0      413 2024-05-11 12:53:20.588642 apicat-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-10 09:24:50.379838 apicat-0.0.4/README.md
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 apicat-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1273 2024-05-11 13:59:32.847933 apicat-0.0.5/apicat/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-11 12:54:32.274728 apicat-0.0.5/apicat/config.py
+-rw-r--r--   0        0        0      578 2024-05-10 12:53:29.917401 apicat-0.0.5/apicat/core.py
+-rw-r--r--   0        0        0      412 2024-05-11 15:32:55.130812 apicat-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-10 09:24:50.379838 apicat-0.0.5/README.md
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 apicat-0.0.5/PKG-INFO
```

### Comparing `apicat-0.0.4/apicat/config.py` & `apicat-0.0.5/apicat/config.py`

 * *Files identical despite different names*

### Comparing `apicat-0.0.4/apicat/core.py` & `apicat-0.0.5/apicat/core.py`

 * *Files identical despite different names*

