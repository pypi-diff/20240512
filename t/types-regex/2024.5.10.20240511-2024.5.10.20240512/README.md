# Comparing `tmp/types-regex-2024.5.10.20240511.tar.gz` & `tmp/types-regex-2024.5.10.20240512.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-regex-2024.5.10.20240511.tar", last modified: Sat May 11 02:17:51 2024, max compression
+gzip compressed data, was "types-regex-2024.5.10.20240512.tar", last modified: Sun May 12 02:22:43 2024, max compression
```

## Comparing `types-regex-2024.5.10.20240511.tar` & `types-regex-2024.5.10.20240512.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:51.062107 types-regex-2024.5.10.20240511/
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-11 02:17:50.000000 types-regex-2024.5.10.20240511/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 02:17:50.000000 types-regex-2024.5.10.20240511/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-11 02:17:51.062107 types-regex-2024.5.10.20240511/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:51.058107 types-regex-2024.5.10.20240511/regex-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 02:17:50.000000 types-regex-2024.5.10.20240511/regex-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 02:17:34.000000 types-regex-2024.5.10.20240511/regex-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-11 02:17:34.000000 types-regex-2024.5.10.20240511/regex-stubs/_regex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-11 02:17:34.000000 types-regex-2024.5.10.20240511/regex-stubs/_regex_core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:50.000000 types-regex-2024.5.10.20240511/regex-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-11 02:17:34.000000 types-regex-2024.5.10.20240511/regex-stubs/regex.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:17:51.062107 types-regex-2024.5.10.20240511/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-11 02:17:50.000000 types-regex-2024.5.10.20240511/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:17:51.062107 types-regex-2024.5.10.20240511/types_regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-11 02:17:51.000000 types-regex-2024.5.10.20240511/types_regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-11 02:17:51.000000 types-regex-2024.5.10.20240511/types_regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:17:51.000000 types-regex-2024.5.10.20240511/types_regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 02:17:51.000000 types-regex-2024.5.10.20240511/types_regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:22:43.481681 types-regex-2024.5.10.20240512/
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-05-12 02:22:41.000000 types-regex-2024.5.10.20240512/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-12 02:22:41.000000 types-regex-2024.5.10.20240512/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-12 02:22:43.481681 types-regex-2024.5.10.20240512/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:22:43.481681 types-regex-2024.5.10.20240512/regex-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-12 02:22:41.000000 types-regex-2024.5.10.20240512/regex-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-12 02:22:31.000000 types-regex-2024.5.10.20240512/regex-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-12 02:22:31.000000 types-regex-2024.5.10.20240512/regex-stubs/_regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-12 02:22:31.000000 types-regex-2024.5.10.20240512/regex-stubs/_regex_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 02:22:41.000000 types-regex-2024.5.10.20240512/regex-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19512 2024-05-12 02:22:31.000000 types-regex-2024.5.10.20240512/regex-stubs/regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 02:22:43.481681 types-regex-2024.5.10.20240512/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-12 02:22:41.000000 types-regex-2024.5.10.20240512/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 02:22:43.481681 types-regex-2024.5.10.20240512/types_regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-12 02:22:43.000000 types-regex-2024.5.10.20240512/types_regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-12 02:22:43.000000 types-regex-2024.5.10.20240512/types_regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 02:22:43.000000 types-regex-2024.5.10.20240512/types_regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 02:22:43.000000 types-regex-2024.5.10.20240512/types_regex.egg-info/top_level.txt
```

### Comparing `types-regex-2024.5.10.20240511/CHANGELOG.md` & `types-regex-2024.5.10.20240512/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2024.5.10.20240512 (2024-05-12)
+
+regex: functions do not accept any buffer for pattern (#11899)
+
 ## 2024.5.10.20240511 (2024-05-11)
 
 [stubsabot] Bump regex to 2024.5.10 (#11894)
 
 Release: https://pypi.org/pypi/regex/2024.5.10
 Homepage: https://github.com/mrabarnett/mrab-regex
 Repository: https://github.com/mrabarnett/mrab-regex
```

### Comparing `types-regex-2024.5.10.20240511/PKG-INFO` & `types-regex-2024.5.10.20240512/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2024.5.10.20240511
+Version: 2024.5.10.20240512
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.5.10`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+This package was generated from typeshed commit `6565e8a0a0efbd8735a473e6c0d57f787c7fa4a2` and was tested
 with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
```

### Comparing `types-regex-2024.5.10.20240511/regex-stubs/_regex.pyi` & `types-regex-2024.5.10.20240512/regex-stubs/_regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2024.5.10.20240511/regex-stubs/_regex_core.pyi` & `types-regex-2024.5.10.20240512/regex-stubs/_regex_core.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2024.5.10.20240511/regex-stubs/regex.pyi` & `types-regex-2024.5.10.20240512/regex-stubs/regex.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     concurrent: bool | None = None,
     timeout: float | None = None,
     ignore_unused: bool = False,
     **kwargs: Any,
 ) -> list[str | Any]: ...
 @overload
 def split(
-    pattern: ReadableBuffer | Pattern[bytes],
+    pattern: bytes | Pattern[bytes],
     string: ReadableBuffer,
     maxsplit: int = 0,
     flags: int = 0,
     concurrent: bool | None = None,
     timeout: float | None = None,
     ignore_unused: bool = False,
     **kwargs: Any,
@@ -130,15 +130,15 @@
     concurrent: bool | None = None,
     timeout: float | None = None,
     ignore_unused: bool = False,
     **kwargs: Any,
 ) -> _regex.Splitter[str]: ...
 @overload
 def splititer(
-    pattern: ReadableBuffer | Pattern[bytes],
+    pattern: bytes | Pattern[bytes],
     string: ReadableBuffer,
     maxsplit: int = 0,
     flags: int = 0,
     concurrent: bool | None = None,
     timeout: float | None = None,
     ignore_unused: bool = False,
     **kwargs: Any,
@@ -154,15 +154,15 @@
     concurrent: bool | None = None,
     timeout: float | None = None,
     ignore_unused: bool = False,
     **kwargs: Any,
 ) -> list[Any]: ...
 @overload
 def findall(
-    pattern: ReadableBuffer | Pattern[bytes],
+    pattern: bytes | Pattern[bytes],
     string: ReadableBuffer,
     flags: int = 0,
     pos: int | None = None,
     endpos: int | None = None,
     overlapped: bool = False,
     concurrent: bool | None = None,
     timeout: float | None = None,
@@ -181,15 +181,15 @@
     concurrent: bool | None = None,
     timeout: float | None = None,
     ignore_unused: bool = False,
     **kwargs: Any,
 ) -> _regex.Scanner[str]: ...
 @overload
 def finditer(
-    pattern: ReadableBuffer | Pattern[bytes],
+    pattern: bytes | Pattern[bytes],
     string: ReadableBuffer,
     flags: int = 0,
     pos: int | None = None,
     endpos: int | None = None,
     overlapped: bool = False,
     partial: bool = False,
     concurrent: bool | None = None,
@@ -209,15 +209,15 @@
     concurrent: bool | None = None,
     timeout: float | None = None,
     ignore_unused: bool = False,
     **kwargs: Any,
 ) -> str: ...
 @overload
 def sub(
-    pattern: ReadableBuffer | Pattern[bytes],
+    pattern: bytes | Pattern[bytes],
     repl: ReadableBuffer | Callable[[Match[bytes]], ReadableBuffer],
     string: ReadableBuffer,
     count: int = 0,
     flags: int = 0,
     pos: int | None = None,
     endpos: int | None = None,
     concurrent: bool | None = None,
@@ -237,15 +237,15 @@
     concurrent: bool | None = None,
     timeout: float | None = None,
     ignore_unused: bool = False,
     **kwargs: Any,
 ) -> str: ...
 @overload
 def subf(
-    pattern: ReadableBuffer | Pattern[bytes],
+    pattern: bytes | Pattern[bytes],
     format: ReadableBuffer | Callable[[Match[bytes]], ReadableBuffer],
     string: ReadableBuffer,
     count: int = 0,
     flags: int = 0,
     pos: int | None = None,
     endpos: int | None = None,
     concurrent: bool | None = None,
@@ -265,15 +265,15 @@
     concurrent: bool | None = None,
     timeout: float | None = None,
     ignore_unused: bool = False,
     **kwargs: Any,
 ) -> tuple[str, int]: ...
 @overload
 def subn(
-    pattern: ReadableBuffer | Pattern[bytes],
+    pattern: bytes | Pattern[bytes],
     repl: ReadableBuffer | Callable[[Match[bytes]], ReadableBuffer],
     string: ReadableBuffer,
     count: int = 0,
     flags: int = 0,
     pos: int | None = None,
     endpos: int | None = None,
     concurrent: bool | None = None,
@@ -293,15 +293,15 @@
     concurrent: bool | None = None,
     timeout: float | None = None,
     ignore_unused: bool = False,
     **kwargs: Any,
 ) -> tuple[str, int]: ...
 @overload
 def subfn(
-    pattern: ReadableBuffer | Pattern[bytes],
+    pattern: bytes | Pattern[bytes],
     format: ReadableBuffer | Callable[[Match[bytes]], ReadableBuffer],
     string: ReadableBuffer,
     count: int = 0,
     flags: int = 0,
     pos: int | None = None,
     endpos: int | None = None,
     concurrent: bool | None = None,
```

### Comparing `types-regex-2024.5.10.20240511/setup.py` & `types-regex-2024.5.10.20240512/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.5.10`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+This package was generated from typeshed commit `6565e8a0a0efbd8735a473e6c0d57f787c7fa4a2` and was tested
 with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2024.5.10.20240511",
+      version="2024.5.10.20240512",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md",
```

### Comparing `types-regex-2024.5.10.20240511/types_regex.egg-info/PKG-INFO` & `types-regex-2024.5.10.20240512/types_regex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2024.5.10.20240511
+Version: 2024.5.10.20240512
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-regex` aims to provide accurate annotations
 for `regex==2024.5.10`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
+This package was generated from typeshed commit `6565e8a0a0efbd8735a473e6c0d57f787c7fa4a2` and was tested
 with mypy 1.10.0, pyright 1.1.362, and
 pytype 2024.4.11.
```

