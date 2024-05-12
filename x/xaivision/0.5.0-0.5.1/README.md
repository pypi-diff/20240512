# Comparing `tmp/xaivision-0.5.0.tar.gz` & `tmp/xaivision-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaivision-0.5.0.tar", max compression
+gzip compressed data, was "xaivision-0.5.1.tar", max compression
```

## Comparing `xaivision-0.5.0.tar` & `xaivision-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1114 2024-04-11 11:21:56.989947 xaivision-0.5.0/README.md
--rw-r--r--   0        0        0      265 2024-04-13 23:53:16.030776 xaivision-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       61 2024-04-13 15:44:32.244089 xaivision-0.5.0/xaivision/__init__.py
--rw-r--r--   0        0        0     2847 2024-04-13 21:30:38.041957 xaivision-0.5.0/xaivision/nmf_func.py
--rw-r--r--   0        0        0    13037 2024-04-13 23:42:42.920222 xaivision-0.5.0/xaivision/utils.py
--rw-r--r--   0        0        0     6904 2024-04-13 23:43:18.076765 xaivision-0.5.0/xaivision/xai_tools.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 xaivision-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-04-11 11:21:56.989947 xaivision-0.5.1/README.md
+-rw-r--r--   0        0        0      265 2024-05-12 21:20:20.976758 xaivision-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-04-13 15:44:32.244089 xaivision-0.5.1/xaivision/__init__.py
+-rw-r--r--   0        0        0     2847 2024-04-13 21:30:38.041957 xaivision-0.5.1/xaivision/nmf_func.py
+-rw-r--r--   0        0        0    13145 2024-04-18 14:10:52.763794 xaivision-0.5.1/xaivision/utils.py
+-rw-r--r--   0        0        0    14105 2024-05-12 21:05:50.728863 xaivision-0.5.1/xaivision/xai_tools.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 xaivision-0.5.1/PKG-INFO
```

### Comparing `xaivision-0.5.0/README.md` & `xaivision-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `xaivision-0.5.0/xaivision/nmf_func.py` & `xaivision-0.5.1/xaivision/nmf_func.py`

 * *Files identical despite different names*

### Comparing `xaivision-0.5.0/xaivision/utils.py` & `xaivision-0.5.1/xaivision/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,22 @@
 
     def forward(self, x):
         # Forward pass through the modified layers
         x = self.features(x)
         return x
 
 
+def full_squeeze(array):
+
+    while 1 in array.shape:
+        array = np.squeeze(array)
+
+    return array
+
+
 def load_models(model):
     """
     Load model and convert it to Python format.
 
     Parameters:
         - model (str): Path to the model or the actual model loaded
```

### Comparing `xaivision-0.5.0/PKG-INFO` & `xaivision-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xaivision
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 Author: philorfa
 Author-email: phil.orfa@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

