# Comparing `tmp/epconversions-0.2.1.tar.gz` & `tmp/epconversions-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epconversions-0.2.1.tar", last modified: Fri May 10 16:45:00 2024, max compression
+gzip compressed data, was "epconversions-0.2.2.tar", last modified: Sun May 12 14:43:38 2024, max compression
```

## Comparing `epconversions-0.2.1.tar` & `epconversions-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.889674 epconversions-0.2.1/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      159 2023-10-28 22:26:04.000000 epconversions-0.2.1/AUTHORS.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1307 2023-10-31 21:07:15.000000 epconversions-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      257 2024-05-10 16:44:22.000000 epconversions-0.2.1/HISTORY.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)    16725 2023-10-28 22:40:28.000000 epconversions-0.2.1/LICENSE
--rw-r--r--   0 santoshphilip   (501) staff       (20)      262 2023-10-28 22:26:04.000000 epconversions-0.2.1/MANIFEST.in
--rw-r--r--   0 santoshphilip   (501) staff       (20)     5079 2024-05-10 16:45:00.889816 epconversions-0.2.1/PKG-INFO
--rw-r--r--   0 santoshphilip   (501) staff       (20)     4040 2023-11-02 16:39:14.000000 epconversions-0.2.1/README.rst
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.885993 epconversions-0.2.1/docs/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      614 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/Makefile
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.879892 epconversions-0.2.1/docs/_build/
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.879966 epconversions-0.2.1/docs/_build/html/
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.886935 epconversions-0.2.1/docs/_build/html/_static/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      286 2023-10-28 22:37:04.000000 epconversions-0.2.1/docs/_build/html/_static/file.png
--rw-r--r--   0 santoshphilip   (501) staff       (20)       90 2023-10-28 22:37:04.000000 epconversions-0.2.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 santoshphilip   (501) staff       (20)       90 2023-10-28 22:37:04.000000 epconversions-0.2.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/authors.rst
--rwxr-xr-x   0 santoshphilip   (501) staff       (20)     4986 2023-11-02 17:04:04.000000 epconversions-0.2.1/docs/conf.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)       33 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/contributing.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      355 2023-11-02 17:09:16.000000 epconversions-0.2.1/docs/epconversions.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/history.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      313 2023-11-01 18:58:46.000000 epconversions-0.2.1/docs/index.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1178 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/installation.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)      811 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/make.bat
--rw-r--r--   0 santoshphilip   (501) staff       (20)       76 2023-11-02 17:09:16.000000 epconversions-0.2.1/docs/modules.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)       27 2023-10-28 22:15:52.000000 epconversions-0.2.1/docs/readme.rst
--rw-r--r--   0 santoshphilip   (501) staff       (20)     1394 2023-11-02 16:42:00.000000 epconversions-0.2.1/docs/usage.rst
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.887379 epconversions-0.2.1/epconversions/
--rw-r--r--   0 santoshphilip   (501) staff       (20)      134 2024-05-10 16:44:22.000000 epconversions-0.2.1/epconversions/__init__.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)    38143 2024-05-10 05:41:36.000000 epconversions-0.2.1/epconversions/epconversions.py
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.888794 epconversions-0.2.1/epconversions.egg-info/
--rw-r--r--   0 santoshphilip   (501) staff       (20)     5079 2024-05-10 16:45:00.000000 epconversions-0.2.1/epconversions.egg-info/PKG-INFO
--rw-r--r--   0 santoshphilip   (501) staff       (20)      685 2024-05-10 16:45:00.000000 epconversions-0.2.1/epconversions.egg-info/SOURCES.txt
--rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2024-05-10 16:45:00.000000 epconversions-0.2.1/epconversions.egg-info/dependency_links.txt
--rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2024-05-10 16:45:00.000000 epconversions-0.2.1/epconversions.egg-info/not-zip-safe
--rw-r--r--   0 santoshphilip   (501) staff       (20)       14 2024-05-10 16:45:00.000000 epconversions-0.2.1/epconversions.egg-info/top_level.txt
--rw-r--r--   0 santoshphilip   (501) staff       (20)      428 2024-05-10 16:45:00.890120 epconversions-0.2.1/setup.cfg
--rwxr-xr-x   0 santoshphilip   (501) staff       (20)     1359 2024-05-10 16:44:22.000000 epconversions-0.2.1/setup.py
-drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-10 16:45:00.889286 epconversions-0.2.1/tests/
--rw-r--r--   0 santoshphilip   (501) staff       (20)       43 2023-10-28 22:15:52.000000 epconversions-0.2.1/tests/__init__.py
--rw-r--r--   0 santoshphilip   (501) staff       (20)    21368 2024-05-10 05:41:59.000000 epconversions-0.2.1/tests/test_epconversions.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-12 14:43:38.502443 epconversions-0.2.2/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      159 2023-10-28 22:26:04.000000 epconversions-0.2.2/AUTHORS.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1307 2023-10-31 21:07:15.000000 epconversions-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      403 2024-05-12 14:41:48.000000 epconversions-0.2.2/HISTORY.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)    16725 2023-10-28 22:40:28.000000 epconversions-0.2.2/LICENSE
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      262 2023-10-28 22:26:04.000000 epconversions-0.2.2/MANIFEST.in
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     5577 2024-05-12 14:43:38.502847 epconversions-0.2.2/PKG-INFO
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     4392 2024-05-12 04:55:57.000000 epconversions-0.2.2/README.rst
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-12 14:43:38.497642 epconversions-0.2.2/docs/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      614 2023-10-28 22:15:52.000000 epconversions-0.2.2/docs/Makefile
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-12 14:43:38.491130 epconversions-0.2.2/docs/_build/
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-12 14:43:38.491222 epconversions-0.2.2/docs/_build/html/
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-12 14:43:38.498556 epconversions-0.2.2/docs/_build/html/_static/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      286 2023-10-28 22:37:04.000000 epconversions-0.2.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       90 2023-10-28 22:37:04.000000 epconversions-0.2.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       90 2023-10-28 22:37:04.000000 epconversions-0.2.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2023-10-28 22:15:52.000000 epconversions-0.2.2/docs/authors.rst
+-rwxr-xr-x   0 santoshphilip   (501) staff       (20)     4986 2023-11-02 17:04:04.000000 epconversions-0.2.2/docs/conf.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       33 2023-10-28 22:15:52.000000 epconversions-0.2.2/docs/contributing.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      492 2024-05-12 14:36:04.000000 epconversions-0.2.2/docs/epconversions.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       28 2023-10-28 22:15:52.000000 epconversions-0.2.2/docs/history.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      313 2023-11-01 18:58:46.000000 epconversions-0.2.2/docs/index.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1178 2023-10-28 22:15:52.000000 epconversions-0.2.2/docs/installation.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      811 2023-10-28 22:15:52.000000 epconversions-0.2.2/docs/make.bat
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       76 2024-05-12 14:36:04.000000 epconversions-0.2.2/docs/modules.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       27 2023-10-28 22:15:52.000000 epconversions-0.2.2/docs/readme.rst
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1394 2023-11-02 16:42:00.000000 epconversions-0.2.2/docs/usage.rst
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-12 14:43:38.499536 epconversions-0.2.2/epconversions/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      134 2024-05-12 05:08:03.000000 epconversions-0.2.2/epconversions/__init__.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      591 2024-05-12 04:32:24.000000 epconversions-0.2.2/epconversions/ec.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)    38143 2024-05-10 05:41:36.000000 epconversions-0.2.2/epconversions/epconversions.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-12 14:43:38.501110 epconversions-0.2.2/epconversions.egg-info/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     5577 2024-05-12 14:43:38.000000 epconversions-0.2.2/epconversions.egg-info/PKG-INFO
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      722 2024-05-12 14:43:38.000000 epconversions-0.2.2/epconversions.egg-info/SOURCES.txt
+-rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2024-05-12 14:43:38.000000 epconversions-0.2.2/epconversions.egg-info/dependency_links.txt
+-rw-r--r--   0 santoshphilip   (501) staff       (20)        1 2024-05-12 14:43:38.000000 epconversions-0.2.2/epconversions.egg-info/not-zip-safe
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       14 2024-05-12 14:43:38.000000 epconversions-0.2.2/epconversions.egg-info/top_level.txt
+-rw-r--r--   0 santoshphilip   (501) staff       (20)      428 2024-05-12 14:43:38.503217 epconversions-0.2.2/setup.cfg
+-rwxr-xr-x   0 santoshphilip   (501) staff       (20)     1359 2024-05-12 05:08:03.000000 epconversions-0.2.2/setup.py
+drwxr-xr-x   0 santoshphilip   (501) staff       (20)        0 2024-05-12 14:43:38.501924 epconversions-0.2.2/tests/
+-rw-r--r--   0 santoshphilip   (501) staff       (20)       43 2023-10-28 22:15:52.000000 epconversions-0.2.2/tests/__init__.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)     1224 2024-05-12 05:14:28.000000 epconversions-0.2.2/tests/test_ec.py
+-rw-r--r--   0 santoshphilip   (501) staff       (20)    21368 2024-05-10 05:41:59.000000 epconversions-0.2.2/tests/test_epconversions.py
```

### Comparing `epconversions-0.2.1/CONTRIBUTING.rst` & `epconversions-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.1/LICENSE` & `epconversions-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.1/PKG-INFO` & `epconversions-0.2.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: epconversions
-Version: 0.2.1
-Summary: Unit conversions for E+
-Home-page: https://github.com/pyenergyplus/epconversions
-Author: Santosh Philip
-Author-email: santosh@noemail.com
-License: MIT license
-Keywords: epconversions
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.6
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 =============
 epconversions
 =============
 
 
 .. image:: https://img.shields.io/pypi/v/epconversions.svg
         :target: https://pypi.python.org/pypi/epconversions
