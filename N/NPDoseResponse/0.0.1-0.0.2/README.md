# Comparing `tmp/npdoseresponse-0.0.1.tar.gz` & `tmp/npdoseresponse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npdoseresponse-0.0.1.tar", last modified: Tue May  7 06:25:20 2024, max compression
+gzip compressed data, was "npdoseresponse-0.0.2.tar", last modified: Sun May 12 19:30:05 2024, max compression
```

## Comparing `npdoseresponse-0.0.1.tar` & `npdoseresponse-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-07 06:25:20.453270 npdoseresponse-0.0.1/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.1/LICENSE
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-07 06:25:20.440583 npdoseresponse-0.0.1/NPDoseResponse/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)    26718 2024-05-07 04:20:17.000000 npdoseresponse-0.0.1/NPDoseResponse/NPDoseResponse.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      119 2024-05-07 06:24:42.000000 npdoseresponse-0.0.1/NPDoseResponse/__init__.py
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2765 2024-03-11 06:18:32.000000 npdoseresponse-0.0.1/NPDoseResponse/rbf.py
-drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-07 06:25:20.450924 npdoseresponse-0.0.1/NPDoseResponse.egg-info/
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1926 2024-05-07 06:25:20.000000 npdoseresponse-0.0.1/NPDoseResponse.egg-info/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      297 2024-05-07 06:25:20.000000 npdoseresponse-0.0.1/NPDoseResponse.egg-info/SOURCES.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-07 06:25:20.000000 npdoseresponse-0.0.1/NPDoseResponse.egg-info/dependency_links.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-07 06:25:20.000000 npdoseresponse-0.0.1/NPDoseResponse.egg-info/requires.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-07 06:25:20.000000 npdoseresponse-0.0.1/NPDoseResponse.egg-info/top_level.txt
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1926 2024-05-07 06:25:20.451999 npdoseresponse-0.0.1/PKG-INFO
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1426 2024-05-07 06:22:29.000000 npdoseresponse-0.0.1/README.md
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-07 06:25:20.453483 npdoseresponse-0.0.1/setup.cfg
--rwxrwxrwx   0 yikun     (1000) yikun     (1000)      796 2024-05-07 06:25:04.000000 npdoseresponse-0.0.1/setup.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-12 19:30:05.513621 npdoseresponse-0.0.2/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1070 2024-05-07 04:36:16.000000 npdoseresponse-0.0.2/LICENSE
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-12 19:30:05.507653 npdoseresponse-0.0.2/NPDoseResponse/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)    22017 2024-05-12 19:24:12.000000 npdoseresponse-0.0.2/NPDoseResponse/NPDoseResponse.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      211 2024-05-12 19:29:36.000000 npdoseresponse-0.0.2/NPDoseResponse/__init__.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     2765 2024-03-11 06:18:32.000000 npdoseresponse-0.0.2/NPDoseResponse/rbf.py
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     5430 2024-05-12 19:21:37.000000 npdoseresponse-0.0.2/NPDoseResponse/utils.py
+drwxrwxrwx   0 yikun     (1000) yikun     (1000)        0 2024-05-12 19:30:05.512094 npdoseresponse-0.0.2/NPDoseResponse.egg-info/
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1926 2024-05-12 19:30:05.000000 npdoseresponse-0.0.2/NPDoseResponse.egg-info/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      321 2024-05-12 19:30:05.000000 npdoseresponse-0.0.2/NPDoseResponse.egg-info/SOURCES.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)        1 2024-05-12 19:30:05.000000 npdoseresponse-0.0.2/NPDoseResponse.egg-info/dependency_links.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       12 2024-05-12 19:30:05.000000 npdoseresponse-0.0.2/NPDoseResponse.egg-info/requires.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       15 2024-05-12 19:30:05.000000 npdoseresponse-0.0.2/NPDoseResponse.egg-info/top_level.txt
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1926 2024-05-12 19:30:05.512911 npdoseresponse-0.0.2/PKG-INFO
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)     1426 2024-05-07 06:22:29.000000 npdoseresponse-0.0.2/README.md
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)       38 2024-05-12 19:30:05.513817 npdoseresponse-0.0.2/setup.cfg
+-rwxrwxrwx   0 yikun     (1000) yikun     (1000)      805 2024-05-12 19:29:33.000000 npdoseresponse-0.0.2/setup.py
```

### Comparing `npdoseresponse-0.0.1/LICENSE` & `npdoseresponse-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.1/NPDoseResponse/NPDoseResponse.py` & `npdoseresponse-0.0.2/NPDoseResponse/NPDoseResponse.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-"""
-@author: Yikun Zhang
-Last Editing: May 5, 2024
-
-This file contains the implementation of local polynomial regression as well as 
-our proposed integral estimator and its derivative estimator.
-"""
+
+# Author: Yikun Zhang
+# Last Editing: May 12, 2024
+
+# Description: This script contains the implementation of local polynomial regression 
+# as well as our proposed integral estimator and its localized derivative estimator.
 
 import numpy as np
