# Comparing `tmp/echordpost-0.1.0.tar.gz` & `tmp/echordpost-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echordpost-0.1.0.tar", max compression
+gzip compressed data, was "echordpost-0.1.1.tar", max compression
```

## Comparing `echordpost-0.1.0.tar` & `echordpost-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10223 2024-01-27 11:57:10.555640 echordpost-0.1.0/eCHORDpost/IPF_V1.py
--rw-r--r--   0        0        0     6608 2024-01-04 08:16:59.256806 echordpost-0.1.0/eCHORDpost/Symetry.py
--rw-r--r--   0        0        0     4541 2024-01-05 09:41:12.000000 echordpost-0.1.0/eCHORDpost/Xallo.py
--rw-r--r--   0        0        0    35823 2024-05-12 20:06:13.943321 echordpost-0.1.0/LICENSE
--rw-r--r--   0        0        0      571 2024-05-12 20:27:12.669182 echordpost-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       12 2024-05-12 20:06:13.944270 echordpost-0.1.0/README.md
--rw-r--r--   0        0        0      891 1970-01-01 00:00:00.000000 echordpost-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10223 2024-01-27 11:57:10.555640 echordpost-0.1.1/eCHORDpost/IPF_V1.py
+-rw-r--r--   0        0        0     6608 2024-01-04 08:16:59.256806 echordpost-0.1.1/eCHORDpost/Symetry.py
+-rw-r--r--   0        0        0     4541 2024-01-05 09:41:12.000000 echordpost-0.1.1/eCHORDpost/Xallo.py
+-rw-r--r--   0        0        0    35823 2024-05-12 20:06:13.943321 echordpost-0.1.1/LICENSE
+-rw-r--r--   0        0        0      577 2024-05-12 20:49:04.289054 echordpost-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-05-12 20:06:13.944270 echordpost-0.1.1/README.md
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 echordpost-0.1.1/PKG-INFO
```

### Comparing `echordpost-0.1.0/eCHORDpost/IPF_V1.py` & `echordpost-0.1.1/eCHORDpost/IPF_V1.py`

 * *Files identical despite different names*

### Comparing `echordpost-0.1.0/eCHORDpost/Symetry.py` & `echordpost-0.1.1/eCHORDpost/Symetry.py`

 * *Files identical despite different names*

### Comparing `echordpost-0.1.0/eCHORDpost/Xallo.py` & `echordpost-0.1.1/eCHORDpost/Xallo.py`

 * *Files identical despite different names*

### Comparing `echordpost-0.1.0/LICENSE` & `echordpost-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `echordpost-0.1.0/pyproject.toml` & `echordpost-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "echordpost"
-version = "0.1.0"
+version = "0.1.1"
 description = "Library to run eCHORD post-treatment program"
 authors = ["Langlois Cyril <cyril.langlois@insa-lyon.fr> L'Hôte Gabriel <gabriel.l-hote@insa-lyon.fr>"]
 license = "CECILL"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pyquaternion = "^0.9.9"
 numpy = "^1.26.4"
-orix = "0"
+orix = "^0.11.1"
 PySide6 = "^6.7.0"
 Dans-Diffraction = "^3.0.0"
 pyqtgraph = "^0.13.7"
 h5py = "^3.11.0"
 wxPython = "^4.2.1"
```

### Comparing `echordpost-0.1.0/PKG-INFO` & `echordpost-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: echordpost
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library to run eCHORD post-treatment program
 License: CECILL
 Author: Langlois Cyril
 Author-email: cyril.langlois@insa-lyon.fr> L'Hôte Gabriel <gabriel.l-hote@insa-lyon.fr
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Dans-Diffraction (>=3.0.0,<4.0.0)
 Requires-Dist: PySide6 (>=6.7.0,<7.0.0)
 Requires-Dist: h5py (>=3.11.0,<4.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: orix (==0)
+Requires-Dist: orix (>=0.11.1,<0.12.0)
 Requires-Dist: pyqtgraph (>=0.13.7,<0.14.0)
 Requires-Dist: pyquaternion (>=0.9.9,<0.10.0)
 Requires-Dist: wxPython (>=4.2.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 # eCHORDpost
```

