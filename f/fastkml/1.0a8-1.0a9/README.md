# Comparing `tmp/fastkml-1.0a8.tar.gz` & `tmp/fastkml-1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkml-1.0a8.tar", last modified: Sat Nov 25 17:01:07 2023, max compression
+gzip compressed data, was "fastkml-1.0a9.tar", last modified: Thu Dec 28 19:48:20 2023, max compression
```

## Comparing `fastkml-1.0a8.tar` & `fastkml-1.0a9.tar`

### file list

```diff
@@ -1,75 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 17:01:07.985956 fastkml-1.0a8/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-11-25 17:01:00.000000 fastkml-1.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2023-11-25 17:01:07.985956 fastkml-1.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2023-11-25 17:01:00.000000 fastkml-1.0a8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 17:01:07.973956 fastkml-1.0a8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/Configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/HISTORY.txt
--rw-r--r--   0 runner    (1001) docker     (127)      837 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/fastkml.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      448 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/reference_guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2023-11-25 17:01:00.000000 fastkml-1.0a8/docs/usage_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 17:01:07.977956 fastkml-1.0a8/fastkml/
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/atom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12996 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27883 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    22479 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14300 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/gx.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/kml.py
--rw-r--r--   0 runner    (1001) docker     (127)    12668 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)    32619 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/overlays.py
--rw-r--r--   0 runner    (1001) docker     (127)    30122 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2023-11-25 17:01:00.000000 fastkml-1.0a8/fastkml/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 17:01:07.981956 fastkml-1.0a8/fastkml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2023-11-25 17:01:07.000000 fastkml-1.0a8/fastkml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-11-25 17:01:07.000000 fastkml-1.0a8/fastkml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-25 17:01:07.000000 fastkml-1.0a8/fastkml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-11-25 17:01:07.000000 fastkml-1.0a8/fastkml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-25 17:01:07.000000 fastkml-1.0a8/fastkml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2023-11-25 17:01:00.000000 fastkml-1.0a8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 17:01:07.977956 fastkml-1.0a8/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    66104 2023-11-25 17:01:00.000000 fastkml-1.0a8/schema/ogckml22.xsd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-25 17:01:07.985956 fastkml-1.0a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 17:01:07.981956 fastkml-1.0a8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/atom_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/containers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10889 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/data_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/features_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 17:01:07.981956 fastkml-1.0a8/tests/geometries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/geometries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13577 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/geometries/geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/geometries/linearring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/geometries/linestring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15225 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/geometries/multigeometry_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/geometries/point_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/geometries/polygon_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/gx_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/links_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    43643 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/oldunit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9758 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/overlays_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22374 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/styles_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13023 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/times_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2023-11-25 17:01:00.000000 fastkml-1.0a8/tests/views_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:48:20.397667 fastkml-1.0a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2023-12-28 19:48:20.397667 fastkml-1.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-12-28 19:48:12.000000 fastkml-1.0a9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:48:20.393667 fastkml-1.0a9/fastkml/
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12374 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28920 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22570 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/gx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/kml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35665 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/overlays.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    36004 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26138 2023-12-28 19:48:12.000000 fastkml-1.0a9/fastkml/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 19:48:20.393667 fastkml-1.0a9/fastkml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2023-12-28 19:48:20.000000 fastkml-1.0a9/fastkml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2023-12-28 19:48:20.000000 fastkml-1.0a9/fastkml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 19:48:20.000000 fastkml-1.0a9/fastkml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2023-12-28 19:48:20.000000 fastkml-1.0a9/fastkml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-28 19:48:20.000000 fastkml-1.0a9/fastkml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2023-12-28 19:48:12.000000 fastkml-1.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 19:48:20.397667 fastkml-1.0a9/setup.cfg
```

### Comparing `fastkml-1.0a8/PKG-INFO` & `fastkml-1.0a9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: fastkml
-Version: 1.0a8
+Version: 1.0a9
 Summary: Fast KML processing in python
 Author-email: Christian Ledermann <christian.ledermann@gmail.com>
 License: LGPL
+Project-URL: Changelog, https://github.com/cleder/fastkml/blob/develop/docs/HISTORY.rst
 Project-URL: Documentation, https://fastkml.readthedocs.org/
 Project-URL: Homepage, https://github.com/cleder/fastkml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
+Classifier: Topic :: Text Processing :: Markup :: XML
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: arrow
 Requires-Dist: pygeoif>=1.1
 Requires-Dist: typing-extensions>4
 Provides-Extra: complexity
 Requires-Dist: lizard; extra == "complexity"
@@ -42,15 +45,14 @@
 Provides-Extra: linting
 Requires-Dist: black; extra == "linting"
 Requires-Dist: flake8; extra == "linting"
 Requires-Dist: flake8-comments; extra == "linting"
 Requires-Dist: flake8-encodings; extra == "linting"
 Requires-Dist: flake8-expression-complexity; extra == "linting"
 Requires-Dist: flake8-length; extra == "linting"
-Requires-Dist: flake8-literal; extra == "linting"
 Requires-Dist: flake8-pep3101; extra == "linting"
 Requires-Dist: flake8-super; extra == "linting"
 Requires-Dist: flake8-typing-imports; extra == "linting"
 Requires-Dist: ruff; extra == "linting"
 Requires-Dist: yamllint; extra == "linting"
 Provides-Extra: lxml
 Requires-Dist: lxml; extra == "lxml"
@@ -59,16 +61,15 @@
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: typing
 Requires-Dist: mypy; extra == "typing"
 
 Introduction
 ============
 
-KML is an XML geospatial data format and an `OGC standard <https://www.ogc.org/search/content/kml>`_
-that deserves a canonical python implementation.
+KML is an XML geospatial data format and an OGC_ standard that deserves a canonical python implementation.
 
 Fastkml is a library to read, write and manipulate KML files. It aims to keep
 it simple and fast (using lxml_ if available). Fast refers to the time you
 spend to write and read KML files as well as the time you spend to get
 acquainted to the library or to create KML objects. It aims to provide all of
 the functionality that KML clients such as `OpenLayers
 <http://openlayers.org/>`_, `Google Maps <http://maps.google.com/>`_, and
@@ -129,14 +130,19 @@
     :target: https://pypi.python.org/pypi/fastkml/
     :alt: Supported Python implementations
 
 .. image:: https://img.shields.io/librariesio/release/pypi/fastkml
     :target: https://libraries.io/pypi/fastkml
     :alt: Libraries.io dependency status for latest release
 
+.. image:: https://static.pepy.tech/badge/fastkml/month
+    :target: https://pepy.tech/project/fastkml
+    :alt: Downloads
+
+
 Documentation
 =============
 
 You can find all of the documentation for FastKML at `fastkml.readthedocs.org
 <https://fastkml.readthedocs.org>`_. If you find something that is missing,
 please submit a pull request on `GitHub <https://github.com/cleder/fastkml>`_
 with the improvement.
@@ -155,36 +161,32 @@
 
 You can install the package with ``pip install fastkml`` which will pull in all requirements.
 
 Requirements
 -------------
 
 * pygeoif_
-* lxml_
 * arrow_
 
 Optional
 ---------
 
-* lxml_
-
-You can install all of the requirements for working with FastKML by using pip_::
-
-    pip install -r requirements.txt
+* lxml_::
 
+    pip install --pre "fastkml[lxml]"
 
 Limitations
 ===========
 
 *Tesselate*, *Extrude* and *Altitude Mode* are assigned to a Geometry or
 Geometry collection (MultiGeometry). You cannot assign different values of
 *Tesselate*, *Extrude* or *Altitude Mode* on parts of a MultiGeometry.
 
 Currently, the only major feature missing for the full Google Earth experience
 is the `gx extension
 <https://developers.google.com/kml/documentation/kmlreference#kmlextensions>`_.
 Please submit a PR with the features you'd like to see implemented.
 
-.. _pygeoif: http://pypi.python.org/pypi/pygeoif/
+.. _pygeoif: https://pypi.python.org/pypi/pygeoif/
 .. _lxml: https://pypi.python.org/pypi/lxml
 .. _arrow: https://pypi.python.org/pypi/arrow
-.. _pip: https://pypi.python.org/pypi/pip
+.. _OGC: https://www.ogc.org/standard/kml/
```

### Comparing `fastkml-1.0a8/README.rst` & `fastkml-1.0a9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Introduction
 ============
 
-KML is an XML geospatial data format and an `OGC standard <https://www.ogc.org/search/content/kml>`_
-that deserves a canonical python implementation.
+KML is an XML geospatial data format and an OGC_ standard that deserves a canonical python implementation.
 
 Fastkml is a library to read, write and manipulate KML files. It aims to keep
 it simple and fast (using lxml_ if available). Fast refers to the time you
 spend to write and read KML files as well as the time you spend to get
 acquainted to the library or to create KML objects. It aims to provide all of
 the functionality that KML clients such as `OpenLayers
 <http://openlayers.org/>`_, `Google Maps <http://maps.google.com/>`_, and
@@ -67,14 +66,19 @@
     :target: https://pypi.python.org/pypi/fastkml/
     :alt: Supported Python implementations
 
 .. image:: https://img.shields.io/librariesio/release/pypi/fastkml
     :target: https://libraries.io/pypi/fastkml
     :alt: Libraries.io dependency status for latest release
 
+.. image:: https://static.pepy.tech/badge/fastkml/month
+    :target: https://pepy.tech/project/fastkml
+    :alt: Downloads
+
+
 Documentation
 =============
 
 You can find all of the documentation for FastKML at `fastkml.readthedocs.org
 <https://fastkml.readthedocs.org>`_. If you find something that is missing,
 please submit a pull request on `GitHub <https://github.com/cleder/fastkml>`_
 with the improvement.
@@ -93,36 +97,32 @@
 
 You can install the package with ``pip install fastkml`` which will pull in all requirements.
 
 Requirements
 -------------
 
 * pygeoif_
-* lxml_
 * arrow_
 
 Optional
 ---------
 
-* lxml_
-
-You can install all of the requirements for working with FastKML by using pip_::
-
-    pip install -r requirements.txt
+* lxml_::
 
+    pip install --pre "fastkml[lxml]"
 
 Limitations
 ===========
 
 *Tesselate*, *Extrude* and *Altitude Mode* are assigned to a Geometry or
 Geometry collection (MultiGeometry). You cannot assign different values of
 *Tesselate*, *Extrude* or *Altitude Mode* on parts of a MultiGeometry.
 
 Currently, the only major feature missing for the full Google Earth experience
 is the `gx extension
 <https://developers.google.com/kml/documentation/kmlreference#kmlextensions>`_.
 Please submit a PR with the features you'd like to see implemented.
 
-.. _pygeoif: http://pypi.python.org/pypi/pygeoif/
+.. _pygeoif: https://pypi.python.org/pypi/pygeoif/
 .. _lxml: https://pypi.python.org/pypi/lxml
 .. _arrow: https://pypi.python.org/pypi/arrow
-.. _pip: https://pypi.python.org/pypi/pip
+.. _OGC: https://www.ogc.org/standard/kml/
```

### Comparing `fastkml-1.0a8/docs/LICENSE.txt` & `fastkml-1.0a9/fastkml/about.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-  fastkml is copyright Christian Ledermann
+# Copyright (C) 2023  Christian Ledermann
+#
+# This library is free software; you can redistribute it and/or modify it under
+# the terms of the GNU Lesser General Public License as published by the Free
+# Software Foundation; either version 2.1 of the License, or (at your option)
+# any later version.
+#
+# This library is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+# FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
+# details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with this library; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301 USA
+"""
+About fastkml.
 
-    Copyright (C) 2012  Christian Ledermann
-
-    This library is free software; you can redistribute it and/or
-    modify it under the terms of the GNU Lesser General Public
-    License as published by the Free Software Foundation; either
-    version 2.1 of the License, or (at your option) any later version.
-
-    This library is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-    Lesser General Public License for more details.
-
-    You should have received a copy of the GNU Lesser General Public
-    License along with this library; if not, write to the Free Software
-    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
+The only purpose of this module is to provide a version number for the package.
+"""
+__version__ = "1.0.a9"
```

### Comparing `fastkml-1.0a8/fastkml/__init__.py` & `fastkml-1.0a9/fastkml/__init__.py`

 * *Files identical despite different names*

### Comparing `fastkml-1.0a8/fastkml/atom.py` & `fastkml-1.0a9/fastkml/atom.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,46 +28,57 @@
 These elements are defined in the Atom Syndication Format. The complete
 specification is found at http://atompub.org.
 
 This library only implements a subset of Atom that is useful with KML
 """
 
 import logging
-import re
 from typing import Any
 from typing import Dict
 from typing import Optional
 
 from fastkml import config
 from fastkml.base import _XMLObject
 from fastkml.config import ATOMNS as NS
 from fastkml.enums import Verbosity
+from fastkml.helpers import subelement_text_kwarg
+from fastkml.helpers import text_subelement
 from fastkml.types import Element
 
 logger = logging.getLogger(__name__)
-regex = r"(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$)"
-email_match = re.compile(regex).match
 
 
-def check_email(email: str) -> bool:
-    """Check if the email address is valid."""
-    return bool(email_match(email))
+class _AtomObject(_XMLObject):
+    """
+    Baseclass for Atom Objects.
+
+    Atom objects are used in KML to provide information about the author and
+    related website in your KML file. This information is displayed in geo
+    search results, both in Earth browsers such as Google Earth, and in other
+    applications such as Google Maps.
+    The atom tag name is the class name in lower case.
+    """
+
+    _default_ns = config.ATOMNS
+
+    @classmethod
+    def get_tag_name(cls) -> str:
+        """Return the tag name."""
+        return cls.__name__.lower()
 
 
-class Link(_XMLObject):
+class Link(_AtomObject):
     """
     Identifies a related Web page. The rel attribute defines the type of relation.
     A feed is limited to one alternate per type and hreflang.
     <link> is patterned after html's link element. It has one required
     attribute, href, and five optional attributes: rel, type, hreflang,
     title, and length.
     """
 
-    __name__ = "link"
-
     href: Optional[str]
     # href is the URI of the referenced resource
 
     rel: Optional[str]
     # rel contains a single link relationship type.
     # It can be a full URI, or one of the following predefined values
     # (default=alternate):
@@ -119,14 +130,17 @@
             f"type={self.type!r}, "
             f"hreflang={self.hreflang!r}, "
             f"title={self.title!r}, "
             f"length={self.length!r}, "
             ")"
         )
 
+    def __bool__(self) -> bool:
+        return bool(self.href)
+
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
         if self.href:
@@ -166,23 +180,21 @@
         kwargs["hreflang"] = element.get("hreflang")
         kwargs["title"] = element.get("title")
         length = element.get("length")
         kwargs["length"] = int(length) if length else None
         return kwargs
 
 
-class _Person(_XMLObject):
+class _Person(_AtomObject):
     """
     <author> and <contributor> describe a person, corporation, or similar
     entity. It has one required element, name, and two optional elements:
     uri, email.
     """
 
-    __name__ = ""
-
     name: Optional[str]
     # conveys a human-readable name for the person.
 
     uri: Optional[str]
     # contains a home page for the person.
 
     email: Optional[str]
@@ -207,41 +219,41 @@
             f"ns={self.ns!r}, "
             f"name={self.name!r}, "
             f"uri={self.uri!r}, "
             f"email={self.email!r}, "
             ")"
         )
 
+    def __bool__(self) -> bool:
+        return bool(self.name)
+
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
-        self.__name__ = self.__class__.__name__.lower()
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.name:
-            name = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}name",
-            )
-            name.text = self.name
-        else:
-            logger.warning("No Name for person defined")
-        if self.uri:
-            uri = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}uri",
-            )
-            uri.text = self.uri
-        if self.email and check_email(self.email):
-            email = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}email",
-            )
-            email.text = self.email
+        text_subelement(
+            self,
+            element=element,
+            attr_name="name",
+            node_name="name",
+        )
+        text_subelement(
+            self,
+            element=element,
+            attr_name="uri",
+            node_name="uri",
+        )
+        text_subelement(
+            self,
+            element=element,
+            attr_name="email",
+            node_name="email",
+        )
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -251,40 +263,54 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        name = element.find(f"{ns}name")
-        if name is not None:
-            kwargs["name"] = name.text
-        uri = element.find(f"{ns}uri")
-        if uri is not None:
-            kwargs["uri"] = uri.text
-        email = element.find(f"{ns}email")
-        if email is not None:
-            kwargs["email"] = email.text
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="name",
+                kwarg="name",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="uri",
+                kwarg="uri",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="email",
+                kwarg="email",
+                strict=strict,
+            ),
+        )
         return kwargs
 
 
 class Author(_Person):
     """
     Return the names one author of the feed/entry.
 
     A feed/entry may have multiple authors.
     """
 
-    __name__ = "author"
-
 
 class Contributor(_Person):
     """
     Return the names one contributor to the feed/entry.
 
     A feed/entry may have multiple contributor elements.
     """
 
-    __name__ = "contributor"
-
 
 __all__ = ["Author", "Contributor", "Link", "NS"]
```

### Comparing `fastkml-1.0a8/fastkml/base.py` & `fastkml-1.0a9/fastkml/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 
 class _XMLObject:
     """XML Baseclass."""
 
     _default_ns: str = ""
     _node_name: str = ""
-    __name__ = ""
     name_spaces: Dict[str, str]
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
     ) -> None:
@@ -54,23 +53,17 @@
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         """Return the KML Object as an Element."""
-        if self.__name__:
-            element: Element = config.etree.Element(  # type: ignore[attr-defined]
-                f"{self.ns}{self.__name__}",
-            )
-        else:
-            msg = "Call of abstract base class, subclasses implement this!"
-            raise NotImplementedError(
-                msg,
-            )
+        element: Element = config.etree.Element(  # type: ignore[attr-defined]
+            f"{self.ns}{self.get_tag_name()}",
+        )
         return element
 
     def to_string(
         self,
         *,
         prettyprint: bool = True,
         precision: Optional[int] = None,
@@ -99,14 +92,19 @@
                     encoding="UTF-8",
                 ).decode(
                     "UTF-8",
                 ),
             )
 
     @classmethod
+    def get_tag_name(cls) -> str:
+        """Return the tag name."""
+        return cls.__name__
+
+    @classmethod
     def _get_ns(cls, ns: Optional[str]) -> str:
         return cls._default_ns if ns is None else ns
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
```

### Comparing `fastkml-1.0a8/fastkml/config.py` & `fastkml-1.0a9/fastkml/config.py`

 * *Files identical despite different names*

### Comparing `fastkml-1.0a8/fastkml/containers.py` & `fastkml-1.0a9/fastkml/containers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,28 @@
+# Copyright (C) 2023  Christian Ledermann
+#
+# This library is free software; you can redistribute it and/or modify it under
+# the terms of the GNU Lesser General Public License as published by the Free
+# Software Foundation; either version 2.1 of the License, or (at your option)
+# any later version.
+#
+# This library is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+# FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
+# details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with this library; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301 USA
 """Container classes for KML elements."""
 import logging
 import urllib.parse as urlparse
 from typing import Any
 from typing import Dict
 from typing import Iterable
-from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Union
 
 from fastkml import atom
 from fastkml import gx
 from fastkml.data import ExtendedData
@@ -18,14 +32,16 @@
 from fastkml.features import Snippet
 from fastkml.features import _Feature
 from fastkml.geometry import LinearRing
 from fastkml.geometry import LineString
 from fastkml.geometry import MultiGeometry
 from fastkml.geometry import Point
 from fastkml.geometry import Polygon
+from fastkml.helpers import xml_subelement_list
+from fastkml.helpers import xml_subelement_list_kwarg
 from fastkml.styles import Style
 from fastkml.styles import StyleMap
 from fastkml.styles import StyleUrl
 from fastkml.times import TimeSpan
 from fastkml.times import TimeStamp
 from fastkml.types import Element
 from fastkml.views import Camera
@@ -51,15 +67,15 @@
     A Container element holds one or more Features and allows the
     creation of nested hierarchies.
     subclasses are:
     Document,
     Folder.
     """
 
-    _features: Optional[List[_Feature]]
+    features: List[_Feature]
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
@@ -75,15 +91,15 @@
         view: Optional[Union[Camera, LookAt]] = None,
         times: Optional[Union[TimeSpan, TimeStamp]] = None,
         style_url: Optional[StyleUrl] = None,
         styles: Optional[Iterable[Union[Style, StyleMap]]] = None,
         region: Optional[Region] = None,
         extended_data: Optional[ExtendedData] = None,
         # Container specific
-        features: Optional[List[_Feature]] = None,
+        features: Optional[Iterable[_Feature]] = None,
     ) -> None:
         super().__init__(
             ns=ns,
             name_spaces=name_spaces,
             id=id,
             target_id=target_id,
             name=name,
@@ -98,38 +114,33 @@
             view=view,
             times=times,
             style_url=style_url,
             styles=styles,
             region=region,
             extended_data=extended_data,
         )
-        self._features = features or []
-
-    def features(self) -> Iterator[_Feature]:
-        """Iterate over features."""
-        assert self._features is not None
-        yield from self._features
+        self.features = list(features) if features else []
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        for feature in self.features():
+        for feature in self.features:
             element.append(feature.etree_element())
         return element
 
     def append(self, kmlobj: _Feature) -> None:
         """Append a feature."""
         if kmlobj is self:
             msg = "Cannot append self"
             raise ValueError(msg)
-        assert self._features is not None
-        self._features.append(kmlobj)
+        assert self.features is not None
+        self.features.append(kmlobj)
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
         name_spaces: Optional[Dict[str, str]] = None,
@@ -139,50 +150,44 @@
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
         kwargs["features"] = []
-        folders = element.findall(f"{ns}Folder")
-        kwargs["features"] += [
-            Folder.class_from_element(ns=ns, element=folder, strict=strict)
-            for folder in folders
-        ]
-        placemarks = element.findall(f"{ns}Placemark")
-        kwargs["features"] += [
-            Placemark.class_from_element(ns=ns, element=placemark, strict=strict)
-            for placemark in placemarks
-        ]
-        documents = element.findall(f"{ns}Document")
-        kwargs["features"] += [
-            Document.class_from_element(ns=ns, element=document, strict=strict)
-            for document in documents
-        ]
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            xml_subelement_list_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="features",
+                obj_classes=(Folder, Placemark, Document),
+                strict=strict,
+            ),
+        )
         return kwargs
 
 
 class Folder(_Container):
     """
     A Folder is used to arrange other Features hierarchically
     (Folders, Placemarks, #NetworkLinks, or #Overlays).
     """
 
-    __name__ = "Folder"
-
 
 class Document(_Container):
     """
     A Document is a container for features and styles. This element is
     required if your KML file uses shared styles or schemata for typed
     extended data.
     """
 
-    __name__ = "Document"
-    _schemata: Optional[List[Schema]]
+    schemata: List[Schema]
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
@@ -222,38 +227,34 @@
             times=times,
             style_url=style_url,
             styles=styles,
             region=region,
             extended_data=extended_data,
             features=features,
         )
