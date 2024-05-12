# Comparing `tmp/pybacting-0.2.8.tar.gz` & `tmp/pybacting-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybacting-0.2.8.tar", last modified: Mon Mar 28 13:05:18 2022, max compression
+gzip compressed data, was "pybacting-0.2.9.tar", last modified: Fri Oct 21 09:45:02 2022, max compression
```

## Comparing `pybacting-0.2.8.tar` & `pybacting-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,33 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-03-28 13:05:18.680743 pybacting-0.2.8/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-03-06 17:33:17.000000 pybacting-0.2.8/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      331 2022-01-03 21:29:47.000000 pybacting-0.2.8/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     2646 2022-03-28 13:05:18.680868 pybacting-0.2.8/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     1589 2022-03-06 17:33:39.000000 pybacting-0.2.8/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-03-28 13:05:18.667313 pybacting-0.2.8/docs/
--rw-r--r--   0 cthoyt     (501) staff       (20)      610 2021-03-15 16:11:56.000000 pybacting-0.2.8/docs/Makefile
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-03-28 13:05:18.670001 pybacting-0.2.8/docs/source/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-03-28 13:05:18.674336 pybacting-0.2.8/docs/source/api/
--rw-r--r--   0 cthoyt     (501) staff       (20)       73 2021-08-05 11:06:22.000000 pybacting-0.2.8/docs/source/api/pybacting.api.biojava.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       76 2021-08-05 11:06:22.000000 pybacting-0.2.8/docs/source/api/pybacting.api.bridgedb.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       61 2021-08-05 11:06:22.000000 pybacting-0.2.8/docs/source/api/pybacting.api.cdk.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       67 2021-08-05 11:06:22.000000 pybacting-0.2.8/docs/source/api/pybacting.api.excel.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       67 2021-08-05 11:06:22.000000 pybacting-0.2.8/docs/source/api/pybacting.api.inchi.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       67 2021-08-05 11:06:22.000000 pybacting-0.2.8/docs/source/api/pybacting.api.opsin.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       67 2021-08-05 11:06:22.000000 pybacting-0.2.8/docs/source/api/pybacting.api.oscar.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       73 2021-08-05 11:06:22.000000 pybacting-0.2.8/docs/source/api/pybacting.api.pubchem.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       61 2021-08-05 11:06:22.000000 pybacting-0.2.8/docs/source/api/pybacting.api.rdf.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       61 2021-08-05 11:06:22.000000 pybacting-0.2.8/docs/source/api/pybacting.api.xml.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     6736 2022-03-28 13:05:16.000000 pybacting-0.2.8/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      291 2021-08-05 11:09:14.000000 pybacting-0.2.8/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      515 2021-08-05 10:59:45.000000 pybacting-0.2.8/docs/source/installation.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      109 2021-08-05 11:06:18.000000 pybacting-0.2.8/docs/source/managers.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      358 2022-03-06 13:15:46.000000 pybacting-0.2.8/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     1619 2022-03-28 13:05:18.681576 pybacting-0.2.8/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-03-28 13:05:18.665088 pybacting-0.2.8/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-03-28 13:05:18.677764 pybacting-0.2.8/src/pybacting/
--rw-r--r--   0 cthoyt     (501) staff       (20)      376 2022-03-06 17:31:11.000000 pybacting-0.2.8/src/pybacting/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      112 2021-08-05 11:11:24.000000 pybacting-0.2.8/src/pybacting/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3690 2022-03-28 13:04:10.000000 pybacting-0.2.8/src/pybacting/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      219 2021-08-05 11:11:24.000000 pybacting-0.2.8/src/pybacting/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      381 2021-08-03 09:49:44.000000 pybacting-0.2.8/src/pybacting/display.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      864 2021-08-03 09:49:56.000000 pybacting-0.2.8/src/pybacting/io.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1018 2022-03-28 13:05:16.000000 pybacting-0.2.8/src/pybacting/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-03-28 13:05:18.679476 pybacting-0.2.8/src/pybacting.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     2646 2022-03-28 13:05:18.000000 pybacting-0.2.8/src/pybacting.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)      989 2022-03-28 13:05:18.000000 pybacting-0.2.8/src/pybacting.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-03-28 13:05:18.000000 pybacting-0.2.8/src/pybacting.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2021-07-29 15:23:11.000000 pybacting-0.2.8/src/pybacting.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)       83 2022-03-28 13:05:18.000000 pybacting-0.2.8/src/pybacting.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       10 2022-03-28 13:05:18.000000 pybacting-0.2.8/src/pybacting.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-03-28 13:05:18.680225 pybacting-0.2.8/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       59 2021-07-29 15:23:05.000000 pybacting-0.2.8/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1079 2022-01-03 21:29:47.000000 pybacting-0.2.8/tests/test_trivial.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-10-21 09:45:02.473766 pybacting-0.2.9/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-03-06 17:33:17.000000 pybacting-0.2.9/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      331 2022-01-03 21:29:47.000000 pybacting-0.2.9/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2626 2022-10-21 09:45:02.473888 pybacting-0.2.9/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1589 2022-03-06 17:33:39.000000 pybacting-0.2.9/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-10-21 09:45:02.457224 pybacting-0.2.9/docs/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      610 2021-03-15 16:11:56.000000 pybacting-0.2.9/docs/Makefile
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-10-21 09:45:02.459090 pybacting-0.2.9/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6736 2022-10-21 09:45:01.000000 pybacting-0.2.9/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      291 2021-08-05 11:09:14.000000 pybacting-0.2.9/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      515 2021-08-05 10:59:45.000000 pybacting-0.2.9/docs/source/installation.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      109 2021-08-05 11:06:18.000000 pybacting-0.2.9/docs/source/managers.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      358 2022-03-06 13:15:46.000000 pybacting-0.2.9/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1634 2022-10-21 09:45:02.474713 pybacting-0.2.9/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-10-21 09:45:02.455135 pybacting-0.2.9/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-10-21 09:45:02.470815 pybacting-0.2.9/src/pybacting/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      376 2022-03-06 17:31:11.000000 pybacting-0.2.9/src/pybacting/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2021-08-05 11:11:24.000000 pybacting-0.2.9/src/pybacting/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3689 2022-10-21 09:35:32.000000 pybacting-0.2.9/src/pybacting/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      219 2021-08-05 11:11:24.000000 pybacting-0.2.9/src/pybacting/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      381 2021-08-03 09:49:44.000000 pybacting-0.2.9/src/pybacting/display.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      864 2021-08-03 09:49:56.000000 pybacting-0.2.9/src/pybacting/io.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1018 2022-10-21 09:45:01.000000 pybacting-0.2.9/src/pybacting/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-10-21 09:45:02.472617 pybacting-0.2.9/src/pybacting.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2626 2022-10-21 09:45:02.000000 pybacting-0.2.9/src/pybacting.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)      588 2022-10-21 09:45:02.000000 pybacting-0.2.9/src/pybacting.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-10-21 09:45:02.000000 pybacting-0.2.9/src/pybacting.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2021-07-29 15:23:11.000000 pybacting-0.2.9/src/pybacting.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)       96 2022-10-21 09:45:02.000000 pybacting-0.2.9/src/pybacting.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       10 2022-10-21 09:45:02.000000 pybacting-0.2.9/src/pybacting.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2022-10-21 09:45:02.473268 pybacting-0.2.9/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       59 2021-07-29 15:23:05.000000 pybacting-0.2.9/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1079 2022-01-03 21:29:47.000000 pybacting-0.2.9/tests/test_trivial.py
```

### Comparing `pybacting-0.2.8/LICENSE` & `pybacting-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybacting-0.2.8/PKG-INFO` & `pybacting-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pybacting
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python wrapper around Bacting
 Home-page: https://github.com/cthoyt/pybacting
 Download-URL: https://github.com/cthoyt/pybacting/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cthoyt/pybacting/issues
 Keywords: CDK,cheminformatics,chemistry
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -76,9 +75,7 @@
 Download and install from source in development mode:
 
 ```shell
 $ git clone https://github.com/cthoyt/pybacting
 $ cd pybacting
 $ pip install --editable .
 ```
