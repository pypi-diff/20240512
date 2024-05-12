# Comparing `tmp/smart_parallelize-2.0.8.tar.gz` & `tmp/smart_parallelize-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_parallelize-2.0.8.tar", max compression
+gzip compressed data, was "smart_parallelize-2.0.9.tar", max compression
```

## Comparing `smart_parallelize-2.0.8.tar` & `smart_parallelize-2.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.8/README.md
--rw-r--r--   0        0        0      317 2024-05-12 17:21:59.829844 smart_parallelize-2.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.8/smart_parallelize/__init__.py
--rw-r--r--   0        0        0     3438 2024-05-12 17:21:05.959857 smart_parallelize-2.0.8/smart_parallelize/parallelize.py
--rw-r--r--   0        0        0     4098 2024-05-12 17:05:36.304463 smart_parallelize-2.0.8/smart_parallelize/parallelize_DEP.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 smart_parallelize-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0      560 2024-03-22 16:57:28.000000 smart_parallelize-2.0.9/README.md
+-rw-r--r--   0        0        0      317 2024-05-12 17:24:00.112372 smart_parallelize-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 13:20:52.000000 smart_parallelize-2.0.9/smart_parallelize/__init__.py
+-rw-r--r--   0        0        0     3455 2024-05-12 17:23:41.861026 smart_parallelize-2.0.9/smart_parallelize/parallelize.py
+-rw-r--r--   0        0        0     4098 2024-05-12 17:05:36.304463 smart_parallelize-2.0.9/smart_parallelize/parallelize_DEP.py
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 smart_parallelize-2.0.9/PKG-INFO
```

### Comparing `smart_parallelize-2.0.8/README.md` & `smart_parallelize-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.0.8/smart_parallelize/parallelize.py` & `smart_parallelize-2.0.9/smart_parallelize/parallelize.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 
                 for k, _ in enumerate(other_args):
                     inp_args[other_args[k]] = kwargs[other_args[k]]
                 workers.append(get_results.remote(**inp_args))
             
             test_inp = {}
             for j, _ in enumerate(par_args):
-                test_inp[par_args[j]] = split_args[j][0]
+                test_inp[par_args[j]] = arg2parallelize_unsplit[j][0]
             for k, _ in enumerate(other_args):
                 test_inp[other_args[k]] = kwargs[other_args[k]]
             try:
                 num_outputs = len(function(**test_inp))
             except TypeError:
                 num_outputs = 1
 
@@ -89,18 +89,18 @@
     return decorator
 
 
 if __name__ == "__main__":
     import timeit
 
     @smart_parallelize(args2parallelize=1)
-    def func(x):
-        return np.sum(x)
+    def func(x, y):
+        return x + y
     
     x = np.ones((30,2))
-    y = np.ones((30,))*2
-    # y = 2
+    # y = np.ones((30,))*2
+    y = 2
     start  = timeit.default_timer()
-    answer = func(x=x)
+    answer = func(x=x, y=y)
     stop  = timeit.default_timer()
     print(stop - start)
     print(answer)
```

### Comparing `smart_parallelize-2.0.8/smart_parallelize/parallelize_DEP.py` & `smart_parallelize-2.0.9/smart_parallelize/parallelize_DEP.py`

 * *Files identical despite different names*

### Comparing `smart_parallelize-2.0.8/PKG-INFO` & `smart_parallelize-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-parallelize
-Version: 2.0.8
+Version: 2.0.9
 Summary: 
 Author: Truman DeWalch
 Author-email: trumandewalch@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