-import rbf as rbf
+from .rbf import KernelRetrieval
 from multiprocessing import Pool
 from functools import partial
+from .utils import *
 
 #=======================================================================================#
 
 def LocalPolyReg(Y, X, x_eval=None, degree=2, deriv_ord=1, h=None, b=None, 
                  kernT="epanechnikov", kernS="epanechnikov", 
                  h_lst=np.linspace(0.5, 15, 30), b_lst=np.linspace(0.2, 6, 30)):
     '''
@@ -86,129 +85,14 @@
     print("The current bandwidth for confounding variables in the local polynomial regression is "+ str(b) + ".\n")
     
     Y_est = LocalPolyRegMain(Y, X, x_eval=x_eval, degree=degree, deriv_ord=deriv_ord, 
                              h=h, b=b, kernT=kernT, kernS=kernS)
     return Y_est
 
 
-def RoTBWLocalPoly(Y, X, kernT="epanechnikov", kernS="epanechnikov", C_h=7, C_b=3):
-    '''
-    Compute the rule-of-thumb bandwidth selector in Eq.(A1) of 
-    Yang and Tschernig (1999).
-    
-    
-    Parameters
-    ----------
-        Y: (n,)-array
-            The outcomes of n observations.
-        
-        X: (n,d+1)-array
-            The first column of X is the treatment/exposure variable, while 
-            the other d columns are confounding variables of n observations.
-            
-        kernT, kernS: str
-            The names of kernel functions for the treatment/exposure variable 
-            and confounding variables. (Default: "epanechnikov".)
-    '''
-    n = X.shape[0]  ## Number of data points
-    d = X.shape[1] - 1
-    
-    kernT, sigmaK_sq, K_sq = rbf.KernelRetrieval(kernT)
-    # Apply the rule-of-thumb bandwidth selector in Eq.(A1) of Yang and Tschernig (1999)
-    p_coeff = np.polyfit(X[:,0], Y, 4)
-    sec_deriv = 12*p_coeff[0]*X[:,0] + 6*p_coeff[1]*X[:,0] + 2*X[:,0]
-    C_fun = np.mean(sec_deriv**2)
-    T = X[:,0].reshape(-1,1)
-    lhs = np.concatenate([np.ones((n,1)), X, T**2, T**3, T**4], axis=1)
-    rcond = np.finfo(lhs.dtype).eps * max(*lhs.shape)
-    beta = np.linalg.lstsq(lhs, Y, rcond=rcond)[0]
-    # Compute the residual sum of squares
-    resid = np.sum((Y - np.dot(lhs, beta))**2) * (np.max(X[:,0]) - np.min(X[:,0]))/ (n-5)
-    sigmaK_sq = sigmaK_sq**2
-    # ROT
-    h = ((K_sq*resid)/(4*n*sigmaK_sq*C_fun))**(1/5) * (n**(d/(5*(d+5)))) * C_h
-    
-    kernS, sigmaK_sq, K_sq = rbf.KernelRetrieval(kernS)
-    sec_deriv = np.zeros((n, d))
-    for i in range(1, d+1):
-        # Fit a fourth-order polynomial to each confounding variable
-        p_coeff = np.polyfit(X[:,i], Y, 4)
-        sec_deriv[:,i-1] = 12*p_coeff[0]*X[:,i] + 6*p_coeff[1]*X[:,i] + 2*X[:,i]
-    C_fun = np.sum(np.diag(np.dot(sec_deriv.T, sec_deriv))/n)
-    lhs = np.concatenate([np.ones((n,1)), X, T**2, T**3, T**4], axis=1)
-    # lhs = np.concatenate([np.ones((n,1)), X[:,1:]], axis=1)
-    rcond = np.finfo(lhs.dtype).eps * max(*lhs.shape)
-    beta = np.linalg.lstsq(lhs, Y, rcond=rcond)[0]
-    resid = np.sum((Y - np.dot(lhs, beta))**2) * (np.max(X[:,1:], axis=0) - np.min(X[:,1:], axis=0)) / (n-5)
-    sigmaK_sq = sigmaK_sq**2
-    K_sq = K_sq**d
-    b = ((K_sq*d*resid)/(4*n*sigmaK_sq*C_fun))**(1/(d+5)) * C_b
-    
-    return h, b
-
-
-def HatMatrix(X, degree=2, deriv_ord=1, h=None, b=None, kernT="epanechnikov", kernS="epanechnikov"):
-    '''
-    Compute the hat matrix of the local polynomial regression when it is viewed 
-    as a linear smoother.
-    
-    
-    Parameters
-    ----------
-        X: (n,d+1)-array
-            The first column of X is the treatment/exposure variable, while 
-            the other d columns are confounding variables of n observations.
-            
-        degree: int
-            Degree of local polynomials. (Default: degree=2.)
-            
-        deriv_ord: int
-            The order of the estimated derivative the conditional mean outcome function. 
-            (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
-            conditional mean outcome function with respect to the treatment variable.)
-            
-        h,b: float
-            The bandwidth parameters for the treatment/exposure variable and confounding variables. 
-            
-        kernT, kernS: str
-            The names of kernel functions for the treatment/exposure variable and confounding variables.
-            (Default: "epanechnikov".)
-    '''
-    n = X.shape[0]  ## Number of data points
-    d = X.shape[1] - 1
-    x_eval = X.copy()
-    
-    print("The current bandwidth for treament variable in the local polynomial regression is "+ str(h) + ".\n")
-    print("The current bandwidth for confounding variables in the local polynomial regression is "+ str(b) + ".\n")
-    
-    kernT, sigmaK_sq, K_sq = rbf.KernelRetrieval(kernT)
-    kernS, sigmaK_sq, K_sq = rbf.KernelRetrieval(kernS)
-    hat_mat = np.zeros((n, n))
-    for i in range(x_eval.shape[0]):
-        weights = kernT((X[:,0] - x_eval[i,0])/h) * np.prod(kernS((X[:,1:] - x_eval[i,1:])/b), axis=1)
-        # Filter out the data points with zero weights to speed up regressions with kernels of compact support
-        inds = np.where(np.abs(weights) > 1e-26)[0]
-        X_dat = np.zeros((n, degree+1+d))
-        # X_dat[:,:(degree+1)] = (((X[:,0] - x_eval[i,0])/h).reshape(-1,1))**(np.arange(degree+1))
-        for p in range(degree + 1):
-            X_dat[:,p] = ((X[:,0] - x_eval[i,0])/h)**p
-        X_dat[:,(degree+1):] = (X[:,1:] - x_eval[i,1:])/b
-        X_dat = X_dat[inds,:]
-        W = np.diag(weights[inds])
-        design_mat = np.dot(np.dot(X_dat.T, W), X_dat)
-        try:
-            hat_mat_samp = np.dot(np.linalg.inv(design_mat), np.dot(X_dat.T, W))
-        except:
-            # Add some small quantities to the diagonal matrix to prevent the singularity of the matrix
-            design_mat = design_mat + 1e-16*np.eye(design_mat.shape[0])
-            hat_mat_samp = np.dot(np.linalg.inv(design_mat), np.dot(X_dat.T, W))
-        hat_mat[i,inds] = hat_mat_samp[deriv_ord,:]
-    return hat_mat
-
-
 def LocalPolyRegMain(Y, X, x_eval=None, degree=2, deriv_ord=0, h=None, b=None, 
                      kernT="epanechnikov", kernS="epanechnikov"):
     '''
     Main function for computing the local polynomial regression.
     
     
     Parameters
