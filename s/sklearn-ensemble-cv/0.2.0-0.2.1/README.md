# Comparing `tmp/sklearn_ensemble_cv-0.2.0.tar.gz` & `tmp/sklearn_ensemble_cv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_ensemble_cv-0.2.0.tar", last modified: Thu Oct 26 23:50:58 2023, max compression
+gzip compressed data, was "sklearn_ensemble_cv-0.2.1.tar", last modified: Sat May 11 23:19:10 2024, max compression
```

## Comparing `sklearn_ensemble_cv-0.2.0.tar` & `sklearn_ensemble_cv-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 23:50:58.853988 sklearn_ensemble_cv-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 23:50:58.849988 sklearn_ensemble_cv-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 23:50:58.849988 sklearn_ensemble_cv-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2023-10-26 23:50:58.853988 sklearn_ensemble_cv-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   125448 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      741 2023-10-26 23:50:58.853988 sklearn_ensemble_cv-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 23:50:58.853988 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22224 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10559 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/simu_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7944 2023-10-26 23:50:49.000000 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 23:50:58.853988 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2023-10-26 23:50:58.000000 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-10-26 23:50:58.000000 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 23:50:58.000000 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-10-26 23:50:58.000000 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-26 23:50:58.000000 sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:19:10.796735 sklearn_ensemble_cv-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:19:10.792735 sklearn_ensemble_cv-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:19:10.796735 sklearn_ensemble_cv-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-11 23:19:10.796735 sklearn_ensemble_cv-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   151098 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-11 23:19:10.796735 sklearn_ensemble_cv-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:19:10.796735 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23001 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11709 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/simu_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-11 23:19:03.000000 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:19:10.796735 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-11 23:19:10.000000 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-11 23:19:10.000000 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:19:10.000000 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-11 23:19:10.000000 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-11 23:19:10.000000 sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv.egg-info/top_level.txt
```

### Comparing `sklearn_ensemble_cv-0.2.0/.gitignore` & `sklearn_ensemble_cv-0.2.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 docs
 pdoc
 update.bash
+update.py
+test.py
+risk_theory.py
 
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `sklearn_ensemble_cv-0.2.0/LICENSE` & `sklearn_ensemble_cv-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_ensemble_cv-0.2.0/PKG-INFO` & `sklearn_ensemble_cv-0.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: sklearn_ensemble_cv
-Version: 0.2.0
+Version: 0.2.1
 Summary: sklearn_ensemble_cv is a Python module for performing accurate and efficient ensemble cross-validation methods.
 Home-page: https://github.com/jaydu1/ensemble-cross-validation
 Project-URL: Bug Tracker, https://github.com/jaydu1/ensemble-cross-validation/issues
 Project-URL: Changelog, https://github.com/jaydu1/ensemble-cross-validation/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: numpy
 
+
+[![PyPI](https://img.shields.io/pypi/v/sklearn_ensemble_cv?label=pypi)](https://pypi.org/project/sklearn-ensemble-cv)
+[![PyPI-Downloads](https://img.shields.io/pepy/dt/sklearn_ensemble_cv)](https://pepy.tech/project/sklearn_ensemble_cv)
+
 # Ensemble-cross-validation
 
 
 `sklearn_ensemble_cv` is a Python module for performing accurate and efficient ensemble cross-validation methods from various [projects](https://jaydu1.github.io/overparameterized-ensembling/).
 
 
 ## Features
@@ -35,14 +39,15 @@
 grid_regr = {    
     'max_depth':np.array([6,7], dtype=int), 
     }
 # Hyperparameters for the ensemble
 grid_ensemble = {
     'max_features':np.array([0.9,1.]),
     'max_samples':np.array([0.6,0.7]),
+    'n_jobs':-1 # use all processors for fitting each ensemble
 }
 
 # Build 50 trees and get estimates until 100 trees
 res_ecv, info_ecv = ECV(
     X_train, y_train, DecisionTreeRegressor, grid_regr, grid_ensemble, 
     M=50, M_max=100, return_df=True
 )
@@ -62,18 +67,23 @@
 - [x] GCV
 - [x] CGCV
 - [ ] CGCV non-square loss
 - [ ] ALOCV
 
 # Usage
 
-Check out Jupyter Notebook [demo.ipynb](https://github.com/jaydu1/ensemble-cross-validation/blob/main/demo.ipynb) about how to apply ECV/CGCV on risk estimation and hyperparameter tuning for ensemble learning.
+Check out Jupyter Notebook [demo.ipynb](https://github.com/jaydu1/ensemble-cross-validation/blob/main/demo.ipynb) about how to apply ECV/CGCV on risk estimation and hyperparameter tuning for ensemble learning. The code is tested with `scikit-learn == 1.3.1`.
 
 The [document](https://jaydu1.github.io/overparameterized-ensembling/sklearn-ensemble-cv/docs/index) is available.
 
+The module can be installed via PyPI:
+```cmd
+pip install sklearn-ensemble-cv
+```
+
 MIT License
 
 Copyright (c) 2023 Du Jinhong
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

### Comparing `sklearn_ensemble_cv-0.2.0/setup.cfg` & `sklearn_ensemble_cv-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/__init__.py` & `sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-__all__ = ['ECV', 'GCV', 'splitCV', 'KFoldCV', 'reset_random_seeds', 'Ensemble', 'generate_data']
+__all__ = ['ECV', 'GCV', 'splitCV', 'KFoldCV', 
+           'comp_empirical_ecv', 'comp_empirical_gcv',
+           'reset_random_seeds', 'Ensemble', 'generate_data']
 