-        self._schemata = list(schemata) if schemata else []
-
-    def schemata(self) -> Iterator[Schema]:
-        if self._schemata:
-            yield from self._schemata
-
-    def append_schema(self, schema: Schema) -> None:
-        assert self._schemata is not None
-        self._schemata.append(schema)
+        self.schemata = list(schemata) if schemata else []
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self._schemata is not None:
-            for schema in self._schemata:
-                element.append(schema.etree_element())
+        xml_subelement_list(
+            obj=self,
+            element=element,
+            attr_name="schemata",
+            precision=precision,
+            verbosity=verbosity,
+        )
         return element
 
     def get_style_by_url(self, style_url: str) -> Optional[Union[Style, StyleMap]]:
         id_ = urlparse.urlparse(style_url).fragment
-        return next((style for style in self.styles() if style.id == id_), None)
+        return next((style for style in self.styles if style.id == id_), None)
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
         name_spaces: Optional[Dict[str, str]] = None,
@@ -262,13 +263,20 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        schemata = element.findall(f"{ns}Schema")
-        kwargs["schemata"] = [
-            Schema.class_from_element(ns=ns, element=schema, strict=strict)
-            for schema in schemata
-        ]
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            xml_subelement_list_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="schemata",
+                obj_classes=(Schema,),
+                strict=strict,
+            ),
+        )
         return kwargs
```

### Comparing `fastkml-1.0a8/fastkml/data.py` & `fastkml-1.0a9/fastkml/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,23 +21,26 @@
 import logging
 from dataclasses import dataclass
 from typing import Any
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
-from typing import Tuple
 from typing import Union
 
 from fastkml import config
 from fastkml.base import _BaseObject
 from fastkml.base import _XMLObject
 from fastkml.enums import DataType
 from fastkml.enums import Verbosity
 from fastkml.exceptions import KMLSchemaError
+from fastkml.helpers import subelement_text_kwarg
+from fastkml.helpers import text_subelement
+from fastkml.helpers import xml_subelement_list
+from fastkml.helpers import xml_subelement_list_kwarg
 from fastkml.types import Element
 
 __all__ = [
     "Data",
     "ExtendedData",
     "Schema",
     "SchemaData",
@@ -83,54 +86,33 @@
     The "id" attribute is required and must be unique within the KML file.
     <Schema> is always a child of <Document>.
 
     https://developers.google.com/kml/documentation/extendeddata#declare-the-schema-element
 
     """
 
-    __name__ = "Schema"
-
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
         name: Optional[str] = None,
         fields: Optional[Iterable[SimpleField]] = None,
     ) -> None:
         if id is None:
             msg = "Id is required for schema"
             raise KMLSchemaError(msg)
         super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
         self.name = name
-        self._simple_fields = list(fields) if fields else []
-
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}("
-            f"ns={self.ns!r}, "
-            f"id={self.id!r}, "
-            f"target_id={self.target_id!r}, "
-            f"name={self.name}, "
-            f"fields={self.simple_fields!r}"
-            ")"
-        )
-
-    @property
-    def simple_fields(self) -> Tuple[SimpleField, ...]:
-        return tuple(self._simple_fields)
-
-    @simple_fields.setter
-    def simple_fields(self, fields: Iterable[SimpleField]) -> None:
-        self._simple_fields = list(fields)
+        self.simple_fields = list(fields) if fields else []
 
     def append(self, field: SimpleField) -> None:
         """Append a field."""
-        self._simple_fields.append(field)
+        self.simple_fields.append(field)
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
@@ -152,14 +134,15 @@
         return element
 
     @classmethod
     def _get_fields_kwargs_from_element(
         cls,
         *,
         ns: str,
+        name_spaces: Optional[Dict[str, str]] = None,
         element: Element,
         strict: bool,
     ) -> List[SimpleField]:
         def get_display_name(field: Element) -> Optional[str]:
             display_name = field.find(f"{ns}displayName")
             return display_name.text if display_name is not None else None
 
@@ -187,24 +170,29 @@
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
         kwargs["name"] = element.get("name")
         kwargs["fields"] = cls._get_fields_kwargs_from_element(
             ns=ns,
+            name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
         return kwargs
 
 
 class Data(_XMLObject):
     """Represents an untyped name/value pair with optional display name."""
 
-    __name__ = "Data"
+    _default_ns = config.KMLNS
+
+    name: Optional[str]
+    value: Optional[str]
+    display_name: Optional[str]
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         name: Optional[str] = None,
         value: Optional[str] = None,
@@ -227,25 +215,26 @@
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
         element.set("name", self.name or "")
-        value = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}value",
-        )
-        value.text = self.value
-        if self.display_name:
-            display_name = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}displayName",
-            )
-            display_name.text = self.display_name
+        text_subelement(
+            self,
+            element=element,
+            attr_name="value",
+            node_name="value",
+        )
+        text_subelement(
+            self,
+            element=element,
+            attr_name="display_name",
+            node_name="displayName",
+        )
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -256,20 +245,33 @@
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
         kwargs["name"] = element.get("name")
-        value = element.find(f"{ns}value")
-        if value is not None:
-            kwargs["value"] = value.text
-        display_name = element.find(f"{ns}displayName")
-        if display_name is not None:
-            kwargs["display_name"] = display_name.text
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="value",
+                kwarg="value",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="displayName",
+                kwarg="display_name",
+                strict=strict,
+            ),
+        )
+
         return kwargs
 
 
 @dataclass(frozen=True)
 class SimpleData:
     name: str
     value: Union[int, str, float, bool]
@@ -284,56 +286,44 @@
     objects ("instances" of the custom data) are defined using the
     SchemaData element.
     The <schemaURL> can be a full URL, a reference to a Schema ID defined
     in an external KML file, or a reference to a Schema ID defined
     in the same KML file.
     """
 
-    __name__ = "SchemaData"
+    _default_ns = config.KMLNS
+
+    schema_url: Optional[str]
+    data: List[SimpleData]
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         schema_url: Optional[str] = None,
         data: Optional[Iterable[SimpleData]] = None,
     ) -> None:
         super().__init__(ns=ns, name_spaces=name_spaces)
-        if (not isinstance(schema_url, str)) or (not schema_url):
-            msg = "required parameter schema_url missing"
-            raise ValueError(msg)
         self.schema_url = schema_url
-        self._data = list(data) if data else []
+        self.data = list(data) if data else []
 
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}("
-            f"ns='{self.ns}',"
-            f"schema_url='{self.schema_url}', "
-            f"data='{self.data}')"
-        )
-
-    @property
-    def data(self) -> Tuple[SimpleData, ...]:
-        return tuple(self._data)
-
-    @data.setter
-    def data(self, data: Iterable[SimpleData]) -> None:
-        self._data = list(data)
+    def __bool__(self) -> bool:
+        return bool(self.data) and bool(self.schema_url)
 
     def append_data(self, data: SimpleData) -> None:
-        self._data.append(data)
+        self.data.append(data)
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        element.set("schemaUrl", self.schema_url)
+        if self.schema_url:
+            element.set("schemaUrl", self.schema_url)
         for data in self.data:
             sd = config.etree.SubElement(  # type: ignore[attr-defined]
                 element,
                 f"{self.ns}SimpleData",
             )
             sd.set("name", data.name)
             sd.text = data.value
@@ -368,40 +358,43 @@
     Represents a list of untyped name/value pairs. See docs:
 
     -> 'Adding Untyped Name/Value Pairs'
        https://developers.google.com/kml/documentation/extendeddata
 
     """
 
-    __name__ = "ExtendedData"
+    _default_ns = config.KMLNS
+
+    elements: List[Union[Data, SchemaData]]
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         elements: Optional[Iterable[Union[Data, SchemaData]]] = None,
     ) -> None:
         super().__init__(ns=ns, name_spaces=name_spaces)
-        self.elements = elements or []
+        self.elements = list(elements) if elements else []
 
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}("
-            f"ns='{self.ns}',"
-            f"elements='{self.elements}')"
-        )
+    def __bool__(self) -> bool:
+        return bool(self.elements)
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        for subelement in self.elements:
-            element.append(subelement.etree_element())
+        xml_subelement_list(
+            self,
+            element=element,
+            attr_name="elements",
+            precision=precision,
+            verbosity=verbosity,
+        )
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -411,22 +404,21 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        elements = []
-        untyped_data = element.findall(f"{ns}Data")
-        for ud in untyped_data:
-            el_data = Data.class_from_element(ns=ns, element=ud, strict=strict)
-            elements.append(el_data)
-        typed_data = element.findall(f"{ns}SchemaData")
-        for sd in typed_data:
-            el_schema_data = SchemaData.class_from_element(
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            xml_subelement_list_kwarg(
+                element=element,
                 ns=ns,
-                element=sd,
+                name_spaces=name_spaces,
+                kwarg="elements",
+                obj_classes=(Data, SchemaData),
                 strict=strict,
-            )
-            elements.append(el_schema_data)
-        kwargs["elements"] = elements
+            ),
+        )
+
         return kwargs
```

### Comparing `fastkml-1.0a8/fastkml/enums.py` & `fastkml-1.0a9/fastkml/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,7 +222,17 @@
 
     Specifies how the <x>, <y> values are interpreted.
     """
 
     fraction = "fraction"
     pixels = "pixels"
     inset_pixels = "insetPixels"
