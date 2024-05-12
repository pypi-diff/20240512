# Comparing `tmp/knockofforigins-0.1.3.tar.gz` & `tmp/knockofforigins-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knockofforigins-0.1.3.tar", max compression
+gzip compressed data, was "knockofforigins-0.1.4.tar", max compression
```

## Comparing `knockofforigins-0.1.3.tar` & `knockofforigins-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/LICENSE
--rw-r--r--   0        0        0     5674 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/__init__.py
--rw-r--r--   0        0        0     3555 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/data_gen.py
--rw-r--r--   0        0        0     2829 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/decompose.py
--rw-r--r--   0        0        0        0 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/evaluation.py
--rw-r--r--   0        0        0     1267 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/gram_matrix.py
--rw-r--r--   0        0        0        0 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/knockoff.py
--rw-r--r--   0        0        0     2659 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/knockoff_construct.py
--rw-r--r--   0        0        0     1499 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/lasso.py
--rw-r--r--   0        0        0        0 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/plots.py
--rw-r--r--   0        0        0        0 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/testatistics.py
--rw-r--r--   0        0        0        0 2024-04-26 23:59:27.295839 knockofforigins-0.1.3/knockofforigins/utils.py
--rw-r--r--   0        0        0      966 2024-04-26 23:59:27.299839 knockofforigins-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6911 1970-01-01 00:00:00.000000 knockofforigins-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5747 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/__init__.py
+-rw-r--r--   0        0        0     3682 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/data_gen.py
+-rw-r--r--   0        0        0     2829 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/decompose.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/evaluation.py
+-rw-r--r--   0        0        0      824 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/gram_matrix.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/knockoff.py
+-rw-r--r--   0        0        0     2104 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/knockoff_construct.py
+-rw-r--r--   0        0        0     1499 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/lasso.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/plots.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/testatistics.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:06:16.168983 knockofforigins-0.1.4/knockofforigins/utils.py
+-rw-r--r--   0        0        0     1079 2024-05-12 16:06:16.172983 knockofforigins-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6984 1970-01-01 00:00:00.000000 knockofforigins-0.1.4/PKG-INFO
```

### Comparing `knockofforigins-0.1.3/LICENSE` & `knockofforigins-0.1.4/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 [Javad Razi]
+Copyright (c) 2024 [Javad Razi, Mohammad Jamal Asadi]
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `knockofforigins-0.1.3/README.md` & `knockofforigins-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## TODO
 
+- [ ] Fix problems with computing S vector and generating Knockoff data.
 - [ ] Implement test statistics for feature evaluation.
 - [ ] Develop FDR control mechanisms as outlined in the original study.
 - [ ] Implement Lasso feature selection using lower-level libraries.
 - [ ] Address some of the bugs and implementation issues.
 - [ ] Create example notebooks demonstrating package usage.
 - [ ] Replicate experiments from the original 2015 knockoff paper.
 - [ ] Develop visualization methods for feature selection analysis.
```

### Comparing `knockofforigins-0.1.3/knockofforigins/data_gen.py` & `knockofforigins-0.1.4/knockofforigins/data_gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,34 +34,40 @@
     def __init__(self, base_generator: SyntheticDataGenerator):
         """
         Initialize the GWAS data generator.
 
         Parameters:
         - base_generator (SyntheticDataGenerator): The base data generator used for data generation.
         """
-        self.base_generator = base_generator
+
+        self._base_generator = base_generator
+
+    @property
+    def p(self):
+        return self._base_generator.p
+
+    @property
+    def n(self):
+        return self._base_generator.n
 
     def generate_data(self):
         """
         Generate synthetic GWAS data.
 
         Returns:
         - X (ndarray): GWAS feature matrix (integers 0, 1, 2).
         - y (ndarray): Binary response vector.
         """
-        X, y_continuous = self.base_generator.generate_data()
+        X, y_continuous = self._base_generator.generate_data()
         X_gwas = np.clip(np.round(X * 2), 0, 2).astype(int)
         y_binary = (y_continuous > np.median(y_continuous)).astype(int)
         return X_gwas, y_binary
 
 
-import numpy as np
-
-
-class InfluentialFeatureGWASDataGenerator(GWASDataGenerator):
+class InfluentialFeatureGWASDataGenerator(SyntheticDataGenerator):
     def __init__(
         self, base_generator: SyntheticDataGenerator, num_influential: int = 10
     ):
         """
         Extend GWASDataGenerator to generate data with a limited number of influential features.
 
         Parameters:
```

### Comparing `knockofforigins-0.1.3/knockofforigins/decompose.py` & `knockofforigins-0.1.4/knockofforigins/decompose.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.3/knockofforigins/gram_matrix.py` & `knockofforigins-0.1.4/knockofforigins/gram_matrix.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,29 +13,14 @@
 
     Returns:
         A 2D numpy array (n x n) representing the Gram matrix of X.
     """
     return X.T @ X
 
 