-from sklearn_ensemble_cv.cross_validation import ECV, GCV, splitCV, KFoldCV
+from sklearn_ensemble_cv.cross_validation import *
 from sklearn_ensemble_cv.ensemble import Ensemble
 from sklearn_ensemble_cv.utils import reset_random_seeds
 from sklearn_ensemble_cv.simu_data import generate_data
 
 
 __license__ = "MIT"
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __author__ = "Jin-Hong Du"
 __email__ = "jinhongd@andrew.cmu.edu"
 __maintainer__ = "Jin-Hong Du"
 __maintainer_email__ = "jinhongd@andrew.cmu.edu"
 __description__ = ("Ensemble Cross-validation is a Python package for performing specialized " 
     "cross-validation on ensemble models, such as extrapolated cross-validation (ECV), "
     "generalized cross-validation (GCV), and etc. The implementation of ensemble models are "
```

### Comparing `sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/cross_validation.py` & `sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/cross_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     X_test, Y_test : numpy.array, optional
         The test samples.
     _check_input : bool, optional
         If True, check the input arguments.
     kwargs_est : dict, optional
         Additional keyword arguments for the risk estimate.
     
-    Return:
+    Returns
     ----------
     risk_ecv : numpy.array
         The empirical ECV estimate.
     '''
     if _check_input:
         kwargs_regr, kwargs_ensemble, kwargs_est = check_input(kwargs_regr, kwargs_ensemble, kwargs_est, M)
 
@@ -301,15 +301,15 @@
     X_test, Y_test : numpy.array, optional
         The test samples.
     _check_input : bool, optional
         If True, check the input arguments.        
     kwargs_est : dict, optional
         Additional keyword arguments for the risk estimate.
     
-    Return:
+    Returns
     ----------
     risk_ecv : numpy.array
         The empirical ECV estimate.
     '''
     if _check_input:
         if M0>M:
             raise ValueError('M0 must be less than or equal to M.')
@@ -378,29 +378,31 @@
     elif np.isscalar(M_max):
         M_max = np.arange(M_max)+1
     n_M_max = len(M_max)
 
     test = X_test is not None and Y_test is not None
     n_res = n_M_max+M if test else n_M_max
     n_grid = len(grid_regr)
-    res_risk = np.full((n_grid,n_res), np.inf)
-    
+    res_risk = np.full((n_grid, n_res), np.inf)
+
     for i in range(n_grid):
         params_ensemble = grid_ensemble[i]
         params_regr = grid_regr[i]
 
         _, res = comp_empirical_ecv(
             X_train, Y_train, regr, 
             {**kwargs_regr, **params_regr}, {**kwargs_ensemble, **params_ensemble},
             M, M0, M_max, n_jobs, X_test, Y_test, _check_input=False, **kwargs_est
         )
         res_risk[i, :] = np.r_[res]
 
     if return_df:
         cols = np.char.add(['risk_val-']*n_M_max, np.char.mod('%d', 1+np.arange(n_M_max)))
+        if np.isinf(M_max[-1]):
+            cols[-1] = 'risk_val-inf'
         if test:
             cols = np.append(cols, np.char.add(['risk_test-']*M, np.char.mod('%d', 1+np.arange(M))))
         res_ecv = pd.concat([pd.DataFrame(grid_regr), pd.DataFrame(grid_ensemble),
                              pd.DataFrame(res_risk, columns=cols)
                              ] ,axis=1)
     else:
         if test:            
@@ -440,15 +442,15 @@
 #
 # Generalized cross-validation
 #
 ############################################################################
 
 
 def comp_empirical_gcv(
-        X_train, Y_train, regr, kwargs_regr={}, kwargs_ensemble={}, M=20, 
+        X_train, Y_train, regr, kwargs_regr={}, kwargs_ensemble={}, M=20, M0=20, M_max=np.inf, 
         corrected=True, type='full',
         n_jobs=-1, X_test=None, Y_test=None, _check_input=True, **kwargs_est, 
         ):
     '''
     Compute the empirical GCV or CGCV estimate for a given ensemble model.
 
     Parameters
@@ -473,36 +475,47 @@
     X_test, Y_test : numpy.array, optional
         The test samples.
     _check_input : bool, optional
         If True, check the input arguments.        
     kwargs_est : dict, optional
         Additional keyword arguments for the risk estimate.
     
-    Return:
+    Returns
     ----------
     risk_ecv : numpy.array
         The empirical ECV estimate.
     '''
     if _check_input:
+        if M0>M:
+            raise ValueError('M0 must be less than or equal to M.')
+        if np.isinf(M_max):
+            M_max = np.append(np.arange(M)+1, np.inf)
+        elif np.isscalar(M_max):
+            M_max = np.arange(M_max)+1
+    
         kwargs_regr, kwargs_ensemble, kwargs_est = check_input(kwargs_regr, kwargs_ensemble, kwargs_est, M)
+
     regr = fit_ensemble(regr,kwargs_regr,kwargs_ensemble).fit(X_train, Y_train)
     if corrected:
-        risk_gcv = regr.compute_cgcv_estimate(X_train, Y_train, type, n_jobs=n_jobs, **kwargs_est)
+        risk_gcv = regr.compute_cgcv_estimate(X_train, Y_train, M0, type, n_jobs=n_jobs, **kwargs_est)
     else:
-        risk_gcv = regr.compute_gcv_estimate(X_train, Y_train, type, n_jobs=n_jobs, **kwargs_est)
+        risk_gcv = regr.compute_gcv_estimate(X_train, Y_train, M0, type, n_jobs=n_jobs, **kwargs_est)
+
+    risk_gcv = regr.extrapolate(risk_gcv, M_max)
+    
     if X_test is not None and Y_test is not None:        
         risk_val = regr.compute_risk(X_test, Y_test, M, n_jobs=n_jobs, **kwargs_est)
         return regr, (risk_gcv, risk_val)
     else:
         return regr, risk_gcv
     
 
 def GCV(
         X_train, Y_train, regr, grid_regr={}, grid_ensemble={}, kwargs_regr={}, kwargs_ensemble={},
-        M=20, corrected=True, type='full', return_df=False, n_jobs=-1, X_test=None, Y_test=None, 
+        M=20, M0=20, M_max=np.inf, corrected=True, type='full', return_df=False, n_jobs=-1, X_test=None, Y_test=None, 
         kwargs_est={}, **kwargs
         ):
     '''
     Cross-validation for ensemble models using the empirical ECV estimate.
     Currently, only the GCV estimates for the Ridge, Lasso, and ElasticNet are implemented.
 
     Parameters
@@ -533,34 +546,44 @@
         performance of ECV with other cross-validation methods that requires sample-splitting.
     kwargs_est : dict, optional
         Additional keyword arguments for the risk estimate.
     '''
     grid_regr, kwargs_regr, grid_ensemble, kwargs_ensemble, kwargs_est = process_grid(
         grid_regr, kwargs_regr, grid_ensemble, kwargs_ensemble, kwargs_est, M)
 
+    if M0>M:
+        raise ValueError('M0 must be less than or equal to M.')
+    if np.isinf(M_max):
+        M_max = np.append(np.arange(M)+1, np.inf)
+    elif np.isscalar(M_max):
+        M_max = np.arange(M_max)+1
+    n_M_max = len(M_max)
+
     test = X_test is not None and Y_test is not None
-    n_res = 2*M if test else M
+    n_res = n_M_max+M if test else n_M_max
     n_grid = len(grid_regr)
-    res_risk = np.full((n_grid,n_res), np.inf)
+    res_risk = np.full((n_grid, n_res), np.inf)
 
     for i in range(n_grid):
         params_ensemble = grid_ensemble[i]
         params_regr = grid_regr[i]
         
         _, res = comp_empirical_gcv(
             X_train, Y_train, regr, 
             {**kwargs_regr, **params_regr}, {**kwargs_ensemble, **params_ensemble},
-            M, corrected, type, n_jobs, X_test, Y_test,  _check_input=False, **kwargs_est
+            M, M0, M_max, corrected, type, n_jobs, X_test, Y_test,  _check_input=False, **kwargs_est
         )
         res_risk[i, :] = np.r_[res]
 
     if return_df:
-        cols = np.char.add(['risk_val-']*M, np.char.mod('%d', 1+np.arange(M)))
+        cols = np.char.add(['risk_val-']*n_M_max, np.char.mod('%d', 1+np.arange(n_M_max)))
+        if np.isinf(M_max[-1]):
+            cols[-1] = 'risk_val-inf'
         if test:
-            cols = np.append(cols, np.char.add(['risk_test-']*M, np.char.mod('%d', 1+np.arange(M))))
+            cols = np.append(cols, np.char.add(['risk_test-']*M, np.char.mod('%d', 1+np.arange(M))))        
         res_gcv = pd.concat([pd.DataFrame(grid_regr), pd.DataFrame(grid_ensemble),
                              pd.DataFrame(res_risk, columns=cols)
                              ] ,axis=1)
     else:
         if test:            
             res_gcv = (res_risk[:,:M], res_risk[:,M:])
         else:
@@ -573,8 +596,12 @@
         'best_params_regr': {**kwargs_regr, **grid_regr[j]},
         'best_params_ensemble': {**kwargs_ensemble, **grid_ensemble[j]},
         'best_n_estimators': M_best,
         'best_params_index':j,
         'best_score':res_risk[j, M_best-1],
     }
 