@@ -238,16 +122,16 @@
             confounding variables. (Default: h=None, b=None. Then, the rule-of-thumb 
             bandwidth selector in Eq.(A1) of Yang and Tschernig (1999) is used.)
             
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
     '''
-    kernT, sigmaK_sq, K_sq = rbf.KernelRetrieval(kernT)
-    kernS, sigmaK_sq, K_sq = rbf.KernelRetrieval(kernS)
+    kernT, sigmaK_sq, K_sq = KernelRetrieval(kernT)
+    kernS, sigmaK_sq, K_sq = KernelRetrieval(kernS)
     
     n = X.shape[0]  ## Number of data points
     d = X.shape[1] - 1
     Y_est = np.zeros((x_eval.shape[0],))
     for i in range(x_eval.shape[0]):
         weights = kernT((X[:,0] - x_eval[i,0])/h) * np.prod(kernS((X[:,1:] - x_eval[i,1:])/b), axis=1)
         # Filter out the data points with zero weights to speed up regressions with kernels of compact support
@@ -403,15 +287,15 @@
     n = X.shape[0]  ## Number of data points
     d = 1
     if h_bar is None:
         # Apply the Silverman's rule of thumb bandwidth in Chen et al.(2016).
         h_bar = (4/(d+2))**(1/(d+4))*(n**(-1/(d+4)))*np.std(X[:,0])
         print("The current bandwidth for the conditional CDF estimator is "+ str(h_bar) + ".\n")
     
-    kernT_bar, sigmaK_sq, K_sq = rbf.KernelRetrieval(kernT_bar)
+    kernT_bar, sigmaK_sq, K_sq = KernelRetrieval(kernT_bar)
         
     weight_mat = kernT_bar((t_eval - X[:,0].reshape(-1,1)) / h_bar)
     weight_mat = weight_mat / np.sum(weight_mat, axis=0)
     weight_mat[np.isnan(weight_mat)] = 0
     if parallel:
         with Pool(processes=processes) as pool:
             part_fun = partial(LocalPolyReg_Fs, Y=Y, X=X, degree=degree, deriv_ord=deriv_ord, 
@@ -425,16 +309,17 @@
             beta_mat[:,i] = LocalPolyReg(Y, X, x_eval=X_mat, degree=degree, deriv_ord=deriv_ord, 
                                          h=h, b=b, kernT=kernT, kernS=kernS)
     
     theta_C = np.sum(weight_mat * beta_mat, axis=0)
     return theta_C
 
 
-def IntegEst(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", 
-                h=None, b=None, degree=2, deriv_ord=1, kernT="epanechnikov", kernS="epanechnikov"):
+def IntegEst(Y, X, t_eval=None, h_bar=None, kernT_bar="gaussian", h=None, b=None, 
+             degree=2, deriv_ord=1, kernT="epanechnikov", kernS="epanechnikov",
+             parallel=False, processes=20):
     '''
     Estimating the dose-response curve via our integral estimator with linear 
     interpolation approximation.
     
     
     Parameters
     ----------
