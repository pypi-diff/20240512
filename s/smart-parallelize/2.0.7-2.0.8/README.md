# Comparing `tmp/smart_parallelize-2.0.7.tar.gz` & `tmp/smart_parallelize-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_parallelize-2.0.7.tar", max compression
+gzip compressed data, was "smart_parallelize-2.0.8.tar", max compression
```

## Comparing `smart_parallelize-2.0.7.tar` & `smart_parallelize-2.0.8.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.7/README.md
--rw-r--r--   0        0        0      317 2024-04-14 20:40:49.394102 smart_parallelize-2.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.7/smart_parallelize/__init__.py
--rw-r--r--   0        0        0     4135 2024-04-14 20:40:24.795287 smart_parallelize-2.0.7/smart_parallelize/parallelize.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 smart_parallelize-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.8/README.md
+-rw-r--r--   0        0        0      317 2024-05-12 17:21:59.829844 smart_parallelize-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.8/smart_parallelize/__init__.py
+-rw-r--r--   0        0        0     3438 2024-05-12 17:21:05.959857 smart_parallelize-2.0.8/smart_parallelize/parallelize.py
+-rw-r--r--   0        0        0     4098 2024-05-12 17:05:36.304463 smart_parallelize-2.0.8/smart_parallelize/parallelize_DEP.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 smart_parallelize-2.0.8/PKG-INFO
```

### Comparing `smart_parallelize-2.0.7/README.md` & `smart_parallelize-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.0.7/smart_parallelize/parallelize.py` & `smart_parallelize-2.0.8/smart_parallelize/parallelize_DEP.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     '''FIRST ARG MUST BE ARG TO BE PARALLELIZED'''
 
     def wrap(**kwargs): 
         def f2(**kwargs):
             par_args = list(kwargs.keys())[:n_args2parallelize]
             data_par_args = [kwargs[i] for i in par_args]
 
-            fnc = np.vectorize(func)
             results = []
             for i, _ in enumerate(data_par_args[0]):
                 kwargs_0 = kwargs.copy()
                 for j, _ in enumerate(data_par_args):
                     kwargs_0[par_args[j]] = data_par_args[j][i]
                 r = func(**kwargs_0)
                 results.append(r)
```

### Comparing `smart_parallelize-2.0.7/PKG-INFO` & `smart_parallelize-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-parallelize
-Version: 2.0.7
+Version: 2.0.8
 Summary: 
 Author: Truman DeWalch
 Author-email: trumandewalch@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