-    return res_gcv, info
+    return res_gcv, info
+
+
+
+
```

### Comparing `sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/ensemble.py` & `sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 from sklearn.ensemble import BaggingRegressor
-from sklearn_ensemble_cv.utils import risk_estimate, degree_of_freedom
+from sklearn_ensemble_cv.utils import risk_estimate, degree_of_freedom, avg_sq_err
 
 from joblib import Parallel, delayed
 n_jobs = 16
 
 import numpy as np
 import pandas as pd
 from functools import reduce
@@ -20,59 +20,67 @@
     Ensemble class is built on top of sklearn.ensemble.BaggingRegressor.
     It provides additional methods for computing ECV estimates.
     '''
     def __init__(self, **kwargs):
         super(BaggingRegressor, self).__init__(**kwargs)
 
 
-    def predict_individual(self: BaggingRegressor, X: np.ndarray, n_jobs: int=-1) -> np.ndarray:
+    def predict_individual(self: BaggingRegressor, X: np.ndarray, M: int=-1, n_jobs: int=-1, verbose: bool=0) -> np.ndarray:
         '''
         Predicts the target values for the given input data using the provided BaggingRegressor model.
 
         Parameters
         ----------
             regr : BaggingRegressor
                 The BaggingRegressor model to use for prediction.
             X : np.ndarray
                 [n, p] The input data to predict target values for.
 