-
-
```

### Comparing `pybacting-0.2.8/README.md` & `pybacting-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pybacting-0.2.8/docs/Makefile` & `pybacting-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybacting-0.2.8/docs/source/conf.py` & `pybacting-0.2.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'pybacting'
 copyright = f'{date.today().year}, Charles Tapley Hoyt'
 author = 'Charles Tapley Hoyt'
 
 # The full version, including alpha/beta/rc tags.
-release = '0.2.8'
+release = '0.2.9'
 
 # The short X.Y version.
 parsed_version = re.match(
     '(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?',
     release,
 )
 version = parsed_version.expand('\g<major>.\g<minor>.\g<patch>')
@@ -83,15 +83,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `pybacting-0.2.8/docs/source/installation.rst` & `pybacting-0.2.9/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pybacting-0.2.8/setup.cfg` & `pybacting-0.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybacting
-version = 0.2.8
+version = 0.2.9
 description = A python wrapper around Bacting
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/pybacting
 download_url = https://github.com/cthoyt/pybacting/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/pybacting/issues
@@ -28,14 +28,16 @@
 keywords = 
 	CDK
 	cheminformatics
 	chemistry
 
 [options]
 install_requires = 
+	numpy
+	pandas
 	scyjava
 zip_safe = false
 include_package_data = True
 python_requires = >=3.7
 packages = find:
 package_dir = 
 	= src
```

