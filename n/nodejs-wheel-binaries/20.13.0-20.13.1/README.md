# Comparing `tmp/nodejs_wheel_binaries-20.13.0.tar.gz` & `tmp/nodejs_wheel_binaries-20.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodejs_wheel_binaries-20.13.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "nodejs_wheel_binaries-20.13.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `nodejs_wheel_binaries-20.13.0.tar` & `nodejs_wheel_binaries-20.13.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/.gitattributes
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/.github/workflows/build_wheel.yml
--rw-r--r--   0        0        0        8 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/.nvmrc
--rw-r--r--   0        0        0     2202 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/CMakeLists.txt
--rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/LICENSE
--rw-r--r--   0        0        0     2666 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/README.md
-lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/cmd/README.md -> ../README.md
--rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/cmd/pyproject.toml
--rw-r--r--   0        0        0      269 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/cmd/setup.py
--rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/nodejs_wheel/__init__.py
--rw-r--r--   0        0        0       98 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/nodejs_wheel/__main__.py
--rw-r--r--   0        0        0     2394 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/nodejs_wheel/executable.py
--rw-r--r--   0        0        0     1132 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/pyproject.toml
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/renovate.json
--rw-r--r--   0        0        0      116 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/tests/test_api.py
--rw-r--r--   0        0        0     4219 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/.gitattributes
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/.github/workflows/build_wheel.yml
+-rw-r--r--   0        0        0        8 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/.nvmrc
+-rw-r--r--   0        0        0      744 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2202 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/LICENSE
+-rw-r--r--   0        0        0     3053 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/README.md
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/cmd/LICENSE
+-rw-r--r--   0        0        0     2159 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/cmd/README.md
+-rw-r--r--   0        0        0      518 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/cmd/hatch_build.py
+-rw-r--r--   0        0        0      929 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/cmd/pyproject.toml
+-rw-r--r--   0        0        0      141 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/nodejs_wheel/__init__.py
+-rw-r--r--   0        0        0      136 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/nodejs_wheel/__main__.py
+-rw-r--r--   0        0        0     6427 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/nodejs_wheel/executable.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/nodejs_wheel/py.typed
+-rw-r--r--   0        0        0     2451 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/pyproject.toml
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/renovate.json
+-rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/tests/test_api.py
+-rw-r--r--   0        0        0     4606 2022-11-09 12:37:21.000000 nodejs_wheel_binaries-20.13.1/PKG-INFO
```

### Comparing `nodejs_wheel_binaries-20.13.0/.github/workflows/build_wheel.yml` & `nodejs_wheel_binaries-20.13.1/.github/workflows/build_wheel.yml`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             platform_id: manylinux_aarch64
 
     steps:
       - uses: actions/checkout@v4
       - uses: ilammy/setup-nasm@v1
         if: matrix.platform_id == 'win_amd64'
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.17
+        uses: pypa/cibuildwheel@v2.18
         env:
           CIBW_BUILD_VERBOSITY: 1
           CIBW_ARCHS: all
           CIBW_BUILD: cp${{ matrix.python }}-${{ matrix.platform_id }}
       - uses: actions/upload-artifact@v4
         with:
           name: cibw-wheels-cp${{ matrix.python }}-${{ matrix.platform_id }}-${{ strategy.job-index }}
```