-        Returns:
+        Returns
+        ----------
             Y_hat : np.ndarray
                 [n, M] The predicted target values of all $M$ estimators for the input data.
         '''
-        with Parallel(n_jobs=n_jobs, max_nbytes=None, verbose=0) as parallel:
+        if M < 0:
+            M = self.n_estimators
+        with Parallel(n_jobs=n_jobs, max_nbytes=None, verbose=verbose) as parallel:
             Y_hat = parallel(
                 delayed(lambda reg,X: reg.predict(X[:,features]).reshape(-1,1))(reg, X)
-                for reg,features in zip(self.estimators_,self.estimators_features_)
+                for reg,features in zip(self.estimators_[:M],self.estimators_features_[:M])
             )
         Y_hat = np.concatenate(Y_hat, axis=-1)
         return Y_hat
     
 
-    def compute_risk(self, X, Y, M_test=None, return_df=False, n_jobs=-1, **kwargs_est):
+    def compute_risk(
+            self, X, Y, M_test=None, return_df=False, 
+            avg=True, n_jobs=-1, verbose=0, **kwargs_est):
         if M_test is None:
             M_test = self.n_estimators
         if M_test>self.n_estimators:
             raise ValueError('The ensemble size M must be less than or equal to the number of estimators in the BaggingRegressor model.')
         if Y.ndim==1:
             Y = Y[:,None]
 
-        Y_hat = self.predict_individual(X, n_jobs)
-        Y_hat = np.cumsum(Y_hat, axis=1) / np.arange(1,M_test+1)
-        err_eval = (Y_hat - Y)**2
+        Y_hat = self.predict_individual(X, M_test, n_jobs, verbose)
+        if avg:
+            err_eval = avg_sq_err(Y_hat - Y)
+        else:
+            Y_hat = np.cumsum(Y_hat, axis=1) / np.arange(1, M_test+1)
+            err_eval = (Y_hat - Y)**2
         risk = risk_estimate(err_eval, axis=0, **kwargs_est)
 
         if return_df:
             df = pd.DataFrame({'M':np.arange(1,M_test+1), 'risk':risk})
             return df
         else:
             return risk
     
     
-    def compute_ecv_estimate(self, X_train, Y_train, M_test=None, M0=None, return_df=False, n_jobs=-1, **kwargs_est):
+    def compute_ecv_estimate(self, X_train, Y_train, M_test=None, M0=None, return_df=False, n_jobs=-1, verbose=0, **kwargs_est):
         '''
         Computes the ECV estimate for the given input data using the provided BaggingRegressor model.
 
         Parameters
         ----------
         X_train : np.ndarray
             [n, p] The input covariates.