+
+
+@unique
+class PairKey(REnum):
+    """
+    Key for Pair.
+    """
+
+    normal = "normal"
+    highlight = "highlight"
```

### Comparing `fastkml-1.0a8/fastkml/exceptions.py` & `fastkml-1.0a9/fastkml/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastkml-1.0a8/fastkml/features.py` & `fastkml-1.0a9/fastkml/styles.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,353 +1,359 @@
-"""
-Feature base, Placemark and NetworkLink.
+# Copyright (C) 2012 - 2022  Christian Ledermann
+#
+# This library is free software; you can redistribute it and/or modify it under
+# the terms of the GNU Lesser General Public License as published by the Free
+# Software Foundation; either version 2.1 of the License, or (at your option)
+# any later version.
+#
+# This library is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+# FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
+# details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with this library; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301 USA
 
-These are the objects that can be added to a KML file.
+"""
+Once you've created features within Google Earth and examined the KML
+code Google Earth generates, you'll notice how styles are an important
+part of how your data is displayed.
 """
 
 import logging
-from dataclasses import dataclass
 from typing import Any
 from typing import Dict
 from typing import Iterable
-from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Union
 
-from fastkml import atom
 from fastkml import config
-from fastkml import gx
 from fastkml.base import _BaseObject
-from fastkml.data import ExtendedData
+from fastkml.base import _XMLObject
+from fastkml.enums import ColorMode
+from fastkml.enums import DisplayMode
+from fastkml.enums import PairKey
+from fastkml.enums import Units
 from fastkml.enums import Verbosity
-from fastkml.geometry import AnyGeometryType
-from fastkml.geometry import LinearRing
-from fastkml.geometry import LineString
-from fastkml.geometry import MultiGeometry
-from fastkml.geometry import Point
-from fastkml.geometry import Polygon
-from fastkml.links import Link
-from fastkml.mixins import TimeMixin
-from fastkml.styles import Style
-from fastkml.styles import StyleMap
-from fastkml.styles import StyleUrl
-from fastkml.styles import _StyleSelector
-from fastkml.times import TimeSpan
-from fastkml.times import TimeStamp
+from fastkml.helpers import bool_subelement
+from fastkml.helpers import enum_subelement
+from fastkml.helpers import float_subelement
+from fastkml.helpers import subelement_bool_kwarg
+from fastkml.helpers import subelement_enum_kwarg
+from fastkml.helpers import subelement_float_kwarg
+from fastkml.helpers import subelement_text_kwarg
+from fastkml.helpers import text_subelement
+from fastkml.helpers import xml_subelement
+from fastkml.helpers import xml_subelement_kwarg
+from fastkml.helpers import xml_subelement_list
+from fastkml.helpers import xml_subelement_list_kwarg
 from fastkml.types import Element
-from fastkml.views import Camera
-from fastkml.views import LookAt
-from fastkml.views import Region
 
 logger = logging.getLogger(__name__)
 
-KmlGeometry = Union[
-    Point,
-    LineString,
-    LinearRing,
-    Polygon,
-    MultiGeometry,
-    gx.MultiTrack,
-    gx.Track,
-]
 
+def strtobool(val: str) -> int:
+    val = val.lower()
+    if val == "false":
+        return 0
+    if val == "true":
+        return 1
+    return int(float(val))
+
+
+class StyleUrl(_BaseObject):
+    """
+    URL of a <Style> or <StyleMap> defined in a Document.
+
+    If the style is in the same file, use a # reference.
+    If the style is defined in an external file,
+    use a full URL along with # referencing.
+    """
 
-@dataclass(frozen=True)
-class Snippet:
-    text: str
-    max_lines: Optional[int] = None
-
-
-class _Feature(TimeMixin, _BaseObject):
-    """
-    abstract element; do not create
-    subclasses are:
-        * Container (Document, Folder)
-        * Placemark
-        * Overlay
-        * NetworkLink.
-    """
-
-    name: Optional[str]
-    # User-defined text displayed in the 3D viewer as the label for the
-    # object (for example, for a Placemark, Folder, or NetworkLink).
-
-    visibility: Optional[bool]
-    # Boolean value. Specifies whether the feature is drawn in the 3D
-    # viewer when it is initially loaded. In order for a feature to be
-    # visible, the <visibility> tag of all its ancestors must also be
-    # set to 1.
-
-    isopen: Optional[bool]
-    # Boolean value. Specifies whether a Document or Folder appears
-    # closed or open when first loaded into the Places panel.
-    # 0=collapsed (the default), 1=expanded.
-
-    _atom_author: Optional[atom.Author]
-    # KML 2.2 supports new elements for including data about the author
-    # and related website in your KML file. This information is displayed
-    # in geo search results, both in Earth browsers such as Google Earth,
-    # and in other applications such as Google Maps.
-
-    _atom_link: Optional[atom.Link]
-    # Specifies the URL of the website containing this KML or KMZ file.
-
-    _address: Optional[str]
-    # A string value representing an unstructured address written as a
-    # standard street, city, state address, and/or as a postal code.
-    # You can use the <address> tag to specify the location of a point
-    # instead of using latitude and longitude coordinates.
-
-    _phone_number: Optional[str]
-    # A string value representing a telephone number.
-    # This element is used by Google Maps Mobile only.
-
-    _snippet: Optional[Snippet]
-    # _snippet is either a tuple of a string Snippet.text and an integer
-    # Snippet.maxLines or a string
-    #
-    # A short description of the feature. In Google Earth, this
-    # description is displayed in the Places panel under the name of the
-    # feature. If a Snippet is not supplied, the first two lines of
-    # the <description> are used. In Google Earth, if a Placemark
-    # contains both a description and a Snippet, the <Snippet> appears
-    # beneath the Placemark in the Places panel, and the <description>
-    # appears in the Placemark's description balloon. This tag does not
-    # support HTML markup. <Snippet> has a maxLines attribute, an integer
-    # that specifies the maximum number of lines to display.
-
-    description: Optional[str]
-    # User-supplied content that appears in the description balloon.
-
-    _style_url: Optional[StyleUrl]
-    # URL of a <Style> or <StyleMap> defined in a Document.
-    # If the style is in the same file, use a # reference.
-    # If the style is defined in an external file, use a full URL
-    # along with # referencing.
-
-    _styles: List[Union[Style, StyleMap]]
-    # One or more Styles and StyleMaps can be defined to customize the
-    # appearance of any element derived from Feature or of the Geometry
-    # in a Placemark.
-    # A style defined within a Feature is called an "inline style" and
-    # applies only to the Feature that contains it. A style defined as
-    # the child of a <Document> is called a "shared style." A shared
-    # style must have an id defined for it. This id is referenced by one
-    # or more Features within the <Document>. In cases where a style
-    # element is defined both in a shared style and in an inline style
-    # for a Feature—that is, a Folder, GroundOverlay, NetworkLink,
-    # Placemark, or ScreenOverlay—the value for the Feature's inline
-    # style takes precedence over the value for the shared style.
-
-    _view: Union[Camera, LookAt, None]
-
-    region: Optional[Region]
-    # Features and geometry associated with a Region are drawn only when
-    # the Region is active.
-
-    extended_data: Optional[ExtendedData]
-    # Allows you to add custom data to a KML file. This data can be
-    # (1) data that references an external XML schema,
-    # (2) untyped data/value pairs, or
-    # (3) typed data.
-    # A given KML Feature can contain a combination of these types of
-    # custom data.
-    #
-    # (2) is already implemented, see UntypedExtendedData
-    #
-    # <Metadata> (deprecated in KML 2.2; use <ExtendedData> instead)
+    url: Optional[str]
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        name: Optional[str] = None,
-        visibility: Optional[bool] = None,
-        isopen: Optional[bool] = None,
-        atom_link: Optional[atom.Link] = None,
-        atom_author: Optional[atom.Author] = None,
-        address: Optional[str] = None,
-        phone_number: Optional[str] = None,
-        snippet: Optional[Snippet] = None,
-        description: Optional[str] = None,
-        view: Optional[Union[Camera, LookAt]] = None,
-        times: Optional[Union[TimeSpan, TimeStamp]] = None,
-        style_url: Optional[StyleUrl] = None,
-        styles: Optional[Iterable[Union[Style, StyleMap]]] = None,
-        region: Optional[Region] = None,
-        extended_data: Optional[ExtendedData] = None,
+        url: Optional[str] = None,
     ) -> None:
         super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
-        self.name = name
-        self.description = description
-        self._style_url = style_url
-        self._styles = list(styles) if styles else []
-        self._view = view
-        self.visibility = visibility
-        self.isopen = isopen
-        self.snippet = snippet
-        self._atom_author = atom_author
-        self._atom_link = atom_link
-        self.address = address
-        self.phone_number = phone_number
-        self.region = region
-        self.extended_data = extended_data
-        self._times = times
+        self.url = url
 
-    @property
-    def style_url(self) -> Optional[str]:
-        """
-        Returns the url only, not a full StyleUrl object.
-        if you need the full StyleUrl object use _style_url.
-        """
-        return self._style_url.url if isinstance(self._style_url, StyleUrl) else None
-
-    @style_url.setter
-    def style_url(self, styleurl: Union[str, StyleUrl, None]) -> None:
-        """You may pass a StyleUrl Object, a string or None."""
-        if isinstance(styleurl, StyleUrl):
-            self._style_url = styleurl
-        elif isinstance(styleurl, str):
-            s = StyleUrl(self.ns, url=styleurl)
-            self._style_url = s
-        elif styleurl is None:
-            self._style_url = None
-        else:
-            raise ValueError
+    def __bool__(self) -> bool:
+        return bool(self.url)
 
-    @property
-    def view(self) -> Optional[Union[Camera, LookAt]]:
-        return self._view
+    def etree_element(
+        self,
+        precision: Optional[int] = None,
+        verbosity: Verbosity = Verbosity.normal,
+    ) -> Element:
+        element = super().etree_element(precision=precision, verbosity=verbosity)
+        element.text = self.url or ""
+        return element
 
-    @view.setter
-    def view(self, camera: Optional[Union[Camera, LookAt]]) -> None:
-        self._view = camera
+    @classmethod
+    def get_tag_name(cls) -> str:
+        """Return the tag name."""
+        return "styleUrl"
 
-    @property
-    def link(self) -> Optional[atom.Link]:
-        return self._atom_link
+    @classmethod
+    def _get_kwargs(
+        cls,
+        *,
+        ns: str,
+        name_spaces: Optional[Dict[str, str]] = None,
+        element: Element,
+        strict: bool,
+    ) -> Dict[str, Any]:
+        kwargs = super()._get_kwargs(
+            ns=ns,
+            name_spaces=name_spaces,
+            element=element,
+            strict=strict,
+        )
+        kwargs["url"] = element.text
+        return kwargs
 
-    @link.setter
-    def link(self, link: Optional[atom.Link]) -> None:
-        self._atom_link = link
 
-    @property
-    def author(self) -> Optional[atom.Author]:
-        return self._atom_author
+class _StyleSelector(_BaseObject):
+    """
+    This is an abstract element and cannot be used directly in a KML file.
+    It is the base type for the <Style> and <StyleMap> elements. The
+    StyleMap element selects a style based on the current mode of the
+    Placemark. An element derived from StyleSelector is uniquely identified
+    by its id and its url.
+    """
 
-    @author.setter
-    def author(self, author: Optional[atom.Author]) -> None:
-        self._atom_author = author
-
-    def append_style(self, style: Union[Style, StyleMap]) -> None:
-        """Append a style to the feature."""
-        if isinstance(style, _StyleSelector):
-            self._styles.append(style)
-        else:
-            raise TypeError
 
-    def styles(self) -> Iterator[Union[Style, StyleMap]]:
-        """Iterate over the styles of this feature."""
-        for style in self._styles:
-            if isinstance(style, _StyleSelector):
-                yield style
-            else:
-                raise TypeError
+class _ColorStyle(_BaseObject):
+    """
+    abstract element; do not create.
+    This is an abstract element and cannot be used directly in a KML file.
+    It provides elements for specifying the color and color mode of
+    extended style types.
+    subclasses are: IconStyle, LabelStyle, LineStyle, PolyStyle.
+    """
 
-    @property
-    def snippet(self) -> Optional[Snippet]:
-        return self._snippet
+    id = None
+    color = None
+    # Color and opacity (alpha) values are expressed in hexadecimal notation.
+    # The range of values for any one color is 0 to 255 (00 to ff).
+    # For alpha, 00 is fully transparent and ff is fully opaque.
+    # The order of expression is aabbggrr, where aa=alpha (00 to ff);
+    # bb=blue (00 to ff); gg=green (00 to ff); rr=red (00 to ff).
+
+    color_mode: Optional[ColorMode]
+    # Values for <colorMode> are normal (no effect) and random.
+    # A value of random applies a random linear scale to the base <color>
 
-    @snippet.setter
-    def snippet(self, snippet: Optional[Snippet]) -> None:
-        self._snippet = snippet
+    def __init__(
+        self,
+        ns: Optional[str] = None,
+        name_spaces: Optional[Dict[str, str]] = None,
+        id: Optional[str] = None,
+        target_id: Optional[str] = None,
+        color: Optional[str] = None,
+        color_mode: Optional[ColorMode] = None,
+    ) -> None:
+        super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
+        self.color = color
+        self.color_mode = color_mode
 
-    @property
-    def address(self) -> Optional[str]:
-        return self._address
+    def etree_element(
+        self,
+        precision: Optional[int] = None,
+        verbosity: Verbosity = Verbosity.normal,
+    ) -> Element:
+        element = super().etree_element(precision=precision, verbosity=verbosity)
+        text_subelement(
+            obj=self,
+            element=element,
+            attr_name="color",
+            node_name="color",
+        )
+        enum_subelement(
+            obj=self,
+            element=element,
+            attr_name="color_mode",
+            node_name="colorMode",
+        )
+        return element
 
-    @address.setter
-    def address(self, address: Optional[str]) -> None:
-        self._address = address
+    @classmethod
+    def _get_kwargs(
+        cls,
+        *,
+        ns: str,
+        name_spaces: Optional[Dict[str, str]] = None,
+        element: Element,
+        strict: bool,
+    ) -> Dict[str, Any]:
+        kwargs = super()._get_kwargs(
+            ns=ns,
+            name_spaces=name_spaces,
+            element=element,
+            strict=strict,
+        )
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="color",
+                kwarg="color",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_enum_kwarg(
+                element=element,
+                ns=ns,
+                node_name="colorMode",
+                kwarg="color_mode",
+                enum_class=ColorMode,
+                strict=strict,
+            ),
+        )
+
+        return kwargs
+
+
+class HotSpot(_XMLObject):
+    """
+    Specifies the position within the Icon that is "anchored" to the <Point>.
+
+    x - Either the number of pixels, a fractional component of the icon,
+    or a pixel inset indicating the x component of a point on the icon.
+    y - Either the number of pixels, a fractional component of the icon,
+    or a pixel inset indicating the y component of a point on the icon.
+    xunits - Units in which the x value is specified.
+    A value of fraction indicates the x value is a fraction of the icon.
+    A value of pixels indicates the x value in pixels.
+    A value of insetPixels indicates the indent from the right edge of the icon.
+    yunits - Units in which the y value is specified.
+
+    https://developers.google.com/kml/documentation/kmlreference#hotspot
+    """
+
+    x: Optional[float]
+    y: Optional[float]
+    xunits: Optional[Units]
+    yunits: Optional[Units]
+
+    _default_ns = config.KMLNS
+
+    def __init__(
+        self,
+        ns: Optional[str] = None,
+        name_spaces: Optional[Dict[str, str]] = None,
+        x: Optional[float] = None,
+        y: Optional[float] = None,
+        xunits: Optional[Units] = None,
+        yunits: Optional[Units] = None,
+    ) -> None:
+        super().__init__(ns=ns, name_spaces=name_spaces)
+        self.x = x
+        self.y = y
+        self.xunits = xunits
+        self.yunits = yunits
+
+    def ___bool__(self) -> bool:
+        return all((self.x is not None, self.y is not None))
+
+    def etree_element(
+        self,
+        precision: Optional[int] = None,
+        verbosity: Verbosity = Verbosity.normal,
+    ) -> Element:
+        element = super().etree_element(precision=precision, verbosity=verbosity)
+        hot_spot = config.etree.SubElement(  # type: ignore[attr-defined]
+            element,
+            f"{self.ns}hotSpot",
+        )
+        hot_spot.attrib["x"] = str(self.x)
+        hot_spot.attrib["y"] = str(self.y)
+        if self.xunits:
+            hot_spot.attrib["xunits"] = self.xunits.value
+        if self.yunits:
+            hot_spot.attrib["yunits"] = self.yunits.value
+        return element
+
+    @classmethod
+    def get_tag_name(cls) -> str:
+        """Return the tag name."""
+        return "hotSpot"
+
+    @classmethod
+    def _get_kwargs(
+        cls,
+        *,
+        ns: str,
+        name_spaces: Optional[Dict[str, str]] = None,
+        element: Element,
+        strict: bool,
+    ) -> Dict[str, Any]:
+        kwargs = super()._get_kwargs(
+            ns=ns,
+            name_spaces=name_spaces,
+            element=element,
+            strict=strict,
+        )
+        kwargs["x"] = float(element.get("x"))
+        kwargs["y"] = float(element.get("y"))
+        if element.get("xunits"):
+            kwargs["xunits"] = Units(element.get("xunits"))
+        if element.get("yunits"):
+            kwargs["yunits"] = Units(element.get("yunits"))
+        return kwargs
 
-    @property
-    def phone_number(self) -> Optional[str]:
-        return self._phone_number
 
-    @phone_number.setter
-    def phone_number(self, phone_number: Optional[str]) -> None:
-        self._phone_number = phone_number
+class Icon(_XMLObject):
+    """
+    A custom Icon.
+
+    In <IconStyle>, the only child element of <Icon> is <href>
+    """
+
+    _default_ns = config.KMLNS
+
+    href: Optional[str]
+    # An HTTP address or a local file specification used to load an icon.
+
+    def __init__(
+        self,
+        ns: Optional[str] = None,
+        name_spaces: Optional[Dict[str, str]] = None,
+        href: Optional[str] = None,
+    ) -> None:
+        super().__init__(ns=ns, name_spaces=name_spaces)
+        self.href = href
+
+    def __bool__(self) -> bool:
+        return bool(self.href)
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.name:
-            name = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}name",
-            )
-            name.text = self.name
-        if self.description:
-            description = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}description",
-            )
-            description.text = self.description
-        if self._view is not None:
-            element.append(self._view.etree_element())
-        if self.visibility is not None:
-            visibility = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}visibility",
-            )
-            visibility.text = str(int(self.visibility))
-        if self.isopen:
-            isopen = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}open",
-            )
-            isopen.text = str(int(self.isopen))
-        if self._style_url is not None:
-            element.append(self._style_url.etree_element())
-        for style in self.styles():
-            element.append(style.etree_element())
-        if self.snippet:
-            snippet = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}Snippet",
-            )
-            snippet.text = self.snippet.text
-            if self.snippet.max_lines:
-                snippet.set("maxLines", str(self.snippet.max_lines))
-        elif self._times is not None:
-            element.append(self._times.etree_element())
-        if self._atom_link is not None:
-            element.append(self._atom_link.etree_element())
-        if self._atom_author is not None:
-            element.append(self._atom_author.etree_element())
-        if self.extended_data is not None:
-            element.append(self.extended_data.etree_element())
-        if self._address is not None:
-            address = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}address",
-            )
-            address.text = self._address
-        if self._phone_number is not None:
-            phone_number = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}phoneNumber",
-            )
-            phone_number.text = self._phone_number
+        text_subelement(
+            obj=self,
+            element=element,
+            attr_name="href",
+            node_name="href",
+        )
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -357,200 +363,387 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        name = element.find(f"{ns}name")
-        if name is not None:
-            kwargs["name"] = name.text
-        description = element.find(f"{ns}description")
-        if description is not None:
-            kwargs["description"] = description.text
-        visibility = element.find(f"{ns}visibility")
-        if visibility is not None and visibility.text:
-            kwargs["visibility"] = visibility.text in ["1", "true"]
-        isopen = element.find(f"{ns}open")
-        if isopen is not None:
-            kwargs["isopen"] = isopen.text in ["1", "true"]
-        style_url = element.find(f"{ns}styleUrl")
-        if style_url is not None:
-            kwargs["style_url"] = StyleUrl.class_from_element(
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
                 ns=ns,
-                name_spaces=name_spaces,
-                element=style_url,
+                node_name="href",
+                kwarg="href",
                 strict=strict,
-            )
-        styles = element.findall(f"{ns}Style")
-        kwargs["styles"] = []
-        if styles is not None:
-            for style in styles:
-                kwargs["styles"].append(
-                    Style.class_from_element(
-                        ns=ns,
-                        name_spaces=name_spaces,
-                        element=style,
-                        strict=strict,
-                    ),
-                )
-        stylemaps = element.findall(f"{ns}StyleMap")
-        if stylemaps is not None:
-            for stylemap in stylemaps:
-                kwargs["styles"].append(
-                    StyleMap.class_from_element(
-                        ns=ns,
-                        name_spaces=name_spaces,
-                        element=stylemap,
-                        strict=strict,
-                    ),
-                )
-        snippet = element.find(f"{ns}Snippet")
-        if snippet is not None:
-            max_lines = snippet.get("maxLines")
-            if max_lines is not None:
-                kwargs["snippet"] = Snippet(text=snippet.text, max_lines=int(max_lines))
-            else:
-                kwargs["snippet"] = Snippet(  # type: ignore[unreachable]
-                    text=snippet.text,
-                )
-        timespan = element.find(f"{ns}TimeSpan")
-        if timespan is not None:
-            kwargs["times"] = TimeSpan.class_from_element(
+            ),
+        )
+        return kwargs
+
+
+class IconStyle(_ColorStyle):
+    """Specifies how icons for point Placemarks are drawn."""
+
+    scale: Optional[float]
+    # Resizes the icon. (float)
+    heading: Optional[float]
+    # Direction (that is, North, South, East, West), in degrees.
+    # Default=0 (North).
+    icon_href: Optional[str]
+    # An HTTP address or a local file specification used to load an icon.
+    hot_spot: Optional[HotSpot]
+
+    def __init__(
+        self,
+        ns: Optional[str] = None,
+        name_spaces: Optional[Dict[str, str]] = None,
+        id: Optional[str] = None,
+        target_id: Optional[str] = None,
+        color: Optional[str] = None,
+        color_mode: Optional[ColorMode] = None,
+        scale: float = 1.0,
+        heading: Optional[float] = None,
+        icon: Optional[Icon] = None,
+        hot_spot: Optional[HotSpot] = None,
+    ) -> None:
+        super().__init__(
+            ns=ns,
+            name_spaces=name_spaces,
+            id=id,
+            target_id=target_id,
+            color=color,
+            color_mode=color_mode,
+        )
+
+        self.scale = scale
+        self.heading = heading
+        self.icon = icon
+        self.hot_spot = hot_spot
+
+    def etree_element(
+        self,
+        precision: Optional[int] = None,
+        verbosity: Verbosity = Verbosity.normal,
+    ) -> Element:
+        element = super().etree_element(precision=precision, verbosity=verbosity)
+        float_subelement(
+            obj=self,
+            element=element,
+            attr_name="scale",
+            node_name="scale",
+            precision=precision,
+        )
+        float_subelement(
+            obj=self,
+            element=element,
+            attr_name="heading",
+            node_name="heading",
+            precision=precision,
+        )
+        xml_subelement(
+            obj=self,
+            element=element,
+            attr_name="icon",
+            precision=precision,
+            verbosity=verbosity,
+        )
+        xml_subelement(
+            obj=self,
+            element=element,
+            attr_name="hot_spot",
+            precision=precision,
+            verbosity=verbosity,
+        )
+        return element
+
+    @classmethod
+    def _get_kwargs(
+        cls,
+        *,
+        ns: str,
+        name_spaces: Optional[Dict[str, str]] = None,
+        element: Element,
+        strict: bool,
+    ) -> Dict[str, Any]:
+        kwargs = super()._get_kwargs(
+            ns=ns,
+            name_spaces=name_spaces,
+            element=element,
+            strict=strict,
+        )
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
                 ns=ns,
-                name_spaces=name_spaces,
-                element=timespan,
+                node_name="scale",
+                kwarg="scale",
                 strict=strict,
-            )
-        timestamp = element.find(f"{ns}TimeStamp")
-        if timestamp is not None:
-            kwargs["times"] = TimeStamp.class_from_element(
+            ),
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
                 ns=ns,
-                name_spaces=name_spaces,
-                element=timestamp,
+                node_name="heading",
+                kwarg="heading",
                 strict=strict,
-            )
-        atom_link = element.find(f"{atom.NS}link")
-        if atom_link is not None:
-            kwargs["atom_link"] = atom.Link.class_from_element(
-                ns=atom.NS,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
                 name_spaces=name_spaces,
-                element=atom_link,
+                kwarg="icon",
+                obj_class=Icon,
                 strict=strict,
-            )
-        atom_author = element.find(f"{atom.NS}author")
-        if atom_author is not None:
-            kwargs["atom_author"] = atom.Author.class_from_element(
-                ns=atom.NS,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
                 name_spaces=name_spaces,
-                element=atom_author,
+                kwarg="hot_spot",
+                obj_class=HotSpot,
                 strict=strict,
-            )
-        extended_data = element.find(f"{ns}ExtendedData")
-        if extended_data is not None:
-            kwargs["extended_data"] = ExtendedData.class_from_element(
+            ),
+        )
+        return kwargs
+
+
+class LineStyle(_ColorStyle):
+    """
+    Specifies the drawing style (color, color mode, and line width)
+    for all line geometry. Line geometry includes the outlines of
+    outlined polygons and the extruded "tether" of Placemark icons
+    (if extrusion is enabled).
+    """
+
+    width: Optional[float]
+    # Width of the line, in pixels.
+
+    def __init__(
+        self,
+        ns: Optional[str] = None,
+        name_spaces: Optional[Dict[str, str]] = None,
+        id: Optional[str] = None,
+        target_id: Optional[str] = None,
+        color: Optional[str] = None,
+        color_mode: Optional[ColorMode] = None,
+        width: Optional[float] = None,
+    ) -> None:
+        super().__init__(
+            ns=ns,
+            name_spaces=name_spaces,
+            id=id,
+            target_id=target_id,
+            color=color,
+            color_mode=color_mode,
+        )
+        self.width = width
+
+    def __bool__(self) -> bool:
+        return self.width is not None
+
+    def etree_element(
+        self,
+        precision: Optional[int] = None,
+        verbosity: Verbosity = Verbosity.normal,
+    ) -> Element:
+        element = super().etree_element(precision=precision, verbosity=verbosity)
+        float_subelement(
+            obj=self,
+            element=element,
+            attr_name="width",
+            node_name="width",
+            precision=precision,
+        )
+        return element
+
+    @classmethod
+    def _get_kwargs(
+        cls,
+        *,
+        ns: str,
+        name_spaces: Optional[Dict[str, str]] = None,
+        element: Element,
+        strict: bool,
+    ) -> Dict[str, Any]:
+        kwargs = super()._get_kwargs(
+            ns=ns,
+            name_spaces=name_spaces,
+            element=element,
+            strict=strict,
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
                 ns=ns,
-                element=extended_data,
+                node_name="width",
+                kwarg="width",
                 strict=strict,
-            )
-        address = element.find(f"{ns}address")
-        if address is not None:
-            kwargs["address"] = address.text
-        phone_number = element.find(f"{ns}phoneNumber")
-        if phone_number is not None:
-            kwargs["phone_number"] = phone_number.text
-        camera = element.find(f"{ns}Camera")
-        if camera is not None:
-            kwargs["view"] = Camera.class_from_element(
+            ),
+        )
+        return kwargs
+
+
+class PolyStyle(_ColorStyle):
+    """
+    Drawing style for polygons.
+
+    Specifies the drawing style for all polygons, including polygon
+    extrusions (which look like the walls of buildings) and line
+    extrusions (which look like solid fences).
+
+    https://developers.google.com/kml/documentation/kmlreference#polystyle
+    """
+
+    fill: Optional[bool]
+    # Boolean value. Specifies whether to fill the polygon.
+    outline: Optional[bool]
+    # Boolean value. Specifies whether to outline the polygon.
+    # Polygon outlines use the current LineStyle.
+
+    def __init__(
+        self,
+        ns: Optional[str] = None,
+        name_spaces: Optional[Dict[str, str]] = None,
+        id: Optional[str] = None,
+        target_id: Optional[str] = None,
+        color: Optional[str] = None,
+        color_mode: Optional[ColorMode] = None,
+        fill: Optional[bool] = None,
+        outline: Optional[bool] = None,
+    ) -> None:
+        super().__init__(
+            ns=ns,
+            name_spaces=name_spaces,
+            id=id,
+            target_id=target_id,
+            color=color,
+            color_mode=color_mode,
+        )
+        self.fill = fill
+        self.outline = outline
+
+    def etree_element(
+        self,
+        precision: Optional[int] = None,
+        verbosity: Verbosity = Verbosity.normal,
+    ) -> Element:
+        element = super().etree_element(precision=precision, verbosity=verbosity)
+        bool_subelement(
+            obj=self,
+            element=element,
+            attr_name="fill",
+            node_name="fill",
+        )
+        bool_subelement(
+            obj=self,
+            element=element,
+            attr_name="outline",
+            node_name="outline",
+        )
+        return element
+
+    @classmethod
+    def _get_kwargs(
+        cls,
+        *,
+        ns: str,
+        name_spaces: Optional[Dict[str, str]] = None,
+        element: Element,
+        strict: bool,
+    ) -> Dict[str, Any]:
+        kwargs = super()._get_kwargs(
+            ns=ns,
+            name_spaces=name_spaces,
+            element=element,
+            strict=strict,
+        )
+        kwargs.update(
+            subelement_bool_kwarg(
+                element=element,
                 ns=ns,
-                element=camera,
+                node_name="fill",
+                kwarg="fill",
                 strict=strict,
-            )
-        lookat = element.find(f"{ns}LookAt")
-        if lookat is not None:
-            kwargs["view"] = LookAt.class_from_element(
+            ),
+        )
+        kwargs.update(
+            subelement_bool_kwarg(
+                element=element,
                 ns=ns,
-                element=lookat,
+                node_name="outline",
+                kwarg="outline",
                 strict=strict,
-            )
+            ),
+        )
+
         return kwargs
 
 
-class Placemark(_Feature):
+class LabelStyle(_ColorStyle):
     """
