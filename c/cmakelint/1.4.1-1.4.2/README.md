# Comparing `tmp/cmakelint-1.4.1.tar.gz` & `tmp/cmakelint-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cmakelint-1.4.1.tar", last modified: Sat Jun 15 13:05:53 2019, max compression
+gzip compressed data, was "cmakelint-1.4.2.tar", last modified: Mon Jan 17 07:40:48 2022, max compression
```

## Comparing `cmakelint-1.4.1.tar` & `cmakelint-1.4.2.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:53.000000 cmakelint-1.4.1/
--rw-r--r--   0 kruset    (1000) kruset    (1000)      174 2019-06-15 13:05:53.000000 cmakelint-1.4.1/setup.cfg
-drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:53.000000 cmakelint-1.4.1/bin/
--rwxr-xr-x   0 kruset    (1000) kruset    (1000)      122 2019-06-01 09:35:24.000000 cmakelint-1.4.1/bin/cmakelint
--rw-r--r--   0 kruset    (1000) kruset    (1000)      386 2019-06-15 13:05:00.000000 cmakelint-1.4.1/tox.ini
-drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:53.000000 cmakelint-1.4.1/cmakelint/
--rw-r--r--   0 kruset    (1000) kruset    (1000)        0 2019-06-01 09:35:24.000000 cmakelint-1.4.1/cmakelint/__init__.py
--rw-r--r--   0 kruset    (1000) kruset    (1000)    20912 2019-06-15 13:05:00.000000 cmakelint-1.4.1/cmakelint/main.py
--rw-r--r--   0 kruset    (1000) kruset    (1000)       18 2019-06-15 13:05:00.000000 cmakelint-1.4.1/cmakelint/__version__.py
-drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:53.000000 cmakelint-1.4.1/cmakelint.egg-info/
--rw-rw-r--   0 kruset    (1000) kruset    (1000)      612 2019-06-15 13:05:53.000000 cmakelint-1.4.1/cmakelint.egg-info/SOURCES.txt
--rw-rw-r--   0 kruset    (1000) kruset    (1000)        1 2019-06-15 13:05:53.000000 cmakelint-1.4.1/cmakelint.egg-info/dependency_links.txt
--rw-rw-r--   0 kruset    (1000) kruset    (1000)     2858 2019-06-15 13:05:53.000000 cmakelint-1.4.1/cmakelint.egg-info/PKG-INFO
--rw-rw-r--   0 kruset    (1000) kruset    (1000)       51 2019-06-15 13:05:53.000000 cmakelint-1.4.1/cmakelint.egg-info/entry_points.txt
--rw-rw-r--   0 kruset    (1000) kruset    (1000)       10 2019-06-15 13:05:53.000000 cmakelint-1.4.1/cmakelint.egg-info/top_level.txt
--rw-r--r--   0 kruset    (1000) kruset    (1000)      309 2019-06-15 13:05:00.000000 cmakelint-1.4.1/MANIFEST.in
-drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:53.000000 cmakelint-1.4.1/test/
--rw-r--r--   0 kruset    (1000) kruset    (1000)    19418 2019-06-15 13:05:00.000000 cmakelint-1.4.1/test/cmakelint_test.py
--rw-r--r--   0 kruset    (1000) kruset    (1000)     5116 2019-06-15 13:05:00.000000 cmakelint-1.4.1/test/cli_test.py
--rw-r--r--   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:00.000000 cmakelint-1.4.1/test/__init__.py
--rw-r--r--   0 kruset    (1000) kruset    (1000)     1446 2019-06-15 13:05:00.000000 cmakelint-1.4.1/setup.py
--rw-r--r--   0 kruset    (1000) kruset    (1000)    11358 2019-06-01 09:35:24.000000 cmakelint-1.4.1/LICENSE
-drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:53.000000 cmakelint-1.4.1/samples/
-drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:53.000000 cmakelint-1.4.1/samples/blender/
--rw-r--r--   0 kruset    (1000) kruset    (1000)      975 2019-06-15 13:05:00.000000 cmakelint-1.4.1/samples/blender/nolinelen.def
--rw-r--r--   0 kruset    (1000) kruset    (1000)    28137 2019-06-15 13:05:00.000000 cmakelint-1.4.1/samples/blender/check.def
-drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:53.000000 cmakelint-1.4.1/samples/blender/src/
--rw-r--r--   0 kruset    (1000) kruset    (1000)    68116 2019-06-15 13:05:00.000000 cmakelint-1.4.1/samples/blender/src/CMakeLists.txt
-drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:53.000000 cmakelint-1.4.1/samples/opencv/
--rw-r--r--   0 kruset    (1000) kruset    (1000)    12088 2019-06-15 13:05:00.000000 cmakelint-1.4.1/samples/opencv/check.def
--rw-r--r--   0 kruset    (1000) kruset    (1000)    68689 2019-06-15 13:05:00.000000 cmakelint-1.4.1/samples/opencv/CMakeLists.txt
-drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:53.000000 cmakelint-1.4.1/samples/llvm/
--rw-r--r--   0 kruset    (1000) kruset    (1000)     7127 2019-06-15 13:05:00.000000 cmakelint-1.4.1/samples/llvm/check.def
--rw-r--r--   0 kruset    (1000) kruset    (1000)    43177 2019-06-15 13:05:00.000000 cmakelint-1.4.1/samples/llvm/CMakeLists.txt
--rw-r--r--   0 kruset    (1000) kruset    (1000)     7112 2019-06-15 13:05:00.000000 cmakelint-1.4.1/samples/llvm/checknofilename.def
--rw-r--r--   0 kruset    (1000) kruset    (1000)     2858 2019-06-15 13:05:53.000000 cmakelint-1.4.1/PKG-INFO
--rw-r--r--   0 kruset    (1000) kruset    (1000)     1770 2019-06-15 13:05:00.000000 cmakelint-1.4.1/README.md
--rw-r--r--   0 kruset    (1000) kruset    (1000)      171 2019-06-15 13:05:00.000000 cmakelint-1.4.1/requirements-test.txt
+drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2022-01-17 07:40:48.284268 cmakelint-1.4.2/
+-rw-r--r--   0 kruset    (1000) kruset    (1000)    11358 2019-06-01 09:35:24.000000 cmakelint-1.4.2/LICENSE
+-rw-r--r--   0 kruset    (1000) kruset    (1000)      425 2021-01-17 04:34:56.000000 cmakelint-1.4.2/MANIFEST.in
+-rw-r--r--   0 kruset    (1000) kruset    (1000)     2798 2022-01-17 07:40:48.284268 cmakelint-1.4.2/PKG-INFO
+-rw-r--r--   0 kruset    (1000) kruset    (1000)     2087 2022-01-17 07:33:59.000000 cmakelint-1.4.2/README.md
+drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2022-01-17 07:40:48.284268 cmakelint-1.4.2/bin/
+-rwxr-xr-x   0 kruset    (1000) kruset    (1000)      122 2019-06-01 09:35:24.000000 cmakelint-1.4.2/bin/cmakelint
+drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2022-01-17 07:40:48.284268 cmakelint-1.4.2/cmakelint/
+-rw-r--r--   0 kruset    (1000) kruset    (1000)        0 2019-06-01 09:35:24.000000 cmakelint-1.4.2/cmakelint/__init__.py
+-rw-r--r--   0 kruset    (1000) kruset    (1000)       18 2022-01-17 07:37:21.000000 cmakelint-1.4.2/cmakelint/__version__.py
+-rw-r--r--   0 kruset    (1000) kruset    (1000)    21071 2022-01-17 07:33:59.000000 cmakelint-1.4.2/cmakelint/main.py
+drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2022-01-17 07:40:48.284268 cmakelint-1.4.2/cmakelint.egg-info/
+-rw-rw-r--   0 kruset    (1000) kruset    (1000)     2798 2022-01-17 07:40:48.000000 cmakelint-1.4.2/cmakelint.egg-info/PKG-INFO
+-rw-rw-r--   0 kruset    (1000) kruset    (1000)      657 2022-01-17 07:40:48.000000 cmakelint-1.4.2/cmakelint.egg-info/SOURCES.txt
+-rw-rw-r--   0 kruset    (1000) kruset    (1000)        1 2022-01-17 07:40:48.000000 cmakelint-1.4.2/cmakelint.egg-info/dependency_links.txt
+-rw-rw-r--   0 kruset    (1000) kruset    (1000)       51 2022-01-17 07:40:48.000000 cmakelint-1.4.2/cmakelint.egg-info/entry_points.txt
+-rw-r--r--   0 kruset    (1000) kruset    (1000)      285 2022-01-17 07:40:48.000000 cmakelint-1.4.2/cmakelint.egg-info/requires.txt
+-rw-rw-r--   0 kruset    (1000) kruset    (1000)       10 2022-01-17 07:40:48.000000 cmakelint-1.4.2/cmakelint.egg-info/top_level.txt
+-rw-r--r--   0 kruset    (1000) kruset    (1000)      260 2021-01-17 04:34:56.000000 cmakelint-1.4.2/dev-requirements
+drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2022-01-17 07:40:48.284268 cmakelint-1.4.2/samples/
+drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2022-01-17 07:40:48.284268 cmakelint-1.4.2/samples/blender/
+-rw-r--r--   0 kruset    (1000) kruset    (1000)    28137 2019-06-15 13:05:00.000000 cmakelint-1.4.2/samples/blender/check.def
+-rw-r--r--   0 kruset    (1000) kruset    (1000)      975 2019-06-15 13:05:00.000000 cmakelint-1.4.2/samples/blender/nolinelen.def
+drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2022-01-17 07:40:48.284268 cmakelint-1.4.2/samples/blender/src/
+-rw-r--r--   0 kruset    (1000) kruset    (1000)    68116 2019-06-15 13:05:00.000000 cmakelint-1.4.2/samples/blender/src/CMakeLists.txt
+drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2022-01-17 07:40:48.284268 cmakelint-1.4.2/samples/llvm/
+-rw-r--r--   0 kruset    (1000) kruset    (1000)    43177 2019-06-15 13:05:00.000000 cmakelint-1.4.2/samples/llvm/CMakeLists.txt
+-rw-r--r--   0 kruset    (1000) kruset    (1000)     7127 2019-06-15 13:05:00.000000 cmakelint-1.4.2/samples/llvm/check.def
+-rw-r--r--   0 kruset    (1000) kruset    (1000)     7112 2019-06-15 13:05:00.000000 cmakelint-1.4.2/samples/llvm/checknofilename.def
+drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2022-01-17 07:40:48.284268 cmakelint-1.4.2/samples/opencv/
+-rw-r--r--   0 kruset    (1000) kruset    (1000)    68689 2019-06-15 13:05:00.000000 cmakelint-1.4.2/samples/opencv/CMakeLists.txt
+-rw-r--r--   0 kruset    (1000) kruset    (1000)    12088 2019-06-15 13:05:00.000000 cmakelint-1.4.2/samples/opencv/check.def
+-rw-r--r--   0 kruset    (1000) kruset    (1000)      180 2022-01-17 07:40:48.284268 cmakelint-1.4.2/setup.cfg
+-rw-r--r--   0 kruset    (1000) kruset    (1000)     2003 2021-01-17 04:34:56.000000 cmakelint-1.4.2/setup.py
+drwxr-xr-x   0 kruset    (1000) kruset    (1000)        0 2022-01-17 07:40:48.284268 cmakelint-1.4.2/test/
+-rw-r--r--   0 kruset    (1000) kruset    (1000)        0 2019-06-15 13:05:00.000000 cmakelint-1.4.2/test/__init__.py
+-rw-r--r--   0 kruset    (1000) kruset    (1000)     5116 2019-06-15 13:05:00.000000 cmakelint-1.4.2/test/cli_test.py
+-rw-r--r--   0 kruset    (1000) kruset    (1000)    19542 2021-01-17 04:34:56.000000 cmakelint-1.4.2/test/cmakelint_test.py
+-rw-r--r--   0 kruset    (1000) kruset    (1000)      215 2021-01-17 04:34:56.000000 cmakelint-1.4.2/test-requirements
+-rw-r--r--   0 kruset    (1000) kruset    (1000)      425 2021-01-17 04:34:56.000000 cmakelint-1.4.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cmakelint-1.4.1/cmakelint/main.py` & `cmakelint-1.4.2/cmakelint/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
       Specify a comma separated list of filters to apply
 
     spaces=N
       Indentation should be a multiple of N spaces
 
     config=file
       Use the given file for configuration. By default the file