@@ -85,15 +93,15 @@
         return_df : bool, optional
             If True, returns the ECV estimate as a pandas.DataFrame object.
         n_jobs : int, optional
             The number of jobs to run in parallel. If -1, all CPUs are used.
         kwargs_est : dict
             Additional keyword arguments for the risk estimate.
 
-        Returns:
+        Returns
         --------
         risk_ecv : np.ndarray or pandas.DataFrame
             [M_test, ] The ECV estimate for each ensemble size in M_test.
         '''
         if M_test is None:
             M_test = self.n_estimators
         if M0 is None:
@@ -103,19 +111,19 @@
         if np.isscalar(M_test):
             M_test = np.arange(1,M_test+1)
         else:
             M_test = np.array(M_test)
         if Y_train.ndim==1:
             Y_train = Y_train[:,None]
         ids_list = self.estimators_samples_[:M0]
-        Y_hat = self.predict_individual(X_train, n_jobs)
+        Y_hat = self.predict_individual(X_train, M0, n_jobs)
         dev_eval = Y_hat - Y_train
         err_eval = dev_eval**2
         
-        with Parallel(n_jobs=n_jobs, max_nbytes=None, verbose=0) as parallel:
+        with Parallel(n_jobs=n_jobs, max_nbytes=None, verbose=verbose) as parallel:
             res_1 = parallel(
                 delayed(lambda j:risk_estimate(
                     np.delete(err_eval[:,j], ids_list[j]), **kwargs_est)
                        )(j)
                 for j in np.arange(M0)
             )
             res_2 = parallel(
@@ -133,16 +141,35 @@
         risk_ecv = - (1-2/M_test) * risk_ecv_1 + 2*(1-1/M_test) * risk_ecv_2
         if return_df:
             df = pd.DataFrame({'M':M_test, 'estimate':risk_ecv})
             return df
         else:
             return risk_ecv
         
+    
+    def extrapolate(self, risk, M_test=None):
+        if M_test is None:
+            M_test = self.n_estimators
+        M0 = risk.shape[0]        
+        if np.isscalar(M_test):
+            M_test = np.arange(1,M_test+1)
+        else:
+            M_test = np.array(M_test)
+        if M0 <2 or np.max(M_test) < M0:
+            raise ValueError('The ensemble size M or M0 must be at least 2.')
+        
+        risk_1 = risk[0]
+        risk_inf = np.sum(risk - risk_1/np.arange(1, M0+1)) / np.sum(1 - 1/np.arange(1, M0+1))
+        
+        risk_ecv = (1/M_test) * risk_1 + (1-1/M_test) * risk_inf
+        risk_ecv[:M0] = risk
+        return risk_ecv
+        
 
-    def compute_gcv_estimate(self, X_train, Y_train, type='full', return_df=False, n_jobs=-1, **kwargs_est):
+    def compute_gcv_estimate(self, X_train, Y_train, M=None, type='full', return_df=False, n_jobs=-1, verbose=0, **kwargs_est):
         '''
         Computes the GCV estimate for the given input data using the provided BaggingRegressor model.
 
         Parameters
         ----------
         X_train : np.ndarray
             [n, p] The input covariates.
