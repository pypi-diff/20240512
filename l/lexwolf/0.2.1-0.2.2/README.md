# Comparing `tmp/lexwolf-0.2.1.tar.gz` & `tmp/lexwolf-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexwolf-0.2.1.tar", last modified: Sun May 12 12:04:00 2024, max compression
+gzip compressed data, was "lexwolf-0.2.2.tar", last modified: Sun May 12 12:10:03 2024, max compression
```

## Comparing `lexwolf-0.2.1.tar` & `lexwolf-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-05-12 12:04:00.582492 lexwolf-0.2.1/
--rwxrwxrwx   0 allem     (1000) allem     (1000)     1098 2023-11-24 20:23:52.000000 lexwolf-0.2.1/LICENSE
--rwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-02-20 19:13:22.000000 lexwolf-0.2.1/MANIFEST.in
--rwxrwxrwx   0 allem     (1000) allem     (1000)     4667 2024-05-12 12:04:00.573475 lexwolf-0.2.1/PKG-INFO
--rwxrwxrwx   0 allem     (1000) allem     (1000)     3804 2024-05-12 11:59:37.000000 lexwolf-0.2.1/README.md
-drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-05-12 12:04:00.424492 lexwolf-0.2.1/lexwolf/
--rwxrwxrwx   0 allem     (1000) allem     (1000)    88811 2024-05-12 11:46:37.000000 lexwolf-0.2.1/lexwolf/__init__.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     5709 2024-03-30 15:39:12.000000 lexwolf-0.2.1/lexwolf/adaptativeminmax.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)    42088 2024-04-05 16:19:22.000000 lexwolf-0.2.1/lexwolf/bitBoard.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     3471 2024-03-29 16:05:20.000000 lexwolf-0.2.1/lexwolf/core.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     1613 2024-03-29 16:00:17.000000 lexwolf-0.2.1/lexwolf/dEvalTest.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)    15853 2024-03-08 11:29:43.000000 lexwolf-0.2.1/lexwolf/genetic.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)      459 2024-03-08 11:29:43.000000 lexwolf-0.2.1/lexwolf/interfpsql.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)    12724 2024-04-05 15:31:20.000000 lexwolf-0.2.1/lexwolf/minmax.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)    18762 2024-03-21 17:08:34.000000 lexwolf-0.2.1/lexwolf/structEl.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     3592 2024-04-01 17:23:48.000000 lexwolf-0.2.1/lexwolf/tests.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     2173 2024-03-31 13:07:22.000000 lexwolf-0.2.1/lexwolf/weights.py
-drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-05-12 12:04:00.560492 lexwolf-0.2.1/lexwolf.egg-info/
--rwxrwxrwx   0 allem     (1000) allem     (1000)     4667 2024-05-12 12:03:59.000000 lexwolf-0.2.1/lexwolf.egg-info/PKG-INFO
--rwxrwxrwx   0 allem     (1000) allem     (1000)      412 2024-05-12 12:04:00.000000 lexwolf-0.2.1/lexwolf.egg-info/SOURCES.txt
--rwxrwxrwx   0 allem     (1000) allem     (1000)        1 2024-05-12 12:03:59.000000 lexwolf-0.2.1/lexwolf.egg-info/dependency_links.txt
--rwxrwxrwx   0 allem     (1000) allem     (1000)       47 2024-05-12 12:03:59.000000 lexwolf-0.2.1/lexwolf.egg-info/requires.txt
--rwxrwxrwx   0 allem     (1000) allem     (1000)        8 2024-05-12 12:03:59.000000 lexwolf-0.2.1/lexwolf.egg-info/top_level.txt
--rwxrwxrwx   0 allem     (1000) allem     (1000)       38 2024-05-12 12:04:00.584497 lexwolf-0.2.1/setup.cfg
--rwxrwxrwx   0 allem     (1000) allem     (1000)     1498 2024-05-12 12:01:40.000000 lexwolf-0.2.1/setup.py
+drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-05-12 12:10:03.862091 lexwolf-0.2.2/
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     1098 2023-11-24 20:23:52.000000 lexwolf-0.2.2/LICENSE
+-rwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-02-20 19:13:22.000000 lexwolf-0.2.2/MANIFEST.in
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     4521 2024-05-12 12:10:03.853093 lexwolf-0.2.2/PKG-INFO
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     3804 2024-05-12 11:59:37.000000 lexwolf-0.2.2/README.md
+drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-05-12 12:10:03.705091 lexwolf-0.2.2/lexwolf/
+-rwxrwxrwx   0 allem     (1000) allem     (1000)    88811 2024-05-12 11:46:37.000000 lexwolf-0.2.2/lexwolf/__init__.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     5709 2024-03-30 15:39:12.000000 lexwolf-0.2.2/lexwolf/adaptativeminmax.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)    42088 2024-04-05 16:19:22.000000 lexwolf-0.2.2/lexwolf/bitBoard.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     3471 2024-03-29 16:05:20.000000 lexwolf-0.2.2/lexwolf/core.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     1613 2024-03-29 16:00:17.000000 lexwolf-0.2.2/lexwolf/dEvalTest.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)    15853 2024-03-08 11:29:43.000000 lexwolf-0.2.2/lexwolf/genetic.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)      459 2024-03-08 11:29:43.000000 lexwolf-0.2.2/lexwolf/interfpsql.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)    12724 2024-04-05 15:31:20.000000 lexwolf-0.2.2/lexwolf/minmax.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)    18762 2024-03-21 17:08:34.000000 lexwolf-0.2.2/lexwolf/structEl.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     3592 2024-04-01 17:23:48.000000 lexwolf-0.2.2/lexwolf/tests.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     2173 2024-03-31 13:07:22.000000 lexwolf-0.2.2/lexwolf/weights.py
+drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-05-12 12:10:03.841092 lexwolf-0.2.2/lexwolf.egg-info/
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     4521 2024-05-12 12:10:03.000000 lexwolf-0.2.2/lexwolf.egg-info/PKG-INFO
+-rwxrwxrwx   0 allem     (1000) allem     (1000)      412 2024-05-12 12:10:03.000000 lexwolf-0.2.2/lexwolf.egg-info/SOURCES.txt
+-rwxrwxrwx   0 allem     (1000) allem     (1000)        1 2024-05-12 12:10:03.000000 lexwolf-0.2.2/lexwolf.egg-info/dependency_links.txt
+-rwxrwxrwx   0 allem     (1000) allem     (1000)        6 2024-05-12 12:10:03.000000 lexwolf-0.2.2/lexwolf.egg-info/requires.txt
+-rwxrwxrwx   0 allem     (1000) allem     (1000)        8 2024-05-12 12:10:03.000000 lexwolf-0.2.2/lexwolf.egg-info/top_level.txt
+-rwxrwxrwx   0 allem     (1000) allem     (1000)       38 2024-05-12 12:10:03.863092 lexwolf-0.2.2/setup.cfg
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     1436 2024-05-12 12:10:00.000000 lexwolf-0.2.2/setup.py
```

### Comparing `lexwolf-0.2.1/LICENSE` & `lexwolf-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/PKG-INFO` & `lexwolf-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexwolf
-Version: 0.2.1
+Version: 0.2.2
 Summary: The LexWolf chess artificial intelligences.
 Home-page: 
 Author: Alexandre Le Mercier
 Author-email: alexandre.le.mercier@ulb.be
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,21 +14,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: chess
-Requires-Dist: numpy
-Requires-Dist: math
-Requires-Dist: random
-Requires-Dist: time
-Requires-Dist: pandas
-Requires-Dist: IPython
-Requires-Dist: os
 
 # LexWolf Chess Library
 
 ## Created by Loup François and Alexandre Le Mercier
 
 ### Duration: February to May 2024
