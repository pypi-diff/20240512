# Comparing `tmp/LVPocket-0.0.3.tar.gz` & `tmp/LVPocket-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/LVPocket-0.0.3.tar", last modified: Sun May 12 02:31:51 2024, max compression
+gzip compressed data, was "dist/LVPocket-0.1.9.tar", last modified: Sun May 12 08:02:08 2024, max compression
```

## Comparing `LVPocket-0.0.3.tar` & `LVPocket-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:31:51.000000 LVPocket-0.0.3/
--rw-rw-r--   0 root         (0) root         (0)     4087 2024-05-11 09:08:57.000000 LVPocket-0.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 02:31:51.000000 LVPocket-0.0.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1060 2024-05-11 09:08:57.000000 LVPocket-0.0.3/LICENSE
--rw-rw-r--   0 root         (0) root         (0)     2082 2024-05-12 02:30:52.000000 LVPocket-0.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:31:51.000000 LVPocket-0.0.3/lvpocket/
--rw-rw-r--   0 root         (0) root         (0)       17 2024-05-11 11:54:48.000000 LVPocket-0.0.3/lvpocket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:31:51.000000 LVPocket-0.0.3/lvpocket/model/
--rw-rw-r--   0 root         (0) root         (0)    39930 2024-05-11 09:08:57.000000 LVPocket-0.0.3/lvpocket/model/LV_former.py
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-11 09:08:57.000000 LVPocket-0.0.3/lvpocket/model/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    18371 2024-05-11 09:08:57.000000 LVPocket-0.0.3/lvpocket/model/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:31:51.000000 LVPocket-0.0.3/LVPocket.egg-info/
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-12 02:31:14.000000 LVPocket-0.0.3/LVPocket.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      253 2024-05-12 02:31:14.000000 LVPocket-0.0.3/LVPocket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1277 2024-05-12 02:31:14.000000 LVPocket-0.0.3/LVPocket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 02:31:14.000000 LVPocket-0.0.3/LVPocket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1277 2024-05-12 02:31:51.000000 LVPocket-0.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:02:08.000000 LVPocket-0.1.9/
+-rw-rw-r--   0 root         (0) root         (0)     4087 2024-05-11 09:08:57.000000 LVPocket-0.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 08:02:08.000000 LVPocket-0.1.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1060 2024-05-11 09:08:57.000000 LVPocket-0.1.9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)     1836 2024-05-12 08:01:40.000000 LVPocket-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:02:08.000000 LVPocket-0.1.9/lvpocket/
+-rw-rw-r--   0 root         (0) root         (0)       17 2024-05-11 11:54:48.000000 LVPocket-0.1.9/lvpocket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:02:08.000000 LVPocket-0.1.9/lvpocket/model/
+-rw-rw-r--   0 root         (0) root         (0)    39930 2024-05-11 09:08:57.000000 LVPocket-0.1.9/lvpocket/model/LV_former.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-11 09:08:57.000000 LVPocket-0.1.9/lvpocket/model/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    18371 2024-05-11 09:08:57.000000 LVPocket-0.1.9/lvpocket/model/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      284 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1277 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 08:02:08.000000 LVPocket-0.1.9/LVPocket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1277 2024-05-12 08:02:08.000000 LVPocket-0.1.9/PKG-INFO
```

### Comparing `LVPocket-0.0.3/README.md` & `LVPocket-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `LVPocket-0.0.3/LICENSE` & `LVPocket-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LVPocket-0.0.3/setup.py` & `LVPocket-0.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="LVPocket",
-    version="0.0.3",
+    version="0.1.9",
     author="CPU-409",
     author_email="3221051463@stu.cpu.edu.cn",
     keywords="protein binding pockets prediction, lvnet",
     description="A Protein Binding Pocket Prediction Methods.",
-    long_description="We proposed LVPocket, a novel method that synergistically captures both local" \
-                     " and global information of protein data through the integration of Transformer" \
-                     " encoders, which help the model achieve better performance in binding pockets prediction. " \
-                     "And then we tailored prediction models for data of four distinct structural classes of " \
-                     "proteins using the transfer learning. The four fine-tuned models were trained on the baseline" \
-                     " LVPocket model which was trained on the sc-PDB dataset. LVPocket exhibits superior performance" \
-                     " on three independent datasets compared to current state-of-the-art methods. Additionally, the " \
-                     "fine-tuned model outperforms the baseline model in terms of performance.",
+    long_description="We proposed LVPocket, a novel method that synergistically captures both local"
+    " and global information of protein data through the integration of Transformer"
+    " encoders, which help the model achieve better performance in binding pockets prediction. "
+    "And then we tailored prediction models for data of four distinct structural classes of "
+    "proteins using the transfer learning. The four fine-tuned models were trained on the baseline"
+    " LVPocket model which was trained on the sc-PDB dataset. LVPocket exhibits superior performance"
+    " on three independent datasets compared to current state-of-the-art methods. Additionally, the "
+    "fine-tuned model outperforms the baseline model in terms of performance.",
     long_description_content_type="text/markdown",
     url="https://github.com/ZRF-ZRF/LVpocket.git",
     packages=setuptools.find_packages(),
     python_requires=">=3.6, <=3.7",
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 2 - Pre-Alpha",
     ],
-    # install_requires=[
-    #     'h5py>=2.7',
-    #     'openbabel>=2.4',
-    #     'tfbio >=0.3, <=0.3',
-    #     'scikit-image>=0.13',
-    #     'numpy>=1.12',
-    #     'scipy>=1',
-    #     'keras>=2.1,<2.3',
-    #     'tensorflow>=1.8,<=1.11',
-    #     'tensorflow-gpu',
-    #     'protobuf >=3.6.1, <=3.6.1',
-    #     'tqdm',
-    #     'biopython >=1.78, <=1.79',
-    #
-    # ],
-)
+    install_requires=[
+        'h5py',
+        'openbabel>=2.4',
+        'numpy>=1.12',
+        'scipy',
+        'keras>=2.0',
+        'tensorflow-gpu',
+        'protobuf >=3.6.1, <=3.6.1',
+        'biopython',
+        'scikit-learn',
+        'numpy',
+        'pandas',
+    ],
+)
```

### Comparing `LVPocket-0.0.3/lvpocket/model/LV_former.py` & `LVPocket-0.1.9/lvpocket/model/LV_former.py`

 * *Files identical despite different names*

### Comparing `LVPocket-0.0.3/lvpocket/model/data.py` & `LVPocket-0.1.9/lvpocket/model/data.py`

 * *Files identical despite different names*

### Comparing `LVPocket-0.0.3/LVPocket.egg-info/PKG-INFO` & `LVPocket-0.1.9/LVPocket.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LVPocket
-Version: 0.0.3
+Version: 0.1.9
 Summary: A Protein Binding Pocket Prediction Methods.
 Home-page: https://github.com/ZRF-ZRF/LVpocket.git
 Author: CPU-409
 Author-email: 3221051463@stu.cpu.edu.cn
 License: UNKNOWN
 Keywords: protein binding pockets prediction,lvnet
 Platform: UNKNOWN
```

### Comparing `LVPocket-0.0.3/PKG-INFO` & `LVPocket-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LVPocket
-Version: 0.0.3
+Version: 0.1.9
 Summary: A Protein Binding Pocket Prediction Methods.
 Home-page: https://github.com/ZRF-ZRF/LVpocket.git
 Author: CPU-409
 Author-email: 3221051463@stu.cpu.edu.cn
 License: UNKNOWN
 Keywords: protein binding pockets prediction,lvnet
 Platform: UNKNOWN
```

