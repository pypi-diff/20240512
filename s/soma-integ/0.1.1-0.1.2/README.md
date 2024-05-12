# Comparing `tmp/soma_integ-0.1.1.tar.gz` & `tmp/soma_integ-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soma_integ-0.1.1.tar", last modified: Sun May 12 08:29:52 2024, max compression
+gzip compressed data, was "soma_integ-0.1.2.tar", last modified: Sun May 12 18:54:28 2024, max compression
```

## Comparing `soma_integ-0.1.1.tar` & `soma_integ-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 08:29:52.127779 soma_integ-0.1.1/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.1/LICENSE
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 08:29:52.127546 soma_integ-0.1.1/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.1/README.md
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-12 08:29:34.000000 soma_integ-0.1.1/pyproject.toml
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-12 08:29:52.127829 soma_integ-0.1.1/setup.cfg
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 08:29:52.123239 soma_integ-0.1.1/src/
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 08:29:52.125815 soma_integ-0.1.1/src/soma_integ/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      409 2024-05-12 08:27:59.000000 soma_integ-0.1.1/src/soma_integ/__init__.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 07:11:25.000000 soma_integ-0.1.1/src/soma_integ/config.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3510 2024-05-11 11:51:59.000000 soma_integ-0.1.1/src/soma_integ/data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     9310 2024-05-12 08:21:50.000000 soma_integ-0.1.1/src/soma_integ/evaluation.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-11 13:16:50.000000 soma_integ-0.1.1/src/soma_integ/methods.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 07:52:23.000000 soma_integ-0.1.1/src/soma_integ/model.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 07:05:14.000000 soma_integ-0.1.1/src/soma_integ/optimization.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.1/src/soma_integ/utils.py
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 08:29:52.127203 soma_integ-0.1.1/src/soma_integ.egg-info/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 08:29:52.000000 soma_integ-0.1.1/src/soma_integ.egg-info/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      455 2024-05-12 08:29:52.000000 soma_integ-0.1.1/src/soma_integ.egg-info/SOURCES.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-12 08:29:52.000000 soma_integ-0.1.1/src/soma_integ.egg-info/dependency_links.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-12 08:29:52.000000 soma_integ-0.1.1/src/soma_integ.egg-info/requires.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-12 08:29:52.000000 soma_integ-0.1.1/src/soma_integ.egg-info/top_level.txt
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 08:29:52.126903 soma_integ-0.1.1/tests/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      576 2024-05-12 08:25:05.000000 soma_integ-0.1.1/tests/test_evaluation.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 18:54:28.155751 soma_integ-0.1.2/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.2/LICENSE
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 18:54:28.155536 soma_integ-0.1.2/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.2/README.md
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-12 18:52:11.000000 soma_integ-0.1.2/pyproject.toml
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-12 18:54:28.155801 soma_integ-0.1.2/setup.cfg
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 18:54:28.150476 soma_integ-0.1.2/src/
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 18:54:28.153385 soma_integ-0.1.2/src/soma_integ/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      409 2024-05-12 08:37:42.000000 soma_integ-0.1.2/src/soma_integ/__init__.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 08:37:42.000000 soma_integ-0.1.2/src/soma_integ/config.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3522 2024-05-12 18:36:38.000000 soma_integ-0.1.2/src/soma_integ/data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     9221 2024-05-12 18:29:39.000000 soma_integ-0.1.2/src/soma_integ/evaluation.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-12 08:37:42.000000 soma_integ-0.1.2/src/soma_integ/methods.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 08:37:42.000000 soma_integ-0.1.2/src/soma_integ/model.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 08:37:42.000000 soma_integ-0.1.2/src/soma_integ/optimization.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.2/src/soma_integ/utils.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 18:54:28.155233 soma_integ-0.1.2/src/soma_integ.egg-info/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 18:54:28.000000 soma_integ-0.1.2/src/soma_integ.egg-info/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      474 2024-05-12 18:54:28.000000 soma_integ-0.1.2/src/soma_integ.egg-info/SOURCES.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-12 18:54:28.000000 soma_integ-0.1.2/src/soma_integ.egg-info/dependency_links.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-12 18:54:28.000000 soma_integ-0.1.2/src/soma_integ.egg-info/requires.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-12 18:54:28.000000 soma_integ-0.1.2/src/soma_integ.egg-info/top_level.txt
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 18:54:28.154901 soma_integ-0.1.2/tests/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      550 2024-05-12 18:49:52.000000 soma_integ-0.1.2/tests/test_data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      576 2024-05-12 08:37:42.000000 soma_integ-0.1.2/tests/test_evaluation.py
```

### Comparing `soma_integ-0.1.1/LICENSE` & `soma_integ-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.1/PKG-INFO` & `soma_integ-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.1/pyproject.toml` & `soma_integ-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "soma_integ"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = ["numpy", "scikit-learn"]
 authors = [
     { name = "Sobhan Ahmadian Moghadam", email = "sobhan.ahmadian.moghadam@gmail.com" },
     { name = "Arman Rezaei", email = "arman.x.rezaei@gmail.com" },
 ]
 description = "A package for integrating implementation and evaluation of machine learning platforms"
 readme = "README.md"
```

### Comparing `soma_integ-0.1.1/src/soma_integ/config.py` & `soma_integ-0.1.2/src/soma_integ/config.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.1/src/soma_integ/data.py` & `soma_integ-0.1.2/src/soma_integ/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 
         Returns:
             dict: A dictionary containing subsets of data, where the keys represent the subset index and the values
                     represent the indices of the elements in the subset.
         """
         subsets = dict()
         subset_size = int(len(self.data) / self.k)
-        remain = set(range(0, len(self.data)))
+        remain = list(range(0, len(self.data)))
         for i in range(self.k - 1):
             subsets[i] = random.sample(remain, subset_size)
-            remain = remain.difference(subsets[i])
+            remain = list(set(remain).difference(subsets[i]))
         subsets[self.k - 1] = remain
         return subsets
 
 
 class PytorchData(Data):
     """
     A class representing PyTorch data.
```

### Comparing `soma_integ-0.1.1/src/soma_integ/evaluation.py` & `soma_integ-0.1.2/src/soma_integ/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,14 @@
             "F1 Score": self.f1,
             "AUPR": self.aupr,
             "Loss": self.loss,
             "Recall": self.recall,
             "Precision": self.precision,
             "MCC": self.mcc,
             "Max F1": self.max_f1,
-            "True Positive Rate": self.tpr,
-            "False Positive Rate": self.fpr,
         }
 
 
 class CrossValidationResult:
     """
     Represents the result of cross-validation for evaluating a model's performance.
```

### Comparing `soma_integ-0.1.1/src/soma_integ/methods.py` & `soma_integ-0.1.2/src/soma_integ/methods.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.1/src/soma_integ/model.py` & `soma_integ-0.1.2/src/soma_integ/model.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.1/src/soma_integ/optimization.py` & `soma_integ-0.1.2/src/soma_integ/optimization.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.1/src/soma_integ.egg-info/PKG-INFO` & `soma_integ-0.1.2/src/soma_integ.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.1/tests/test_evaluation.py` & `soma_integ-0.1.2/tests/test_evaluation.py`

 * *Files identical despite different names*