-    A Placemark is a Feature with associated Geometry.
-    In Google Earth, a Placemark appears as a list item in the Places
-    panel. A Placemark with a Point has an icon associated with it that
-    marks a point on the Earth in the 3D viewer.
+    Specifies how the <name> of a Feature is drawn in the 3D viewer.
+
+    A custom color, color mode, and scale for the label (name) can be specified.
+
+    https://developers.google.com/kml/documentation/kmlreference#labelstyle
     """
 
-    __name__ = "Placemark"
-    _geometry: Optional[KmlGeometry]
+    scale: Optional[float]
+    # Resizes the label.
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        name: Optional[str] = None,
-        visibility: Optional[bool] = None,
-        isopen: Optional[bool] = None,
-        atom_link: Optional[atom.Link] = None,
-        atom_author: Optional[atom.Author] = None,
-        address: Optional[str] = None,
-        phone_number: Optional[str] = None,
-        snippet: Optional[Snippet] = None,
-        description: Optional[str] = None,
-        view: Optional[Union[Camera, LookAt]] = None,
-        times: Optional[Union[TimeSpan, TimeStamp]] = None,
-        style_url: Optional[StyleUrl] = None,
-        styles: Optional[Iterable[Union[Style, StyleMap]]] = None,
-        region: Optional[Region] = None,
-        extended_data: Optional[ExtendedData] = None,
-        # Placemark specific
-        geometry: Optional[KmlGeometry] = None,
+        color: Optional[str] = None,
+        color_mode: Optional[ColorMode] = None,
+        scale: Optional[float] = None,
     ) -> None:
         super().__init__(
             ns=ns,
             name_spaces=name_spaces,
             id=id,
             target_id=target_id,
-            name=name,
-            visibility=visibility,
-            isopen=isopen,
-            atom_link=atom_link,
-            atom_author=atom_author,
-            address=address,
-            phone_number=phone_number,
-            snippet=snippet,
-            description=description,
-            view=view,
-            times=times,
-            style_url=style_url,
-            styles=styles,
-            region=region,
-            extended_data=extended_data,
+            color=color,
+            color_mode=color_mode,
         )
-        self._geometry = geometry
+        self.scale = scale
 
-    @property
-    def geometry(self) -> Optional[AnyGeometryType]:
-        return self._geometry.geometry if self._geometry is not None else None
+    def __bool__(self) -> bool:
+        return any(
+            (
+                self.scale is not None,
+                self.color is not None,
+                self.color_mode is not None,
+            ),
+        )
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self._geometry is not None:
-            element.append(self._geometry.etree_element())
-        else:
-            logger.error("Object does not have a geometry")
+        float_subelement(
+            obj=self,
+            element=element,
+            attr_name="scale",
+            node_name="scale",
+            precision=precision,
+        )
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -560,196 +753,433 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        point = element.find(f"{ns}Point")
-        if point is not None:
-            kwargs["geometry"] = Point.class_from_element(
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
                 ns=ns,
-                element=point,
+                node_name="scale",
+                kwarg="scale",
                 strict=strict,
-            )
-            return kwargs
-        line = element.find(f"{ns}LineString")
-        if line is not None:
-            kwargs["geometry"] = LineString.class_from_element(
+            ),
+        )
+
+        return kwargs
+
+
+class BalloonStyle(_BaseObject):
+    """
+    Specifies how the description balloon for placemarks is drawn.
+
+    The <bgColor>, if specified, is used as the background color of the balloon.
+    """
+
+    bg_color: Optional[str]
+    # Background color of the balloon (optional). Color and opacity (alpha)
+    # values are expressed in hexadecimal notation. The range of values for
+    # any one color is 0 to 255 (00 to ff). The order of expression is
+    # aabbggrr, where aa=alpha (00 to ff); bb=blue (00 to ff);
+    # gg=green (00 to ff); rr=red (00 to ff).
+    # For alpha, 00 is fully transparent and ff is fully opaque.
+    # For example, if you want to apply a blue color with 50 percent
+    # opacity to an overlay, you would specify the following:
+    # <bgColor>7fff0000</bgColor>, where alpha=0x7f, blue=0xff, green=0x00,
+    # and red=0x00. The default is opaque white (ffffffff).
+    # Note: The use of the <color> element within <BalloonStyle> has been
+    # deprecated. Use <bgColor> instead.
+
+    text_color: Optional[str]
+    # Foreground color for text. The default is black (ff000000).
+
+    text: Optional[str]
+    # Text displayed in the balloon. If no text is specified, Google Earth
+    # draws the default balloon (with the Feature <name> in boldface,
+    # the Feature <description>, links for driving directions, a white
+    # background, and a tail that is attached to the point coordinates of
+    # the Feature, if specified).
+    # You can add entities to the <text> tag using the following format to
+    # refer to a child element of Feature: $[name], $[description], $[address],
+    # $[id], $[Snippet]. Google Earth looks in the current Feature for the
+    # corresponding string entity and substitutes that information in the
+    # balloon.
+    # To include To here - From here driving directions in the balloon,
+    # use the $[geDirections] tag. To prevent the driving directions links
+    # from appearing in a balloon, include the <text> element with some content
+    # or with $[description] to substitute the basic Feature <description>.
+    # For example, in the following KML excerpt, $[name] and $[description]
+    # fields will be replaced by the <name> and <description> fields found
+    # in the Feature elements that use this BalloonStyle:
+    # <text>This is $[name], whose description is:<br/>$[description]</text>
+
+    display_mode: Optional[DisplayMode]
+    # If <displayMode> is default, Google Earth uses the information supplied
+    # in <text> to create a balloon . If <displayMode> is hide, Google Earth
+    # does not display the balloon. In Google Earth, clicking the List View
+    # icon for a Placemark whose balloon's <displayMode> is hide causes
+    # Google Earth to fly to the Placemark.
+
+    def __init__(
+        self,
+        ns: Optional[str] = None,
+        name_spaces: Optional[Dict[str, str]] = None,
+        id: Optional[str] = None,
+        target_id: Optional[str] = None,
+        bg_color: Optional[str] = None,
+        text_color: Optional[str] = None,
+        text: Optional[str] = None,
+        display_mode: Optional[DisplayMode] = None,
+    ) -> None:
+        super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
+        self.bg_color = bg_color
+        self.text_color = text_color
+        self.text = text
+        self.display_mode = display_mode
+
+    def etree_element(
+        self,
+        precision: Optional[int] = None,
+        verbosity: Verbosity = Verbosity.normal,
+    ) -> Element:
+        element = super().etree_element(precision=precision, verbosity=verbosity)
+        text_subelement(
+            obj=self,
+            element=element,
+            attr_name="bg_color",
+            node_name="bgColor",
+        )
+        text_subelement(
+            obj=self,
+            element=element,
+            attr_name="text_color",
+            node_name="textColor",
+        )
+        text_subelement(
+            obj=self,
+            element=element,
+            attr_name="text",
+            node_name="text",
+        )
+        enum_subelement(
+            obj=self,
+            element=element,
+            attr_name="display_mode",
+            node_name="displayMode",
+        )
+        return element
+
+    @classmethod
+    def _get_kwargs(
+        cls,
+        *,
+        ns: str,
+        name_spaces: Optional[Dict[str, str]] = None,
+        element: Element,
+        strict: bool,
+    ) -> Dict[str, Any]:
+        kwargs = super()._get_kwargs(
+            ns=ns,
+            name_spaces=name_spaces,
+            element=element,
+            strict=strict,
+        )
+
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
                 ns=ns,
-                element=line,
+                node_name="color",
+                kwarg="bg_color",
                 strict=strict,
-            )
-            return kwargs
-        polygon = element.find(f"{ns}Polygon")
-        if polygon is not None:
-            kwargs["geometry"] = Polygon.class_from_element(
+            ),
+        )
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
                 ns=ns,
-                element=polygon,
+                node_name="bgColor",
+                kwarg="bg_color",
                 strict=strict,
-            )
-            return kwargs
-        linearring = element.find(f"{ns}LinearRing")
-        if linearring is not None:
-            kwargs["geometry"] = LinearRing.class_from_element(
+            ),
+        )
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
                 ns=ns,
-                element=linearring,
+                node_name="textColor",
+                kwarg="text_color",
                 strict=strict,
-            )
-            return kwargs
-        multigeometry = element.find(f"{ns}MultiGeometry")
-        if multigeometry is not None:
-            kwargs["geometry"] = MultiGeometry.class_from_element(
+            ),
+        )
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
                 ns=ns,
-                element=multigeometry,
+                node_name="text",
+                kwarg="text",
                 strict=strict,
-            )
-            return kwargs
-        track = element.find(f"{ns}Track")
-        if track is not None:
-            kwargs["geometry"] = gx.Track.class_from_element(
-                ns=config.GXNS,
-                element=track,
-                strict=strict,
-            )
-            return kwargs
-        multitrack = element.find(f"{ns}MultiTrack")
-        if multitrack is not None:
-            kwargs["geometry"] = gx.MultiTrack.class_from_element(
-                ns=config.GXNS,
-                element=multitrack,
+            ),
+        )
+        kwargs.update(
+            subelement_enum_kwarg(
+                element=element,
+                ns=ns,
+                node_name="displayMode",
+                kwarg="display_mode",
+                enum_class=DisplayMode,
                 strict=strict,
-            )
-            return kwargs
-        logger.warning("No geometries found")
-        logger.debug(
-            "Problem with element: %",
-            config.etree.tostring(element),  # type: ignore[attr-defined]
+            ),
         )
         return kwargs
 
 
-class NetworkLink(_Feature):
+AnyStyle = Union[BalloonStyle, IconStyle, LabelStyle, LineStyle, PolyStyle]
+
+
+class Style(_StyleSelector):
+    """
+    A Style defines an addressable style group.
+
+    It can be referenced by StyleMaps and Features.
+    Styles affect how Geometry is presented in the 3D viewer and how Features
+    appear in the Places panel of the List view.
+    Shared styles are collected in a <Document> and must have an id defined for them
+    so that they can be referenced by the individual Features that use them.
     """
-    References a KML file or KMZ archive on a local or remote network.
 
-    Use the <Link> element to specify the location of the KML file.
-    Within that element, you can define the refresh options for updating the file,
-    based on time and camera change.
-    NetworkLinks can be used in combination with Regions to handle very large datasets
-    efficiently.
-    https://developers.google.com/kml/documentation/kmlreference#networklink
+    def __init__(
+        self,
+        ns: Optional[str] = None,
+        name_spaces: Optional[Dict[str, str]] = None,
+        id: Optional[str] = None,
+        target_id: Optional[str] = None,
+        styles: Optional[Iterable[AnyStyle]] = None,
+    ) -> None:
+        super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
+        self.styles = list(styles) if styles else []
+
+    def append_style(
+        self,
+        style: AnyStyle,
+    ) -> None:
+        if isinstance(style, (_ColorStyle, BalloonStyle)):
+            self.styles.append(style)
+        else:
+            raise TypeError
+
+    def etree_element(
+        self,
+        precision: Optional[int] = None,
+        verbosity: Verbosity = Verbosity.normal,
+    ) -> Element:
+        element = super().etree_element(precision=precision, verbosity=verbosity)
+        xml_subelement_list(
+            obj=self,
+            element=element,
+            attr_name="styles",
+            precision=precision,
+            verbosity=verbosity,
+        )
+
+        return element
+
+    @classmethod
+    def _get_kwargs(
+        cls,
+        *,
+        ns: str,
+        name_spaces: Optional[Dict[str, str]] = None,
+        element: Element,
+        strict: bool,
+    ) -> Dict[str, Any]:
+        kwargs = super()._get_kwargs(
+            ns=ns,
+            name_spaces=name_spaces,
+            element=element,
+            strict=strict,
+        )
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+
+        kwargs.update(
+            xml_subelement_list_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="styles",
+                obj_classes=(BalloonStyle, IconStyle, LabelStyle, LineStyle, PolyStyle),
+                strict=strict,
+            ),
+        )
+        return kwargs
 
 
-    Elements Specific to NetworkLink
-    <refreshVisibility>
-    Boolean value.
-    A value of 0 leaves the visibility of features within the control of the
-    Google Earth user.
-    Set the value to 1 to reset the visibility of features each time the NetworkLink is
-    refreshed.
-    For example, suppose a Placemark within the linked KML file has <visibility>
-    set to 1 and the NetworkLink has <refreshVisibility> set to 1.
-    When the file is first loaded into Google Earth, the user can clear the check box
-    next to the item to turn off display in the 3D viewer.
-    However, when the NetworkLink is refreshed, the Placemark will be made
-    visible again, since its original visibility state was TRUE.
-    <flyToView>
-    Boolean value.
-    A value of 1 causes Google Earth to fly to the view of the LookAt or Camera in the
-    NetworkLinkControl (if it exists).
-    If the NetworkLinkControl does not contain an AbstractView element,
-    Google Earth flies to the LookAt or Camera element in the Feature child
-    within the <kml> element in the refreshed file.
-    If the <kml> element does not have a LookAt or Camera specified,
-    the view is unchanged.
-    For example, Google Earth would fly to the <LookAt> view of the parent Document,
-    not the <LookAt> of the Placemarks contained within the Document.
-    <Link>(required)
-       https://developers.google.com/kml/documentation/kmlreference#link
+class Pair(_BaseObject):
     """
+    Stylemap pair.
+
+    Defines a key/value pair that maps a mode (normal or highlight) to the predefined
+    <styleUrl>.
+    <Pair> contains two elements (both are required):
+        <key>, which identifies the key
+        <styleUrl> or <Style>, which references the style.
+        In <styleUrl>, for referenced style elements that are local to the KML document,
+        a simple # referencing is used.
+        For styles that are contained in external files, use a full URL along with
+        # referencing.
 
-    refresh_visibility: Optional[bool]
-    fly_to_view: Optional[bool]
-    _link: Optional[Link]
+    https://developers.google.com/kml/documentation/kmlreference#stylemap
+    """
 
-    __name__ = "NetworkLink"
+    key: Optional[PairKey]
+    style: Optional[Union[StyleUrl, Style]]
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        name: Optional[str] = None,
-        visibility: Optional[bool] = None,
-        isopen: Optional[bool] = None,
-        atom_link: Optional[atom.Link] = None,
-        atom_author: Optional[atom.Author] = None,
-        address: Optional[str] = None,
-        phone_number: Optional[str] = None,
-        snippet: Optional[Snippet] = None,
-        description: Optional[str] = None,
-        view: Optional[Union[Camera, LookAt]] = None,
-        times: Optional[Union[TimeSpan, TimeStamp]] = None,
-        style_url: Optional[StyleUrl] = None,
-        styles: Optional[Iterable[Union[Style, StyleMap]]] = None,
-        region: Optional[Region] = None,
-        extended_data: Optional[ExtendedData] = None,
-        # NetworkLink specific
-        refresh_visibility: Optional[bool] = None,
-        fly_to_view: Optional[bool] = None,
-        link: Optional[Link] = None,
+        key: Optional[PairKey] = None,
+        style: Optional[Union[StyleUrl, Style]] = None,
     ) -> None:
-        super().__init__(
+        super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
+        self.key = key
+        self.style = style
+
+    def __bool__(self) -> bool:
+        return all((self.key is not None, self.style is not None))
+
+    def etree_element(
+        self,
+        precision: Optional[int] = None,
+        verbosity: Verbosity = Verbosity.normal,
+    ) -> Element:
+        element = super().etree_element(precision=precision, verbosity=verbosity)
+        enum_subelement(
+            obj=self,
+            element=element,
+            attr_name="key",
+            node_name="key",
+        )
+        xml_subelement(
+            obj=self,
+            element=element,
+            attr_name="style",
+            precision=precision,
+            verbosity=verbosity,
+        )
+        return element
+
+    @classmethod
+    def _get_kwargs(
+        cls,
+        *,
+        ns: str,
+        name_spaces: Optional[Dict[str, str]] = None,
+        element: Element,
+        strict: bool,
+    ) -> Dict[str, Any]:
+        kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
-            id=id,
-            target_id=target_id,
-            name=name,
-            visibility=visibility,
-            isopen=isopen,
-            atom_link=atom_link,
-            atom_author=atom_author,
-            address=address,
-            phone_number=phone_number,
-            snippet=snippet,
-            description=description,
-            view=view,
-            times=times,
-            style_url=style_url,
-            styles=styles,
-            region=region,
-            extended_data=extended_data,
+            element=element,
+            strict=strict,
+        )
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_enum_kwarg(
+                element=element,
+                ns=ns,
+                node_name="key",
+                kwarg="key",
+                enum_class=PairKey,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="style",
+                obj_class=Style,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="style",
+                obj_class=StyleUrl,
+                strict=strict,
+            ),
+        )
+        return kwargs
+
+
+class StyleMap(_StyleSelector):
+    """
+    A <StyleMap> maps between two different Styles.
+    Typically a <StyleMap> element is used to provide separate normal and highlighted
+    styles for a placemark, so that the highlighted version appears when
+    the user mouses over the icon in Google Earth.
+
+    https://developers.google.com/kml/documentation/kmlreference#stylemap
+    """
+
+    pairs: List[Pair]
+
+    def __init__(
+        self,
+        ns: Optional[str] = None,
+        name_spaces: Optional[Dict[str, str]] = None,
+        id: Optional[str] = None,
+        target_id: Optional[str] = None,
+        pairs: Optional[Iterable[Pair]] = None,
+    ) -> None:
+        super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
+        self.pairs = list(pairs) if pairs else []
+
+    def __bool__(self) -> bool:
+        return bool(self.pairs)
+
+    @property
+    def normal(self) -> Optional[Union[StyleUrl, Style]]:
+        return next(
+            (pair.style for pair in self.pairs if pair.key == PairKey.normal),
+            None,
+        )
+
+    @property
+    def highlight(self) -> Optional[Union[StyleUrl, Style]]:
+        return next(
+            (pair.style for pair in self.pairs if pair.key == PairKey.highlight),
+            None,
         )
-        self.refresh_visibility = refresh_visibility
-        self.fly_to_view = fly_to_view
-        self._link = link
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.refresh_visibility is not None:
-            refresh_visibility = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}refreshVisibility",
-            )
-            refresh_visibility.text = str(int(self.refresh_visibility))
-
-        if self.fly_to_view is not None:
-            fly_to_view = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}flyToView",
-            )
-            fly_to_view.text = str(int(self.fly_to_view))
-        if self.link is not None:
-            element.append(self.link.etree_element())
+        xml_subelement_list(
+            obj=self,
+            element=element,
+            attr_name="pairs",
+            precision=precision,
+            verbosity=verbosity,
+        )
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -759,22 +1189,32 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        visibility = element.find(f"{ns}refreshVisibility")
-        if visibility is not None:
-            kwargs["refresh_visibility"] = bool(int(visibility.text))
-        flyto = element.find(f"{ns}flyToView")
-        if flyto is not None:
-            kwargs["fly_to_view"] = bool(int(flyto.text))
-        link = element.find(f"{ns}Link")
-        if link is not None:
-            kwargs["link"] = Link.class_from_element(
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            xml_subelement_list_kwarg(
+                element=element,
                 ns=ns,
                 name_spaces=name_spaces,
-                element=link,
+                kwarg="pairs",
+                obj_classes=(Pair,),
                 strict=strict,
-            )
+            ),
+        )
         return kwargs
+
+
+__all__ = [
+    "BalloonStyle",
+    "IconStyle",
+    "LabelStyle",
+    "LineStyle",
+    "PolyStyle",
+    "Style",
+    "StyleMap",
+    "StyleUrl",
+]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fastkml-1.0a8/fastkml/geometry.py` & `fastkml-1.0a9/fastkml/geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,35 +10,41 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301 USA
 
-import contextlib
 import logging
 import re
 from functools import partial
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Union
 from typing import cast
 
 import pygeoif.geometry as geo
+from pygeoif.factories import shape
+from pygeoif.types import GeoCollectionType
+from pygeoif.types import GeoType
 from pygeoif.types import PointType
 
 from fastkml import config
 from fastkml.base import _BaseObject
 from fastkml.enums import AltitudeMode
 from fastkml.enums import Verbosity
 from fastkml.exceptions import KMLParseError
 from fastkml.exceptions import KMLWriteError
+from fastkml.helpers import bool_subelement
+from fastkml.helpers import enum_subelement
+from fastkml.helpers import subelement_bool_kwarg
+from fastkml.helpers import subelement_enum_kwarg
 from fastkml.types import Element
 
 __all__ = [
     "AnyGeometryType",
     "GeometryType",
     "LineString",
     "LinearRing",
@@ -70,23 +76,28 @@
                 tessellate: boolean -->  Specifies whether to allow the LineString
                                          to follow the terrain.
                 altitudeMode: --> Specifies how altitude components in the <coordinates>
                                   element are interpreted.
 
     """
 
+    extrude: Optional[bool]
+    tessellate: Optional[bool]
+    altitude_mode: Optional[AltitudeMode]
+    geometry: Optional[AnyGeometryType]
+
     def __init__(
         self,
         *,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        extrude: Optional[bool] = False,
-        tessellate: Optional[bool] = False,
+        extrude: Optional[bool] = None,
+        tessellate: Optional[bool] = None,
         altitude_mode: Optional[AltitudeMode] = None,
         geometry: Optional[AnyGeometryType] = None,
     ) -> None:
         """
 
         Args:
         ----
@@ -95,17 +106,17 @@
             target_id: Target id of the object
             extrude: Specifies whether to connect the feature to the ground with a line.
             tessellate: Specifies whether to allow the LineString to follow the terrain.
             altitude_mode: Specifies how altitude components in the <coordinates>
                            element are interpreted.
         """
         super().__init__(ns=ns, id=id, name_spaces=name_spaces, target_id=target_id)
-        self._extrude = extrude
-        self._tessellate = tessellate
-        self._altitude_mode = altitude_mode
+        self.extrude = extrude
+        self.tessellate = tessellate
+        self.altitude_mode = altitude_mode
         self.geometry = geometry
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}("
             f"ns={self.ns!r}, "
             f"id={self.id!r}, "
@@ -113,98 +124,66 @@
             f"extrude={self.extrude!r}, "
             f"tessellate={self.tessellate!r}, "
             f"altitude_mode={self.altitude_mode} "
             f"geometry={self.geometry!r}"
             f")"
         )
 
-    @property
-    def extrude(self) -> Optional[bool]:
-        return self._extrude
-
-    @extrude.setter
-    def extrude(self, extrude: bool) -> None:
-        self._extrude = extrude
-
-    @property
-    def tessellate(self) -> Optional[bool]:
-        return self._tessellate
-
-    @tessellate.setter
-    def tessellate(self, tessellate: bool) -> None:
-        self._tessellate = tessellate
-
-    @property
-    def altitude_mode(self) -> Optional[AltitudeMode]:
-        return self._altitude_mode
-
-    @altitude_mode.setter
-    def altitude_mode(self, altitude_mode: Optional[AltitudeMode]) -> None:
-        self._altitude_mode = altitude_mode
+    def __bool__(self) -> bool:
+        return bool(self.geometry)
 
     def _etree_coordinates(
         self,
         coordinates: Sequence[PointType],
+        precision: Optional[int],
     ) -> Element:
         element = cast(
             Element,
             config.etree.Element(f"{self.ns}coordinates"),  # type: ignore[attr-defined]
         )
         if not coordinates:
             return element
         if len(coordinates[0]) == 2:
             tuples = (f"{c[0]:f},{c[1]:f}" for c in coordinates)
         elif len(coordinates[0]) == 3:
-            tuples = (f"{c[0]:f},{c[1]:f},{c[2]:f}" for c in coordinates)
+            tuples = (
+                f"{c[0]:f},{c[1]:f},{c[2]:f}" for c in coordinates  # type: ignore[misc]
+            )
         else:
-            msg = f"Invalid dimensions in coordinates '{coordinates}'"
+            msg = (  # type: ignore[unreachable]
+                f"Invalid dimensions in coordinates '{coordinates}'"
+            )
             raise KMLWriteError(msg)
         element.text = " ".join(tuples)
         return element
 
