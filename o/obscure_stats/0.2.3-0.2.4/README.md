# Comparing `tmp/obscure_stats-0.2.3.tar.gz` & `tmp/obscure_stats-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obscure_stats-0.2.3.tar", max compression
+gzip compressed data, was "obscure_stats-0.2.4.tar", max compression
```

## Comparing `obscure_stats-0.2.3.tar` & `obscure_stats-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1070 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0     1284 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/LICENSES_bundled.txt
--rw-r--r--   0        0        0     5568 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/README.md
--rw-r--r--   0        0        0     1988 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       56 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/__init__.py
--rw-r--r--   0        0        0      625 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/association/__init__.py
--rw-r--r--   0        0        0    15006 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/association/association.py
--rw-r--r--   0        0        0      455 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/central_tendency/__init__.py
--rw-r--r--   0        0        0     7026 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/central_tendency/central_tendency.py
--rw-r--r--   0        0        0      885 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/dispersion/__init__.py
--rw-r--r--   0        0        0    10102 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/dispersion/dispersion.py
--rw-r--r--   0        0        0      293 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/kurtosis/__init__.py
--rw-r--r--   0        0        0     4945 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/kurtosis/kurtosis.py
--rw-r--r--   0        0        0      627 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/skewness/__init__.py
--rw-r--r--   0        0        0    10304 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/skewness/skewness.py
--rw-r--r--   0        0        0      355 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/variation/__init__.py
--rw-r--r--   0        0        0     7599 2024-03-16 10:52:14.350094 obscure_stats-0.2.3/src/obscure_stats/variation/variation.py
--rw-r--r--   0        0        0     6565 1970-01-01 00:00:00.000000 obscure_stats-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/LICENSE.txt
+-rw-r--r--   0        0        0     1285 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/LICENSES_bundled.txt
+-rw-r--r--   0        0        0     5568 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/README.md
+-rw-r--r--   0        0        0     1988 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/association/__init__.py
+-rw-r--r--   0        0        0    15121 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/association/association.py
+-rw-r--r--   0        0        0      455 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/central_tendency/__init__.py
+-rw-r--r--   0        0        0     7026 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/central_tendency/central_tendency.py
+-rw-r--r--   0        0        0      885 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/dispersion/__init__.py
+-rw-r--r--   0        0        0    10102 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/dispersion/dispersion.py
+-rw-r--r--   0        0        0      293 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/kurtosis/__init__.py
+-rw-r--r--   0        0        0     4945 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/kurtosis/kurtosis.py
+-rw-r--r--   0        0        0      627 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/skewness/__init__.py
+-rw-r--r--   0        0        0    10304 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/skewness/skewness.py
+-rw-r--r--   0        0        0      355 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/variation/__init__.py
+-rw-r--r--   0        0        0     7693 2024-05-12 14:53:09.367253 obscure_stats-0.2.4/src/obscure_stats/variation/variation.py
+-rw-r--r--   0        0        0     6565 1970-01-01 00:00:00.000000 obscure_stats-0.2.4/PKG-INFO
```

### Comparing `obscure_stats-0.2.3/LICENSE.txt` & `obscure_stats-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `obscure_stats-0.2.3/LICENSES_bundled.txt` & `obscure_stats-0.2.4/LICENSES_bundled.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   license: BSD 3-Clause "New" or "Revised" License
   repository: https://github.com/numpy/numpy
   homepage: https://numpy.org/
   dependency: production
 
 SciPy
   name: scipy
-  version: 1.12.0
+  version: 1.13.0
   license: BSD 3-Clause "New" or "Revised" License
   repository: https://github.com/scipy/scipy
   homepage: https://scipy.org/
   dependency: production
 
 Poetry
   name: poetry
@@ -20,36 +20,36 @@
   license: The MIT License
   repository: https://github.com/python-poetry/poetry
   homepage: https://python-poetry.org/
   dependency: dev
 
 MyPy
   name: mypy
-  version: 1.9.0
+  version: 1.10.0
   license: The MIT License
   repository: https://github.com/python/mypy
   homepage: https://www.mypy-lang.org/
   dependency: dev
 
 Ruff
   name: ruff
-  version: 0.2.2
+  version: 0.4.3
   license: The MIT license 
   repository: https://github.com/astral-sh/ruff
   homepage: https://docs.astral.sh/ruff/
   dependency: dev
 
 Pytest
   name: pytest
-  version: 7.4.4
+  version: 8.2.0
   license: The MIT License
   repository: https://github.com/pytest-dev/pytest
   homepage: https://docs.pytest.org/en/latest/
   dependency: dev
 
 Pytest-cov
   name: pytest-cov
-  version: 4.1.0
+  version: 5.0.0
   license: The MIT License
   repository: https://github.com/pytest-dev/pytest-cov
   homepage: https://pytest-cov.readthedocs.io/en/latest/
   dependency: dev
```