@@ -469,25 +354,33 @@
             The order of the estimated derivative the conditional mean outcome function. 
             (Default: deriv_ord=1. Then, it estimates the partial derivative of the 
             conditional mean outcome function with respect to the treatment variable.)
             
         kernT, kernS: str
             The names of kernel functions for the treatment/exposure variable 
             and confounding variables. (Default: "epanechnikov".)
+        
+        parallel: boolean
+            The indicator of whether the function should be parallel executed by
+            multi-processing. (Default: parallel=False.)
+            
+        processes: int
+            The number of processes for parallel execution. (Default: processes=20.)
     '''
     
     if t_eval is None: 
         t_eval = X[:,0].copy()
     
     T_sort = np.sort(X[:,0])
     n = X.shape[0]  ## Number of data points
     
     # Compute theta_C at the order statistics of T
     theta_est = DerivEffect(Y, X, t_eval=T_sort, h_bar=h_bar, kernT_bar=kernT_bar, 
-                            h=h, b=b, degree=degree, deriv_ord=deriv_ord, kernT=kernT, kernS=kernS)
+                            h=h, b=b, degree=degree, deriv_ord=deriv_ord, kernT=kernT, kernS=kernS,
+                            parallel=parallel, processes=processes)
     T_delta = T_sort[1:] - T_sort[:(n-1)]
     
     int_mat_up = np.ones((n,)) * (T_delta*(np.arange(1, n)*theta_est[:(n-1)])).reshape(-1,1)
     int_mat_up = int_mat_up * (np.arange(n-1).reshape(-1,1) < np.arange(n))
     
     int_mat_down = np.ones((n,)) * (T_delta*((n-np.arange(1, n))*theta_est[1:])).reshape(-1,1)
     int_mat_down = int_mat_down * (np.arange(n-1).reshape(-1,1) >= np.arange(n))
@@ -524,15 +417,15 @@
             (Default: deriv_ord=0. Then, it is the usual local polynomial regression.)
     '''
     if x_eval is None: 
         x_eval = X.copy()
         
     n = X.shape[0]  ## Number of data points
         