### Comparing `pybacting-0.2.8/src/pybacting/api.py` & `pybacting-0.2.9/src/pybacting/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,35 +15,35 @@
     "pubchem",
     "qudt",
     "rdf",
     "xml",
 ]
 
 WORKSPACE = "."
-VERSION = "0.0.34"
+VERSION = "0.1.2"
 
 # The ones marked with "no" can't be loaded because they are POM-only
 # artifacts. See the excellent explanation given by @ctrueden why at:
 # https://github.com/scijava/scyjava/issues/30#issuecomment-892061823
 endpoints = (
     # f"io.github.egonw.bacting:managers-semweb:{VERSION}", # no
+    f"io.github.egonw.bacting:bacting-core:{VERSION}",
+    f"io.github.egonw.bacting:managers-cdk:{VERSION}",
     f"io.github.egonw.bacting:managers-inchi:{VERSION}",
     f"io.github.egonw.bacting:managers-pubchem:{VERSION}",
     f"io.github.egonw.bacting:managers-xml:{VERSION}",
     f"io.github.egonw.bacting:managers-rdf:{VERSION}",
     # f"io.github.egonw.bacting:managers-bioinfo:{VERSION}", # no
     f"io.github.egonw.bacting:managers-oscar:{VERSION}",
     # f"io.github.egonw.bacting:managers-cheminfo:{VERSION}",# no
     f"io.github.egonw.bacting:managers-ui:{VERSION}",
     f"io.github.egonw.bacting:managers-excel:{VERSION}",
     f"io.github.egonw.bacting:managers-opsin:{VERSION}",
-    f"io.github.egonw.bacting:managers-cdk:{VERSION}",
     f"io.github.egonw.bacting:managers-biojava:{VERSION}",
     f"io.github.egonw.bacting:managers-bridgedb:{VERSION}",
-    f"io.github.egonw.bacting:bacting-core:{VERSION}",
 )
 config.endpoints.extend(endpoints)
 
 # Connecting to the JVM is usually done implicitly, but since spreading
 # the endpoints and instantiation across many classes causes a problem,
 # it's better to consolidate them here and make instantiation explicit
 start_jvm()
```

### Comparing `pybacting-0.2.8/src/pybacting/io.py` & `pybacting-0.2.9/src/pybacting/io.py`

 * *Files identical despite different names*

### Comparing `pybacting-0.2.8/src/pybacting/version.py` & `pybacting-0.2.9/src/pybacting/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.2.8"
+VERSION = "0.2.9"
 
 
 def get_git_hash() -> Optional[str]:
     """Get the git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `pybacting-0.2.8/src/pybacting.egg-info/PKG-INFO` & `pybacting-0.2.9/src/pybacting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: pybacting
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python wrapper around Bacting
 Home-page: https://github.com/cthoyt/pybacting
 Download-URL: https://github.com/cthoyt/pybacting/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cthoyt/pybacting/issues
 Keywords: CDK,cheminformatics,chemistry
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -76,9 +75,7 @@
 Download and install from source in development mode:
 
 ```shell
 $ git clone https://github.com/cthoyt/pybacting
 $ cd pybacting
 $ pip install --editable .
 ```
-
-
```

### Comparing `pybacting-0.2.8/tests/test_trivial.py` & `pybacting-0.2.9/tests/test_trivial.py`

 * *Files identical despite different names*