@@ -154,38 +132,30 @@
     'years']
 
     # around 128 now
 
     # also try out ``allipunits()``
 
 
+This is all to complicated. Don't you have an easy way to convert from Fahrenheit to Celsius ?
+
+Yes! There is an easier way::
+
+    from epconversions import ec
+    c = ec.f2c(77)
+    print(c)
+    
+    >> 25.0
+
+That is as easy as it gets. Right now we have ``f2c`` and ``c2f``. If you want more easy functions, open an issue and add to them yourself.
+
+
 Thats all for now
 
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-
-
-=======
-History
-=======
-
-
-
-2024-05-10
-----------
-
-fixed issue #16
-
-:Problem: convert2ip and convert2si do not convert strings to floats
-:Solution: strings are converted to floats if possible
-
-
-0.1.0 (2023-10-28)
-------------------
-
-* First release on PyPI.
```

### Comparing `epconversions-0.2.1/docs/Makefile` & `epconversions-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.1/docs/conf.py` & `epconversions-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.1/docs/installation.rst` & `epconversions-0.2.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.1/docs/make.bat` & `epconversions-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.1/docs/usage.rst` & `epconversions-0.2.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.1/epconversions/epconversions.py` & `epconversions-0.2.2/epconversions/epconversions.py`

 * *Files identical despite different names*

### Comparing `epconversions-0.2.1/epconversions.egg-info/PKG-INFO` & `epconversions-0.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epconversions
-Version: 0.2.1
+Version: 0.2.2
 Summary: Unit conversions for E+
 Home-page: https://github.com/pyenergyplus/epconversions
 Author: Santosh Philip
 Author-email: santosh@noemail.com
 License: MIT license
 Keywords: epconversions
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -154,14 +154,27 @@
     'years']
 
     # around 128 now
 
     # also try out ``allipunits()``
 
 