@@ -154,59 +181,61 @@
         return_df : bool, optional
             If True, returns the GCV estimate as a pandas.DataFrame object.
         n_jobs : int, optional
             The number of jobs to run in parallel. If -1, all CPUs are used.
         kwargs_est : dict
             Additional keyword arguments for the risk estimate.
 
-        Returns:
+        Returns
         --------
         risk_gcv : np.ndarray or pandas.DataFrame
             [M_test, ] The GCV estimate for each ensemble size in M_test.
         '''
         if self.base_estimator_.__class__.__name__ not in ['Ridge', 'Lasso', 'ElasticNet']:
             raise ValueError('GCV is only implemented for Ridge, Lasso, and ElasticNet regression.')
         if Y_train.ndim==1:
             Y_train = Y_train[:,None]
-        M = self.n_estimators
+        if M is None:
+            M = self.n_estimators        
         M_arr = np.arange(M)
         ids_list = self.estimators_samples_
-        Y_hat = self.predict_individual(X_train, n_jobs)
-        Y_hat = np.cumsum(Y_hat, axis=1) / (M_arr+1)
+        Y_hat = self.predict_individual(X_train, M, n_jobs)        
         n = X_train.shape[0]
-        err_eval = (Y_hat - Y_train)**2
 
-        with Parallel(n_jobs=n_jobs, max_nbytes=None, verbose=0) as parallel:
+        with Parallel(n_jobs=n_jobs, max_nbytes=None, verbose=verbose) as parallel:
             dof = parallel(
                 delayed(lambda j:degree_of_freedom(self.estimators_[j], X_train[ids_list[j]])
                        )(j)
                 for j in M_arr
             )
             dof = np.mean(dof)
 
         if type=='full':
+            err_eval = avg_sq_err(Y_hat - Y_train)
             err_train = np.mean(err_eval, axis=0)
             deno = (1 - dof/n)**2
             risk_gcv = err_train / deno
-        else:            
+        else:
+            Y_hat = np.cumsum(Y_hat, axis=1) / (M_arr+1)
+            err_eval = (Y_hat - Y_train)**2
             ids_union_list = [reduce(np.union1d, ids_list[:j+1]) for j in M_arr]
             n_ids = np.array([len(ids) for ids in ids_union_list])
             err_train = np.array([np.mean(err_eval[ids_union_list[j],j]) for j in M_arr])
             deno = (1 - dof/n_ids)**2
             risk_gcv = err_train / deno
         
         if return_df:
             df = pd.DataFrame({'M':M_arr+1, 'estimate':risk_gcv, 'err_train':err_train, 'deno':deno})
             return df
         else:
             return risk_gcv
         
     
 
-    def compute_cgcv_estimate(self, X_train, Y_train, type='full', return_df=False, n_jobs=-1, **kwargs_est):
+    def compute_cgcv_estimate(self, X_train, Y_train, M=None, type='full', return_df=False, n_jobs=-1, verbose=0, **kwargs_est):
         '''
         Computes the GCV estimate for the given input data using the provided BaggingRegressor model.
 
         Parameters
         ----------
         X_train : np.ndarray
             [n, p] The input covariates.
@@ -218,52 +247,53 @@
         return_df : bool, optional
             If True, returns the GCV estimate as a pandas.DataFrame object.
         n_jobs : int, optional
             The number of jobs to run in parallel. If -1, all CPUs are used.
         kwargs_est : dict
             Additional keyword arguments for the risk estimate.
 