-    def _set_altitude_mode(self, element: Element) -> None:
-        if self.altitude_mode:
-            am_element = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}altitudeMode",
-            )
-            am_element.text = self.altitude_mode.value
-
-    def _set_extrude(self, element: Element) -> None:
-        if self.extrude is not None:
-            et_element = cast(
-                Element,
-                config.etree.SubElement(  # type: ignore[attr-defined]
-                    element,
-                    f"{self.ns}extrude",
-                ),
-            )
-            et_element.text = str(int(self.extrude))
-
-    def _set_tessellate(self, element: Element) -> None:
-        if self.tessellate is not None:
-            t_element = cast(
-                Element,
-                config.etree.SubElement(  # type: ignore[attr-defined]
-                    element,
-                    f"{self.ns}tessellate",
-                ),
-            )
-            t_element.text = str(int(self.tessellate))
-
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
-        self.__name__ = self.__class__.__name__
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        self._set_extrude(element)
-        self._set_altitude_mode(element)
-        self._set_tessellate(element)
+        bool_subelement(
+            self,
+            element=element,
+            attr_name="extrude",
+            node_name="extrude",
+        )
+        bool_subelement(
+            self,
+            element=element,
+            attr_name="tessellate",
+            node_name="tessellate",
+        )
+        enum_subelement(
+            self,
+            element=element,
+            attr_name="altitude_mode",
+            node_name="altitudeMode",
+        )
         return element
 
     @classmethod
     def _get_coordinates(
         cls,
         *,
         ns: str,
@@ -231,77 +210,14 @@
             return [
                 cast(PointType, tuple(float(c) for c in latlon.split(",")))
                 for latlon in latlons
             ]
         return []
 
     @classmethod
-    def _get_extrude(
-        cls,
-        *,
-        ns: str,
-        element: Element,
-        strict: bool,
-    ) -> Optional[bool]:
-        extrude = element.find(f"{ns}extrude")
-        if extrude is None:
-            return None
-        with contextlib.suppress(ValueError, AttributeError):
-            return bool(int(extrude.text.strip()))
-        return None
-
-    @classmethod
-    def _get_tessellate(
-        cls,
-        *,
-        ns: str,
-        element: Element,
-        strict: bool,
-    ) -> Optional[bool]:
-        tessellate = element.find(f"{ns}tessellate")
-        if tessellate is None:
-            return None
-        with contextlib.suppress(ValueError):
-            return bool(int(tessellate.text.strip()))
-        return None
-
-    @classmethod
-    def _get_altitude_mode(
-        cls,
-        *,
-        ns: str,
-        element: Element,
-        strict: bool,
-    ) -> Optional[AltitudeMode]:
-        altitude_mode = element.find(f"{ns}altitudeMode")
-        if altitude_mode is None:
-            return None
-        with contextlib.suppress(ValueError):
-            return AltitudeMode(altitude_mode.text.strip())
-        return None
-
-    @classmethod
-    def _get_geometry_kwargs(
-        cls,
-        *,
-        ns: str,
-        element: Element,
-        strict: bool,
-    ) -> Dict[str, Any]:
-        return {
-            "extrude": cls._get_extrude(ns=ns, element=element, strict=strict),
-            "tessellate": cls._get_tessellate(ns=ns, element=element, strict=strict),
-            "altitude_mode": cls._get_altitude_mode(
-                ns=ns,
-                element=element,
-                strict=strict,
-            ),
-        }
-
-    @classmethod
     def _get_geometry(
         cls,
         *,
         ns: str,
         element: Element,
         strict: bool,
     ) -> Optional[AnyGeometryType]:
@@ -318,31 +234,58 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        kwargs.update(cls._get_geometry_kwargs(ns=ns, element=element, strict=strict))
+        kwargs.update(
+            subelement_bool_kwarg(
+                element=element,
+                ns=ns,
+                node_name="extrude",
+                kwarg="extrude",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_bool_kwarg(
+                element=element,
+                ns=ns,
+                node_name="tessellate",
+                kwarg="tessellate",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_enum_kwarg(
+                element=element,
+                ns=ns,
+                node_name="altitudeMode",
+                kwarg="altitude_mode",
+                enum_class=AltitudeMode,
+                strict=strict,
+            ),
+        )
         kwargs.update(
             {"geometry": cls._get_geometry(ns=ns, element=element, strict=strict)},
         )
         return kwargs
 
 
 class Point(_Geometry):
     def __init__(
         self,
         *,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        extrude: Optional[bool] = False,
-        tessellate: Optional[bool] = False,
+        extrude: Optional[bool] = None,
+        tessellate: Optional[bool] = None,
         altitude_mode: Optional[AltitudeMode] = None,
         geometry: geo.Point,
     ) -> None:
         super().__init__(
             ns=ns,
             id=id,
             name_spaces=name_spaces,
@@ -354,19 +297,18 @@
         )
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
-        self.__name__ = self.__class__.__name__
         element = super().etree_element(precision=precision, verbosity=verbosity)
         assert isinstance(self.geometry, geo.Point)
         coords = self.geometry.coords
-        element.append(self._etree_coordinates(coords))
+        element.append(self._etree_coordinates(coords, precision=precision))
         return element
 
     @classmethod
     def _get_geometry(
         cls,
         *,
         ns: str,
@@ -391,16 +333,16 @@
     def __init__(
         self,
         *,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        extrude: Optional[bool] = False,
-        tessellate: Optional[bool] = False,
+        extrude: Optional[bool] = None,
+        tessellate: Optional[bool] = None,
         altitude_mode: Optional[AltitudeMode] = None,
         geometry: geo.LineString,
     ) -> None:
         super().__init__(
             ns=ns,
             name_spaces=name_spaces,
             id=id,
@@ -412,19 +354,18 @@
         )
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
-        self.__name__ = self.__class__.__name__
         element = super().etree_element(precision=precision, verbosity=verbosity)
         assert isinstance(self.geometry, geo.LineString)
         coords = self.geometry.coords
-        element.append(self._etree_coordinates(coords))
+        element.append(self._etree_coordinates(coords, precision=precision))
         return element
 
     @classmethod
     def _get_geometry(
         cls,
         *,
         ns: str,
@@ -449,16 +390,16 @@
     def __init__(
         self,
         *,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        extrude: Optional[bool] = False,
-        tessellate: Optional[bool] = False,
+        extrude: Optional[bool] = None,
+        tessellate: Optional[bool] = None,
         altitude_mode: Optional[AltitudeMode] = None,
         geometry: geo.LinearRing,
     ) -> None:
         super().__init__(
             ns=ns,
             name_spaces=name_spaces,
             id=id,
@@ -495,16 +436,16 @@
     def __init__(
         self,
         *,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        extrude: Optional[bool] = False,
-        tessellate: Optional[bool] = False,
+        extrude: Optional[bool] = None,
+        tessellate: Optional[bool] = None,
         altitude_mode: Optional[AltitudeMode] = None,
         geometry: geo.Polygon,
     ) -> None:
         super().__init__(
             ns=ns,
             name_spaces=name_spaces,
             id=id,
@@ -516,15 +457,14 @@
         )
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
-        self.__name__ = self.__class__.__name__
         element = super().etree_element(precision=precision, verbosity=verbosity)
         assert isinstance(self.geometry, geo.Polygon)
         linear_ring = partial(LinearRing, ns=self.ns, extrude=None, tessellate=None)
         outer_boundary = cast(
             Element,
             config.etree.SubElement(  # type: ignore[attr-defined]
                 element,
@@ -617,15 +557,15 @@
         map_to_geometries = {
             geo.Point.__name__: geo.MultiPoint.from_points,
             geo.LineString.__name__: geo.MultiLineString.from_linestrings,
             geo.Polygon.__name__: geo.MultiPolygon.from_polygons,
         }
         for geometry_name, constructor in map_to_geometries.items():
             if geom_type == geometry_name:
-                return constructor(
+                return constructor(  # type: ignore[operator, no-any-return]
                     *geometries,
                 )
 
     return geo.GeometryCollection(geometries)
 
 
 class MultiGeometry(_Geometry):
@@ -645,16 +585,16 @@
     def __init__(
         self,
         *,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        extrude: Optional[bool] = False,
-        tessellate: Optional[bool] = False,
+        extrude: Optional[bool] = None,
+        tessellate: Optional[bool] = None,
         altitude_mode: Optional[AltitudeMode] = None,
         geometry: MultiGeometryType,
     ) -> None:
         super().__init__(
             ns=ns,
             name_spaces=name_spaces,
             id=id,
@@ -666,30 +606,30 @@
         )
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
-        self.__name__ = self.__class__.__name__
         element = super().etree_element(precision=precision, verbosity=verbosity)
         _map_to_kml = {mg: self.__class__ for mg in self.multi_geometries}
         _map_to_kml.update(self.map_to_kml)
         if self.geometry is None:
             return element
         assert isinstance(self.geometry, self.multi_geometries)
         for geometry in self.geometry.geoms:
             geometry_class = _map_to_kml[type(geometry)]
             element.append(
                 geometry_class(
                     ns=self.ns,
+                    name_spaces=self.name_spaces,
                     extrude=None,
                     tessellate=None,
                     altitude_mode=None,
-                    geometry=geometry,
+                    geometry=geometry,  # type: ignore[arg-type]
                 ).etree_element(precision=precision, verbosity=verbosity),
             )
         return element
 
     @classmethod
     def _get_geometry(
         cls,
@@ -706,7 +646,67 @@
                     ns=ns,
                     element=e,
                     strict=strict,
                 )
                 if geometry is not None:
                     geometries.append(geometry)
         return create_multigeometry(geometries)
+
+
+def create_kml_geometry(
+    geometry: Union[GeoType, GeoCollectionType],
+    *,
+    ns: Optional[str] = None,
+    name_spaces: Optional[Dict[str, str]] = None,
+    id: Optional[str] = None,
+    target_id: Optional[str] = None,
+    extrude: Optional[bool] = None,
+    tessellate: Optional[bool] = None,
+    altitude_mode: Optional[AltitudeMode] = None,
+) -> _Geometry:
+    """
+    Create a KML geometry from a geometry object.
+
+    Args:
+    ----
+        geometry: Geometry object.
+        ns: Namespace of the object
+        id: Id of the object
+        target_id: Target id of the object
+        extrude: Specifies whether to connect the feature to the ground with a line.
+        tessellate: Specifies whether to allow the LineString to follow the terrain.
+        altitude_mode: Specifies how altitude components in the <coordinates>
+                       element are interpreted.
+
+    Returns:
+    -------
+        KML geometry object.
+
+    """
+    _map_to_kml = {
+        geo.Point: Point,
+        geo.Polygon: Polygon,
+        geo.LinearRing: LinearRing,
+        geo.LineString: LineString,
+        geo.MultiPoint: MultiGeometry,
+        geo.MultiLineString: MultiGeometry,
+        geo.MultiPolygon: MultiGeometry,
+        geo.GeometryCollection: MultiGeometry,
+    }
+    geom = shape(geometry)
+    for geometry_class, kml_class in _map_to_kml.items():
+        if isinstance(geom, geometry_class):
+            return cast(
+                _Geometry,
+                kml_class(
+                    ns=ns,
+                    name_spaces=name_spaces,
+                    id=id,
+                    target_id=target_id,
+                    extrude=extrude,
+                    tessellate=tessellate,
+                    altitude_mode=altitude_mode,
+                    geometry=geom,
+                ),
+            )
+    msg = f"Unsupported geometry type {type(geometry)}"
+    raise KMLWriteError(msg)
```

### Comparing `fastkml-1.0a8/fastkml/gx.py` & `fastkml-1.0a9/fastkml/gx.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 * gx:Wait
 * gx:x
 * gx:y
 
 The complete XML schema for elements in this extension namespace is
 located at http://developers.google.com/kml/schema/kml22gx.xsd.
 """
-import contextlib
 import datetime
 import logging
 from dataclasses import dataclass
 from itertools import zip_longest
 from typing import Any
 from typing import Dict
 from typing import Iterator
@@ -91,14 +90,18 @@
 import arrow
 import pygeoif.geometry as geo
 
 from fastkml import config
 from fastkml.enums import AltitudeMode
 from fastkml.enums import Verbosity
 from fastkml.geometry import _Geometry
+from fastkml.helpers import bool_subelement
+from fastkml.helpers import subelement_bool_kwarg
+from fastkml.helpers import xml_subelement_list
+from fastkml.helpers import xml_subelement_list_kwarg
 from fastkml.types import Element
 
 __all__ = [
     "Angle",
     "MultiTrack",
     "Track",
     "TrackItem",
@@ -192,16 +195,16 @@
     def __init__(
         self,
         *,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        extrude: Optional[bool] = False,
-        tessellate: Optional[bool] = False,
+        extrude: Optional[bool] = None,
+        tessellate: Optional[bool] = None,
         altitude_mode: Optional[AltitudeMode] = None,
         geometry: Optional[geo.LineString] = None,
         track_items: Optional[Sequence[TrackItem]] = None,
     ) -> None:
         if geometry and track_items:
             msg = "Cannot specify both geometry and track_items"
             raise ValueError(msg)
@@ -217,34 +220,20 @@
             target_id=target_id,
             extrude=extrude,
             tessellate=tessellate,
             altitude_mode=altitude_mode,
             geometry=geometry,
         )
 
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}("
-            f"ns={self.ns!r}, "
-            f"id={self.id!r}, "
-            f"target_id={self.target_id!r}, "
-            f"extrude={self.extrude!r}, "
-            f"tessellate={self.tessellate!r}, "
-            f"altitude_mode={self.altitude_mode}, "
-            f"track_items={self.track_items!r}"
-            ")"
-        )
-
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
         name_spaces: Optional[Dict[str, str]] = None,
     ) -> Element:
-        self.__name__ = self.__class__.__name__
         element = super().etree_element(precision=precision, verbosity=verbosity)
         if self.track_items:
             for track_item in self.track_items:
                 for track_item_element in track_item.etree_elements(
                     precision=precision,
                     verbosity=verbosity,
                     name_spaces=name_spaces,
@@ -325,117 +314,63 @@
     def __init__(
         self,
         *,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        extrude: Optional[bool] = False,
-        tessellate: Optional[bool] = False,
+        extrude: Optional[bool] = None,
+        tessellate: Optional[bool] = None,
         altitude_mode: Optional[AltitudeMode] = None,
         geometry: Optional[geo.MultiLineString] = None,
         tracks: Optional[Sequence[Track]] = None,
         interpolate: Optional[bool] = None,
     ) -> None:
         if geometry and tracks:
             msg = "Cannot specify both geometry and track_items"
             raise ValueError(msg)
         if geometry:
             tracks = multilinestring_to_tracks(geometry, ns=ns)
         elif tracks:
             geometry = tracks_to_geometry(tracks)
-        self.tracks = tracks
+        self.tracks = tracks or []
         self.interpolate = interpolate
         super().__init__(
             ns=ns,
             name_spaces=name_spaces,
             id=id,
             target_id=target_id,
             extrude=extrude,
             tessellate=tessellate,
             altitude_mode=altitude_mode,
             geometry=geometry,
         )
 
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}("
-            f"ns={self.ns!r}, "
-            f"id={self.id!r}, "
-            f"target_id={self.target_id!r}, "
-            f"extrude={self.extrude!r}, "
-            f"tessellate={self.tessellate!r}, "
-            f"altitude_mode={self.altitude_mode}, "
-            f"tracks={self.tracks!r}, "
-            f"interpolate={self.interpolate!r}"
-            ")"
-        )
-
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
         name_spaces: Optional[Dict[str, str]] = None,
     ) -> Element:
-        self.__name__ = self.__class__.__name__
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.interpolate is not None:
-            i_element = cast(
-                Element,
-                config.etree.SubElement(  # type: ignore[attr-defined]
-                    element,
-                    f"{self.ns}interpolate",
-                ),
-            )
-            i_element.text = str(int(self.interpolate))
-        for track in self.tracks or []:
-            element.append(
-                track.etree_element(
-                    precision=precision,
-                    verbosity=verbosity,
-                    name_spaces=name_spaces,
-                ),
-            )
-        return element
-
-    @classmethod
-    def _get_interpolate(
-        cls,
-        *,
-        ns: str,
-        element: Element,
-        strict: bool,
-    ) -> Optional[bool]:
-        interpolate = element.find(f"{ns}interpolate")
-        if interpolate is None:
-            return None
-        with contextlib.suppress(ValueError):
-            return bool(int(interpolate.text.strip()))
-        return None
+        bool_subelement(
+            self,
+            element=element,
+            attr_name="interpolate",
+            node_name="interpolate",
+        )
+        xml_subelement_list(
+            self,
+            element=element,
+            attr_name="tracks",
+            precision=precision,
+            verbosity=verbosity,
+        )
 
-    @classmethod
-    def _get_track_kwargs_from_element(
-        cls,
-        *,
-        ns: str,
-        element: Element,
-        strict: bool,
-    ) -> List[Track]:
-        return [
-            cast(
-                Track,
-                Track.class_from_element(
-                    ns=ns,
-                    element=track,
-                    strict=strict,
-                ),
-            )
-            for track in element.findall(f"{ns}Track")
-            if track is not None
-        ]
+        return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
         name_spaces: Optional[Dict[str, str]] = None,
@@ -444,18 +379,30 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        kwargs["interpolate"] = cls._get_interpolate(
-            ns=ns,
-            element=element,
-            strict=strict,
-        )
-        kwargs["tracks"] = cls._get_track_kwargs_from_element(
-            ns=kwargs["name_spaces"].get("gx", ""),
-            element=element,
-            strict=strict,
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_bool_kwarg(
+                element=element,
+                ns=ns,
+                node_name="interpolate",
+                kwarg="interpolate",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_list_kwarg(
+                element=element,
+                ns=name_spaces["gx"],
+                name_spaces=name_spaces,
+                kwarg="tracks",
+                obj_classes=(Track,),
+                strict=strict,
+            ),
         )
+
         return kwargs
```

### Comparing `fastkml-1.0a8/fastkml/kml.py` & `fastkml-1.0a9/fastkml/kml.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2012-2022  Christian Ledermann
+# Copyright (C) 2012-2023 Christian Ledermann
 #
 # This library is free software; you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation; either version 2.1 of the License, or (at your option)
 # any later version.
 #
 # This library is distributed in the hope that it will be useful, but WITHOUT
@@ -24,36 +24,39 @@
 http://schemas.opengis.net/kml/.
 
 """
 import logging
 from typing import Any
 from typing import Dict
 from typing import Iterable
-from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Union
 from typing import cast
 
 from fastkml import config
 from fastkml.base import _XMLObject
 from fastkml.containers import Document
 from fastkml.containers import Folder
 from fastkml.enums import Verbosity
 from fastkml.features import Placemark
+from fastkml.helpers import xml_subelement_list
+from fastkml.helpers import xml_subelement_list_kwarg
 from fastkml.overlays import GroundOverlay
 from fastkml.overlays import PhotoOverlay
 from fastkml.types import Element
 
 logger = logging.getLogger(__name__)
 
 
 class KML(_XMLObject):
     """represents a KML File."""
 
+    _default_ns = config.KMLNS
+
     _features: List[Union[Folder, Document, Placemark]]
     ns: str
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
@@ -64,15 +67,15 @@
         undesired. Note that all child elements like Document or Placemark need
         to be initialized with empty namespace as well in this case.
         """
         super().__init__(
             ns=ns,
             name_spaces=name_spaces,
         )
-        self._features = list(features) if features is not None else []
+        self.features = list(features) if features is not None else []
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         # self.ns may be empty, which leads to unprefixed kml elements.
@@ -81,34 +84,34 @@
         if not self.ns:
             root = config.etree.Element(f"{self.ns}kml")  # type: ignore[attr-defined]
             root.set("xmlns", config.KMLNS[1:-1])
         else:
             try:
                 root = config.etree.Element(  # type: ignore[attr-defined]
                     f"{self.ns}kml",
-                    # nsmap={None: self.ns[1:-1]},
                 )
             except TypeError:
                 root = config.etree.Element(  # type: ignore[attr-defined]
                     f"{self.ns}kml",
                 )
-        for feature in self.features():
-            root.append(feature.etree_element(precision=precision, verbosity=verbosity))
+        xml_subelement_list(
+            obj=self,
+            element=root,
+            attr_name="features",
+            precision=precision,
+            verbosity=verbosity,
+        )
         return cast(Element, root)
 
-    def features(self) -> Iterator[Union[Folder, Document, Placemark]]:
-        """Iterate over features."""
-        yield from self._features
-
     def append(self, kmlobj: Union[Folder, Document, Placemark]) -> None:
         """Append a feature."""
-        if id(kmlobj) == id(self):
+        if kmlobj is self:
             msg = "Cannot append self"
             raise ValueError(msg)
-        self._features.append(kmlobj)
+        self.features.append(kmlobj)
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
         name_spaces: Optional[Dict[str, str]] = None,
@@ -117,60 +120,27 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
         kwargs["features"] = []
-        documents = element.findall(f"{ns}Document")
-        for document in documents:
-            kwargs["features"].append(
-                Document.class_from_element(
-                    ns=ns,
-                    element=document,
-                    strict=False,
-                ),
-            )
-        folders = element.findall(f"{ns}Folder")
-        for folder in folders:
-            kwargs["features"].append(
-                Folder.class_from_element(
-                    ns=ns,
-                    element=folder,
-                    strict=False,
-                ),
-            )
-        placemarks = element.findall(f"{ns}Placemark")
-        for placemark in placemarks:
-            kwargs["features"].append(
-                Placemark.class_from_element(
-                    ns=ns,
-                    element=placemark,
-                    strict=False,
-                ),
-            )
-        groundoverlays = element.findall(f"{ns}GroundOverlay")
-        for groundoverlay in groundoverlays:
-            kwargs["features"].append(
-                GroundOverlay.class_from_element(
-                    ns=ns,
-                    element=groundoverlay,
-                    strict=False,
-                ),
-            )
-        photo_overlays = element.findall(f"{ns}PhotoOverlay")
-        for photo_overlay in photo_overlays:
-            kwargs["features"].append(
-                PhotoOverlay.class_from_element(
-                    ns=ns,
-                    element=photo_overlay,
-                    strict=False,
-                ),
-            )
+        kwargs.update(
+            xml_subelement_list_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="features",
+                obj_classes=(Document, Folder, Placemark, GroundOverlay, PhotoOverlay),
+                strict=strict,
+            ),
+        )
         return kwargs
 
     @classmethod
     def class_from_string(
         cls,
         string: str,
         *,
@@ -199,23 +169,20 @@
             )
         except TypeError:
             element = config.etree.XML(string)  # type: ignore[attr-defined]
         if not element.tag.endswith("kml"):
             raise TypeError
         if ns is None:
             ns = cast(str, element.tag.rstrip("kml"))
+        name_spaces = name_spaces or {}
+        name_spaces = {**config.NAME_SPACES, **name_spaces}
         return cls.class_from_element(
             ns=ns,
             name_spaces=name_spaces,
             strict=strict,
             element=element,
         )
 
 
 __all__ = [
-    "Document",
-    "Folder",
-    "PhotoOverlay",
-    "GroundOverlay",
     "KML",
-    "Placemark",
 ]
```

### Comparing `fastkml-1.0a8/fastkml/mixins.py` & `fastkml-1.0a9/fastkml/mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 from fastkml.times import TimeSpan
 from fastkml.times import TimeStamp
 
 logger = logging.getLogger(__name__)
 
 
 class TimeMixin:
-    _times: Optional[Union[TimeSpan, TimeStamp]] = None
+    times: Optional[Union[TimeSpan, TimeStamp]] = None
 
     @property
     def time_stamp(self) -> Optional[KmlDateTime]:
         """This just returns the datetime portion of the timestamp."""
-        return self._times.timestamp if isinstance(self._times, TimeStamp) else None
+        return self.times.timestamp if isinstance(self.times, TimeStamp) else None
 
     @property
     def begin(self) -> Optional[KmlDateTime]:
-        return self._times.begin if isinstance(self._times, TimeSpan) else None
+        return self.times.begin if isinstance(self.times, TimeSpan) else None
 
     @property
     def end(self) -> Optional[KmlDateTime]:
-        return self._times.end if isinstance(self._times, TimeSpan) else None
+        return self.times.end if isinstance(self.times, TimeSpan) else None
```

### Comparing `fastkml-1.0a8/fastkml/overlays.py` & `fastkml-1.0a9/fastkml/overlays.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,30 @@
+# Copyright (C) 2023  Christian Ledermann
+#
+# This library is free software; you can redistribute it and/or modify it under
+# the terms of the GNU Lesser General Public License as published by the Free
+# Software Foundation; either version 2.1 of the License, or (at your option)
+# any later version.
+#
+# This library is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+# FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
+# details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with this library; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301 USA
 """Overlays."""
 
 import logging
 from typing import Any
 from typing import Dict
 from typing import Iterable
 from typing import Optional
 from typing import Union
-from typing import cast
 
 from fastkml import atom
 from fastkml import config
 from fastkml import gx
 from fastkml.base import _XMLObject
 from fastkml.data import ExtendedData
 from fastkml.enums import AltitudeMode
@@ -20,14 +34,24 @@
 from fastkml.features import Snippet
 from fastkml.features import _Feature
 from fastkml.geometry import LinearRing
 from fastkml.geometry import LineString
 from fastkml.geometry import MultiGeometry
 from fastkml.geometry import Point
 from fastkml.geometry import Polygon
+from fastkml.helpers import enum_subelement
+from fastkml.helpers import float_subelement
+from fastkml.helpers import int_subelement
+from fastkml.helpers import subelement_enum_kwarg
+from fastkml.helpers import subelement_float_kwarg
+from fastkml.helpers import subelement_int_kwarg
+from fastkml.helpers import subelement_text_kwarg
+from fastkml.helpers import text_subelement
+from fastkml.helpers import xml_subelement
+from fastkml.helpers import xml_subelement_kwarg
 from fastkml.links import Icon
 from fastkml.styles import Style
 from fastkml.styles import StyleMap
 from fastkml.styles import StyleUrl
 from fastkml.times import TimeSpan
 from fastkml.times import TimeStamp
 from fastkml.types import Element
@@ -54,26 +78,26 @@
 
     Base type for image overlays drawn on the planet surface or on the screen
 
     A Container element holds one or more Features and allows the creation of
     nested hierarchies.
     """
 
-    _color: Optional[str]
+    color: Optional[str]
     # Color values expressed in hexadecimal notation, including opacity (alpha)
     # values. The order of expression is alphaOverlay, blue, green, red
     # (AABBGGRR). The range of values for any one color is 0 to 255 (00 to ff).
     # For opacity, 00 is fully transparent and ff is fully opaque.
 
-    _draw_order: Optional[int]
+    draw_order: Optional[int]
     # Defines the stacking order for the images in overlapping overlays.
     # Overlays with higher <drawOrder> values are drawn on top of those with
     # lower <drawOrder> values.
 
-    _icon: Optional[Icon]
+    icon: Optional[Icon]
     # Defines the image associated with the overlay. Contains an <href> html
     # tag which defines the location of the image to be used as the overlay.
     # The location can be either on a local file system or on a webserver. If
     # this element is omitted or contains no <href>, a rectangle is drawn using
     # the color and size defined by the ground or screen overlay.
 
     def __init__(
@@ -119,62 +143,43 @@
             view=view,
             times=times,
             style_url=style_url,
             styles=styles,
             region=region,
             extended_data=extended_data,
         )
-        self._icon = icon
-        self._color = color
-        self._draw_order = draw_order
-
-    @property
-    def color(self) -> Optional[str]:
-        return self._color
-
-    @color.setter
-    def color(self, color: Optional[str]) -> None:
-        self._color = color
-
-    @property
-    def draw_order(self) -> Optional[int]:
-        return self._draw_order
-
-    @draw_order.setter
-    def draw_order(self, value: Optional[int]) -> None:
-        self._draw_order = value
-
-    @property
-    def icon(self) -> Optional[Icon]:
-        return self._icon
-
-    @icon.setter
-    def icon(self, value: Optional[Icon]) -> None:
-        self._icon = value
+        self.icon = icon
+        self.color = color
+        self.draw_order = draw_order
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self._color:
-            color = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}color",
-            )
-            color.text = self._color
-        if self._draw_order:
-            draw_order = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}drawOrder",
-            )
-            draw_order.text = str(self._draw_order)
-        if self._icon:
-            element.append(self._icon.etree_element())
+        text_subelement(
+            self,
+            element=element,
+            attr_name="color",
+            node_name="color",
+        )
+        int_subelement(
+            self,
+            element=element,
+            attr_name="draw_order",
+            node_name="drawOrder",
+        )
+        xml_subelement(
+            self,
+            element=element,
+            attr_name="icon",
+            precision=precision,
+            verbosity=verbosity,
+        )
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -184,31 +189,44 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        color = element.find(f"{ns}color")
-        if color is not None:
-            kwargs["color"] = color.text
-        draw_order = element.find(f"{ns}drawOrder")
-        if draw_order is not None:
-            kwargs["draw_order"] = int(draw_order.text)
-        icon = element.find(f"{ns}Icon")
-        if icon is not None:
-            kwargs["icon"] = cast(
-                Icon,
-                Icon.class_from_element(
-                    ns=ns,
-                    name_spaces=name_spaces,
-                    element=icon,
-                    strict=strict,
-                ),
-            )
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="color",
+                kwarg="color",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_int_kwarg(
+                element=element,
+                ns=ns,
+                node_name="drawOrder",
+                kwarg="draw_order",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="icon",
+                obj_class=Icon,
+                strict=strict,
+            ),
+        )
         return kwargs
 
 
 class ViewVolume(_XMLObject):
     """
     The ViewVolume defines how much of the current scene is visible.
 
@@ -216,14 +234,16 @@
     physical camera.
     A small field of view, like a telephoto lens, focuses on a small part of the scene.
     A large field of view, like a wide-angle lens, focuses on a large part of the scene.
 
     https://developers.google.com/kml/documentation/kmlreference#viewvolume
     """
 
+    _default_ns = config.KMLNS
+
     left_fow: Optional[float]
     # Angle, in degrees, between the camera's viewing direction and the left side
     # of the view volume.
 
     right_fov: Optional[float]
     # Angle, in degrees, between the camera's viewing direction and the right side
     # of the view volume.
@@ -270,39 +290,49 @@
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        left_fov = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}leftFov",
-        )
-        left_fov.text = str(self.left_fov)
-        right_fov = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}rightFov",
-        )
-        right_fov.text = str(self.right_fov)
-        bottom_fov = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}bottomFov",
-        )
-        bottom_fov.text = str(self.bottom_fov)
-        top_fov = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}topFov",
-        )
-        top_fov.text = str(self.top_fov)
-        near = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}near",
+        float_subelement(
+            self,
+            element=element,
+            attr_name="left_fov",
+            node_name="leftFov",
+            precision=precision,
+        )
+        float_subelement(
+            self,
+            element=element,
+            attr_name="right_fov",
+            node_name="rightFov",
+            precision=precision,
+        )
+        float_subelement(
+            self,
+            element=element,
+            attr_name="bottom_fov",
+            node_name="bottomFov",
+            precision=precision,
+        )
+        float_subelement(
+            self,
+            element=element,
+            attr_name="top_fov",
+            node_name="topFov",
+            precision=precision,
+        )
+        float_subelement(
+            self,
+            element=element,
+            attr_name="near",
+            node_name="near",
+            precision=precision,
         )