### Comparing `obscure_stats-0.2.3/README.md` & `obscure_stats-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `obscure_stats-0.2.3/pyproject.toml` & `obscure_stats-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "obscure_stats"
-version = "0.2.3"
+version = "0.2.4"
 description = "Collection of lesser-known statistical functions"
 authors = ["Hleb Levitski"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
@@ -25,17 +25,17 @@
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 numpy = "^1.23.5"
 scipy = "^1.9.1"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.6.1"
-pytest = "^7.4.3"
-pytest-cov = "^4.1.0"
-ruff = "^0.2.1"
+pytest = "^8.0.0"
+pytest-cov = "^5.0.0"
+ruff = "^0.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = [
```

### Comparing `obscure_stats-0.2.3/src/obscure_stats/association/__init__.py` & `obscure_stats-0.2.4/src/obscure_stats/association/__init__.py`

 * *Files identical despite different names*

### Comparing `obscure_stats-0.2.3/src/obscure_stats/association/association.py` & `obscure_stats-0.2.4/src/obscure_stats/association/association.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,19 +187,20 @@
         return np.nan
     x, y = _prep_arrays(x, y)
     n = len(x)
     mean_x = np.sum(x) / n
     mean_y = np.sum(y) / n
     sem_x = np.std(x, ddof=0) / n**0.5
     sem_y = np.std(y, ddof=0) / n**0.5
-    n_q1 = np.sum((x > mean_x + sem_x) & (y > mean_y + sem_y))
-    n_q2 = np.sum((x < mean_x - sem_x) & (y > mean_y + sem_y))
-    n_q3 = np.sum((x < mean_x - sem_x) & (y < mean_y - sem_y))
-    n_q4 = np.sum((x > mean_x + sem_x) & (y < mean_y - sem_y))
-    return (n_q1 + n_q3 - n_q2 - n_q4) / n
+    return (
+        np.sum((x > mean_x + sem_x) & (y > mean_y + sem_y))
+        + np.sum((x < mean_x - sem_x) & (y > mean_y + sem_y))
+        - np.sum((x < mean_x - sem_x) & (y < mean_y - sem_y))
+        - np.sum((x > mean_x + sem_x) & (y < mean_y - sem_y))
+    ) / n
 
 
 def symmetric_chatterjeexi(x: np.ndarray, y: np.ndarray) -> float:
     """Calculate symmetric Xi correlation coefficient.
 
     Another variation of rank correlation which does not make any assumptions about
     underlying distributions of the variable.
@@ -453,19 +454,20 @@
     Concordance rate.
     Concordance correlation coefficient.
     """
     if _check_arrays(x, y):
         return np.nan
     x, y = _prep_arrays(x, y)
     n_sq = len(x) ** 2
-    rank_x_inc = (np.argsort(x) + 1) ** 2 / n_sq - 0.5
-    rank_y_inc = (np.argsort(y) + 1) ** 2 / n_sq - 0.5
-    rank_y_dec = 0.5 - (np.argsort(-y) + 1) ** 2 / n_sq
-    lower = np.sum((-rank_x_inc < rank_y_inc) * (rank_x_inc + rank_y_inc) ** 2)
-    higher = np.sum((rank_x_inc > rank_y_dec) * (rank_x_inc - rank_y_dec) ** 2)
+    ranks = np.argsort(np.vstack([x, y, -y]).T, axis=0)
+    rank_x_inc = (ranks[0, :] + 1) ** 2 / n_sq - 0.5
+    rank_y_inc = (ranks[1, :] + 1) ** 2 / n_sq - 0.5
+    rank_y_dec = -((ranks[2, :] + 1) ** 2) / n_sq + 0.5
+    lower = np.sum(np.less(-rank_x_inc, rank_y_inc) * (rank_x_inc + rank_y_inc) ** 2)
+    higher = np.sum(np.greater(rank_x_inc, rank_y_dec) * (rank_x_inc - rank_y_dec) ** 2)
     return (lower - higher) / (lower + higher)
 
 
 def tukey_correlation(x: np.ndarray, y: np.ndarray) -> float:
     """Calculate Tukey's correlation coefficient.
 
     It is not quite as robust as rank correlations, but it is more
@@ -530,12 +532,14 @@
     The Gaussian rank correlation estimator: robustness properties.
     Statistics and Computing, 22, 471-483.
     """
     if _check_arrays(x, y):
         return np.nan
     x, y = _prep_arrays(x, y)
     n = len(x)
-    x_ranks_norm = (np.argsort(x) + 1) / (n + 1)
-    y_ranks_norm = (np.argsort(y) + 1) / (n + 1)
+    norm_factor = 1 / (n + 1)
+    ranks = np.argsort(np.vstack([x, y]).T, axis=0)
+    x_ranks_norm = ranks[0, :] * norm_factor
+    y_ranks_norm = ranks[1, :] * norm_factor
     return np.sum(stats.norm.ppf(x_ranks_norm) * stats.norm.ppf(y_ranks_norm)) / np.sum(
         stats.norm.ppf(np.arange(1, n + 1) / (n + 1)) ** 2
     )
```

### Comparing `obscure_stats-0.2.3/src/obscure_stats/central_tendency/central_tendency.py` & `obscure_stats-0.2.4/src/obscure_stats/central_tendency/central_tendency.py`

 * *Files identical despite different names*

### Comparing `obscure_stats-0.2.3/src/obscure_stats/dispersion/__init__.py` & `obscure_stats-0.2.4/src/obscure_stats/dispersion/__init__.py`

 * *Files identical despite different names*

### Comparing `obscure_stats-0.2.3/src/obscure_stats/dispersion/dispersion.py` & `obscure_stats-0.2.4/src/obscure_stats/dispersion/dispersion.py`

 * *Files identical despite different names*

### Comparing `obscure_stats-0.2.3/src/obscure_stats/kurtosis/kurtosis.py` & `obscure_stats-0.2.4/src/obscure_stats/kurtosis/kurtosis.py`

 * *Files identical despite different names*

### Comparing `obscure_stats-0.2.3/src/obscure_stats/skewness/__init__.py` & `obscure_stats-0.2.4/src/obscure_stats/skewness/__init__.py`

 * *Files identical despite different names*

### Comparing `obscure_stats-0.2.3/src/obscure_stats/skewness/skewness.py` & `obscure_stats-0.2.4/src/obscure_stats/skewness/skewness.py`

 * *Files identical despite different names*

### Comparing `obscure_stats-0.2.3/src/obscure_stats/variation/variation.py` & `obscure_stats-0.2.4/src/obscure_stats/variation/variation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Module for measures of categorical variations."""
 
 import math
-from collections import Counter
 
 import numpy as np
 from scipy import stats  # type: ignore[import-untyped]
 
 
 def mod_vr(x: np.ndarray) -> float:
     """Calculate Mode Variation Ratio.
@@ -28,15 +27,15 @@
 
     References
     ----------
     Wilcox, A. R. (1973).
     Indices of Qualitative Variation and Political Measurement.
     The Western Political Quarterly. 26 (2): 325-343.
     """
-    cnts = np.asarray(list(Counter(x).values()))
+    cnts = np.unique(x, return_counts=True, equal_nan=True)[1]
     return 1 - np.max(cnts) / len(x)
 
 
 def range_vr(x: np.ndarray) -> float:
     """Calculate Range Variation Ratio.
 
     Ratio of frequencies of the least and the most common categories.
@@ -57,15 +56,15 @@
 
     References
     ----------
     Wilcox, A. R. (1973).
     Indices of Qualitative Variation and Political Measurement.
     The Western Political Quarterly. 26 (2): 325-343.
     """
-    cnts = np.asarray(list(Counter(x).values()))
+    cnts = np.unique(x, return_counts=True, equal_nan=True)[1]
     return np.min(cnts) / np.max(cnts)
 
 
 def gibbs_m1(x: np.ndarray) -> float:
     """Calculate Gibbs M1 Index.
 
     M1 can be interpreted as one minus the likelihood that a random pair
@@ -99,15 +98,15 @@
     Bachi's index of linguistic homogeneity;
     Mueller and Schuessler's index of qualitative variation;
     Gibbs and Martin's index of industry diversification;
     Lieberson's index;
     Blau's index in sociology, psychology and management studies;
     Special case of Tsallis entropy (alpha = 2).
     """
-    freq = np.asarray(list(Counter(x).values())) / len(x)
+    freq = np.unique(x, return_counts=True, equal_nan=True)[1] / len(x)
     return 1 - np.sum(freq**2)
 
 
 def gibbs_m2(x: np.ndarray) -> float:
     """Calculate Gibbs M2 Index.
 
     M2 can be interpreted as the ratio of the variance of
@@ -128,15 +127,15 @@
 
     References
     ----------
     Gibbs, J. P.; Poston Jr, D. L. (1975).
     The Division of Labor: Conceptualization and Related Measures.
     Social Forces, 53 (3): 468-476.
     """
-    freq = np.asarray(list(Counter(x).values())) / len(x)
+    freq = np.unique(x, return_counts=True, equal_nan=True)[1] / len(x)
     k = len(freq)
     return (k / (k - 1)) * (1 - np.sum(freq**2))
 
 
 def b_index(x: np.ndarray) -> float:
     """Calculate B Index.
 
@@ -158,15 +157,15 @@
     References
     ----------
     Wilcox, A. R. (1973).
     Indices of Qualitative Variation and Political Measurement.
     The Western Political Quarterly. 26 (2): 325-343.
     """
     n = len(x)
-    freq = np.asarray(list(Counter(x).values())) / n
+    freq = np.unique(x, return_counts=True, equal_nan=True)[1] / n
     return 1 - (1 - (stats.gmean(freq * len(freq) / n)) ** 2) ** 0.5
 
 
 def avdev(x: np.ndarray) -> float:
     """Calculate Average Deviation Analogue.
 
     Normalized to 0-1 range categorical analogue of the mean deviation.
@@ -187,15 +186,15 @@
     References
     ----------
     Wilcox, A. R. (1973).
     Indices of Qualitative Variation and Political Measurement.
     The Western Political Quarterly. 26 (2): 325-343.
     """
     n = len(x)
-    freq = np.asarray(list(Counter(x).values())) / n
+    freq = np.unique(x, return_counts=True, equal_nan=True)[1] / n
     k = len(freq)
     mean = n / k
     return 1 - (np.sum(np.abs(freq - mean)) / (2 * mean * max(k - 1, 1)))
 
 
 def renyi_entropy(x: np.ndarray, alpha: float = 2) -> float:
     """Calculate Renyi entropy (bits).
@@ -224,15 +223,15 @@
     On measures of information and entropy.
     Proceedings of the fourth Berkeley Symposium on Mathematics,
     Statistics and Probability 1960. pp. 547-561.
     """
     if alpha < 0:
         msg = "Parameter alpha should be positive!"
         raise ValueError(msg)
-    freq = np.asarray(list(Counter(x).values())) / len(x)
+    freq = np.unique(x, return_counts=True, equal_nan=True)[1] / len(x)
     if alpha == 1:
         # return Shannon entropy to avoid division by 0
         return -np.sum(freq * np.log2(freq))
     return 1 / (1 - alpha) * math.log2(np.sum(freq**alpha))
 
 
 def negative_extropy(x: np.ndarray) -> float:
@@ -257,15 +256,15 @@
 
     References
     ----------
     Lad, F.; Sanfilippo, G.; Agro, G. (2015).
     Extropy: Complementary dual of entropy.
     Statistical Science, 30(1), 40-58.
     """
-    freq = np.asarray(list(Counter(x).values())) / len(x)
+    freq = np.unique(x, return_counts=True, equal_nan=True)[1] / len(x)
     p_inv = 1.0 - freq
     return -np.sum(p_inv * np.log2(p_inv))
 
 
 def mcintosh_d(x: np.ndarray) -> float:
     """Calculate McIntosh's D.
 
@@ -285,9 +284,9 @@
     References
     ----------
     McIntosh, R. P. (1967).
     An index of diversity and the relation of certain concepts to diversity.
     Ecology, 48(3), 392-404.
     """
     n = len(x)
-    counts = np.asarray(list(Counter(x).values()))
+    counts = np.unique(x, return_counts=True, equal_nan=True)[1]
     return (n - np.sum(counts**2) ** 0.5) / (n - n**0.5)
```

### Comparing `obscure_stats-0.2.3/PKG-INFO` & `obscure_stats-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obscure_stats
-Version: 0.2.3
+Version: 0.2.4
 Summary: Collection of lesser-known statistical functions
 Author: Hleb Levitski
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

