# Comparing `tmp/soma_integ-0.1.0.tar.gz` & `tmp/soma_integ-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soma_integ-0.1.0.tar", last modified: Thu May  9 11:56:42 2024, max compression
+gzip compressed data, was "soma_integ-0.1.1.tar", last modified: Sun May 12 08:29:52 2024, max compression
```

## Comparing `soma_integ-0.1.0.tar` & `soma_integ-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-09 11:56:42.008566 soma_integ-0.1.0/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.0/LICENSE
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-09 11:56:42.008342 soma_integ-0.1.0/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.0/README.md
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-09 11:55:35.000000 soma_integ-0.1.0/pyproject.toml
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-09 11:56:42.008611 soma_integ-0.1.0/setup.cfg
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-09 11:56:42.004392 soma_integ-0.1.0/src/
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-09 11:56:42.006980 soma_integ-0.1.0/src/soma_integ/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      482 2024-05-09 11:53:16.000000 soma_integ-0.1.0/src/soma_integ/__init__.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1841 2024-03-04 18:10:58.000000 soma_integ-0.1.0/src/soma_integ/config.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2331 2024-05-09 11:53:16.000000 soma_integ-0.1.0/src/soma_integ/data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2038 2024-03-04 18:10:58.000000 soma_integ-0.1.0/src/soma_integ/evaluation.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      272 2024-03-04 18:10:58.000000 soma_integ-0.1.0/src/soma_integ/methods.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      693 2024-05-09 11:28:06.000000 soma_integ-0.1.0/src/soma_integ/model.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     5245 2024-05-09 11:49:16.000000 soma_integ-0.1.0/src/soma_integ/optimization.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.0/src/soma_integ/utils.py
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-09 11:56:42.008019 soma_integ-0.1.0/src/soma_integ.egg-info/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-09 11:56:42.000000 soma_integ-0.1.0/src/soma_integ.egg-info/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      444 2024-05-09 11:56:42.000000 soma_integ-0.1.0/src/soma_integ.egg-info/SOURCES.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-09 11:56:42.000000 soma_integ-0.1.0/src/soma_integ.egg-info/dependency_links.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-09 11:56:42.000000 soma_integ-0.1.0/src/soma_integ.egg-info/requires.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-09 11:56:42.000000 soma_integ-0.1.0/src/soma_integ.egg-info/top_level.txt
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-09 11:56:42.007856 soma_integ-0.1.0/tests/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:14:17.000000 soma_integ-0.1.0/tests/test.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 08:29:52.127779 soma_integ-0.1.1/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.1/LICENSE
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 08:29:52.127546 soma_integ-0.1.1/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.1/README.md
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-12 08:29:34.000000 soma_integ-0.1.1/pyproject.toml
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-12 08:29:52.127829 soma_integ-0.1.1/setup.cfg
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 08:29:52.123239 soma_integ-0.1.1/src/
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 08:29:52.125815 soma_integ-0.1.1/src/soma_integ/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      409 2024-05-12 08:27:59.000000 soma_integ-0.1.1/src/soma_integ/__init__.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 07:11:25.000000 soma_integ-0.1.1/src/soma_integ/config.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3510 2024-05-11 11:51:59.000000 soma_integ-0.1.1/src/soma_integ/data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     9310 2024-05-12 08:21:50.000000 soma_integ-0.1.1/src/soma_integ/evaluation.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-11 13:16:50.000000 soma_integ-0.1.1/src/soma_integ/methods.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 07:52:23.000000 soma_integ-0.1.1/src/soma_integ/model.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 07:05:14.000000 soma_integ-0.1.1/src/soma_integ/optimization.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.1/src/soma_integ/utils.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 08:29:52.127203 soma_integ-0.1.1/src/soma_integ.egg-info/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 08:29:52.000000 soma_integ-0.1.1/src/soma_integ.egg-info/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      455 2024-05-12 08:29:52.000000 soma_integ-0.1.1/src/soma_integ.egg-info/SOURCES.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-12 08:29:52.000000 soma_integ-0.1.1/src/soma_integ.egg-info/dependency_links.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-12 08:29:52.000000 soma_integ-0.1.1/src/soma_integ.egg-info/requires.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-12 08:29:52.000000 soma_integ-0.1.1/src/soma_integ.egg-info/top_level.txt
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 08:29:52.126903 soma_integ-0.1.1/tests/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      576 2024-05-12 08:25:05.000000 soma_integ-0.1.1/tests/test_evaluation.py
```

### Comparing `soma_integ-0.1.0/LICENSE` & `soma_integ-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.0/PKG-INFO` & `soma_integ-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.0/pyproject.toml` & `soma_integ-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "soma_integ"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = ["numpy", "scikit-learn"]
 authors = [
     { name = "Sobhan Ahmadian Moghadam", email = "sobhan.ahmadian.moghadam@gmail.com" },
     { name = "Arman Rezaei", email = "arman.x.rezaei@gmail.com" },
 ]
 description = "A package for integrating implementation and evaluation of machine learning platforms"
 readme = "README.md"
```

### Comparing `soma_integ-0.1.0/src/soma_integ/config.py` & `soma_integ-0.1.1/src/soma_integ/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,78 +2,62 @@
 
 
 class Config(abc.ABC):
     @abc.abstractmethod
     def get_configuration(self):
         pass
 
-    @abc.abstractmethod
-    def get_summary(self):
-        pass
-
 
 class ModelConfig(Config):
     def __init__(self):
         super().__init__()
         self.model_name = None
         self.embedding_dim = None  # dimension of embedding
         self.device = None
 
     def get_configuration(self):
         return {
             "model_name": self.model_name,
             "embed_dim": self.embedding_dim,
-        }
-
-    def get_summary(self):
-        return {
-            "model_name": self.model_name,
-            "embed_dim": self.embedding_dim,
+            "device": self.device,
         }
 
 
 class MethodConfig(Config):
     def __init__(self):
         super().__init__()
         self.method_name = None
 
     def get_configuration(self):
         return {
             "method_name": self.method_name,
         }
 
-    def get_summary(self):
-        return {
-            "method_name": self.method_name,
-        }
-
 
 class OptimizerConfig(Config):
     def __init__(self) -> None:
         super().__init__()
         self.optimizer = None
         self.criterion = None
         self.lr = None  # learning rate
         self.batch_size = None
         self.n_epoch = None
         self.exp_name = None
         self.save = False
         self.save_path = None
-        self.device = 'cpu'
+        self.device = "cpu"
         self.report_size = 100  # batch to report ratio
         self.threshold = 0.5
 
     def get_configuration(self):
         return {
             "optimizer": self.optimizer,
             "lr": self.lr,
             "batch_size": self.batch_size,
             "n_epoch": self.n_epoch,
-        }
-
-    def get_summary(self):
-        return {
-            "optimizer": self.optimizer,
-            "lr": self.lr,
-            "batch_size": self.batch_size,
-            "n_epoch": self.n_epoch,
+            "exp_name": self.exp_name,
+            "save": self.save,
+            "save_path": self.save_path,
+            "device": self.device,
+            "report_size": self.report_size,
+            "threshold": self.threshold,
         }
```

### Comparing `soma_integ-0.1.0/src/soma_integ.egg-info/PKG-INFO` & `soma_integ-0.1.1/src/soma_integ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