-        near.text = str(self.near)
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -312,29 +342,71 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        left_fov = element.find(f"{ns}leftFov")
-        if left_fov is not None:
-            kwargs["left_fov"] = float(left_fov.text)
-        right_fov = element.find(f"{ns}rightFov")
-        if right_fov is not None:
-            kwargs["right_fov"] = float(right_fov.text)
-        bottom_fov = element.find(f"{ns}bottomFov")
-        if bottom_fov is not None:
-            kwargs["bottom_fov"] = float(bottom_fov.text)
-        top_fov = element.find(f"{ns}topFov")
-        if top_fov is not None:
-            kwargs["top_fov"] = float(top_fov.text)
-        near = element.find(f"{ns}near")
-        if near is not None:
-            kwargs["near"] = float(near.text)
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="leftFov",
+                kwarg="left_fov",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="rightFov",
+                kwarg="right_fov",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="bottomFov",
+                kwarg="bottom_fov",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="topFov",
+                kwarg="top_fov",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="near",
+                kwarg="near",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="near",
+                kwarg="near",
+                strict=strict,
+            ),
+        )
+
         return kwargs
 
 
 class ImagePyramid(_XMLObject):
     """
     For very large images, you'll need to construct an image pyramid.
 
@@ -351,14 +423,16 @@
     loads only the portions of the image that are in view, and only the pixel details
     that can be discerned by the user at the current viewpoint.
 
     When you specify an image pyramid, you also need to modify the <href> in the <Icon>
     element to include specifications for which tiles to load.
     """
 
+    _default_ns = config.KMLNS
+
     tile_size: Optional[int]
     # Size of the tiles, in pixels. Tiles must be square, and <tileSize> must be a power
     # of 2. A tile size of 256 (the default) or 512 is recommended.
     # The original image is divided into tiles of this size, at varying resolutions.
 
     max_width: Optional[int]
     # Width in pixels of the original image.
@@ -396,35 +470,39 @@
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        tile_size = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}tileSize",
-        )
-        tile_size.text = str(self.tile_size)
-        max_width = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}maxWidth",
-        )
-        max_width.text = str(self.max_width)
-        max_height = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}maxHeight",
-        )
-        max_height.text = str(self.max_height)
-        grid_origin = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}gridOrigin",
+        int_subelement(
+            self,
+            element=element,
+            attr_name="tile_size",
+            node_name="tileSize",
+        )
+        int_subelement(
+            self,
+            element=element,
+            attr_name="max_width",
+            node_name="maxWidth",
+        )
+        int_subelement(
+            self,
+            element=element,
+            attr_name="max_height",
+            node_name="maxHeight",
+        )
+        enum_subelement(
+            self,
+            element=element,
+            attr_name="grid_origin",
+            node_name="gridOrigin",
         )
-        assert self.grid_origin is not None
-        grid_origin.text = self.grid_origin.value
+
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -434,26 +512,53 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        tile_size = element.find(f"{ns}tileSize")
-        if tile_size is not None:
-            kwargs["tile_size"] = int(tile_size.text)
-        max_width = element.find(f"{ns}maxWidth")
-        if max_width is not None:
-            kwargs["max_width"] = int(max_width.text)
-        max_height = element.find(f"{ns}maxHeight")
-        if max_height is not None:
-            kwargs["max_height"] = int(max_height.text)
-        grid_origin = element.find(f"{ns}gridOrigin")
-        if grid_origin is not None:
-            kwargs["grid_origin"] = GridOrigin(grid_origin.text)
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_int_kwarg(
+                element=element,
+                ns=ns,
+                node_name="tileSize",
+                kwarg="tile_size",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_int_kwarg(
+                element=element,
+                ns=ns,
+                node_name="maxWidth",
+                kwarg="max_width",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_int_kwarg(
+                element=element,
+                ns=ns,
+                node_name="maxHeight",
+                kwarg="max_height",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_enum_kwarg(
+                element=element,
+                ns=ns,
+                node_name="gridOrigin",
+                kwarg="grid_origin",
+                enum_class=GridOrigin,
+                strict=strict,
+            ),
+        )
         return kwargs
 
 
 class PhotoOverlay(_Overlay):
     """
     The <PhotoOverlay> element allows you to geographically locate a photograph
     on the Earth and to specify viewing parameters for this PhotoOverlay.
@@ -475,16 +580,14 @@
     element that specifies the image file to use for the PhotoOverlay.
     In the case of a very large image, the <href> is a special URL that
     indexes into a pyramid of images of varying resolutions (see ImagePyramid).
 
     https://developers.google.com/kml/documentation/kmlreference#photooverlay
     """
 
-    __name__ = "PhotoOverlay"
-
     rotation: Optional[float]
     # Adjusts how the photo is placed inside the field of view. This element is
     # useful if your photo has been rotated and deviates slightly from a desired
     # horizontal view.
 
     view_volume: Optional[ViewVolume]
     # Defines how much of the current scene is visible.
@@ -573,32 +676,48 @@
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.rotation is not None:
-            rotation = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}rotation",
-            )
-            rotation.text = str(self.rotation)
-        if self.view_volume:
-            element.append(self.view_volume.etree_element())
-        if self.image_pyramid:
-            element.append(self.image_pyramid.etree_element())
-        if self.point:
-            element.append(self.point.etree_element())
-        if self.shape:
-            shape = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}shape",
-            )
-            shape.text = self.shape.value
+        float_subelement(
+            self,
+            element=element,
+            attr_name="rotation",
+            node_name="rotation",
+            precision=precision,
+        )
+        xml_subelement(
+            self,
+            element=element,
+            attr_name="view_volume",
+            precision=precision,
+            verbosity=verbosity,
+        )
+        xml_subelement(
+            self,
+            element=element,
+            attr_name="image_pyramid",
+            precision=precision,
+            verbosity=verbosity,
+        )
+        xml_subelement(
+            self,
+            element=element,
+            attr_name="point",
+            precision=precision,
+            verbosity=verbosity,
+        )
+        enum_subelement(
+            self,
+            element=element,
+            attr_name="shape",
+            node_name="shape",
+        )
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -608,53 +727,66 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        rotation = element.find(f"{ns}rotation")
-        if rotation is not None:
-            kwargs["rotation"] = float(rotation.text)
-        view_volume = element.find(f"{ns}ViewVolume")
-        if view_volume is not None:
-            kwargs["view_volume"] = cast(
-                ViewVolume,
-                ViewVolume.class_from_element(
-                    ns=ns,
-                    name_spaces=name_spaces,
-                    element=view_volume,
-                    strict=strict,
-                ),
-            )
-        image_pyramid = element.find(f"{ns}ImagePyramid")
-        if image_pyramid is not None:
-            kwargs["image_pyramid"] = cast(
-                ImagePyramid,
-                ImagePyramid.class_from_element(
-                    ns=ns,
-                    name_spaces=name_spaces,
-                    element=image_pyramid,
-                    strict=strict,
-                ),
-            )
-        point = element.find(f"{ns}Point")
-        if point is not None:
-            kwargs["point"] = cast(
-                Point,
-                Point.class_from_element(
-                    ns=ns,
-                    name_spaces=name_spaces,
-                    element=point,
-                    strict=strict,
-                ),
-            )
-        shape = element.find(f"{ns}shape")
-        if shape is not None:
-            kwargs["shape"] = Shape(shape.text)
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="rotation",
+                kwarg="rotation",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="view_volume",
+                obj_class=ViewVolume,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="image_pyramid",
+                obj_class=ImagePyramid,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="point",
+                obj_class=Point,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_enum_kwarg(
+                element=element,
+                ns=ns,
+                node_name="shape",
+                kwarg="shape",
+                enum_class=Shape,
+                strict=strict,
+            ),
+        )
+
         return kwargs
 
 
 class LatLonBox(_XMLObject):
     """
     Specifies where the top, bottom, right, and left sides of a bounding box for the
     ground overlay are aligned.
@@ -673,15 +805,16 @@
     (For overlays that overlap the meridian of 180° longitude,
     values can extend beyond that range.)
     <rotation> Specifies a rotation of the overlay about its center, in degrees.
     Values can be ±180. The default is 0 (north).
     Rotations are specified in a counterclockwise direction.
     """
 
-    __name__ = "LatLonBox"
+    _default_ns = config.KMLNS
+
     north: Optional[float]
     south: Optional[float]
     east: Optional[float]
     west: Optional[float]
     rotation: Optional[float]
 
     def __init__(
@@ -713,40 +846,50 @@
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        north = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}north",
-        )
-        north.text = str(self.north)
-        south = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}south",
-        )
-        south.text = str(self.south)
-        east = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}east",
-        )
-        east.text = str(self.east)
-        west = config.etree.SubElement(  # type: ignore[attr-defined]
-            element,
-            f"{self.ns}west",
-        )
-        west.text = str(self.west)
-        if self.rotation is not None:
-            rotation = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}rotation",
-            )
-            rotation.text = str(self.rotation)
+        float_subelement(
+            self,
+            element=element,
+            attr_name="north",
+            node_name="north",
+            precision=precision,
+        )
+        float_subelement(
+            self,
+            element=element,
+            attr_name="south",
+            node_name="south",
+            precision=precision,
+        )
+        float_subelement(
+            self,
+            element=element,
+            attr_name="east",
+            node_name="east",
+            precision=precision,
+        )
+        float_subelement(
+            self,
+            element=element,
+            attr_name="west",
+            node_name="west",
+            precision=precision,
+        )
+        float_subelement(
+            self,
+            element=element,
+            attr_name="rotation",
+            node_name="rotation",
+            precision=precision,
+        )
+
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -756,45 +899,75 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        north = element.find(f"{ns}north")
-        if north is not None:
-            kwargs["north"] = float(north.text)
-        south = element.find(f"{ns}south")
-        if south is not None:
-            kwargs["south"] = float(south.text)
-        east = element.find(f"{ns}east")
-        if east is not None:
-            kwargs["east"] = float(east.text)
-        west = element.find(f"{ns}west")
-        if west is not None:
-            kwargs["west"] = float(west.text)
-        rotation = element.find(f"{ns}rotation")
-        if rotation is not None:
-            kwargs["rotation"] = float(rotation.text)
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="north",
+                kwarg="north",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="south",
+                kwarg="south",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="east",
+                kwarg="east",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="west",
+                kwarg="west",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="rotation",
+                kwarg="rotation",
+                strict=strict,
+            ),
+        )
         return kwargs
 
 
 class GroundOverlay(_Overlay):
     """
     This element draws an image overlay draped onto the terrain. The <href>
     child of <Icon> specifies the image to be used as the overlay. This file
     can be either on a local file system or on a web server. If this element
     is omitted or contains no <href>, a rectangle is drawn using the color and
     LatLonBox bounds defined by the ground overlay.
 
     https://developers.google.com/kml/documentation/kmlreference#groundoverlay
     """
 
-    __name__ = "GroundOverlay"
-
     altitude: Optional[float]
     # Specifies the distance above the earth's surface, in meters, and is
     # interpreted according to the altitude mode.
 
     altitude_mode: Optional[AltitudeMode]
     # Specifies how the <altitude> is interpreted. Possible values are:
     #   clampToGround -
@@ -873,28 +1046,34 @@
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.altitude:
-            altitude = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}altitude",
-            )
-            altitude.text = str(self.altitude)
-            if self.altitude_mode:
-                altitude_mode = config.etree.SubElement(  # type: ignore[attr-defined]
-                    element,
-                    f"{self.ns}altitudeMode",
-                )
-                altitude_mode.text = self.altitude_mode.value
-        if self.lat_lon_box:
-            element.append(self.lat_lon_box.etree_element())
+        float_subelement(
+            self,
+            element=element,
+            attr_name="altitude",
+            node_name="altitude",
+            precision=precision,
+        )
+        enum_subelement(
+            self,
+            element=element,
+            attr_name="altitude_mode",
+            node_name="altitudeMode",
+        )
+        xml_subelement(
+            self,
+            element=element,
+            attr_name="lat_lon_box",
+            precision=precision,
+            verbosity=verbosity,
+        )
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -904,25 +1083,40 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        altitude = element.find(f"{ns}altitude")
-        if altitude is not None:
-            kwargs["altitude"] = float(altitude.text)
-        altitude_mode = element.find(f"{ns}altitudeMode")
-        if altitude_mode is not None:
-            kwargs["altitude_mode"] = AltitudeMode(altitude_mode.text)
-        lat_lon_box = element.find(f"{ns}LatLonBox")
-        if lat_lon_box is not None:
-            kwargs["lat_lon_box"] = cast(
-                LatLonBox,
-                LatLonBox.class_from_element(
-                    ns=ns,
-                    name_spaces=name_spaces,
-                    element=lat_lon_box,
-                    strict=strict,
-                ),
-            )
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_float_kwarg(
+                element=element,
+                ns=ns,
+                node_name="altitude",
+                kwarg="altitude",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_enum_kwarg(
+                element=element,
+                ns=ns,
+                node_name="altitudeMode",
+                kwarg="altitude_mode",
+                enum_class=AltitudeMode,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="lat_lon_box",
+                obj_class=LatLonBox,
+                strict=strict,
+            ),
+        )
+
         return kwargs
```

### Comparing `fastkml-1.0a8/fastkml/styles.py` & `fastkml-1.0a9/fastkml/features.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,396 +1,380 @@
-# Copyright (C) 2012 - 2022  Christian Ledermann
+# Copyright (C) 2023  Christian Ledermann
 #
 # This library is free software; you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation; either version 2.1 of the License, or (at your option)
 # any later version.
 #
 # This library is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301 USA
-
 """
-Once you've created features within Google Earth and examined the KML
-code Google Earth generates, you'll notice how styles are an important
-part of how your data is displayed.
+Feature base, Placemark and NetworkLink.
+
+These are the objects that can be added to a KML file.
 """
 
 import logging
-from dataclasses import dataclass
 from typing import Any
 from typing import Dict
 from typing import Iterable
-from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Union
-from typing import cast
 
+from pygeoif.types import GeoCollectionType
+from pygeoif.types import GeoType
+
+from fastkml import atom
 from fastkml import config
+from fastkml import gx
 from fastkml.base import _BaseObject
-from fastkml.enums import ColorMode
-from fastkml.enums import DisplayMode
-from fastkml.enums import Units
+from fastkml.base import _XMLObject
+from fastkml.data import ExtendedData
 from fastkml.enums import Verbosity
+from fastkml.geometry import AnyGeometryType
+from fastkml.geometry import LinearRing
+from fastkml.geometry import LineString
+from fastkml.geometry import MultiGeometry
+from fastkml.geometry import Point
+from fastkml.geometry import Polygon
+from fastkml.geometry import create_kml_geometry
+from fastkml.helpers import bool_subelement
+from fastkml.helpers import subelement_bool_kwarg
+from fastkml.helpers import subelement_text_kwarg
+from fastkml.helpers import text_subelement
+from fastkml.helpers import xml_subelement
+from fastkml.helpers import xml_subelement_kwarg
+from fastkml.helpers import xml_subelement_list
+from fastkml.helpers import xml_subelement_list_kwarg
+from fastkml.links import Link
+from fastkml.mixins import TimeMixin
+from fastkml.styles import Style
+from fastkml.styles import StyleMap
+from fastkml.styles import StyleUrl
+from fastkml.times import TimeSpan
+from fastkml.times import TimeStamp
 from fastkml.types import Element
+from fastkml.views import Camera
+from fastkml.views import LookAt
+from fastkml.views import Region
 
 logger = logging.getLogger(__name__)
 
-
-def strtobool(val: str) -> int:
-    val = val.lower()
-    if val == "false":
-        return 0
-    if val == "true":
-        return 1
-    return int(float(val))
+KmlGeometry = Union[
+    Point,
+    LineString,
+    LinearRing,
+    Polygon,
+    MultiGeometry,
+    gx.MultiTrack,
+    gx.Track,
+]
 
 
-class StyleUrl(_BaseObject):
+class Snippet(_XMLObject):
     """
-    URL of a <Style> or <StyleMap> defined in a Document.
-
-    If the style is in the same file, use a # reference.
-    If the style is defined in an external file,
-    use a full URL along with # referencing.
+    A short description of the feature.
+    In Google Earth, this description is displayed in the Places panel
+    under the name of the feature.
+    If a Snippet is not supplied, the first two lines of the <description>
+    are used.
+    In Google Earth, if a Placemark contains both a description and a
+    Snippet, the <Snippet> appears beneath the Placemark in the Places
+    panel, and the <description> appears in the Placemark's description
+    balloon.
+    This tag does not support HTML markup.
+    <Snippet> has a maxLines attribute, an integer that specifies the
+    maximum number of lines to display.
     """
 
-    __name__ = "styleUrl"
-    url = None
+    _default_ns = config.KMLNS
+
+    text: Optional[str]
+    max_lines: Optional[int] = None
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
-        id: Optional[str] = None,
-        target_id: Optional[str] = None,
-        url: Optional[str] = None,
+        text: Optional[str] = None,
+        max_lines: Optional[int] = None,
     ) -> None:
-        super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
-        self.url = url
+        super().__init__(ns=ns, name_spaces=name_spaces)
+        self.text = text
+        self.max_lines = max_lines
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.url:
-            element.text = self.url
-        else:
-            logger.warning("StyleUrl is missing required url.")
+        element.text = self.text or ""
+        if self.max_lines is not None:
+            element.set("maxLines", str(self.max_lines))
         return element
 
+    def __bool__(self) -> bool:
+        return bool(self.text)
+
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
         name_spaces: Optional[Dict[str, str]] = None,
         element: Element,
         strict: bool,
     ) -> Dict[str, Any]:
-        kwargs = super()._get_kwargs(
-            ns=ns,
-            name_spaces=name_spaces,
-            element=element,
-            strict=strict,
-        )
-        kwargs["url"] = element.text
+        kwargs: Dict[str, Any] = {"text": element.text}
+        if max_lines := element.get("maxLines"):
+            kwargs["max_lines"] = int(max_lines)
         return kwargs
 
 
-class _StyleSelector(_BaseObject):
-    """
-    This is an abstract element and cannot be used directly in a KML file.
-    It is the base type for the <Style> and <StyleMap> elements. The
-    StyleMap element selects a style based on the current mode of the
-    Placemark. An element derived from StyleSelector is uniquely identified
-    by its id and its url.
-    """
-
-
-class _ColorStyle(_BaseObject):
-    """
-    abstract element; do not create.
-    This is an abstract element and cannot be used directly in a KML file.
-    It provides elements for specifying the color and color mode of
-    extended style types.
-    subclasses are: IconStyle, LabelStyle, LineStyle, PolyStyle.
+class _Feature(TimeMixin, _BaseObject):
     """