-def generate_gram_matrix(X: np.ndarray) -> np.ndarray:
-    """
-    Generate the Gram matrix from the original feature matrix after normalizing features.
-
-    Args:
-        X: A 2D numpy array (n x p) representing the original feature matrix.
-
-    Returns:
-        A 2D numpy array (n x n) representing the Gram matrix of the normalized features.
-    """
-
-    normalized_X = normalize_features(X)
-    return compute_gram_matrix(normalized_X)
-
-
 def normalize_features(X: ndarray) -> ndarray:
     """
     Normalize the columns of the feature matrix so that each feature's L2 norm is 1.
 
     Args:
         X: A 2D numpy array (n x p) representing the feature matrix.
```

### Comparing `knockofforigins-0.1.3/knockofforigins/knockoff_construct.py` & `knockofforigins-0.1.4/knockofforigins/knockoff_construct.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,43 @@
 import numpy as np
 from numpy import ndarray
-from knockofforigins.decompose import CholeskyDecomposition, Decompose
+from scipy.linalg import qr
+from knockofforigins.decompose import CholeskyDecomposition
 from knockofforigins.gram_matrix import (
     compute_gram_matrix,
-    generate_gram_matrix,
     normalize_features,
 )
-from scipy.linalg import qr
 
 
-def choose_s_vector(Sigma: ndarray, tau: float = None) -> ndarray:
+def choose_s_vector(Sigma: ndarray, tau: float = np.inf) -> ndarray:
     """
     Choose the vector s based on the constraints that diag{s} <= 2 * Sigma.
 
     Parameters:
         Sigma: Covariance matrix of the original features (p, p).
         tau: Optional upper limit for the values of s to ensure positive semidefinite matrix.
 
     Returns:
         A vector s that satisfies the constraints for knockoff feature generation.
     """
-    # Compute the diagonal matrix diag(s)
-    s = np.zeros(Sigma.shape[0])  # Initialize s as zeros
+    s = np.zeros(Sigma.shape[0])
 
     # Ensure diag(s) <= 2 * Sigma
-    EPSILON = 1e-6
+    EPSILON = 1e-3
     for j in range(Sigma.shape[0]):
         s_j = (
             min(2 * Sigma[j, j] - EPSILON, tau)
             if tau is not None
             else 2 * Sigma[j, j] - EPSILON
         )
         s[j] = s_j
 
     return s
 
 
-def generate_random_matrix(shape, random_state=None):
-    """
-    Generate a random matrix with the specified shape.
-
-    Args:
-        shape: Tuple representing the desired shape of the random matrix.
-        random_state: Optional seed for the random number generator.
-
-    Returns:
-        A random matrix of the specified shape.
-    """
-    if random_state is not None:
-        np.random.seed(random_state)
-    return np.random.normal(size=shape)
-
-
 def generate_knockoff_features(
     X: np.ndarray, s: np.ndarray, random_state=42, normalize=True
 ) -> np.ndarray:
     """
     Construct knockoff features based on the original feature matrix X.
 
     Args:
```

### Comparing `knockofforigins-0.1.3/knockofforigins/lasso.py` & `knockofforigins-0.1.4/knockofforigins/lasso.py`

 * *Files identical despite different names*

### Comparing `knockofforigins-0.1.3/pyproject.toml` & `knockofforigins-0.1.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "KnockoffOrigins"
-version = "v0.1.3"
+version = "v0.1.4"
 description = "This repository is dedicated to implementing the methodologies from the 2015 paper \"False Discovery Rate via Knockoffs\". It provides code for generating knockoff features and applying selection procedures. The aim is to help users understand and apply the knockoff method for feature selection. Please refer to the original paper for a complete understanding."
-authors = ["Javad Razi <j.razi@outlook.com>"]
+authors = ["Javad Razi <j.razi@outlook.com>", "Mohammad Jamal Asadi <asadimohammad331@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jrazi/KnockoffOrigins"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 scipy = "^1.13.0"
@@ -19,13 +19,16 @@
 [tool.poetry.dev-dependencies]
 pytest = "^8.1.1"
 pep8 = "^1.7.1"
 black = "^24.4.2"
 isort = "^5.13.2"
 pylint = "^3.1.0"
 
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.29.4"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `knockofforigins-0.1.3/PKG-INFO` & `knockofforigins-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KnockoffOrigins
-Version: 0.1.3
+Version: 0.1.4
 Summary: This repository is dedicated to implementing the methodologies from the 2015 paper "False Discovery Rate via Knockoffs". It provides code for generating knockoff features and applying selection procedures. The aim is to help users understand and apply the knockoff method for feature selection. Please refer to the original paper for a complete understanding.
 Home-page: https://github.com/jrazi/KnockoffOrigins
 License: MIT
 Author: Javad Razi
 Author-email: j.razi@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -157,14 +157,15 @@
 
 ## License
 
 This project is licensed under the MIT License.
 
 ## TODO
 
+- [ ] Fix problems with computing S vector and generating Knockoff data.
 - [ ] Implement test statistics for feature evaluation.
 - [ ] Develop FDR control mechanisms as outlined in the original study.
 - [ ] Implement Lasso feature selection using lower-level libraries.
 - [ ] Address some of the bugs and implementation issues.
 - [ ] Create example notebooks demonstrating package usage.
 - [ ] Replicate experiments from the original 2015 knockoff paper.
 - [ ] Develop visualization methods for feature selection analysis.
```

