# Comparing `tmp/pytubefix-5.4rc2.tar.gz` & `tmp/pytubefix-5.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubefix-5.4rc2.tar", last modified: Thu May  2 12:27:25 2024, max compression
+gzip compressed data, was "pytubefix-5.5rc1.tar", last modified: Sat May 11 22:35:27 2024, max compression
```

## Comparing `pytubefix-5.4rc2.tar` & `pytubefix-5.5rc1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-02 12:27:25.318414 pytubefix-5.4rc2/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1101 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/LICENSE
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       18 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/MANIFEST.in
--rw-r--r--   0 estoque   (1000) estoque   (1000)     4342 2024-05-02 12:27:25.318414 pytubefix-5.4rc2/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3010 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/README.md
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1524 2024-05-02 12:22:31.000000 pytubefix-5.4rc2/pyproject.toml
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-02 12:27:25.310415 pytubefix-5.4rc2/pytubefix/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      614 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/pytubefix/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    20063 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     6593 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/captions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1358 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/pytubefix/chapters.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     5645 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/pytubefix/cipher.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    16972 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      781 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/colors.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-02 12:27:25.314414 pytubefix-5.4rc2/pytubefix/contrib/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        0 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/pytubefix/contrib/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    19995 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/pytubefix/contrib/channel.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    14600 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/pytubefix/contrib/playlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    11072 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/pytubefix/contrib/search.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     4099 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/exceptions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18315 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/extract.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     9943 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/helpers.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    17742 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/innertube.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     4276 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/itags.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    41663 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/pytubefix/jsinterp.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1483 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/pytubefix/metadata.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      478 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/pytubefix/monostate.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     5948 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/parser.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    14359 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/query.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     8736 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/request.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    16049 2024-05-02 12:21:27.000000 pytubefix-5.4rc2/pytubefix/streams.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-05-02 12:22:20.000000 pytubefix-5.4rc2/pytubefix/version.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-02 12:27:25.318414 pytubefix-5.4rc2/pytubefix.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     4342 2024-05-02 12:27:25.000000 pytubefix-5.4rc2/pytubefix.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1029 2024-05-02 12:27:25.000000 pytubefix-5.4rc2/pytubefix.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-02 12:27:25.000000 pytubefix-5.4rc2/pytubefix.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       49 2024-05-02 12:27:25.000000 pytubefix-5.4rc2/pytubefix.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       10 2024-05-02 12:27:25.000000 pytubefix-5.4rc2/pytubefix.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-02 12:27:25.318414 pytubefix-5.4rc2/setup.cfg
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-02 12:27:25.318414 pytubefix-5.4rc2/tests/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     6579 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_captions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1360 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_cipher.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18009 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3626 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_exceptions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2963 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_extract.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     5060 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_helpers.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      279 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_itags.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1939 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_main.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      501 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_metadata.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1412 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_parser.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     6172 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_query.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1882 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_request.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    13661 2024-05-02 12:20:46.000000 pytubefix-5.4rc2/tests/test_streams.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-11 22:35:27.893305 pytubefix-5.5rc1/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/LICENSE
+-rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/MANIFEST.in
+-rw-r--r--   0 juan      (1000) juan      (1000)     4343 2024-05-11 22:35:27.893305 pytubefix-5.5rc1/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3011 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-05-11 22:32:47.000000 pytubefix-5.5rc1/pyproject.toml
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-11 22:35:27.885305 pytubefix-5.5rc1/pytubefix/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    20063 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6593 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/chapters.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    16972 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      781 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/colors.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-11 22:35:27.889305 pytubefix-5.5rc1/pytubefix/contrib/
+-rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/contrib/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/contrib/channel.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/contrib/playlist.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/contrib/search.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4099 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18343 2024-05-11 22:30:55.000000 pytubefix-5.5rc1/pytubefix/extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     9943 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17742 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/innertube.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4276 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/jsinterp.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/monostate.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5948 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14359 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     8736 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    16049 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/pytubefix/streams.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-05-11 22:34:05.000000 pytubefix-5.5rc1/pytubefix/version.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-11 22:35:27.893305 pytubefix-5.5rc1/pytubefix.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     4343 2024-05-11 22:35:27.000000 pytubefix-5.5rc1/pytubefix.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1029 2024-05-11 22:35:27.000000 pytubefix-5.5rc1/pytubefix.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-11 22:35:27.000000 pytubefix-5.5rc1/pytubefix.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-05-11 22:35:27.000000 pytubefix-5.5rc1/pytubefix.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-05-11 22:35:27.000000 pytubefix-5.5rc1/pytubefix.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-11 22:35:27.893305 pytubefix-5.5rc1/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-11 22:35:27.893305 pytubefix-5.5rc1/tests/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_main.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-05-11 22:26:33.000000 pytubefix-5.5rc1/tests/test_streams.py
```

### Comparing `pytubefix-5.4rc2/LICENSE` & `pytubefix-5.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/PKG-INFO` & `pytubefix-5.5rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.4rc2
+Version: 5.5rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
@@ -27,14 +27,15 @@
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytubefix
+
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pytubefix)
 ![PyPI - License](https://img.shields.io/pypi/l/pytubefix)
 ![Read the Docs](https://img.shields.io/readthedocs/pytubefix)
 ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/pytubefix?include_prereleases)
 <a href="https://pypi.org/project/pytubefix/"><img src="https://img.shields.io/pypi/v/pytubefix" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.4rc2 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.5rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.4rc2/README.md` & `pytubefix-5.5rc1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # pytubefix
+
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pytubefix)
 ![PyPI - License](https://img.shields.io/pypi/l/pytubefix)
 ![Read the Docs](https://img.shields.io/readthedocs/pytubefix)
 ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/pytubefix?include_prereleases)
 <a href="https://pypi.org/project/pytubefix/"><img src="https://img.shields.io/pypi/v/pytubefix" /></a>
```

### Comparing `pytubefix-5.4rc2/pyproject.toml` & `pytubefix-5.5rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubefix"
-version = "5.4-rc2"
+version = "5.5-rc1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python3 library for downloading YouTube Videos."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT license"}
```

### Comparing `pytubefix-5.4rc2/pytubefix/__init__.py` & `pytubefix-5.5rc1/pytubefix/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/__main__.py` & `pytubefix-5.5rc1/pytubefix/__main__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/captions.py` & `pytubefix-5.5rc1/pytubefix/captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/chapters.py` & `pytubefix-5.5rc1/pytubefix/chapters.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/cipher.py` & `pytubefix-5.5rc1/pytubefix/cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/cli.py` & `pytubefix-5.5rc1/pytubefix/cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/colors.py` & `pytubefix-5.5rc1/pytubefix/colors.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/contrib/channel.py` & `pytubefix-5.5rc1/pytubefix/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/contrib/playlist.py` & `pytubefix-5.5rc1/pytubefix/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/contrib/search.py` & `pytubefix-5.5rc1/pytubefix/contrib/search.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/exceptions.py` & `pytubefix-5.5rc1/pytubefix/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/extract.py` & `pytubefix-5.5rc1/pytubefix/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
             query_params['n'] = new_n
 
         url = f'{parsed_url.scheme}://{parsed_url.netloc}{parsed_url.path}?{urlencode(query_params)}'  # noqa:E501
 
         stream_manifest[i]["url"] = url
 
 
-def apply_descrambler(stream_data: Dict) -> None:
+def apply_descrambler(stream_data: Dict) -> Optional[List[Dict]]:
     """Apply various in-place transforms to YouTube's media stream data.
 
     Creates a ``list`` of dictionaries by string splitting on commas, then
     taking each list item, parsing it as a query string, converting it to a
     ``dict`` and unquoting the value.
 
     :param dict stream_data:
@@ -482,15 +482,15 @@
     {'foo': [{'bar': '1', 'var': 'test'}, {'em': '5', 't': 'url encoded'}]}
 
     """
     if 'url' in stream_data:
         return None
 
     # Merge formats and adaptiveFormats into a single list
-    formats = []
+    formats: list[Dict] = []
     if 'formats' in stream_data.keys():
         formats.extend(stream_data['formats'])
     if 'adaptiveFormats' in stream_data.keys():
         formats.extend(stream_data['adaptiveFormats'])
 
     # Extract url and s from signatureCiphers as necessary
     for data in formats:
```

### Comparing `pytubefix-5.4rc2/pytubefix/helpers.py` & `pytubefix-5.5rc1/pytubefix/helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/innertube.py` & `pytubefix-5.5rc1/pytubefix/innertube.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/itags.py` & `pytubefix-5.5rc1/pytubefix/itags.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/jsinterp.py` & `pytubefix-5.5rc1/pytubefix/jsinterp.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/metadata.py` & `pytubefix-5.5rc1/pytubefix/metadata.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/parser.py` & `pytubefix-5.5rc1/pytubefix/parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/query.py` & `pytubefix-5.5rc1/pytubefix/query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/request.py` & `pytubefix-5.5rc1/pytubefix/request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix/streams.py` & `pytubefix-5.5rc1/pytubefix/streams.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/pytubefix.egg-info/PKG-INFO` & `pytubefix-5.5rc1/pytubefix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.4rc2
+Version: 5.5rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
@@ -27,14 +27,15 @@
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytubefix
+
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pytubefix)
 ![PyPI - License](https://img.shields.io/pypi/l/pytubefix)
 ![Read the Docs](https://img.shields.io/readthedocs/pytubefix)
 ![GitHub Tag](https://img.shields.io/github/v/tag/JuanBindez/pytubefix?include_prereleases)
 <a href="https://pypi.org/project/pytubefix/"><img src="https://img.shields.io/pypi/v/pytubefix" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.4rc2 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.5rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.4rc2/pytubefix.egg-info/SOURCES.txt` & `pytubefix-5.5rc1/pytubefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_captions.py` & `pytubefix-5.5rc1/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_cipher.py` & `pytubefix-5.5rc1/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_cli.py` & `pytubefix-5.5rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_exceptions.py` & `pytubefix-5.5rc1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_extract.py` & `pytubefix-5.5rc1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_helpers.py` & `pytubefix-5.5rc1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_main.py` & `pytubefix-5.5rc1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_parser.py` & `pytubefix-5.5rc1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_query.py` & `pytubefix-5.5rc1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_request.py` & `pytubefix-5.5rc1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.4rc2/tests/test_streams.py` & `pytubefix-5.5rc1/tests/test_streams.py`

 * *Files identical despite different names*