-
-    id = None
-    color = None
-    # Color and opacity (alpha) values are expressed in hexadecimal notation.
-    # The range of values for any one color is 0 to 255 (00 to ff).
-    # For alpha, 00 is fully transparent and ff is fully opaque.
-    # The order of expression is aabbggrr, where aa=alpha (00 to ff);
-    # bb=blue (00 to ff); gg=green (00 to ff); rr=red (00 to ff).
-
-    color_mode: Optional[ColorMode]
-    # Values for <colorMode> are normal (no effect) and random.
-    # A value of random applies a random linear scale to the base <color>
+    abstract element; do not create
+    subclasses are:
+        * Container (Document, Folder)
+        * Placemark
+        * Overlay
+        * NetworkLink.
+    """
+
+    name: Optional[str]
+    # User-defined text displayed in the 3D viewer as the label for the
+    # object (for example, for a Placemark, Folder, or NetworkLink).
+
+    visibility: Optional[bool]
+    # Boolean value. Specifies whether the feature is drawn in the 3D
+    # viewer when it is initially loaded. In order for a feature to be
+    # visible, the <visibility> tag of all its ancestors must also be
+    # set to 1.
+
+    isopen: Optional[bool]
+    # Boolean value. Specifies whether a Document or Folder appears
+    # closed or open when first loaded into the Places panel.
+    # 0=collapsed (the default), 1=expanded.
+
+    atom_author: Optional[atom.Author]
+    # KML 2.2 supports new elements for including data about the author
+    # and related website in your KML file. This information is displayed
+    # in geo search results, both in Earth browsers such as Google Earth,
+    # and in other applications such as Google Maps.
+
+    atom_link: Optional[atom.Link]
+    # Specifies the URL of the website containing this KML or KMZ file.
+
+    address: Optional[str]
+    # A string value representing an unstructured address written as a
+    # standard street, city, state address, and/or as a postal code.
+    # You can use the <address> tag to specify the location of a point
+    # instead of using latitude and longitude coordinates.
+
+    phone_number: Optional[str]
+    # A string value representing a telephone number.
+    # This element is used by Google Maps Mobile only.
+
+    snippet: Optional[Snippet]
+    # _snippet is either a tuple of a string Snippet.text and an integer
+    # Snippet.maxLines or a string
+    #
+    # A short description of the feature. In Google Earth, this
+    # description is displayed in the Places panel under the name of the
+    # feature. If a Snippet is not supplied, the first two lines of
+    # the <description> are used. In Google Earth, if a Placemark
+    # contains both a description and a Snippet, the <Snippet> appears
+    # beneath the Placemark in the Places panel, and the <description>
+    # appears in the Placemark's description balloon. This tag does not
+    # support HTML markup. <Snippet> has a maxLines attribute, an integer
+    # that specifies the maximum number of lines to display.
+
+    description: Optional[str]
+    # User-supplied content that appears in the description balloon.
+
+    style_url: Optional[StyleUrl]
+    # URL of a <Style> or <StyleMap> defined in a Document.
+    # If the style is in the same file, use a # reference.
+    # If the style is defined in an external file, use a full URL
+    # along with # referencing.
+
+    styles: List[Union[Style, StyleMap]]
+    # One or more Styles and StyleMaps can be defined to customize the
+    # appearance of any element derived from Feature or of the Geometry
+    # in a Placemark.
+    # A style defined within a Feature is called an "inline style" and
+    # applies only to the Feature that contains it. A style defined as
+    # the child of a <Document> is called a "shared style." A shared
+    # style must have an id defined for it. This id is referenced by one
+    # or more Features within the <Document>. In cases where a style
+    # element is defined both in a shared style and in an inline style
+    # for a Feature—that is, a Folder, GroundOverlay, NetworkLink,
+    # Placemark, or ScreenOverlay—the value for the Feature's inline
+    # style takes precedence over the value for the shared style.
+
+    view: Union[Camera, LookAt, None]
+
+    region: Optional[Region]
+    # Features and geometry associated with a Region are drawn only when
+    # the Region is active.
+
+    extended_data: Optional[ExtendedData]
+    # Allows you to add custom data to a KML file. This data can be
+    # (1) data that references an external XML schema,
+    # (2) untyped data/value pairs, or
+    # (3) typed data.
+    # A given KML Feature can contain a combination of these types of
+    # custom data.
+    #
+    # (2 and 3) are already implemented, see data.py for more information.
+    #
+    # <Metadata> (deprecated in KML 2.2; use <ExtendedData> instead)
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        color: Optional[str] = None,
-        color_mode: Optional[ColorMode] = None,
+        name: Optional[str] = None,
+        visibility: Optional[bool] = None,
+        isopen: Optional[bool] = None,
+        atom_link: Optional[atom.Link] = None,
+        atom_author: Optional[atom.Author] = None,
+        address: Optional[str] = None,
+        phone_number: Optional[str] = None,
+        snippet: Optional[Snippet] = None,
+        description: Optional[str] = None,
+        view: Optional[Union[Camera, LookAt]] = None,
+        times: Optional[Union[TimeSpan, TimeStamp]] = None,
+        style_url: Optional[StyleUrl] = None,
+        styles: Optional[Iterable[Union[Style, StyleMap]]] = None,
+        region: Optional[Region] = None,
+        extended_data: Optional[ExtendedData] = None,
     ) -> None:
         super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
-        self.color = color
-        self.color_mode = color_mode
+        self.name = name
+        self.description = description
+        self.style_url = style_url
+        self.styles = list(styles) if styles else []
+        self.view = view
+        self.visibility = visibility
+        self.isopen = isopen
+        self.snippet = snippet
+        self.atom_author = atom_author
+        self.atom_link = atom_link
+        self.address = address
+        self.phone_number = phone_number
+        self.region = region
+        self.extended_data = extended_data
+        self.times = times
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.color:
-            color = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}color",
-            )
-            color.text = self.color
-        if self.color_mode:
-            color_mode = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}colorMode",
-            )
-            color_mode.text = self.color_mode.value
-        return element
-
-    @classmethod
-    def _get_kwargs(
-        cls,
-        *,
-        ns: str,
-        name_spaces: Optional[Dict[str, str]] = None,
-        element: Element,
-        strict: bool,
-    ) -> Dict[str, Any]:
-        kwargs = super()._get_kwargs(
-            ns=ns,
-            name_spaces=name_spaces,
+        xml_subelement(
+            self,
             element=element,
-            strict=strict,
+            attr_name="times",
+            precision=precision,
+            verbosity=verbosity,
         )
-        color_mode = element.find(f"{ns}colorMode")
-        if color_mode is not None:
-            kwargs["color_mode"] = ColorMode(color_mode.text)
-        color = element.find(f"{ns}color")
-        if color is not None:
-            kwargs["color"] = color.text
-        return kwargs
-
-
-@dataclass(frozen=True)
-class HotSpot:
-    x: float
-    y: float
-    xunits: Units
-    yunits: Units
-
-    @classmethod
-    def class_from_element(
-        cls,
-        *,
-        ns: str,
-        name_spaces: Optional[Dict[str, str]] = None,
-        element: Element,
-        strict: bool,
-    ) -> Optional["HotSpot"]:
-        hot_spot = element.find(f"{ns}hotSpot")
-        if hot_spot is not None:
-            x = hot_spot.attrib.get("x")  # type: ignore[attr-defined]
-            y = hot_spot.attrib.get("y")  # type: ignore[attr-defined]
-            xunits = hot_spot.attrib.get("xunits")  # type: ignore[attr-defined]
-            yunits = hot_spot.attrib.get("yunits")  # type: ignore[attr-defined]
-            x = float(x) if x is not None else 0
-            y = float(y) if y is not None else 0
-            xunits = Units(xunits) if xunits is not None else None
-            yunits = Units(yunits) if yunits is not None else None
-            element.remove(hot_spot)
-            return HotSpot(
-                x=x,
-                y=y,
-                xunits=xunits,
-                yunits=yunits,
-            )
-        return None
-
-
-class IconStyle(_ColorStyle):
-    """Specifies how icons for point Placemarks are drawn."""
-
-    __name__ = "IconStyle"
-    scale = 1.0
-    # Resizes the icon. (float)
-    heading = None
-    # Direction (that is, North, South, East, West), in degrees.
-    # Default=0 (North).
-    icon_href = None
-    # An HTTP address or a local file specification used to load an icon.
-    hot_spot = None
-
-    def __init__(
-        self,
-        ns: Optional[str] = None,
-        name_spaces: Optional[Dict[str, str]] = None,
-        id: Optional[str] = None,
-        target_id: Optional[str] = None,
-        color: Optional[str] = None,
-        color_mode: Optional[ColorMode] = None,
-        scale: float = 1.0,
-        heading: Optional[float] = None,
-        icon_href: Optional[str] = None,
-        hot_spot: Optional[HotSpot] = None,
-    ) -> None:
-        super().__init__(
-            ns=ns,
-            name_spaces=name_spaces,
-            id=id,
-            target_id=target_id,
-            color=color,
-            color_mode=color_mode,
+        xml_subelement(
+            self,
+            element=element,
+            attr_name="atom_link",
+            precision=precision,
+            verbosity=verbosity,
         )
-
-        self.scale = scale
-        self.heading = heading
-        self.icon_href = icon_href
-        self.hot_spot = hot_spot
-
-    def etree_element(
-        self,
-        precision: Optional[int] = None,
-        verbosity: Verbosity = Verbosity.normal,
-    ) -> Element:
-        element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.scale is not None:
-            scale = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}scale",
-            )
-            scale.text = str(self.scale)
-        if self.heading is not None:
-            heading = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}heading",
-            )
-            heading.text = str(self.heading)
-        if self.icon_href:
-            icon = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}Icon",
-            )
-            href = config.etree.SubElement(  # type: ignore[attr-defined]
-                icon,
-                f"{self.ns}href",
-            )
-            href.text = self.icon_href
-        if self.hot_spot:
-            hot_spot = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}hotSpot",
-            )
-            hot_spot.attrib["x"] = str(self.hot_spot.x)
-            hot_spot.attrib["y"] = str(self.hot_spot.y)
-            hot_spot.attrib["xunits"] = self.hot_spot.xunits.value
-            hot_spot.attrib["yunits"] = self.hot_spot.yunits.value
-        return element
-
-    @classmethod
-    def _get_kwargs(
-        cls,
-        *,
-        ns: str,
-        name_spaces: Optional[Dict[str, str]] = None,
-        element: Element,
-        strict: bool,
-    ) -> Dict[str, Any]:
-        kwargs = super()._get_kwargs(
-            ns=ns,
-            name_spaces=name_spaces,
+        xml_subelement(
+            self,
             element=element,
-            strict=strict,
+            attr_name="atom_author",
+            precision=precision,
+            verbosity=verbosity,
         )
-        scale = element.find(f"{ns}scale")
-        if scale is not None:
-            kwargs["scale"] = float(scale.text)
-        heading = element.find(f"{ns}heading")
-        if heading is not None:
-            kwargs["heading"] = float(heading.text)
-        icon = element.find(f"{ns}Icon")
-        if icon is not None:
-            href = icon.find(f"{ns}href")
-            if href is not None:
-                kwargs["icon_href"] = href.text
-        kwargs["hot_spot"] = HotSpot.class_from_element(
-            ns=ns,
-            name_spaces=name_spaces,
+        xml_subelement(
+            self,
             element=element,
-            strict=strict,
+            attr_name="extended_data",
+            precision=precision,
+            verbosity=verbosity,
+        )
+        xml_subelement(
+            self,
+            element=element,
+            attr_name="view",
+            precision=precision,
+            verbosity=verbosity,
+        )
+        xml_subelement(
+            self,
+            element=element,
+            attr_name="style_url",
+            precision=precision,
+            verbosity=verbosity,
+        )
+        xml_subelement(
+            self,
+            element=element,
+            attr_name="snippet",
+            precision=precision,
+            verbosity=verbosity,
         )
-        return kwargs
-
-
-class LineStyle(_ColorStyle):
-    """
-    Specifies the drawing style (color, color mode, and line width)
-    for all line geometry. Line geometry includes the outlines of
-    outlined polygons and the extruded "tether" of Placemark icons
-    (if extrusion is enabled).
-    """
-
-    __name__ = "LineStyle"
-    width = 1.0
-    # Width of the line, in pixels.
 
-    def __init__(
-        self,
-        ns: Optional[str] = None,
-        name_spaces: Optional[Dict[str, str]] = None,
-        id: Optional[str] = None,
-        target_id: Optional[str] = None,
-        color: Optional[str] = None,
-        color_mode: Optional[ColorMode] = None,
-        width: Union[int, float] = 1,
-    ) -> None:
-        super().__init__(
-            ns=ns,
-            name_spaces=name_spaces,
-            id=id,
-            target_id=target_id,
-            color=color,
-            color_mode=color_mode,
+        xml_subelement_list(
+            self,
+            element=element,
+            attr_name="styles",
+            precision=precision,
+            verbosity=verbosity,
         )
-        self.width = width
 
-    def etree_element(
-        self,
-        precision: Optional[int] = None,
-        verbosity: Verbosity = Verbosity.normal,
-    ) -> Element:
-        element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.width is not None:
-            width = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}width",
-            )
-            width.text = str(self.width)
+        text_subelement(
+            self,
+            element=element,
+            attr_name="address",
+            node_name="address",
+        )
+        text_subelement(
+            self,
+            element=element,
+            attr_name="phone_number",
+            node_name="phoneNumber",
+        )
+        text_subelement(
+            self,
+            element=element,
+            attr_name="description",
+            node_name="description",
+        )
+        text_subelement(
+            self,
+            element=element,
+            attr_name="name",
+            node_name="name",
+        )
+        bool_subelement(
+            self,
+            element=element,
+            attr_name="visibility",
+            node_name="visibility",
+        )
+        bool_subelement(self, element=element, attr_name="isopen", node_name="open")
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -400,74 +384,257 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        width = element.find(f"{ns}width")
-        if width is not None:
-            kwargs["width"] = float(width.text)
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            xml_subelement_list_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="styles",
+                obj_classes=(Style, StyleMap),
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="style_url",
+                obj_class=StyleUrl,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="times",
+                obj_class=TimeSpan,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="times",
+                obj_class=TimeStamp,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="extended_data",
+                obj_class=ExtendedData,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="view",
+                obj_class=Camera,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="view",
+                obj_class=LookAt,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="snippet",
+                obj_class=Snippet,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=name_spaces["atom"],
+                name_spaces=name_spaces,
+                kwarg="atom_link",
+                obj_class=atom.Link,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=name_spaces["atom"],
+                name_spaces=name_spaces,
+                kwarg="atom_author",
+                obj_class=atom.Author,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="address",
+                kwarg="address",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="phoneNumber",
+                kwarg="phone_number",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="description",
+                kwarg="description",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_text_kwarg(
+                element=element,
+                ns=ns,
+                node_name="name",
+                kwarg="name",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_bool_kwarg(
+                element=element,
+                ns=ns,
+                node_name="visibility",
+                kwarg="visibility",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_bool_kwarg(
+                element=element,
+                ns=ns,
+                node_name="open",
+                kwarg="isopen",
+                strict=strict,
+            ),
+        )
         return kwargs
 
 
-class PolyStyle(_ColorStyle):
+class Placemark(_Feature):
     """
-    Specifies the drawing style for all polygons, including polygon
-    extrusions (which look like the walls of buildings) and line
-    extrusions (which look like solid fences).
+    A Placemark is a Feature with associated Geometry.
+    In Google Earth, a Placemark appears as a list item in the Places
+    panel. A Placemark with a Point has an icon associated with it that
+    marks a point on the Earth in the 3D viewer.
     """
 
-    __name__ = "PolyStyle"
-    fill = 1
-    # Boolean value. Specifies whether to fill the polygon.
-    outline = 1
-    # Boolean value. Specifies whether to outline the polygon.
-    # Polygon outlines use the current LineStyle.
+    _geometry: Optional[KmlGeometry]
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        color: Optional[str] = None,
-        color_mode: Optional[ColorMode] = None,
-        fill: int = 1,
-        outline: int = 1,
+        name: Optional[str] = None,
+        visibility: Optional[bool] = None,
+        isopen: Optional[bool] = None,
+        atom_link: Optional[atom.Link] = None,
+        atom_author: Optional[atom.Author] = None,
+        address: Optional[str] = None,
+        phone_number: Optional[str] = None,
+        snippet: Optional[Snippet] = None,
+        description: Optional[str] = None,
+        view: Optional[Union[Camera, LookAt]] = None,
+        times: Optional[Union[TimeSpan, TimeStamp]] = None,
+        style_url: Optional[StyleUrl] = None,
+        styles: Optional[Iterable[Union[Style, StyleMap]]] = None,
+        region: Optional[Region] = None,
+        extended_data: Optional[ExtendedData] = None,
+        # Placemark specific
+        kml_geometry: Optional[KmlGeometry] = None,
+        geometry: Optional[Union[GeoType, GeoCollectionType]] = None,
     ) -> None:
         super().__init__(
             ns=ns,
             name_spaces=name_spaces,
             id=id,
             target_id=target_id,
-            color=color,
-            color_mode=color_mode,
-        )
-        self.fill = fill
-        self.outline = outline
+            name=name,
+            visibility=visibility,
+            isopen=isopen,
+            atom_link=atom_link,
+            atom_author=atom_author,
+            address=address,
+            phone_number=phone_number,
+            snippet=snippet,
+            description=description,
+            view=view,
+            times=times,
+            style_url=style_url,
+            styles=styles,
+            region=region,
+            extended_data=extended_data,
+        )
+        if kml_geometry and geometry:
+            msg = "You can only specify one of kml_geometry or geometry"
+            raise ValueError(msg)
+        if geometry:
+            kml_geometry = create_kml_geometry(  # type: ignore[assignment]
+                geometry=geometry,
+                ns=ns,
+                name_spaces=name_spaces,
+            )
+        self._geometry = kml_geometry
+
+    @property
+    def geometry(self) -> Optional[AnyGeometryType]:
+        return self._geometry.geometry if self._geometry is not None else None
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.fill is not None:
-            fill = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}fill",
-            )
-            fill.text = str(self.fill)
-        if self.outline is not None:
-            outline = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}outline",
-            )
-            outline.text = str(self.outline)
+        xml_subelement(
+            self,
+            element=element,
+            attr_name="_geometry",
+            precision=precision,
+            verbosity=verbosity,
+        )
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -477,363 +644,209 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        fill = element.find(f"{ns}fill")
-        if fill is not None:
-            kwargs["fill"] = strtobool(fill.text)
-        outline = element.find(f"{ns}outline")
-        if outline is not None:
-            kwargs["outline"] = strtobool(outline.text)
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="kml_geometry",
+                obj_class=Point,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="kml_geometry",
+                obj_class=LineString,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="kml_geometry",
+                obj_class=Polygon,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="kml_geometry",
+                obj_class=LinearRing,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="kml_geometry",
+                obj_class=MultiGeometry,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=name_spaces["gx"],
+                name_spaces=name_spaces,
+                kwarg="kml_geometry",
+                obj_class=gx.MultiTrack,
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=name_spaces["gx"],
+                name_spaces=name_spaces,
+                kwarg="kml_geometry",
+                obj_class=gx.Track,
+                strict=strict,
+            ),
+        )
         return kwargs
 
 
-class LabelStyle(_ColorStyle):
-    """Specifies how the <name> of a Feature is drawn in the 3D viewer."""
+class NetworkLink(_Feature):
+    """
+    References a KML file or KMZ archive on a local or remote network.
 