-      ~/.config/cmakelintrc, $XDG_CONFIG_DIR/cmakelintrc or ~/.cmakelintrc is
-      used if it exists.  Use the value "None" to use no configuration file
-      (./None for a file called literally None) Only the option "filter=" is
-      currently supported in this file.
+      $PWD/.cmakelintrc, ~/.config/cmakelintrc, $XDG_CONFIG_DIR/cmakelintrc or
+      ~/.cmakelintrc is used if it exists. Use the value "None" to use no
+      configuration file (./None for a file called literally None) Only the
+      option "filter=" is currently supported in this file.
 
     quiet makes output quiet unless errors occurs
       Mainly used by automation tools when parsing huge amount of files.
       In those cases actual error might get lost in the pile of other stats
       prints.
 
       This argument is also handy for build system integration, so it's
@@ -87,16 +87,19 @@
         whitespace/newline
         whitespace/tabs
 """
 _DEFAULT_FILENAME = 'CMakeLists.txt'
 
 def DefaultRC():
     """
-    Check XDG_CONFIG_DIR before ~/.cmakelintrc
+    Check current working directory and XDG_CONFIG_DIR before ~/.cmakelintrc
     """
+    cwdfile = os.path.join(os.getcwd(), '.cmakelintrc')
+    if os.path.exists(cwdfile):
+        return cwdfile
     xdg = os.path.join(os.path.expanduser('~'), '.config')
     if 'XDG_CONFIG_DIR' in os.environ:
         xdg = os.environ['XDG_CONFIG_DIR']
     xdgfile = os.path.join(xdg, 'cmakelintrc')
     if os.path.exists(xdgfile):
         return xdgfile
     return os.path.join(os.path.expanduser('~'), '.cmakelintrc')
```

### Comparing `cmakelint-1.4.1/cmakelint.egg-info/SOURCES.txt` & `cmakelint-1.4.2/cmakelint.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
-requirements-test.txt
+dev-requirements
 setup.cfg
 setup.py
+test-requirements
 tox.ini
 bin/cmakelint
 cmakelint/__init__.py
 cmakelint/__version__.py
 cmakelint/main.py
 cmakelint.egg-info/PKG-INFO
 cmakelint.egg-info/SOURCES.txt
 cmakelint.egg-info/dependency_links.txt
 cmakelint.egg-info/entry_points.txt
+cmakelint.egg-info/requires.txt
 cmakelint.egg-info/top_level.txt
 samples/blender/check.def
 samples/blender/nolinelen.def
 samples/blender/src/CMakeLists.txt
 samples/llvm/CMakeLists.txt
 samples/llvm/check.def
 samples/llvm/checknofilename.def
```

### Comparing `cmakelint-1.4.1/cmakelint.egg-info/PKG-INFO` & `cmakelint-1.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,98 @@
 Metadata-Version: 2.1
 Name: cmakelint
-Version: 1.4.1
+Version: 1.4.2
 Summary: Static code checker for CMake files
 Home-page: https://github.com/cmake-lint/cmake-lint
 Author: Richard Quirk
 Author-email: richard.quirk@gmail.com
 License: Apache 2.0
 Download-URL: https://github.com/cmake-lint/cmake-lint
-Description: # CMakeLint
-        
-        [![Build Status](https://travis-ci.org/cmake-lint/cmake-lint.svg?branch=develop)](https://travis-ci.org/cmake-lint/cmake-lint)
-        ![PyPI](https://img.shields.io/pypi/v/cmakelint.svg)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dd/cmakelint.svg)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/cmakelint.svg)
-        
-        cmakelint parses CMake files and reports style issues.
-        
-        cmakelint requires Python.
-        
-        ## Installation
-        
-        To install cpplint from PyPI, run:
-        
-        .. code-block:: bash
-        
-            $ pip install cmakelint
-        
-        ## Usage
-        
-            Syntax: cmakelint [--config=file] [--filter=-x,+y] <file> [file] ...
-            filter=-x,+y,...
-              Specify a comma separated list of filters to apply
-        
-            config=file
-              Use the given file for configuration. By default the file
-              $HOME/.cmakelintrc is used if it exists.  Use the value "None" to use no
-              configuration file (./None for a file called literally None)
-              Only the option "filter=" is currently supported in this file.
-        
-        Run the `--filter=` option with no filter to see available options. Currently
-        these are:
-        
-            convention/filename
-            linelength
-            package/consistency
-            readability/logic
-            readability/mixedcase
-            readability/wonkycase
-            syntax
-            whitespace/eol
-            whitespace/extra
-            whitespace/indent
-            whitespace/mismatch
-            whitespace/newline
-            whitespace/tabs
-        
-        An example .cmakelintrc file would be as follows:
-        
-            filter=-whitespace/indent
-        
-        With this file in your home directory, running these commands would have the
-        same effect:
-        
-            cmakelint.py CMakeLists.txt
-            cmakelint.py --filter=-whitespace/indent CMakeLists.txt
-        
-        # Output status codes
-        
-        The program should exit with the following status codes:
-        
-        * 0 if everything went fine
-        * 1 if an error message was issued
-        * 32 on usage error
-        
 Keywords: cmake,lint
 Platform: UNKNOWN
 Classifier: Topic :: Software Development
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
 Classifier: Programming Language :: Other
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+License-File: LICENSE
+
+# CMakeLint
+
+[![Build Status](https://travis-ci.org/cmake-lint/cmake-lint.svg?branch=develop)](https://travis-ci.org/cmake-lint/cmake-lint)
+![PyPI](https://img.shields.io/pypi/v/cmakelint.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/cmakelint.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/cmakelint.svg)
+
+cmakelint parses CMake files and reports style issues.
+
+cmakelint requires Python.
+
+## Installation
+
+To install cmakelint from PyPI, run:
+
+.. code-block:: bash
+
+    $ pip install cmakelint
+
+## Usage
+
+    Syntax: cmakelint [--config=file] [--filter=-x,+y] <file> [file] ...
+    filter=-x,+y,...
+      Specify a comma separated list of filters to apply
+
+    config=file
+      Use the given file for configuration. By default the file
+      $PWD/.cmakelintrc, ~/.config/cmakelintrc, $XDG_CONFIG_DIR/cmakelintrc or
+      ~/.cmakelintrc is used if it exists. Use the value "None" to use no
+      configuration file (./None for a file called literally None) Only the
+      option "filter=" is currently supported in this file.
+
+Run the `--filter=` option with no filter to see available options. Currently
+these are:
+
+    convention/filename
+    linelength
+    package/consistency
+    readability/logic
+    readability/mixedcase
+    readability/wonkycase
+    syntax
+    whitespace/eol
+    whitespace/extra
+    whitespace/indent
+    whitespace/mismatch
+    whitespace/newline
+    whitespace/tabs
+
+An example .cmakelintrc file would be as follows:
+
+    filter=-whitespace/indent
+
+With this file in your home directory, running these commands would have the
+same effect:
+
+    cmakelint.py CMakeLists.txt
+    cmakelint.py --filter=-whitespace/indent CMakeLists.txt
+
+cmakelint can also be run with [pre-commit](https://pre-commit.com). Add the following configuration block to your `.pre-commit-config.yaml`:
+
+``` yaml
+  - repo: https://github.com/cmake-lint/cmake-lint
+    hooks:
+      - id: cmakelint
+```
+
+# Output status codes
+
+The program should exit with the following status codes:
+
+* 0 if everything went fine
+* 1 if an error message was issued
+* 32 on usage error
+
+
```

### Comparing `cmakelint-1.4.1/test/cmakelint_test.py` & `cmakelint-1.4.2/test/cmakelint_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 the License.
 """
 import contextlib
 import os
 import sys
 import unittest
 