```

### Comparing `lexwolf-0.2.1/README.md` & `lexwolf-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf/__init__.py` & `lexwolf-0.2.2/lexwolf/__init__.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf/adaptativeminmax.py` & `lexwolf-0.2.2/lexwolf/adaptativeminmax.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf/bitBoard.py` & `lexwolf-0.2.2/lexwolf/bitBoard.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf/core.py` & `lexwolf-0.2.2/lexwolf/core.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf/dEvalTest.py` & `lexwolf-0.2.2/lexwolf/dEvalTest.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf/genetic.py` & `lexwolf-0.2.2/lexwolf/genetic.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf/minmax.py` & `lexwolf-0.2.2/lexwolf/minmax.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf/structEl.py` & `lexwolf-0.2.2/lexwolf/structEl.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf/tests.py` & `lexwolf-0.2.2/lexwolf/tests.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf/weights.py` & `lexwolf-0.2.2/lexwolf/weights.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.2.1/lexwolf.egg-info/PKG-INFO` & `lexwolf-0.2.2/lexwolf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexwolf
-Version: 0.2.1
+Version: 0.2.2
 Summary: The LexWolf chess artificial intelligences.
 Home-page: 
 Author: Alexandre Le Mercier
 Author-email: alexandre.le.mercier@ulb.be
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,21 +14,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: chess
-Requires-Dist: numpy
-Requires-Dist: math
-Requires-Dist: random
-Requires-Dist: time
-Requires-Dist: pandas
-Requires-Dist: IPython
-Requires-Dist: os
 
 # LexWolf Chess Library
 
 ## Created by Loup François and Alexandre Le Mercier
 
 ### Duration: February to May 2024
```

### Comparing `lexwolf-0.2.1/setup.py` & `lexwolf-0.2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="lexwolf",
-    version="0.2.1",
+    version="0.2.2",
     description="The LexWolf chess artificial intelligences.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Alexandre Le Mercier",
     author_email="alexandre.le.mercier@ulb.be",
     license="MIT",
@@ -34,15 +34,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["lexwolf"],
     include_package_data=True,
-    install_requires=["chess", "numpy", "math", "random", "time", "pandas", "IPython", "os"]
+    install_requires=["chess"]
 )
 
 """
 python setup.py sdist bdist_wheel
 twine check dist/*
 twine upload dist/*
 """
```