+This is all to complicated. Don't you have an easy way to convert from Fahrenheit to Celsius ?
+
+Yes! There is an easier way::
+
+    from epconversions import ec
+    c = ec.f2c(77)
+    print(c)
+    
+    >> 25.0
+
+That is as easy as it gets. Right now we have ``f2c`` and ``c2f``. If you want more easy functions, open an issue and add to them yourself.
+
+
 Thats all for now
 
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
@@ -170,22 +183,34 @@
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
 
+release 0.2.2
+-------------
+
+
+2024-05-11
+----------
+
+fixed issue #19
+
+:Problem: easy functions needed like f2c and c2f
+:Solutions: added ec.f2c and ec.c2f
+
 
 
 2024-05-10
 ----------
 
 fixed issue #16
 
 :Problem: convert2ip and convert2si do not convert strings to floats
 :Solution: strings are converted to floats if possible
 
 
-0.1.0 (2023-10-28)
-------------------
+release 0.1.0
+-------------
 
 * First release on PyPI.
```

### Comparing `epconversions-0.2.1/epconversions.egg-info/SOURCES.txt` & `epconversions-0.2.2/epconversions.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 docs/modules.rst
 docs/readme.rst
 docs/usage.rst
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 epconversions/__init__.py
+epconversions/ec.py
 epconversions/epconversions.py
 epconversions.egg-info/PKG-INFO
 epconversions.egg-info/SOURCES.txt
 epconversions.egg-info/dependency_links.txt
 epconversions.egg-info/not-zip-safe
 epconversions.egg-info/top_level.txt
 tests/__init__.py
+tests/test_ec.py
 tests/test_epconversions.py
```

### Comparing `epconversions-0.2.1/setup.py` & `epconversions-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="epconversions",
     name="epconversions",
     packages=find_packages(include=["epconversions", "epconversions.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/pyenergyplus/epconversions",
-    version="0.2.1",
+    version="0.2.2",
     zip_safe=False,
 )
```

### Comparing `epconversions-0.2.1/tests/test_epconversions.py` & `epconversions-0.2.2/tests/test_epconversions.py`

 * *Files identical despite different names*