-import mock
-
 import cmakelint.__version__
 import cmakelint.main
+import mock
 
 
 # stderr suppression from https://stackoverflow.com/a/1810086
 @contextlib.contextmanager
 def nostderr():
     savestderr = sys.stderr
 
@@ -386,19 +385,23 @@
             cmakelint.main.ParseArgs(['--config=None', 'foo.cmake'])
             self.assertEqual(None, cmakelint.main._lint_state.config)
             cmakelint.main.ParseArgs(['foo.cmake'])
             self.assertEqual(os.path.expanduser('~') + os.path.sep +
                              '.cmakelintrc', cmakelint.main._lint_state.config)
             config = {'return_value': True}
             patcher = mock.patch('os.path.isfile', **config)
-            patcher.start()
-            self.assertEqual(['CMakeLists.txt'], cmakelint.main.ParseArgs([]))
-            self.assertEqual(os.path.expanduser('~')+os.path.sep +
-                             '.cmakelintrc', cmakelint.main._lint_state.config)
-
+            try:
+                patcher.start()
+                self.assertEqual(
+                    ['CMakeLists.txt'],
+                    cmakelint.main.ParseArgs([]))
+                self.assertEqual(os.path.expanduser('~')+os.path.sep +
+                                 '.cmakelintrc', cmakelint.main._lint_state.config)
+            finally:
+                patcher.stop()
         finally:
             cmakelint.main._USAGE = old_usage
             cmakelint.main._ERROR_CATEGORIES = old_cats
             cmakelint.main._VERSION = old_version
             cmakelint.main._lint_state.filters = []
             cmakelint.main._lint_state.spaces = old_spaces
