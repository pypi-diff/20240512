# Comparing `tmp/nchuchain-1.0.1.tar.gz` & `tmp/nchuchain-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nchuchain-1.0.1.tar", last modified: Sat May 11 20:49:21 2024, max compression
+gzip compressed data, was "nchuchain-1.0.2.tar", last modified: Sun May 12 21:50:23 2024, max compression
```

## Comparing `nchuchain-1.0.1.tar` & `nchuchain-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-11 20:49:21.816630 nchuchain-1.0.1/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1068 2024-05-07 09:39:28.000000 nchuchain-1.0.1/LICENSE
--rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      709 2024-05-11 20:49:21.816630 nchuchain-1.0.1/PKG-INFO
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        4 2024-05-07 09:38:57.000000 nchuchain-1.0.1/README.md
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-11 20:49:21.816630 nchuchain-1.0.1/nchuchain.egg-info/
--rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      709 2024-05-11 20:49:21.000000 nchuchain-1.0.1/nchuchain.egg-info/PKG-INFO
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      190 2024-05-11 20:49:21.000000 nchuchain-1.0.1/nchuchain.egg-info/SOURCES.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        1 2024-05-11 20:49:21.000000 nchuchain-1.0.1/nchuchain.egg-info/dependency_links.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      138 2024-05-11 20:49:21.000000 nchuchain-1.0.1/nchuchain.egg-info/requires.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        1 2024-05-11 20:49:21.000000 nchuchain-1.0.1/nchuchain.egg-info/top_level.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       38 2024-05-11 20:49:21.816630 nchuchain-1.0.1/setup.cfg
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1282 2024-05-11 20:47:23.000000 nchuchain-1.0.1/setup.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-12 21:50:23.894053 nchuchain-1.0.2/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1068 2024-05-07 09:39:28.000000 nchuchain-1.0.2/LICENSE
+-rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      825 2024-05-12 21:50:23.890053 nchuchain-1.0.2/PKG-INFO
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        4 2024-05-07 09:38:57.000000 nchuchain-1.0.2/README.md
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-12 21:50:23.890053 nchuchain-1.0.2/nchuchain.egg-info/
+-rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      825 2024-05-12 21:50:23.000000 nchuchain-1.0.2/nchuchain.egg-info/PKG-INFO
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      190 2024-05-12 21:50:23.000000 nchuchain-1.0.2/nchuchain.egg-info/SOURCES.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        1 2024-05-12 21:50:23.000000 nchuchain-1.0.2/nchuchain.egg-info/dependency_links.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      179 2024-05-12 21:50:23.000000 nchuchain-1.0.2/nchuchain.egg-info/requires.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        1 2024-05-12 21:50:23.000000 nchuchain-1.0.2/nchuchain.egg-info/top_level.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       38 2024-05-12 21:50:23.894053 nchuchain-1.0.2/setup.cfg
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1285 2024-05-12 21:50:21.000000 nchuchain-1.0.2/setup.py
```

### Comparing `nchuchain-1.0.1/LICENSE` & `nchuchain-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.1/PKG-INFO` & `nchuchain-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nchuchain
-Version: 1.0.1
+Version: 1.0.2
 Summary: A set of data tools in Python
 Home-page: 
 Download-URL: 
 Author: WenChuan Hsu
 Author-email: wenchuan19991111@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
@@ -18,9 +18,12 @@
 Requires-Dist: faiss-cpu==1.7.4
 Requires-Dist: pyserini==0.22.1
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: transformers>=4.36.0
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: torchvision
+Provides-Extra: dev
+Requires-Dist: pyserini==0.22.1; extra == "dev"
+Requires-Dist: faiss-cpu==1.7.4; extra == "dev"
 
 test
```

### Comparing `nchuchain-1.0.1/nchuchain.egg-info/PKG-INFO` & `nchuchain-1.0.2/nchuchain.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nchuchain
-Version: 1.0.1
+Version: 1.0.2
 Summary: A set of data tools in Python
 Home-page: 
 Download-URL: 
 Author: WenChuan Hsu
 Author-email: wenchuan19991111@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
@@ -18,9 +18,12 @@
 Requires-Dist: faiss-cpu==1.7.4
 Requires-Dist: pyserini==0.22.1
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: transformers>=4.36.0
 Requires-Dist: torch
 Requires-Dist: torchaudio
 Requires-Dist: torchvision
+Provides-Extra: dev
+Requires-Dist: pyserini==0.22.1; extra == "dev"
+Requires-Dist: faiss-cpu==1.7.4; extra == "dev"
 
 test
```

### Comparing `nchuchain-1.0.1/setup.py` & `nchuchain-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 PACKAGE_NAME = "nchuchain"
 AUTHOR = "WenChuan Hsu"
 AUTHOR_EMAIL = "wenchuan19991111@gmail.com"
 URL = ""
 DOWNLOAD_URL = ""
  
 LICENSE = "MIT"
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DESCRIPTION = "A set of data tools in Python"
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
  
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
  
-#dev_requirements = (HERE / "dev_requirements.txt").read_text(encoding="utf8")
-#EXTRAS_REQUIRE = {"dev": [s.strip() for s in dev_requirements.split("\n")]}
+extra_requirements = (HERE / "extra_requirements.txt").read_text(encoding="utf8")
+EXTRAS_REQUIRE = {"dev": [s.strip() for s in extra_requirements.split("\n")]}
  
 CLASSIFIERS = [f"Programming Language :: Python :: 3.{str(v)}" for v in range(8, 11)]
 PYTHON_REQUIRES = ">=3.8"
  
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
@@ -34,11 +34,11 @@
     author=AUTHOR,
     license=LICENSE,
     author_email=AUTHOR_EMAIL,
     url=URL,
     download_url=DOWNLOAD_URL,
     python_requires=PYTHON_REQUIRES,
     install_requires=INSTALL_REQUIRES,
-    #extras_require=EXTRAS_REQUIRE,
+    extras_require=EXTRAS_REQUIRE,
     packages=find_packages(),
     classifiers=CLASSIFIERS,
 )
```