### Comparing `nodejs_wheel_binaries-20.13.0/CMakeLists.txt` & `nodejs_wheel_binaries-20.13.1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `nodejs_wheel_binaries-20.13.0/LICENSE` & `nodejs_wheel_binaries-20.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nodejs_wheel_binaries-20.13.0/README.md` & `nodejs_wheel_binaries-20.13.1/cmd/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,47 @@
 # Unoffical Node.js wheels
 
 [![Pypi version](https://img.shields.io/pypi/v/nodejs-wheel)](https://pypi.org/project/nodejs-wheel/)
 [![Pypi downloads](https://img.shields.io/pypi/dm/nodejs-wheel)](https://pypi.org/project/nodejs-wheel/)
 [![Pypi downloads](https://img.shields.io/pypi/dw/nodejs-wheel)](https://pypi.org/project/nodejs-wheel/)
 [![Pypi downloads](https://img.shields.io/pypi/dd/nodejs-wheel)](https://pypi.org/project/nodejs-wheel/)
 
-`nodejs-wheel` is an unofficial repository to distribute Node.js prebuilt wheels through PyPI using 
+`nodejs-wheel` is an unofficial repository to distribute Node.js prebuilt wheels through PyPI using
 
 ```sh
 pip install nodejs-wheel
 ```
 
-*New in v20.13.0*: If you don't need command line interface (CLI), install only `nodejs-wheel-binaries`, which is a direct dependency of `nodejs-wheel`.
+If you don't need command line interface (CLI), install only `nodejs-wheel-binaries`, which is a direct dependency of `nodejs-wheel`.
 
 ```sh
 pip install nodejs-wheel-binaries
 ```
 
 The package requires Python 3.7 and above.
 
 The project is powered by [scikit-build-core](https://github.com/scikit-build/scikit-build-core) and [cibuildwheel](https://github.com/pypa/cibuildwheel).
 
 ## Available Builds
 
-| OS      | Arch    | Bit | Conditions     | New in      |
-| ------- | ------- | --- | -------------- | ----------- |
-| Linux   | x86_64  | 64  | glibc >= 2.17  | v18.18.0    |
-| Linux   | aarch64 | 64  | glibc >= 2.17  | v20.13.0    |
-| macOS   | x86_64  | 64  | >= macOS-10.9  | v18.18.0    |
-| macOS   | arm64   | 64  | >= macOS-11    | v20.11.1    |
-| Windows | amd64   | 64  |                | v18.18.0    |
+| OS      | Arch    | Bit | Conditions     |
+| ------- | ------- | --- | -------------- |
+| Linux   | x86_64  | 64  | glibc >= 2.17  |
+| macOS   | x86_64  | 64  | >= macOS-10.9  |
+| macOS   | arm64   | 64  | >= macOS-11    |
+| Windows | amd64   | 64  |                |
 
 ## Usage
 
-### Command line
-
-Only available in the `nodejs-wheel` package.
-
 ```sh
 node -h
 npm -h
 npx -h
 ```
 
-### Run library module as a script
-
-*New in v20.13.0*.
-
-Only support `node`.
-
-```sh
-python -m nodejs_wheel --version
-```
-
-### Python API
-
-*New in v20.13.0*.
-
-```py
-from nodejs_wheel import (
-    node,
-    npm,
-    npx,
-)
-
-node("--version")
-npm("--version")
-npx("--version")
-```
-
 ## License
 
 `nodejs-wheel` distributed under the same MIT [license](LICENSE) as [Node.js](https://github.com/nodejs/node).
 
 ## Other projects
 
 The project is inspired by many other similiar projects:
```

### Comparing `nodejs_wheel_binaries-20.13.0/PKG-INFO` & `nodejs_wheel_binaries-20.13.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodejs-wheel-binaries
-Version: 20.13.0
+Version: 20.13.1
 Summary: unoffical Node.js package
 Keywords: nodejs
 Author-Email: Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License: Copyright 2023 Jinzhe Zeng
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -21,15 +21,15 @@
 # Unoffical Node.js wheels
 
 [![Pypi version](https://img.shields.io/pypi/v/nodejs-wheel)](https://pypi.org/project/nodejs-wheel/)
 [![Pypi downloads](https://img.shields.io/pypi/dm/nodejs-wheel)](https://pypi.org/project/nodejs-wheel/)
 [![Pypi downloads](https://img.shields.io/pypi/dw/nodejs-wheel)](https://pypi.org/project/nodejs-wheel/)
 [![Pypi downloads](https://img.shields.io/pypi/dd/nodejs-wheel)](https://pypi.org/project/nodejs-wheel/)
 
-`nodejs-wheel` is an unofficial repository to distribute Node.js prebuilt wheels through PyPI using 
+`nodejs-wheel` is an unofficial repository to distribute Node.js prebuilt wheels through PyPI using
 
 ```sh
 pip install nodejs-wheel
 ```
 
 *New in v20.13.0*: If you don't need command line interface (CLI), install only `nodejs-wheel-binaries`, which is a direct dependency of `nodejs-wheel`.
 
@@ -43,15 +43,15 @@
 
 ## Available Builds
 
 | OS      | Arch    | Bit | Conditions     | New in      |
 | ------- | ------- | --- | -------------- | ----------- |
 | Linux   | x86_64  | 64  | glibc >= 2.17  | v18.18.0    |
 | Linux   | aarch64 | 64  | glibc >= 2.17  | v20.13.0    |
-| macOS   | x86_64  | 64  | >= macOS-10.9  | v18.18.0    |
+| macOS   | x86_64  | 64  | >= macOS-10.15 | v18.18.0    |
 | macOS   | arm64   | 64  | >= macOS-11    | v20.11.1    |
 | Windows | amd64   | 64  |                | v18.18.0    |
 
 ## Usage
 
 ### Command line
 
@@ -80,17 +80,25 @@
 ```py
 from nodejs_wheel import (
     node,
     npm,
     npx,
 )
 
-node("--version")
-npm("--version")
-npx("--version")
+return_code0 = node(["--version"])
+return_code1 = npm(["--version"])
+return_code2 = npx(["--version"])
+```
+
+*New in v20.13.1*: pass `return_completed_process=True` to get `subprocess.CompletedProcess` instead of `int`.
+
+```py
+completed_process0 = node(["--version"], return_completed_process=True)
+completed_process1 = npm(["--version"], return_completed_process=True)
+completed_process2 = npx(["--version"], return_completed_process=True)
 ```
 
 ## License
 
 `nodejs-wheel` distributed under the same MIT [license](LICENSE) as [Node.js](https://github.com/nodejs/node).
 
 ## Other projects
```