-        Returns:
+        Returns
         --------
         risk_gcv : np.ndarray or pandas.DataFrame
             [M_test, ] The CGCV estimate for each ensemble size in M_test.
         '''
         if self.base_estimator_.__class__.__name__ not in ['Ridge', 'Lasso', 'ElasticNet']:
             raise ValueError('GCV is only implemented for Ridge, Lasso, and ElasticNet regression.')
         if Y_train.ndim==1:
             Y_train = Y_train[:,None]
-        M = self.n_estimators
+        if M is None:
+            M = self.n_estimators            
         M_arr = np.arange(M)
         ids_list = self.estimators_samples_
-        Y_hat = self.predict_individual(X_train, n_jobs)
+        Y_hat = self.predict_individual(X_train, M, n_jobs)
           
         n, p = X_train.shape
         if self.estimators_[0].fit_intercept:
             p += 1
         phi = p/n
         k = int(n * self.max_samples)
         psi = p/k
 
-        with Parallel(n_jobs=n_jobs, max_nbytes=None, verbose=0) as parallel:
+        with Parallel(n_jobs=n_jobs, max_nbytes=None, verbose=verbose) as parallel:
             dof = parallel(
-                delayed(lambda j:degree_of_freedom(self.estimators_[j], X_train[ids_list[j]])
-                       )(j)
+                delayed(lambda j:degree_of_freedom(self.estimators_[j], X_train[ids_list[j]]))(j)
                 for j in M_arr
             )
             dof = np.mean(dof)
 
         err_train = (Y_hat-Y_train)**2
         if type=='full':
-            correct_term = np.mean(err_train) / (1 - 2* dof/n + dof**2/(k*n))
+            correct_term = np.mean(err_train) / (1 - 2*dof/n + dof**2/(k*n))
+        elif type=='ovlp':
+            correct_term = np.mean([np.mean(err_train[ids_list[j],j]) for j in M_arr]) / (1 - dof/k)**2
         else:
-            correct_term = np.mean([np.mean(err_train[ids_list[j],j]) for j in M_arr]) / (1 - dof/n)**2
-
-        Y_hat = np.cumsum(Y_hat, axis=1) / (M_arr+1)
-        err_eval = (Y_hat - Y_train)**2
-        err_train = np.array([np.mean(err_eval[:,j]) for j in M_arr])
+            raise ValueError('The type must be either "full" or "ovlp".')
+        
+        err_eval = avg_sq_err(Y_hat - Y_train)
+        err_train = np.mean(err_eval, axis=0)
         deno = (1 - dof/n)**2
         C = 1/ (n/dof - 1)**2 / (M_arr+1) * (psi/phi - 1) * correct_term
         risk_cgcv = err_train / deno - C
         
         if return_df:
             df = pd.DataFrame({'M':M_arr+1, 'estimate':risk_cgcv, 'err_train':err_train, 'deno':deno, 'C':C})
             return df
```

### Comparing `sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/simu_data.py` & `sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/simu_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Parameters
     ----------
     sigma_sq: float
         scalar_like,
     first_column_except_1: array
         1d-array, except diagonal 1.
     
-    Return:
+    Returns
     ----------
         2d-array with dimension (len(first_column)+1, len(first_column)+1)
     '''
     first_column = np.append(1, first_column_except_1)
     cov_mat = sigma_sq * toeplitz(first_column)
     return cov_mat
 
@@ -30,15 +30,15 @@
     rho : float
         scalar, should be within -1 and 1.
     n : int
         scalar, number of rows and columns of the covariance matrix.
     sigma_sq : float
         scalar, multiplicative factor of the covariance matrix.
     
-    Return
+    Returns
     ----------
         2d-matrix of (n,n)
     """
     if rho != 0.:
         rho_tile = rho * np.ones([n - 1])
         first_column_except_1 = np.cumprod(rho_tile)
         cov_mat = create_toeplitz_cov_mat(sigma_sq, first_column_except_1)
@@ -51,15 +51,15 @@
     """
     Parameters
     ----------
     rhos : float
         array, should be within -1 and 1.
     n : int
     
