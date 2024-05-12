# Comparing `tmp/mNSF-0.1.1.tar.gz` & `tmp/mNSF-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mNSF-0.1.1.tar", last modified: Wed Apr 24 15:33:20 2024, max compression
+gzip compressed data, was "mNSF-0.1.3.tar", last modified: Sun May 12 17:33:42 2024, max compression
```

## Comparing `mNSF-0.1.1.tar` & `mNSF-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-04-24 15:33:20.128174 mNSF-0.1.1/
--rw-r--r--   0 ywang    (41982) hansen_lab1  (4128)      949 2024-04-24 15:33:20.057173 mNSF-0.1.1/PKG-INFO
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     1332 2024-04-24 15:32:45.000000 mNSF-0.1.1/README.txt
-drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-04-24 15:33:19.502159 mNSF-0.1.1/mNSF/
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)       58 2024-04-24 15:32:47.000000 mNSF-0.1.1/mNSF/__init__.py
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)    21513 2024-04-24 15:32:47.000000 mNSF-0.1.1/mNSF/pf_multiSample.py
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     6762 2024-04-24 15:32:47.000000 mNSF-0.1.1/mNSF/process_multiSample.py
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)    19708 2024-04-24 15:32:47.000000 mNSF-0.1.1/mNSF/training_multiSample.py
-drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-04-24 15:33:19.912169 mNSF-0.1.1/mNSF.egg-info/
--rw-r--r--   0 ywang    (41982) hansen_lab1  (4128)      949 2024-04-24 15:33:18.000000 mNSF-0.1.1/mNSF.egg-info/PKG-INFO
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)      294 2024-04-24 15:33:18.000000 mNSF-0.1.1/mNSF.egg-info/SOURCES.txt
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)        1 2024-04-24 15:33:18.000000 mNSF-0.1.1/mNSF.egg-info/dependency_links.txt
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)      116 2024-04-24 15:33:18.000000 mNSF-0.1.1/mNSF.egg-info/requires.txt
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)        5 2024-04-24 15:33:18.000000 mNSF-0.1.1/mNSF.egg-info/top_level.txt
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     1280 2024-04-24 15:32:48.000000 mNSF-0.1.1/pyproject.toml
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)       38 2024-04-24 15:33:20.145175 mNSF-0.1.1/setup.cfg
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     1361 2024-04-24 15:32:48.000000 mNSF-0.1.1/setup.py
-drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-04-24 15:33:19.981171 mNSF-0.1.1/tests/
--rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     2830 2024-04-24 15:32:48.000000 mNSF-0.1.1/tests/test_small_run.py
+drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-12 17:33:42.517919 mNSF-0.1.3/
+-rw-r--r--   0 ywang    (41982) hansen_lab1  (4128)      949 2024-05-12 17:33:42.474918 mNSF-0.1.3/PKG-INFO
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     1204 2024-04-30 13:10:22.000000 mNSF-0.1.3/README.txt
+drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-12 17:33:41.570895 mNSF-0.1.3/mNSF/
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)       58 2024-04-30 13:10:24.000000 mNSF-0.1.3/mNSF/__init__.py
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)    21513 2024-04-30 13:10:24.000000 mNSF-0.1.3/mNSF/pf_multiSample.py
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     6762 2024-04-30 13:10:25.000000 mNSF-0.1.3/mNSF/process_multiSample.py
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)    19708 2024-04-30 13:10:25.000000 mNSF-0.1.3/mNSF/training_multiSample.py
+drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-12 17:33:42.307914 mNSF-0.1.3/mNSF.egg-info/
+-rw-r--r--   0 ywang    (41982) hansen_lab1  (4128)      949 2024-05-12 17:33:40.000000 mNSF-0.1.3/mNSF.egg-info/PKG-INFO
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)      279 2024-05-12 17:33:40.000000 mNSF-0.1.3/mNSF.egg-info/SOURCES.txt
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)        1 2024-05-12 17:33:40.000000 mNSF-0.1.3/mNSF.egg-info/dependency_links.txt
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)      116 2024-05-12 17:33:40.000000 mNSF-0.1.3/mNSF.egg-info/requires.txt
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)        5 2024-05-12 17:33:40.000000 mNSF-0.1.3/mNSF.egg-info/top_level.txt
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)       38 2024-05-12 17:33:42.529919 mNSF-0.1.3/setup.cfg
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     1227 2024-05-12 17:32:43.000000 mNSF-0.1.3/setup.py
+drwxr-s---   0 ywang    (41982) hansen_lab1  (4128)        0 2024-05-12 17:33:42.382916 mNSF-0.1.3/tests/
+-rw-r-----   0 ywang    (41982) hansen_lab1  (4128)     2830 2024-04-30 13:10:26.000000 mNSF-0.1.3/tests/test_small_run.py
```

### Comparing `mNSF-0.1.1/PKG-INFO` & `mNSF-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mNSF
-Version: 0.1.1
+Version: 0.1.3
 Summary: multi-sample non-negative spatial factorization
 Home-page: https://github.com/hansenlab/mNSF/
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Yi Wang, Kyla Woyshner, Chaichontat Sriworarat, Loyal Goff, Genevieve Stein-O'Brien, Kasper D. Hansen
 Author-email: yiwangthu4@gmail.com
 License: MIT
 Keywords: spatial,factorization,multi-sample