-    kernel, sigmaK_sq, K_sq = rbf.KernelRetrieval(kernel)
+    kernel, sigmaK_sq, K_sq = KernelRetrieval(kernel)
     if h is None:
         # Apply the rule-of-thumb bandwidth selector in Eq.(A1) of Yang and Tschernig (1999)
         p_coeff = np.polyfit(X, Y, 4)
         sec_deriv = 12*p_coeff[0]*X + 6*p_coeff[1]*X + 2*X
         C_fun = np.mean(sec_deriv**2)
         lhs = np.concatenate([np.ones((n,1)), X.reshape(-1,1)], axis=1)
         rcond = np.finfo(lhs.dtype).eps * max(*lhs.shape)
```

### Comparing `npdoseresponse-0.0.1/NPDoseResponse/rbf.py` & `npdoseresponse-0.0.2/NPDoseResponse/rbf.py`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.1/NPDoseResponse.egg-info/PKG-INFO` & `npdoseresponse-0.0.2/NPDoseResponse.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NPDoseResponse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
 Home-page: https://github.com/zhangyk8/NPDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `npdoseresponse-0.0.1/PKG-INFO` & `npdoseresponse-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NPDoseResponse
-Version: 0.0.1
+Version: 0.0.2
 Summary: Nonparametric Estimation and Inference on Dose-Response Curves
 Home-page: https://github.com/zhangyk8/NPDoseResponse
 Author: Yikun Zhang
 Author-email: yikunzhang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `npdoseresponse-0.0.1/README.md` & `npdoseresponse-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `npdoseresponse-0.0.1/setup.py` & `npdoseresponse-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="NPDoseResponse",
-    version="0.0.1",
+    version="0.0.2",
     author="Yikun Zhang",
     author_email="yikunzhang@foxmail.com",
     description="Nonparametric Estimation and Inference on Dose-Response Curves",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhangyk8/NPDoseResponse",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    packages=setuptools.find_packages(include=["NPDoseResponse"]),
+    packages=setuptools.find_packages(),
+    # packages=["NPDoseResponse"],
     install_requires=["numpy >= 1.16"],
     python_requires=">=3.8",
 )
```