-    __name__ = "LabelStyle"
-    scale = 1.0
-    # Resizes the label.
+    Use the <Link> element to specify the location of the KML file.
+    Within that element, you can define the refresh options for updating the file,
+    based on time and camera change.
+    NetworkLinks can be used in combination with Regions to handle very large datasets
+    efficiently.
+    https://developers.google.com/kml/documentation/kmlreference#networklink
+
+
+    Elements Specific to NetworkLink
+    <refreshVisibility>
+    Boolean value.
+    A value of 0 leaves the visibility of features within the control of the
+    Google Earth user.
+    Set the value to 1 to reset the visibility of features each time the NetworkLink is
+    refreshed.
+    For example, suppose a Placemark within the linked KML file has <visibility>
+    set to 1 and the NetworkLink has <refreshVisibility> set to 1.
+    When the file is first loaded into Google Earth, the user can clear the check box
+    next to the item to turn off display in the 3D viewer.
+    However, when the NetworkLink is refreshed, the Placemark will be made
+    visible again, since its original visibility state was TRUE.
+    <flyToView>
+    Boolean value.
+    A value of 1 causes Google Earth to fly to the view of the LookAt or Camera in the
+    NetworkLinkControl (if it exists).
+    If the NetworkLinkControl does not contain an AbstractView element,
+    Google Earth flies to the LookAt or Camera element in the Feature child
+    within the <kml> element in the refreshed file.
+    If the <kml> element does not have a LookAt or Camera specified,
+    the view is unchanged.
+    For example, Google Earth would fly to the <LookAt> view of the parent Document,
+    not the <LookAt> of the Placemarks contained within the Document.
+    <Link>(required)
+       https://developers.google.com/kml/documentation/kmlreference#link
+    """
+
+    refresh_visibility: Optional[bool]
+    fly_to_view: Optional[bool]
+    link: Optional[Link]
 
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
-        color: Optional[str] = None,
-        color_mode: Optional[ColorMode] = None,
-        scale: float = 1.0,
+        name: Optional[str] = None,
+        visibility: Optional[bool] = None,
+        isopen: Optional[bool] = None,
+        atom_link: Optional[atom.Link] = None,
+        atom_author: Optional[atom.Author] = None,
+        address: Optional[str] = None,
+        phone_number: Optional[str] = None,
+        snippet: Optional[Snippet] = None,
+        description: Optional[str] = None,
+        view: Optional[Union[Camera, LookAt]] = None,
+        times: Optional[Union[TimeSpan, TimeStamp]] = None,
+        style_url: Optional[StyleUrl] = None,
+        styles: Optional[Iterable[Union[Style, StyleMap]]] = None,
+        region: Optional[Region] = None,
+        extended_data: Optional[ExtendedData] = None,
+        # NetworkLink specific
+        refresh_visibility: Optional[bool] = None,
+        fly_to_view: Optional[bool] = None,
+        link: Optional[Link] = None,
     ) -> None:
         super().__init__(
             ns=ns,
             name_spaces=name_spaces,
             id=id,
             target_id=target_id,
-            color=color,
-            color_mode=color_mode,
-        )
-        self.scale = scale
+            name=name,
+            visibility=visibility,
+            isopen=isopen,
+            atom_link=atom_link,
+            atom_author=atom_author,
+            address=address,
+            phone_number=phone_number,
+            snippet=snippet,
+            description=description,
+            view=view,
+            times=times,
+            style_url=style_url,
+            styles=styles,
+            region=region,
+            extended_data=extended_data,
+        )
+        self.refresh_visibility = refresh_visibility
+        self.fly_to_view = fly_to_view
+        self.link = link
 
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.scale is not None:
-            scale = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}scale",
-            )
-            scale.text = str(self.scale)
-        return element
-
-    @classmethod
-    def _get_kwargs(
-        cls,
-        *,
-        ns: str,
-        name_spaces: Optional[Dict[str, str]] = None,
-        element: Element,
-        strict: bool,
-    ) -> Dict[str, Any]:
-        kwargs = super()._get_kwargs(
-            ns=ns,
-            name_spaces=name_spaces,
+        bool_subelement(
+            self,
             element=element,
-            strict=strict,
+            attr_name="refresh_visibility",
+            node_name="refreshVisibility",
         )
-        scale = element.find(f"{ns}scale")
-        if scale is not None:
-            kwargs["scale"] = float(scale.text)
-        return kwargs
-
-
-class BalloonStyle(_BaseObject):
-    """
-    Specifies how the description balloon for placemarks is drawn.
-
-    The <bgColor>, if specified, is used as the background color of the balloon.
-    """
-
-    __name__ = "BalloonStyle"
-
-    bg_color = None
-    # Background color of the balloon (optional). Color and opacity (alpha)
-    # values are expressed in hexadecimal notation. The range of values for
-    # any one color is 0 to 255 (00 to ff). The order of expression is
-    # aabbggrr, where aa=alpha (00 to ff); bb=blue (00 to ff);
-    # gg=green (00 to ff); rr=red (00 to ff).
-    # For alpha, 00 is fully transparent and ff is fully opaque.
-    # For example, if you want to apply a blue color with 50 percent
-    # opacity to an overlay, you would specify the following:
-    # <bgColor>7fff0000</bgColor>, where alpha=0x7f, blue=0xff, green=0x00,
-    # and red=0x00. The default is opaque white (ffffffff).
-    # Note: The use of the <color> element within <BalloonStyle> has been
-    # deprecated. Use <bgColor> instead.
-
-    text_color = None
-    # Foreground color for text. The default is black (ff000000).
-
-    text = None
-    # Text displayed in the balloon. If no text is specified, Google Earth
-    # draws the default balloon (with the Feature <name> in boldface,
-    # the Feature <description>, links for driving directions, a white
-    # background, and a tail that is attached to the point coordinates of
-    # the Feature, if specified).
-    # You can add entities to the <text> tag using the following format to
-    # refer to a child element of Feature: $[name], $[description], $[address],
-    # $[id], $[Snippet]. Google Earth looks in the current Feature for the
-    # corresponding string entity and substitutes that information in the
-    # balloon.
-    # To include To here - From here driving directions in the balloon,
-    # use the $[geDirections] tag. To prevent the driving directions links
-    # from appearing in a balloon, include the <text> element with some content
-    # or with $[description] to substitute the basic Feature <description>.
-    # For example, in the following KML excerpt, $[name] and $[description]
-    # fields will be replaced by the <name> and <description> fields found
-    # in the Feature elements that use this BalloonStyle:
-    # <text>This is $[name], whose description is:<br/>$[description]</text>
-
-    display_mode: Optional[DisplayMode]
-    # If <displayMode> is default, Google Earth uses the information supplied
-    # in <text> to create a balloon . If <displayMode> is hide, Google Earth
-    # does not display the balloon. In Google Earth, clicking the List View
-    # icon for a Placemark whose balloon's <displayMode> is hide causes
-    # Google Earth to fly to the Placemark.
-
-    def __init__(
-        self,
-        ns: Optional[str] = None,
-        name_spaces: Optional[Dict[str, str]] = None,
-        id: Optional[str] = None,
-        target_id: Optional[str] = None,
-        bg_color: Optional[str] = None,
-        text_color: Optional[str] = None,
-        text: Optional[str] = None,
-        display_mode: Optional[DisplayMode] = None,
-    ) -> None:
-        super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
-        self.bg_color = bg_color
-        self.text_color = text_color
-        self.text = text
-        self.display_mode = display_mode
-
-    def etree_element(
-        self,
-        precision: Optional[int] = None,
-        verbosity: Verbosity = Verbosity.normal,
-    ) -> Element:
-        element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.bg_color is not None:
-            elem = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}bgColor",
-            )
-            elem.text = self.bg_color
-        if self.text_color is not None:
-            elem = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}textColor",
-            )
-            elem.text = self.text_color
-        if self.text is not None:
-            elem = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}text",
-            )
-            elem.text = self.text
-        if self.display_mode is not None:
-            elem = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}displayMode",
-            )
-            elem.text = self.display_mode.value
-        return element
-
-    @classmethod
-    def _get_kwargs(
-        cls,
-        *,
-        ns: str,
-        name_spaces: Optional[Dict[str, str]] = None,
-        element: Element,
-        strict: bool,
-    ) -> Dict[str, Any]:
-        kwargs = super()._get_kwargs(
-            ns=ns,
-            name_spaces=name_spaces,
+        bool_subelement(
+            self,
             element=element,
-            strict=strict,
+            attr_name="fly_to_view",
+            node_name="flyToView",
         )
-        bg_color = element.find(f"{ns}bgColor")
-        if bg_color is not None:
-            kwargs["bg_color"] = bg_color.text
-        else:
-            bg_color = element.find(f"{ns}color")
-            if bg_color is not None:
-                kwargs["bg_color"] = bg_color.text
-        text_color = element.find(f"{ns}textColor")
-        if text_color is not None:
-            kwargs["text_color"] = text_color.text
-        text = element.find(f"{ns}text")
-        if text is not None:
-            kwargs["text"] = text.text
-        display_mode = element.find(f"{ns}displayMode")
-        if display_mode is not None:
-            kwargs["display_mode"] = DisplayMode(display_mode.text)
-        return kwargs
-
-
-AnyStyle = Union[BalloonStyle, IconStyle, LabelStyle, LineStyle, PolyStyle]
-
-
-class Style(_StyleSelector):
-    """
-    A Style defines an addressable style group.
-
-    It can be referenced by StyleMaps and Features.
-    Styles affect how Geometry is presented in the 3D viewer and how Features
-    appear in the Places panel of the List view.
-    Shared styles are collected in a <Document> and must have an id defined for them
-    so that they can be referenced by the individual Features that use them.
-    """
-
-    __name__ = "Style"
-
-    def __init__(
-        self,
-        ns: Optional[str] = None,
-        name_spaces: Optional[Dict[str, str]] = None,
-        id: Optional[str] = None,
-        target_id: Optional[str] = None,
-        styles: Optional[Iterable[AnyStyle]] = None,
-    ) -> None:
-        super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
-        self._styles: List[AnyStyle] = []
-        if styles:
-            for style in styles:
-                self.append_style(style)
-
-    def append_style(
-        self,
-        style: AnyStyle,
-    ) -> None:
-        if isinstance(style, (_ColorStyle, BalloonStyle)):
-            self._styles.append(style)
-        else:
-            raise TypeError
-
-    def styles(
-        self,
-    ) -> Iterator[AnyStyle]:
-        for style in self._styles:
-            if isinstance(style, (_ColorStyle, BalloonStyle)):
-                yield style
-            else:
-                raise TypeError
-
-    def etree_element(
-        self,
-        precision: Optional[int] = None,
-        verbosity: Verbosity = Verbosity.normal,
-    ) -> Element:
-        element = super().etree_element(precision=precision, verbosity=verbosity)
-        for style in self.styles():
-            element.append(style.etree_element())
-        return element
-
-    @classmethod
-    def _get_kwargs(
-        cls,
-        *,
-        ns: str,
-        name_spaces: Optional[Dict[str, str]] = None,
-        element: Element,
-        strict: bool,
-    ) -> Dict[str, Any]:
-        kwargs = super()._get_kwargs(
-            ns=ns,
-            name_spaces=name_spaces,
+        xml_subelement(
+            self,
             element=element,
-            strict=strict,
+            attr_name="link",
+            precision=precision,
+            verbosity=verbosity,
         )
-        styles = []
-        for style in [BalloonStyle, IconStyle, LabelStyle, LineStyle, PolyStyle]:
-            style_element = element.find(f"{ns}{style.__name__}")
-            if style_element is not None:
-                styles.append(
-                    style.class_from_element(  # type: ignore[attr-defined]
-                        ns=ns,
-                        name_spaces=name_spaces,
-                        element=style_element,
-                        strict=strict,
-                    ),
-                )
-        kwargs["styles"] = styles
-        return kwargs
-
-
-class StyleMap(_StyleSelector):
-    """
-    A <StyleMap> maps between two different Styles.
-    Typically a <StyleMap> element is used to provide separate normal and highlighted
-    styles for a placemark, so that the highlighted version appears when
-    the user mouses over the icon in Google Earth.
-    """
-
-    __name__ = "StyleMap"
-    normal = None
-    highlight = None
-
-    def __init__(
-        self,
-        ns: Optional[str] = None,
-        name_spaces: Optional[Dict[str, str]] = None,
-        id: Optional[str] = None,
-        target_id: Optional[str] = None,
-        normal: Optional[Union[Style, StyleUrl]] = None,
-        highlight: Optional[Union[Style, StyleUrl]] = None,
-    ) -> None:
-        super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
-        self.normal = normal
-        self.highlight = highlight
-
-    def etree_element(
-        self,
-        precision: Optional[int] = None,
-        verbosity: Verbosity = Verbosity.normal,
-    ) -> Element:
-        element = super().etree_element(precision=precision, verbosity=verbosity)
-        if self.normal and isinstance(self.normal, (Style, StyleUrl)):
-            pair = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}Pair",
-            )
-            key = config.etree.SubElement(  # type: ignore[attr-defined]
-                pair,
-                f"{self.ns}key",
-            )
-            key.text = "normal"
-            pair.append(self.normal.etree_element())
-        if self.highlight and isinstance(self.highlight, (Style, StyleUrl)):
-            pair = config.etree.SubElement(  # type: ignore[attr-defined]
-                element,
-                f"{self.ns}Pair",
-            )
-            key = config.etree.SubElement(  # type: ignore[attr-defined]
-                pair,
-                f"{self.ns}key",
-            )
-            key.text = "highlight"
-            pair.append(self.highlight.etree_element())
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
@@ -843,75 +856,38 @@
     ) -> Dict[str, Any]:
         kwargs = super()._get_kwargs(
             ns=ns,
             name_spaces=name_spaces,
             element=element,
             strict=strict,
         )
-        pairs = element.findall(f"{ns}Pair")
-        for pair in pairs:
-            key = pair.find(f"{ns}key")
-            style = pair.find(f"{ns}Style")
-            style_url = pair.find(f"{ns}styleUrl")
-            if key is None or key.text not in ["highlight", "normal"]:
-                raise ValueError
-            elif key.text == "highlight":
-                if style is not None:
-                    highlight = cast(
-                        Style,
-                        Style.class_from_element(
-                            ns=ns,
-                            name_spaces=name_spaces,
-                            element=style,
-                            strict=strict,
-                        ),
-                    )
-                elif style_url is not None:
-                    highlight = cast(  # type: ignore[assignment]
-                        StyleUrl,
-                        StyleUrl.class_from_element(
-                            ns=ns,
-                            name_spaces=name_spaces,
-                            element=style_url,
-                            strict=strict,
-                        ),
-                    )
-                else:
-                    raise ValueError
-                kwargs["highlight"] = highlight
-            else:
-                if style is not None:
-                    normal = cast(
-                        Style,
-                        Style.class_from_element(
-                            ns=ns,
-                            name_spaces=name_spaces,
-                            element=style,
-                            strict=strict,
-                        ),
-                    )
-                elif style_url is not None:
-                    normal = cast(  # type: ignore[assignment]
-                        StyleUrl,
-                        StyleUrl.class_from_element(
-                            ns=ns,
-                            name_spaces=name_spaces,
-                            element=style_url,
-                            strict=strict,
-                        ),
-                    )
-                else:
-                    raise ValueError
-                kwargs["normal"] = normal
+        name_spaces = kwargs["name_spaces"]
+        assert name_spaces is not None
+        kwargs.update(
+            subelement_bool_kwarg(
+                element=element,
+                ns=ns,
+                node_name="refreshVisibility",
+                kwarg="refresh_visibility",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            subelement_bool_kwarg(
+                element=element,
+                ns=ns,
+                node_name="flyToView",
+                kwarg="fly_to_view",
+                strict=strict,
+            ),
+        )
+        kwargs.update(
+            xml_subelement_kwarg(
+                element=element,
+                ns=ns,
+                name_spaces=name_spaces,
+                kwarg="link",
+                obj_class=Link,
+                strict=strict,
+            ),
+        )
         return kwargs
-
-
-__all__ = [
-    "BalloonStyle",
-    "IconStyle",
-    "LabelStyle",
-    "LineStyle",
-    "PolyStyle",
-    "Style",
-    "StyleMap",
-    "StyleUrl",
-]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fastkml-1.0a8/fastkml/times.py` & `fastkml-1.0a9/fastkml/times.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,16 +121,15 @@
         raise ValueError
 
     @classmethod
     def parse(cls, datestr: str) -> Optional["KmlDateTime"]:
         """Parse a KML DateTime string into a KmlDateTime object."""
         resolution = None
         dt = None
-        year_month_day_match = year_month_day.match(datestr)
-        if year_month_day_match:
+        if year_month_day_match := year_month_day.match(datestr):
             year = int(year_month_day_match.group("year"))
             month = int(year_month_day_match.group("month") or 1)
             day = int(year_month_day_match.group("day") or 1)
             dt = arrow.get(year, month, day).datetime
             resolution = DateTimeResolution.date
             if year_month_day_match.group("day") is None:
                 resolution = DateTimeResolution.year_month
@@ -150,27 +149,29 @@
     https://developers.google.com/kml/documentation/kmlreference#timeprimitive
     """
 
 
 class TimeStamp(_TimePrimitive):
     """Represents a single moment in time."""
 
-    __name__ = "TimeStamp"
-
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
         timestamp: Optional[KmlDateTime] = None,
     ) -> None:
         super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
         self.timestamp = timestamp
 
+    def __bool__(self) -> bool:
+        """Return True if the timestamp is valid."""
+        return bool(self.timestamp)
+
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
         when = config.etree.SubElement(  # type: ignore[attr-defined]
@@ -200,55 +201,51 @@
             kwargs["timestamp"] = KmlDateTime.parse(when.text)
         return kwargs
 
 
 class TimeSpan(_TimePrimitive):
     """Represents an extent in time bounded by begin and end dateTimes."""
 
-    __name__ = "TimeSpan"
-
     def __init__(
         self,
         ns: Optional[str] = None,
         name_spaces: Optional[Dict[str, str]] = None,
         id: Optional[str] = None,
         target_id: Optional[str] = None,
         begin: Optional[KmlDateTime] = None,
         end: Optional[KmlDateTime] = None,
     ) -> None:
         super().__init__(ns=ns, name_spaces=name_spaces, id=id, target_id=target_id)
         self.begin = begin
         self.end = end
 
+    def __bool__(self) -> bool:
+        """Return True if the begin or end date is valid."""
+        return bool(self.begin) or bool(self.end)
+
     def etree_element(
         self,
         precision: Optional[int] = None,
         verbosity: Verbosity = Verbosity.normal,
     ) -> Element:
         element = super().etree_element(precision=precision, verbosity=verbosity)
         if self.begin is not None:
-            text = str(self.begin)
-            if text:
+            if text := str(self.begin):
                 begin = config.etree.SubElement(  # type: ignore[attr-defined]
                     element,
                     f"{self.ns}begin",
                 )
                 begin.text = text
         if self.end is not None:
-            text = str(self.end)
-            if text:
+            if text := str(self.end):
                 end = config.etree.SubElement(  # type: ignore[attr-defined]
                     element,
                     f"{self.ns}end",
                 )
                 end.text = text
-        if self.begin == self.end is None:
-            msg = "Either begin, end or both must be set"
-            raise ValueError(msg)
-        # TODO test if end > begin
         return element
 
     @classmethod
     def _get_kwargs(
         cls,
         *,
         ns: str,
```

### Comparing `fastkml-1.0a8/fastkml/types.py` & `fastkml-1.0a9/fastkml/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,29 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301 USA
 
+# Copyright (C) 2023  Christian Ledermann
+#
+# This library is free software; you can redistribute it and/or modify it under
+# the terms of the GNU Lesser General Public License as published by the Free
+# Software Foundation; either version 2.1 of the License, or (at your option)
+# any later version.
+#
+# This library is distributed in the hope that it will be useful, but WITHOUT
+# ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+# FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
+# details.
+#
+# You should have received a copy of the GNU Lesser General Public License
+# along with this library; if not, write to the Free Software Foundation, Inc.,
+# 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301 USA
 """Types for fastkml."""
 from typing import Iterable
 from typing import Optional
 
 from typing_extensions import Protocol
 
 __all__ = ["Element"]
```

### Comparing `fastkml-1.0a8/fastkml.egg-info/PKG-INFO` & `fastkml-1.0a9/fastkml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: fastkml
-Version: 1.0a8
+Version: 1.0a9
 Summary: Fast KML processing in python
 Author-email: Christian Ledermann <christian.ledermann@gmail.com>
 License: LGPL
+Project-URL: Changelog, https://github.com/cleder/fastkml/blob/develop/docs/HISTORY.rst
 Project-URL: Documentation, https://fastkml.readthedocs.org/
 Project-URL: Homepage, https://github.com/cleder/fastkml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
+Classifier: Topic :: Text Processing :: Markup :: XML
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: arrow
 Requires-Dist: pygeoif>=1.1
 Requires-Dist: typing-extensions>4
 Provides-Extra: complexity
 Requires-Dist: lizard; extra == "complexity"
@@ -42,15 +45,14 @@
 Provides-Extra: linting
 Requires-Dist: black; extra == "linting"
 Requires-Dist: flake8; extra == "linting"
 Requires-Dist: flake8-comments; extra == "linting"
 Requires-Dist: flake8-encodings; extra == "linting"
 Requires-Dist: flake8-expression-complexity; extra == "linting"
 Requires-Dist: flake8-length; extra == "linting"
-Requires-Dist: flake8-literal; extra == "linting"
 Requires-Dist: flake8-pep3101; extra == "linting"
 Requires-Dist: flake8-super; extra == "linting"
 Requires-Dist: flake8-typing-imports; extra == "linting"
 Requires-Dist: ruff; extra == "linting"
 Requires-Dist: yamllint; extra == "linting"
 Provides-Extra: lxml
 Requires-Dist: lxml; extra == "lxml"
@@ -59,16 +61,15 @@
 Requires-Dist: pytest-cov; extra == "tests"
 Provides-Extra: typing
 Requires-Dist: mypy; extra == "typing"
 
 Introduction
 ============
 
-KML is an XML geospatial data format and an `OGC standard <https://www.ogc.org/search/content/kml>`_
-that deserves a canonical python implementation.
+KML is an XML geospatial data format and an OGC_ standard that deserves a canonical python implementation.
 
 Fastkml is a library to read, write and manipulate KML files. It aims to keep
 it simple and fast (using lxml_ if available). Fast refers to the time you
 spend to write and read KML files as well as the time you spend to get
 acquainted to the library or to create KML objects. It aims to provide all of
 the functionality that KML clients such as `OpenLayers
 <http://openlayers.org/>`_, `Google Maps <http://maps.google.com/>`_, and
@@ -129,14 +130,19 @@
     :target: https://pypi.python.org/pypi/fastkml/
     :alt: Supported Python implementations
 
 .. image:: https://img.shields.io/librariesio/release/pypi/fastkml
     :target: https://libraries.io/pypi/fastkml
     :alt: Libraries.io dependency status for latest release
 
+.. image:: https://static.pepy.tech/badge/fastkml/month
+    :target: https://pepy.tech/project/fastkml
+    :alt: Downloads
+
+
 Documentation
 =============
 
 You can find all of the documentation for FastKML at `fastkml.readthedocs.org
 <https://fastkml.readthedocs.org>`_. If you find something that is missing,
 please submit a pull request on `GitHub <https://github.com/cleder/fastkml>`_
 with the improvement.
@@ -155,36 +161,32 @@
 
 You can install the package with ``pip install fastkml`` which will pull in all requirements.
 
 Requirements
 -------------
 
 * pygeoif_
-* lxml_
 * arrow_
 
 Optional
 ---------
 
-* lxml_
-
-You can install all of the requirements for working with FastKML by using pip_::
-
-    pip install -r requirements.txt
+* lxml_::
 
+    pip install --pre "fastkml[lxml]"
 
 Limitations
 ===========
 
 *Tesselate*, *Extrude* and *Altitude Mode* are assigned to a Geometry or
 Geometry collection (MultiGeometry). You cannot assign different values of
 *Tesselate*, *Extrude* or *Altitude Mode* on parts of a MultiGeometry.
 
 Currently, the only major feature missing for the full Google Earth experience
 is the `gx extension
 <https://developers.google.com/kml/documentation/kmlreference#kmlextensions>`_.
 Please submit a PR with the features you'd like to see implemented.
 
-.. _pygeoif: http://pypi.python.org/pypi/pygeoif/
+.. _pygeoif: https://pypi.python.org/pypi/pygeoif/
 .. _lxml: https://pypi.python.org/pypi/lxml
 .. _arrow: https://pypi.python.org/pypi/arrow
-.. _pip: https://pypi.python.org/pypi/pip
+.. _OGC: https://www.ogc.org/standard/kml/
```

### Comparing `fastkml-1.0a8/pyproject.toml` & `fastkml-1.0a9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: GIS",
+    "Topic :: Text Processing :: Markup :: XML",
+    "Typing :: Typed",
 ]
 dependencies = [
     "arrow",
     "pygeoif>=1.1",
     "typing-extensions>4",
 ]
 description = "Fast KML processing in python"
@@ -60,15 +62,14 @@
 linting = [
     "black",
     "flake8",
     "flake8-comments",
     "flake8-encodings",
     "flake8-expression-complexity",
     "flake8-length",
-    "flake8-literal",
     "flake8-pep3101",
     "flake8-super",
     "flake8-typing-imports",
     "ruff",
     "yamllint",
 ]
 lxml = [
@@ -90,26 +91,36 @@
     "Google",
     "KML",
     "Maps",
     "OpenLayers",
 ]
 
 [project.urls]
+Changelog = "https://github.com/cleder/fastkml/blob/develop/docs/HISTORY.rst"
 Documentation = "https://fastkml.readthedocs.org/"
 Homepage = "https://github.com/cleder/fastkml"
 
 [tool.check-manifest]
 ignore = [
     ".*",
     "examples/*",
     "mutmut_config.py",
     "test-requirements.txt",
     "tox.ini",
 ]
 
+[tool.coverage.paths]
+source = [
+    "fastkml",
+    "tests",
+]
+
+[tool.coverage.run]
+branch = true
+
 [tool.flake8]
 max_line_length = 89
 
 [tool.isort]
 force_single_line = true
 line_length = 88
 
@@ -122,14 +133,17 @@
 enable_error_code = [
     "ignore-without-code",
 ]
 ignore_errors = false
 ignore_missing_imports = true
 implicit_reexport = false
 no_implicit_optional = true
+overrides = [
+    { disable_error_code = "attr-defined, union-attr", module = "tests.*" },
+]
 show_error_codes = true
 strict_equality = true
 strict_optional = true
 warn_no_return = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
@@ -238,10 +252,14 @@
 include-package-data = true
 
 [tool.setuptools.dynamic.version]
 attr = "fastkml.about.__version__"
 
 [tool.setuptools.packages.find]
 exclude = [
-    "ez_setup",
+    "docs/*",
+]
+include = [
+    "fastkml*",
+    "fastkml/py.typed",
 ]
 namespaces = false
```