```

### Comparing `mNSF-0.1.1/README.txt` & `mNSF-0.1.3/README.txt`

 * *Files 22% similar despite different names*

```diff
@@ -5,38 +5,29 @@
 You can use pip to install, by firstly install tensorflow with the version written in file environment.yml, then install everything else from the PyPI repository using `pip install -e .` . Using `pip install -e .` without proper version of tensorflow installed could lead to version confliction problem.
 
 Another way would be to use conda to setup most of the packages then use pip to install.
 
 ### Install using pip
 
 1. Git clone and activate your environment of choice.
-2. [Install tensorflow](https://www.tensorflow.org/install).
-3. `pip install -e .`
+2. Install tensorflow (https://www.tensorflow.org/install).
+3. pip install -e .
 
 ### Install using conda/mamba
 
 1. Git clone this repo `git clone https://github.com/hansenlab/mNSF/` and enter `cd mNSF`.
 2. Install `conda`. I recommend this distribution: https://github.com/conda-forge/miniforge. Do not install the full `anaconda`, it's highly bloated.
 3. Create a new environment and install using
 
-```sh
 conda env create -n mnsf -f environment.yml
 conda activate mnsf
-```
+
 The package should be available right away.
 
 3. Install tensorflow.
 
-<details>
-  <summary>CPU only</summary>
-    ```sh
+  CPU only
     conda install tensorflow
-    ```
-</details>
 
-<details>
-  <summary>GPU</summary>
+  GPU
     If you have a GPU and is operating in a Linux system, you can in the `mnsf` environment.
-    ```sh
     conda install tensorflow-gpu
-    ```
-</details>
```

### Comparing `mNSF-0.1.1/mNSF/pf_multiSample.py` & `mNSF-0.1.3/mNSF/pf_multiSample.py`

 * *Files identical despite different names*

### Comparing `mNSF-0.1.1/mNSF/process_multiSample.py` & `mNSF-0.1.3/mNSF/process_multiSample.py`

 * *Files identical despite different names*

### Comparing `mNSF-0.1.1/mNSF/training_multiSample.py` & `mNSF-0.1.3/mNSF/training_multiSample.py`

 * *Files identical despite different names*

### Comparing `mNSF-0.1.1/mNSF.egg-info/PKG-INFO` & `mNSF-0.1.3/mNSF.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mNSF
-Version: 0.1.1
+Version: 0.1.3
 Summary: multi-sample non-negative spatial factorization
 Home-page: https://github.com/hansenlab/mNSF/
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: Yi Wang, Kyla Woyshner, Chaichontat Sriworarat, Loyal Goff, Genevieve Stein-O'Brien, Kasper D. Hansen
 Author-email: yiwangthu4@gmail.com
 License: MIT
 Keywords: spatial,factorization,multi-sample
```

### Comparing `mNSF-0.1.1/setup.py` & `mNSF-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from distutils.core import setup
 setup(
   name = 'mNSF',       
   packages = ['mNSF'],   
-  version = '0.1.1',     
+  version = '0.1.3',     
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = 'multi-sample non-negative spatial factorization',   # Give a short description about your library
+  description = 'multi-sample non-negative spatial factorization',   #
   author = "Yi Wang, Kyla Woyshner, Chaichontat Sriworarat, Loyal Goff, Genevieve Stein-O'Brien, Kasper D. Hansen",                   
   author_email = 'yiwangthu4@gmail.com',      
   url = 'https://github.com/hansenlab/mNSF/',   
-  download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    
   keywords = ['spatial', 'factorization', 'multi-sample'],   
-install_requires=[
+  install_requires=[
           'python==3.10','anndata', 'click', 'matplotlib', 'numpy', 'pandas', 'pip', 
           'scanpy', 'squidpy', 'tensorflow==2.13', 'tensorflow-probability==0.21'],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
 
-    'Intended Audience :: Developers',      # Define that your audience are developers
+    'Intended Audience :: Developers',     
     'Topic :: Software Development :: Build Tools',
 
-    'License :: OSI Approved :: MIT License',   # Again, pick a license
-
+    'License :: OSI Approved :: MIT License',   
     'Programming Language :: Python :: 3.10',      
 
   ],
 )
```

### Comparing `mNSF-0.1.1/tests/test_small_run.py` & `mNSF-0.1.3/tests/test_small_run.py`

 * *Files identical despite different names*