-    Return
+    Returns
     ----------
         2d-matrix of (n,n)
     """
     n_block = len(rhos)
     s_block = n // n_block
     covs = []
     for i in range(n_block):
```

### Comparing `sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv/utils.py` & `sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import random
 import numpy as np
 import pandas as pd
-from itertools import product
+from itertools import product, combinations
 
 
 def reset_random_seeds(seed):
     os.environ['PYTHONHASHSEED']=str(seed)
     random.seed(seed)
     np.random.seed(seed)
 
@@ -41,15 +41,15 @@
 
 def risk_estimate(sq_err, axis=None, method='AVG', **kwargs):
     '''
     Compute the risk estimate from the squared error.
 
     Parameters
     ----------
-    sq_err : 1d-array
+    sq_err : 2d-array
         The squared error.
     method : str
         The method to use for risk estimation. Either 'AVG' or 'MOM'.
     kwargs : dict
         Additional keyword arguments for the risk estimation method.
     '''
 
@@ -116,14 +116,67 @@
     Estimate the null risk of the data for regression problems.
     '''
     mu = 0.
     return np.mean((Y-mu)**2)
 
 
 
+def _avg_sq_err_M(x, M, M_max, axis=0, **kwargs_est):
+    '''
+    Compute the average of all combinations of M of all columns.
+
+    Parameters
+    ----------
+    x : 2d-array
+        The data of shape [n,M].
+    M : int
+        The number of columns to combine.
+    M_max : int
+        The maximum combinations number of columns to combine.
+
+    Returns
+    -------
+    avg_sq_err : float
+        The average squared error of the M-ensemble.
+    '''
+    if M==1:
+        return np.mean(x**2, axis=1)
+    else:
+        iter = 0
+        err = []
+        for id in combinations(np.arange(x.shape[1]), M):
+            if iter >= M_max:
+                break
+            err.append(np.mean(x[:,id], axis=1))
+            iter += 1
+        err = np.c_[err]**2
+        return np.mean(err, axis=0)
+
+
+def avg_sq_err(err, M_max=None):
+    '''
+    Compute the average squared error.
+
+    Parameters
+    ----------
+    err : 2d-array
+        The squared errors of shape [n,M].
+
+    Returns
+    -------
+    risk : 1d-array
+        The estimated squared errors of the M-ensembles.
+    '''
+    if M_max is None:
+        M_max = np.ones(err.shape[1]) * 500
+        M_max[np.arange(err.shape[1])>10] = 10
+        M_max = M_max.astype(int)
+    risk = np.fromiter((_avg_sq_err_M(err, M+1, M_max[M]) for M in np.arange(err.shape[1])), 
+                       dtype=np.dtype((float, err.shape[0]))).T
+    return risk
 
 ####################################################################################################
 #
 # Grid processing functions
 #
 ####################################################################################################
```

### Comparing `sklearn_ensemble_cv-0.2.0/sklearn_ensemble_cv.egg-info/PKG-INFO` & `sklearn_ensemble_cv-0.2.1/sklearn_ensemble_cv.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
-Name: sklearn-ensemble-cv
-Version: 0.2.0
+Name: sklearn_ensemble_cv
+Version: 0.2.1
 Summary: sklearn_ensemble_cv is a Python module for performing accurate and efficient ensemble cross-validation methods.
 Home-page: https://github.com/jaydu1/ensemble-cross-validation
 Project-URL: Bug Tracker, https://github.com/jaydu1/ensemble-cross-validation/issues
 Project-URL: Changelog, https://github.com/jaydu1/ensemble-cross-validation/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: numpy
 
+
+[![PyPI](https://img.shields.io/pypi/v/sklearn_ensemble_cv?label=pypi)](https://pypi.org/project/sklearn-ensemble-cv)
+[![PyPI-Downloads](https://img.shields.io/pepy/dt/sklearn_ensemble_cv)](https://pepy.tech/project/sklearn_ensemble_cv)
+
 # Ensemble-cross-validation
 
 
 `sklearn_ensemble_cv` is a Python module for performing accurate and efficient ensemble cross-validation methods from various [projects](https://jaydu1.github.io/overparameterized-ensembling/).
 
 
 ## Features
@@ -35,14 +39,15 @@
 grid_regr = {    
     'max_depth':np.array([6,7], dtype=int), 
     }
 # Hyperparameters for the ensemble
 grid_ensemble = {
     'max_features':np.array([0.9,1.]),
     'max_samples':np.array([0.6,0.7]),
+    'n_jobs':-1 # use all processors for fitting each ensemble
 }
 
 # Build 50 trees and get estimates until 100 trees
 res_ecv, info_ecv = ECV(
     X_train, y_train, DecisionTreeRegressor, grid_regr, grid_ensemble, 
     M=50, M_max=100, return_df=True
 )
@@ -62,18 +67,23 @@
 - [x] GCV
 - [x] CGCV
 - [ ] CGCV non-square loss
 - [ ] ALOCV
 
 # Usage
 
-Check out Jupyter Notebook [demo.ipynb](https://github.com/jaydu1/ensemble-cross-validation/blob/main/demo.ipynb) about how to apply ECV/CGCV on risk estimation and hyperparameter tuning for ensemble learning.
+Check out Jupyter Notebook [demo.ipynb](https://github.com/jaydu1/ensemble-cross-validation/blob/main/demo.ipynb) about how to apply ECV/CGCV on risk estimation and hyperparameter tuning for ensemble learning. The code is tested with `scikit-learn == 1.3.1`.
 
 The [document](https://jaydu1.github.io/overparameterized-ensembling/sklearn-ensemble-cv/docs/index) is available.
 
+The module can be installed via PyPI:
+```cmd
+pip install sklearn-ensemble-cv
+```
+
 MIT License
 
 Copyright (c) 2023 Du Jinhong
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
```

