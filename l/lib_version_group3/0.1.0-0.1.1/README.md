# Comparing `tmp/lib_version_group3-0.1.0.tar.gz` & `tmp/lib_version_group3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_version_group3-0.1.0.tar", max compression
+gzip compressed data, was "lib_version_group3-0.1.1.tar", max compression
```

## Comparing `lib_version_group3-0.1.0.tar` & `lib_version_group3-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2024-05-10 15:23:27.917798 lib_version_group3-0.1.0/LICENSE
--rw-r--r--   0        0        0      103 2024-05-10 15:48:43.943216 lib_version_group3-0.1.0/README.md
--rw-r--r--   0        0        0      418 2024-05-10 16:03:06.072417 lib_version_group3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       83 2024-05-10 15:51:23.170799 lib_version_group3-0.1.0/src/lib_version_group3/__init__.py
--rw-r--r--   0        0        0       22 2024-05-10 16:01:36.012524 lib_version_group3-0.1.0/src/lib_version_group3/version.py
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 lib_version_group3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-12 19:07:45.839952 lib_version_group3-0.1.1/LICENSE
+-rw-r--r--   0        0        0      431 2024-05-12 19:07:45.839952 lib_version_group3-0.1.1/README.md
+-rw-r--r--   0        0        0      459 2024-05-12 19:07:45.839952 lib_version_group3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      234 2024-05-12 19:07:45.839952 lib_version_group3-0.1.1/src/lib_version_group3/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-12 19:08:02.040108 lib_version_group3-0.1.1/src/lib_version_group3/version.py
+-rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 lib_version_group3-0.1.1/PKG-INFO
```

### Comparing `lib_version_group3-0.1.0/LICENSE` & `lib_version_group3-0.1.1/LICENSE`

 * *Files identical despite different names*