```

### Comparing `cmakelint-1.4.1/test/cli_test.py` & `cmakelint-1.4.2/test/cli_test.py`

 * *Files identical despite different names*

### Comparing `cmakelint-1.4.1/setup.py` & `cmakelint-1.4.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,35 +15,50 @@
         version = vermod.VERSION
         return version
     finally:
         if ver_file is not None:
             ver_file.close()
 
 
-with open('requirements-test.txt') as f:
-    required = f.read().splitlines()
+def read_without_comments(filename):
+    """some pip versions bark on comments (e.g. on travis)"""
+    with open(filename) as f:
+        return [line for line in f.read().splitlines() if not len(line) == 0 and not line.startswith('#')]
+
+
+test_required = read_without_comments('test-requirements')
 
 setup(name='cmakelint',
       version=get_version(),
       packages=['cmakelint'],
       scripts=['bin/cmakelint'],
       entry_points={
           'console_scripts': [
               'cmakelint = cmakelint.main:main'
           ]
       },
-      install_requires=[''],
-      tests_require=required,
+      install_requires=[],
+      setup_requires=[
+          "pytest-runner"
+      ],
+      tests_require=test_required,
+      # extras_require allow pip install .[dev]
+      extras_require={
+          'test': test_required,
+          'dev': read_without_comments('dev-requirements') + test_required
+      },
       author="Richard Quirk",
       author_email="richard.quirk@gmail.com",
       url="https://github.com/cmake-lint/cmake-lint",
       download_url="https://github.com/cmake-lint/cmake-lint",
       keywords=["cmake", "lint"],
       classifiers=[
         "Topic :: Software Development",
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Console",
         "Programming Language :: Other",
         "Programming Language :: Python",
         "License :: OSI Approved :: Apache Software License"],
       description="Static code checker for CMake files",
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
       license="Apache 2.0"
```

### Comparing `cmakelint-1.4.1/LICENSE` & `cmakelint-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmakelint-1.4.1/samples/blender/nolinelen.def` & `cmakelint-1.4.2/samples/blender/nolinelen.def`

 * *Files identical despite different names*

### Comparing `cmakelint-1.4.1/samples/blender/check.def` & `cmakelint-1.4.2/samples/blender/check.def`

 * *Files identical despite different names*

### Comparing `cmakelint-1.4.1/samples/blender/src/CMakeLists.txt` & `cmakelint-1.4.2/samples/blender/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmakelint-1.4.1/samples/opencv/check.def` & `cmakelint-1.4.2/samples/opencv/check.def`

 * *Files identical despite different names*

### Comparing `cmakelint-1.4.1/samples/opencv/CMakeLists.txt` & `cmakelint-1.4.2/samples/opencv/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmakelint-1.4.1/samples/llvm/check.def` & `cmakelint-1.4.2/samples/llvm/check.def`

 * *Files identical despite different names*

### Comparing `cmakelint-1.4.1/samples/llvm/CMakeLists.txt` & `cmakelint-1.4.2/samples/llvm/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmakelint-1.4.1/samples/llvm/checknofilename.def` & `cmakelint-1.4.2/samples/llvm/checknofilename.def`

 * *Files identical despite different names*

### Comparing `cmakelint-1.4.1/PKG-INFO` & `cmakelint-1.4.2/cmakelint.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,82 +1,98 @@
 Metadata-Version: 2.1
 Name: cmakelint
-Version: 1.4.1
+Version: 1.4.2
 Summary: Static code checker for CMake files
 Home-page: https://github.com/cmake-lint/cmake-lint
 Author: Richard Quirk
 Author-email: richard.quirk@gmail.com
 License: Apache 2.0
 Download-URL: https://github.com/cmake-lint/cmake-lint
-Description: # CMakeLint
-        
-        [![Build Status](https://travis-ci.org/cmake-lint/cmake-lint.svg?branch=develop)](https://travis-ci.org/cmake-lint/cmake-lint)
-        ![PyPI](https://img.shields.io/pypi/v/cmakelint.svg)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dd/cmakelint.svg)
-        ![PyPI - Downloads](https://img.shields.io/pypi/dm/cmakelint.svg)
-        
-        cmakelint parses CMake files and reports style issues.
-        
-        cmakelint requires Python.
-        
-        ## Installation
-        
-        To install cpplint from PyPI, run:
-        
-        .. code-block:: bash
-        
-            $ pip install cmakelint
-        
-        ## Usage
-        
-            Syntax: cmakelint [--config=file] [--filter=-x,+y] <file> [file] ...
-            filter=-x,+y,...
-              Specify a comma separated list of filters to apply
-        
-            config=file
-              Use the given file for configuration. By default the file
-              $HOME/.cmakelintrc is used if it exists.  Use the value "None" to use no
-              configuration file (./None for a file called literally None)
-              Only the option "filter=" is currently supported in this file.
-        
-        Run the `--filter=` option with no filter to see available options. Currently
-        these are:
-        
-            convention/filename
-            linelength
-            package/consistency
-            readability/logic
-            readability/mixedcase
-            readability/wonkycase
-            syntax
-            whitespace/eol
-            whitespace/extra
-            whitespace/indent
-            whitespace/mismatch
-            whitespace/newline
-            whitespace/tabs
-        
-        An example .cmakelintrc file would be as follows:
-        
-            filter=-whitespace/indent
-        
-        With this file in your home directory, running these commands would have the
-        same effect:
-        
-            cmakelint.py CMakeLists.txt
-            cmakelint.py --filter=-whitespace/indent CMakeLists.txt
-        
-        # Output status codes
-        
-        The program should exit with the following status codes:
-        
-        * 0 if everything went fine
-        * 1 if an error message was issued
-        * 32 on usage error
-        
 Keywords: cmake,lint
 Platform: UNKNOWN
 Classifier: Topic :: Software Development
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
 Classifier: Programming Language :: Other
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
+License-File: LICENSE
+
+# CMakeLint
+
+[![Build Status](https://travis-ci.org/cmake-lint/cmake-lint.svg?branch=develop)](https://travis-ci.org/cmake-lint/cmake-lint)
+![PyPI](https://img.shields.io/pypi/v/cmakelint.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dd/cmakelint.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/cmakelint.svg)
+
+cmakelint parses CMake files and reports style issues.
+
+cmakelint requires Python.
+
+## Installation
+
+To install cmakelint from PyPI, run:
+
+.. code-block:: bash
+
+    $ pip install cmakelint
+
+## Usage
+
+    Syntax: cmakelint [--config=file] [--filter=-x,+y] <file> [file] ...
+    filter=-x,+y,...
+      Specify a comma separated list of filters to apply
+
+    config=file
+      Use the given file for configuration. By default the file
+      $PWD/.cmakelintrc, ~/.config/cmakelintrc, $XDG_CONFIG_DIR/cmakelintrc or
+      ~/.cmakelintrc is used if it exists. Use the value "None" to use no
+      configuration file (./None for a file called literally None) Only the
+      option "filter=" is currently supported in this file.
+
+Run the `--filter=` option with no filter to see available options. Currently
+these are:
+
+    convention/filename
+    linelength
+    package/consistency
+    readability/logic
+    readability/mixedcase
+    readability/wonkycase
+    syntax
+    whitespace/eol
+    whitespace/extra
+    whitespace/indent
+    whitespace/mismatch
+    whitespace/newline
+    whitespace/tabs
+
+An example .cmakelintrc file would be as follows:
+
+    filter=-whitespace/indent
+
+With this file in your home directory, running these commands would have the
+same effect:
+
+    cmakelint.py CMakeLists.txt
+    cmakelint.py --filter=-whitespace/indent CMakeLists.txt
+
+cmakelint can also be run with [pre-commit](https://pre-commit.com). Add the following configuration block to your `.pre-commit-config.yaml`:
+
+``` yaml
+  - repo: https://github.com/cmake-lint/cmake-lint
+    hooks:
+      - id: cmakelint
+```
+
+# Output status codes
+
+The program should exit with the following status codes:
+
+* 0 if everything went fine
+* 1 if an error message was issued
+* 32 on usage error
+
+
```

### Comparing `cmakelint-1.4.1/README.md` & `cmakelint-1.4.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,31 +7,32 @@
 
 cmakelint parses CMake files and reports style issues.
 
 cmakelint requires Python.
 
 ## Installation
 
-To install cpplint from PyPI, run:
+To install cmakelint from PyPI, run:
 
 .. code-block:: bash
 
     $ pip install cmakelint
 
 ## Usage
 
     Syntax: cmakelint [--config=file] [--filter=-x,+y] <file> [file] ...
     filter=-x,+y,...
       Specify a comma separated list of filters to apply
 
     config=file
       Use the given file for configuration. By default the file
-      $HOME/.cmakelintrc is used if it exists.  Use the value "None" to use no
-      configuration file (./None for a file called literally None)
-      Only the option "filter=" is currently supported in this file.
+      $PWD/.cmakelintrc, ~/.config/cmakelintrc, $XDG_CONFIG_DIR/cmakelintrc or
+      ~/.cmakelintrc is used if it exists. Use the value "None" to use no
+      configuration file (./None for a file called literally None) Only the
+      option "filter=" is currently supported in this file.
 
 Run the `--filter=` option with no filter to see available options. Currently
 these are:
 
     convention/filename
     linelength
     package/consistency
@@ -52,14 +53,22 @@
 
 With this file in your home directory, running these commands would have the
 same effect:
 
     cmakelint.py CMakeLists.txt
     cmakelint.py --filter=-whitespace/indent CMakeLists.txt
 
+cmakelint can also be run with [pre-commit](https://pre-commit.com). Add the following configuration block to your `.pre-commit-config.yaml`:
+
+``` yaml
+  - repo: https://github.com/cmake-lint/cmake-lint
+    hooks:
+      - id: cmakelint
+```
+
 # Output status codes
 
 The program should exit with the following status codes:
 
 * 0 if everything went fine
 * 1 if an error message was issued
 * 32 on usage error
```

