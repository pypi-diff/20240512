# Comparing `tmp/pymle-diffusion-0.0.8.tar.gz` & `tmp/pymle-diffusion-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymle-diffusion-0.0.8.tar", last modified: Sun Oct 29 23:34:37 2023, max compression
+gzip compressed data, was "pymle-diffusion-0.0.9.tar", last modified: Sun May 12 16:30:50 2024, max compression
```

## Comparing `pymle-diffusion-0.0.8.tar` & `pymle-diffusion-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,84 @@
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.328682 pymle-diffusion-0.0.8/
--rw-rw-rw-   0        0        0     1096 2023-01-16 00:38:30.000000 pymle-diffusion-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      851 2023-10-29 23:34:37.328682 pymle-diffusion-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5934 2023-04-14 00:21:59.000000 pymle-diffusion-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.263814 pymle-diffusion-0.0.8/pymle/
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:07.000000 pymle-diffusion-0.0.8/pymle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.266806 pymle-diffusion-0.0.8/pymle/core/
--rw-rw-rw-   0        0        0     6568 2023-09-02 18:00:29.000000 pymle-diffusion-0.0.8/pymle/core/Model.py
--rw-rw-rw-   0        0        0    11771 2023-10-29 17:37:24.000000 pymle-diffusion-0.0.8/pymle/core/TransitionDensity.py
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.272794 pymle-diffusion-0.0.8/pymle/ctmc/
--rw-rw-rw-   0        0        0     3789 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/ctmc/CTMCEstimator.py
--rw-rw-rw-   0        0        0     3905 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/ctmc/Generator1D.py
--rw-rw-rw-   0        0        0     3043 2023-04-16 00:27:35.000000 pymle-diffusion-0.0.8/pymle/ctmc/StateSpace.py
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/ctmc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.278777 pymle-diffusion-0.0.8/pymle/data/
--rw-rw-rw-   0        0        0   236026 2021-04-14 16:41:45.000000 pymle-diffusion-0.0.8/pymle/data/10yrCMrate.csv
--rw-rw-rw-   0        0        0   100149 2021-05-25 00:05:40.000000 pymle-diffusion-0.0.8/pymle/data/FX_EUR_USD.csv
--rw-rw-rw-   0        0        0   133138 2021-05-17 23:32:17.000000 pymle-diffusion-0.0.8/pymle/data/VIX.csv
--rw-rw-rw-   0        0        0        0 2023-10-29 22:23:56.000000 pymle-diffusion-0.0.8/pymle/data/__init__.py
--rw-rw-rw-   0        0        0      508 2023-04-14 00:14:06.000000 pymle-diffusion-0.0.8/pymle/data/loader.py
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.284801 pymle-diffusion-0.0.8/pymle/fit/
--rw-rw-rw-   0        0        0     2314 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/fit/AnalyticalMLE.py
--rw-rw-rw-   0        0        0     4942 2023-10-29 17:59:23.000000 pymle-diffusion-0.0.8/pymle/fit/Estimator.py
--rw-rw-rw-   0        0        0     3662 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/fit/LikelihoodEstimator.py
--rw-rw-rw-   0        0        0     3598 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/fit/Minimizer.py
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/fit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.310731 pymle-diffusion-0.0.8/pymle/models/
--rw-rw-rw-   0        0        0     3810 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/AitSahalia96.py
--rw-rw-rw-   0        0        0     1874 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/BrownianMotion.py
--rw-rw-rw-   0        0        0     3059 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/CEV.py
--rw-rw-rw-   0        0        0     5379 2023-10-29 14:18:11.000000 pymle-diffusion-0.0.8/pymle/models/CIR.py
--rw-rw-rw-   0        0        0     1084 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/CKLS.py
--rw-rw-rw-   0        0        0     3979 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/FellerRoot.py
--rw-rw-rw-   0        0        0     3512 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/GeometricBM.py
--rw-rw-rw-   0        0        0      936 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/Hyperbolic.py
--rw-rw-rw-   0        0        0     1024 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/Hyperbolic2.py
--rw-rw-rw-   0        0        0     2898 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/IGBM.py
--rw-rw-rw-   0        0        0     3848 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/Jacobi.py
--rw-rw-rw-   0        0        0     2253 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/LinearSDE1.py
--rw-rw-rw-   0        0        0     2536 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/LinearSDE2.py
--rw-rw-rw-   0        0        0     3070 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/Logistic.py
--rw-rw-rw-   0        0        0     3741 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/ModifiedCIR.py
--rw-rw-rw-   0        0        0     3250 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/NonLinearSDE.py
--rw-rw-rw-   0        0        0     2485 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/OrnsteinUhlenbeck.py
--rw-rw-rw-   0        0        0     3927 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/Pearson.py
--rw-rw-rw-   0        0        0     3465 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/PeralVerhulst.py
--rw-rw-rw-   0        0        0     3401 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/RadialOU.py
--rw-rw-rw-   0        0        0     3783 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/Threehalf.py
--rw-rw-rw-   0        0        0      924 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.313725 pymle-diffusion-0.0.8/pymle/sim/
--rw-rw-rw-   0        0        0     3877 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/sim/Simulator1D.py
--rw-rw-rw-   0        0        0     7678 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/sim/Stepper.py
--rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.8/pymle/sim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.320706 pymle-diffusion-0.0.8/pymle_diffusion.egg-info/
--rw-rw-rw-   0        0        0      851 2023-10-29 23:34:37.000000 pymle-diffusion-0.0.8/pymle_diffusion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2023-10-29 23:34:37.000000 pymle-diffusion-0.0.8/pymle_diffusion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-29 23:34:37.000000 pymle-diffusion-0.0.8/pymle_diffusion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-29 23:34:37.000000 pymle-diffusion-0.0.8/pymle_diffusion.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       44 2023-10-29 23:34:37.000000 pymle-diffusion-0.0.8/pymle_diffusion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-10-29 23:34:37.000000 pymle-diffusion-0.0.8/pymle_diffusion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-04-14 22:19:45.000000 pymle-diffusion-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      179 2023-10-29 23:34:37.329681 pymle-diffusion-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1122 2023-10-29 23:34:34.000000 pymle-diffusion-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.322701 pymle-diffusion-0.0.8/tests/
--rw-rw-rw-   0        0        0        0 2023-10-29 23:33:18.000000 pymle-diffusion-0.0.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.324695 pymle-diffusion-0.0.8/tests/fit/
--rw-rw-rw-   0        0        0     3929 2023-03-10 16:44:26.000000 pymle-diffusion-0.0.8/tests/fit/Test_AnalyticalMLE.py
--rw-rw-rw-   0        0        0        0 2023-01-01 00:52:35.000000 pymle-diffusion-0.0.8/tests/fit/__init__.py
--rw-rw-rw-   0        0        0      361 2023-01-01 00:53:32.000000 pymle-diffusion-0.0.8/tests/fit/suite.py
-drwxrwxrwx   0        0        0        0 2023-10-29 23:34:37.327689 pymle-diffusion-0.0.8/tests/models/
--rw-rw-rw-   0        0        0      658 2023-01-01 00:51:44.000000 pymle-diffusion-0.0.8/tests/models/Test_CEV.py
--rw-rw-rw-   0        0        0        0 2022-12-31 23:16:13.000000 pymle-diffusion-0.0.8/tests/models/__init__.py
--rw-rw-rw-   0        0        0      334 2022-12-31 23:17:37.000000 pymle-diffusion-0.0.8/tests/models/suite.py
--rw-rw-rw-   0        0        0      415 2023-01-01 00:54:06.000000 pymle-diffusion-0.0.8/tests/test_runner.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.489388 pymle-diffusion-0.0.9/
+-rw-rw-rw-   0        0        0       70 2023-04-13 23:55:37.000000 pymle-diffusion-0.0.9/.gitignore
+-rw-rw-rw-   0        0        0     1096 2023-01-16 00:38:30.000000 pymle-diffusion-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      718 2024-05-12 16:30:50.489388 pymle-diffusion-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5934 2023-04-14 00:21:59.000000 pymle-diffusion-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.417322 pymle-diffusion-0.0.9/examples/
+-rw-rw-rw-   0        0        0     2894 2023-03-10 16:44:26.000000 pymle-diffusion-0.0.9/examples/Example_CIR_MLE.py
+-rw-rw-rw-   0        0        0     3570 2024-05-12 16:27:54.000000 pymle-diffusion-0.0.9/examples/Example_TimeDependent_MLE.py
+-rw-rw-rw-   0        0        0     3470 2023-10-29 17:26:57.000000 pymle-diffusion-0.0.9/examples/RealDataExample_CIR_Fit_Interest.py
+-rw-rw-rw-   0        0        0     2537 2023-04-14 00:18:54.000000 pymle-diffusion-0.0.9/examples/RealDataExample_CKLS_Fit_Interest.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.418321 pymle-diffusion-0.0.9/pymle/
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:07.000000 pymle-diffusion-0.0.9/pymle/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.421364 pymle-diffusion-0.0.9/pymle/core/
+-rw-rw-rw-   0        0        0     7174 2024-05-12 16:09:15.000000 pymle-diffusion-0.0.9/pymle/core/Model.py
+-rw-rw-rw-   0        0        0    12781 2024-05-12 16:20:49.000000 pymle-diffusion-0.0.9/pymle/core/TransitionDensity.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.424419 pymle-diffusion-0.0.9/pymle/ctmc/
+-rw-rw-rw-   0        0        0     3789 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/ctmc/CTMCEstimator.py
+-rw-rw-rw-   0        0        0     3905 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/ctmc/Generator1D.py
+-rw-rw-rw-   0        0        0     3043 2023-04-16 00:27:35.000000 pymle-diffusion-0.0.9/pymle/ctmc/StateSpace.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/ctmc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.425653 pymle-diffusion-0.0.9/pymle/ctmc/utility/
+-rw-rw-rw-   0        0        0        0 2021-04-11 22:51:41.000000 pymle-diffusion-0.0.9/pymle/ctmc/utility/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.431339 pymle-diffusion-0.0.9/pymle/data/
+-rw-rw-rw-   0        0        0   236026 2021-04-14 16:41:45.000000 pymle-diffusion-0.0.9/pymle/data/10yrCMrate.csv
+-rw-rw-rw-   0        0        0   100149 2021-05-25 00:05:40.000000 pymle-diffusion-0.0.9/pymle/data/FX_EUR_USD.csv
+-rw-rw-rw-   0        0        0   133138 2021-05-17 23:32:17.000000 pymle-diffusion-0.0.9/pymle/data/VIX.csv
+-rw-rw-rw-   0        0        0        0 2023-10-29 22:23:56.000000 pymle-diffusion-0.0.9/pymle/data/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-04-14 00:14:06.000000 pymle-diffusion-0.0.9/pymle/data/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.437078 pymle-diffusion-0.0.9/pymle/fit/
+-rw-rw-rw-   0        0        0     2314 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/fit/AnalyticalMLE.py
+-rw-rw-rw-   0        0        0     4979 2023-10-31 00:05:02.000000 pymle-diffusion-0.0.9/pymle/fit/Estimator.py
+-rw-rw-rw-   0        0        0     3662 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/fit/LikelihoodEstimator.py
+-rw-rw-rw-   0        0        0     3598 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/fit/Minimizer.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/fit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.467815 pymle-diffusion-0.0.9/pymle/models/
+-rw-rw-rw-   0        0        0     3810 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/AitSahalia96.py
+-rw-rw-rw-   0        0        0     3866 2024-05-12 16:09:15.000000 pymle-diffusion-0.0.9/pymle/models/BrownianMotion.py
+-rw-rw-rw-   0        0        0     3059 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/CEV.py
+-rw-rw-rw-   0        0        0     5379 2023-10-29 14:18:11.000000 pymle-diffusion-0.0.9/pymle/models/CIR.py
+-rw-rw-rw-   0        0        0     3428 2024-05-08 19:04:39.000000 pymle-diffusion-0.0.9/pymle/models/CKLS.py
+-rw-rw-rw-   0        0        0     3979 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/FellerRoot.py
+-rw-rw-rw-   0        0        0     3512 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/GeometricBM.py
+-rw-rw-rw-   0        0        0      963 2024-05-12 16:09:15.000000 pymle-diffusion-0.0.9/pymle/models/Hyperbolic.py
+-rw-rw-rw-   0        0        0     1051 2024-05-12 16:09:15.000000 pymle-diffusion-0.0.9/pymle/models/Hyperbolic2.py
+-rw-rw-rw-   0        0        0     2898 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/IGBM.py
+-rw-rw-rw-   0        0        0     3848 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/Jacobi.py
+-rw-rw-rw-   0        0        0     2253 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/LinearSDE1.py
+-rw-rw-rw-   0        0        0     2536 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/LinearSDE2.py
+-rw-rw-rw-   0        0        0     3070 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/Logistic.py
+-rw-rw-rw-   0        0        0     3741 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/ModifiedCIR.py
+-rw-rw-rw-   0        0        0     3250 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/NonLinearSDE.py
+-rw-rw-rw-   0        0        0     2485 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/OrnsteinUhlenbeck.py
+-rw-rw-rw-   0        0        0     3927 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/Pearson.py
+-rw-rw-rw-   0        0        0     3465 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/PeralVerhulst.py
+-rw-rw-rw-   0        0        0     3405 2024-05-12 16:09:15.000000 pymle-diffusion-0.0.9/pymle/models/RadialOU.py
+-rw-rw-rw-   0        0        0     3783 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/Threehalf.py
+-rw-rw-rw-   0        0        0      924 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.473789 pymle-diffusion-0.0.9/pymle/sim/
+-rw-rw-rw-   0        0        0     3877 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/sim/Simulator1D.py
+-rw-rw-rw-   0        0        0     7678 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/sim/Stepper.py
+-rw-rw-rw-   0        0        0        0 2023-04-01 23:54:17.000000 pymle-diffusion-0.0.9/pymle/sim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.479884 pymle-diffusion-0.0.9/pymle_diffusion.egg-info/
+-rw-rw-rw-   0        0        0      718 2024-05-12 16:30:50.000000 pymle-diffusion-0.0.9/pymle_diffusion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1764 2024-05-12 16:30:50.000000 pymle-diffusion-0.0.9/pymle_diffusion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:30:50.000000 pymle-diffusion-0.0.9/pymle_diffusion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-12 16:30:50.000000 pymle-diffusion-0.0.9/pymle_diffusion.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2024-05-12 16:30:50.000000 pymle-diffusion-0.0.9/pymle_diffusion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-12 16:30:50.000000 pymle-diffusion-0.0.9/pymle_diffusion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-04-14 22:19:45.000000 pymle-diffusion-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      113 2023-04-14 00:01:59.000000 pymle-diffusion-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0      179 2024-05-12 16:30:50.490549 pymle-diffusion-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1122 2024-05-12 15:40:05.000000 pymle-diffusion-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.482159 pymle-diffusion-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-29 23:33:18.000000 pymle-diffusion-0.0.9/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.484208 pymle-diffusion-0.0.9/tests/fit/
+-rw-rw-rw-   0        0        0     3929 2023-03-10 16:44:26.000000 pymle-diffusion-0.0.9/tests/fit/Test_AnalyticalMLE.py
+-rw-rw-rw-   0        0        0        0 2023-01-01 00:52:35.000000 pymle-diffusion-0.0.9/tests/fit/__init__.py
+-rw-rw-rw-   0        0        0      361 2023-01-01 00:53:32.000000 pymle-diffusion-0.0.9/tests/fit/suite.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:30:50.488386 pymle-diffusion-0.0.9/tests/models/
+-rw-rw-rw-   0        0        0      658 2023-01-01 00:51:44.000000 pymle-diffusion-0.0.9/tests/models/Test_CEV.py
+-rw-rw-rw-   0        0        0        0 2022-12-31 23:16:13.000000 pymle-diffusion-0.0.9/tests/models/__init__.py
+-rw-rw-rw-   0        0        0      334 2022-12-31 23:17:37.000000 pymle-diffusion-0.0.9/tests/models/suite.py
+-rw-rw-rw-   0        0        0      415 2023-01-01 00:54:06.000000 pymle-diffusion-0.0.9/tests/test_runner.py
```

### Comparing `pymle-diffusion-0.0.8/LICENSE` & `pymle-diffusion-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/README.md` & `pymle-diffusion-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/core/Model.py` & `pymle-diffusion-0.0.9/pymle/core/Model.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,32 @@
 from abc import ABC, abstractmethod
 import numpy as np
 
 
 class Model1D(ABC):
     def __init__(self,
                  has_exact_density: bool = False,
-                 default_sim_method: str = "Milstein"):
+                 default_sim_method: str = "Milstein",
+                 has_constant_diffusion: bool = False):
         """
         Base 1D model for SDE, defined by
 
         dX(t) = mu(X,t)dt + sigma(X,t)dW_t
 
         :param has_exact_density: bool, set to true if an exact density is implemented
         :param default_sim_method: str, the default method for simulating. This can be overriden by simulator,
             but this allows you to set a good default (or perhaps exact method) per model
+        :param has_constant_diffusion: bool, override to True to indicate the model has a constant diffusion coefficent.
+            Some estimation methods, like Ozaki and Shoji-Ozaki, are not designed for non-constant diffusion coefficents
+            and will produce a warning if applied in such cases
         """
         self._has_exact_density = has_exact_density
         self._params: Optional[np.ndarray] = None  # model parameters
         self._positive = False  # updated when params are set, indicates positivity of process
+        self._constant_diffusion = has_constant_diffusion
         self._default_sim_method = default_sim_method
 
         # Numerical derivative parameters
         self.h_x = 1e-05  # Controls the finite difference stepsize for first derivatives in x variable
         self.h_xx = 1e-05  # Controls the finite difference stepsize for second derivatives in x variable
         self.h_t = 1e-05  # Controls the finite difference stepsize for first derivatives in t variable
 
@@ -60,14 +65,19 @@
     # ==============================
 
     @property
     def has_exact_density(self) -> bool:
         """ Return true if model has an exact density implemented """
         return self._has_exact_density
 
+    @property
+    def has_constant_diffusion_coefficient(self) -> bool:
+        """ Return true if model has a constant diffusion coefficient """
+        return self._positive
+
     def exact_density(self, x0: float, xt: float, t0: float, dt: float) -> float:
         """
         In the case where the exact transition density,
         P(Xt, t | X0) is known, override this method
         :param x0: float, the current value
         :param xt: float, the value to transition to
         :param t0: float, the time of observing x0
```

### Comparing `pymle-diffusion-0.0.8/pymle/core/TransitionDensity.py` & `pymle-diffusion-0.0.9/pymle/core/TransitionDensity.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,19 @@
 class OzakiDensity(TransitionDensity):
     def __init__(self, model: Model1D):
         """
         Class which represents the Ozaki approximation transition density for a model
         :param model: the SDE model, referenced during calls to the transition density
         """
         super().__init__(model=model)
+        if not model.has_constant_diffusion_coefficient:
+            print(f"Warning: the Ozaki density approximation assumes a constant diffusion coefficient, but this model"
+                  f"does not satisfy that requirement. The approximation will be thus based on the value of the "
+                  f"diffusion at the initial time and x values. Consider first applying the Lamperti transform"
+                  f" to the model to convert the diffusion coefficient to a constant (one).")
 
     def __call__(self,
                  x0: Union[float, np.ndarray],
                  xt: Union[float, np.ndarray],
                  t0: Union[float, np.ndarray],
                  dt: float) -> Union[float, np.ndarray]:
         """
@@ -123,25 +128,30 @@
 class ShojiOzakiDensity(TransitionDensity):
     def __init__(self, model: Model1D):
         """
         Class which represents the Shoji-Ozaki approximation transition density for a model
         :param model: the SDE model, referenced during calls to the transition density
         """
         super().__init__(model=model)
+        if not model.has_constant_diffusion_coefficient:
+            print(f"Warning: the Shoji-Ozaki density approximation assumes a constant diffusion coefficient, but this "
+                  f"model does not satisfy that requirement. The approximation will be thus based on the value of the "
+                  f"diffusion at the initial time and x values. Consider first applying the Lamperti transform"
+                  f" to the model to convert the diffusion coefficient to a constant (one).")
 
     def __call__(self,
                  x0: Union[float, np.ndarray],
                  xt: Union[float, np.ndarray],
                  t0: Union[float, np.ndarray],
                  dt: float) -> Union[float, np.ndarray]:
         """
         The transition density obtained via Shoji-Ozaki expansion
         :param x0: float or array, the current value
         :param xt: float or array, the value to transition to  (must be same dimension as x0)
-        :param t0: float, the time of at which to evalate the coefficients. Irrelevant For time inhomogenous models
+        :param t0: float, the time of at which to evaluate the coefficients. Irrelevant For time inhomogenous models
         :param dt: float, the time step between x0 and xt
         :return: probability (same dimension as x0 and xt)
         """
         sig = self._model.diffusion(x0, t0)
         mu = self._model.drift(x0, t0)
 
         Mt = 0.5 * sig ** 2 * self._model.drift_xx(x0, t0) + self._model.drift_t(x0, t0)
```

### Comparing `pymle-diffusion-0.0.8/pymle/ctmc/CTMCEstimator.py` & `pymle-diffusion-0.0.9/pymle/ctmc/CTMCEstimator.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/ctmc/Generator1D.py` & `pymle-diffusion-0.0.9/pymle/ctmc/Generator1D.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/ctmc/StateSpace.py` & `pymle-diffusion-0.0.9/pymle/ctmc/StateSpace.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/data/10yrCMrate.csv` & `pymle-diffusion-0.0.9/pymle/data/10yrCMrate.csv`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/data/FX_EUR_USD.csv` & `pymle-diffusion-0.0.9/pymle/data/FX_EUR_USD.csv`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/data/VIX.csv` & `pymle-diffusion-0.0.9/pymle/data/VIX.csv`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/fit/AnalyticalMLE.py` & `pymle-diffusion-0.0.9/pymle/fit/AnalyticalMLE.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/fit/Estimator.py` & `pymle-diffusion-0.0.9/pymle/fit/Estimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import ABC
+from abc import ABC, abstractmethod
 import numpy as np
 from typing import List, Tuple, Union
 
 from pymle.core.Model import Model1D
 
 
 class EstimatedResult(object):
@@ -97,14 +97,15 @@
 
         if isinstance(t0, np.ndarray):
             if len(t0) != len(sample) - 1:
                 raise ValueError("If you supply a sequence of t0, it must be the same size as the sample - 1")
             if len(t0.shape) != len(self._sample.shape):
                 raise ValueError("The second dimension of the t0 and sample vectors must agree, should be 1")
 
+    @abstractmethod
     def estimate_params(self, params0: np.ndarray) -> EstimatedResult:
         """
         Main estimation function
         :param params0: array, the initial guess params
         :return: result, the estimated params and final likelihood
         """
         raise NotImplementedError
```

### Comparing `pymle-diffusion-0.0.8/pymle/fit/LikelihoodEstimator.py` & `pymle-diffusion-0.0.9/pymle/fit/LikelihoodEstimator.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/fit/Minimizer.py` & `pymle-diffusion-0.0.9/pymle/fit/Minimizer.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/AitSahalia96.py` & `pymle-diffusion-0.0.9/pymle/models/AitSahalia96.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/BrownianMotion.py` & `pymle-diffusion-0.0.9/pymle/models/Hyperbolic2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,33 @@
 from typing import Union
 import numpy as np
-from scipy.stats import norm
+
 from pymle.core.Model import Model1D
 
 
-class BrownianMotion(Model1D):
+class Hyperbolic2(Model1D):
     """
-    Model for (drifted) Brownian Motion
-    Parameters:  [mu, sigma]
+    Model for Hyperbolic process II
+    Parameters: [beta,gamma,delta,mu,sigma]
 
-    dX(t) = mu(X,t)dt + sigma(X,t)dW_t
+    dX(t) = mu(X,t)*dt + sigma(X,t)*dW_t
 
     where:
-        mu(X,t)    = mu   (constant)
-        sigma(X,t) = sigma   (constant, >0)
+        mu(X,t)    = sigma**2/2(beta-gamma*X/sqrt(delta**2+(X-mu)))
+        sigma(X,t) = sigma
     """
 
     def __init__(self):
-        super().__init__(has_exact_density=True, default_sim_method='Exact')
+        super().__init__(has_constant_diffusion=True)
 
     def drift(self, x: Union[float, np.ndarray], t: float) -> Union[float, np.ndarray]:
-        return self._params[0] * (x > -10000)  # todo: reshape?
+        return self._params[4]**2/2*(self._params[0]-self._params[1]*x/np.sqrt(self._params[2]**2+(x-self._params[3])**2))
 
     def diffusion(self, x: Union[float, np.ndarray], t: float) -> Union[float, np.ndarray]:
-        return self._params[1] * (x > -10000)
-
-    def exact_density(self, x0: float, xt: float, t0: float, dt: float) -> float:
-        mu, sigma = self._params
-        mean_ = x0 + mu * dt
-        return norm.pdf(xt, loc=mean_, scale=sigma * np.sqrt(dt))
-
-    def exact_step(self,
-                   t: float,
-                   dt: float,
-                   x: Union[float, np.ndarray],
-                   dZ: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
-        """ Simple Brownian motion can be simulated exactly """
-        sig_sq_dt = self._params[1] * np.sqrt(dt)
-        return x + self._params[0] * dt + sig_sq_dt * dZ
+        return self._params[4]
 
     # =======================
     # (Optional) Overrides for numerical derivatives to improve performance
     # =======================
 
     def drift_t(self, x: Union[float, np.ndarray], t: float) -> Union[float, np.ndarray]:
         return 0.
-
-    def diffusion_x(self, x: Union[float, np.ndarray], t: float) -> Union[float, np.ndarray]:
-        return 0.
-
-    def diffusion_xx(self, x: Union[float, np.ndarray], t: float) -> Union[float, np.ndarray]:
-        return 0.
```

### Comparing `pymle-diffusion-0.0.8/pymle/models/CEV.py` & `pymle-diffusion-0.0.9/pymle/models/CEV.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/CIR.py` & `pymle-diffusion-0.0.9/pymle/models/CIR.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/FellerRoot.py` & `pymle-diffusion-0.0.9/pymle/models/FellerRoot.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/GeometricBM.py` & `pymle-diffusion-0.0.9/pymle/models/GeometricBM.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/Hyperbolic.py` & `pymle-diffusion-0.0.9/pymle/models/Hyperbolic.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     where:
         mu(X,t)    = -kappa*X / sqrt(1 + X^2)
         sigma(X,t) = sigma
     """
 
     def __init__(self):
-        super().__init__()
+        super().__init__(has_constant_diffusion=True)
 
     def drift(self, x: Union[float, np.ndarray], t: float) -> Union[float, np.ndarray]:
         return -self._params[0] * x / (np.sqrt(1 + x * x))
 
     def diffusion(self, x: Union[float, np.ndarray], t: float) -> Union[float, np.ndarray]:
         return self._params[1] * (x > -10000)
```

### Comparing `pymle-diffusion-0.0.8/pymle/models/IGBM.py` & `pymle-diffusion-0.0.9/pymle/models/IGBM.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/Jacobi.py` & `pymle-diffusion-0.0.9/pymle/models/Jacobi.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/LinearSDE1.py` & `pymle-diffusion-0.0.9/pymle/models/LinearSDE1.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/LinearSDE2.py` & `pymle-diffusion-0.0.9/pymle/models/LinearSDE2.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/Logistic.py` & `pymle-diffusion-0.0.9/pymle/models/Logistic.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/ModifiedCIR.py` & `pymle-diffusion-0.0.9/pymle/models/ModifiedCIR.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/NonLinearSDE.py` & `pymle-diffusion-0.0.9/pymle/models/NonLinearSDE.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/OrnsteinUhlenbeck.py` & `pymle-diffusion-0.0.9/pymle/models/OrnsteinUhlenbeck.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/Pearson.py` & `pymle-diffusion-0.0.9/pymle/models/Pearson.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/PeralVerhulst.py` & `pymle-diffusion-0.0.9/pymle/models/PeralVerhulst.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/RadialOU.py` & `pymle-diffusion-0.0.9/pymle/models/RadialOU.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     where:
         mu(X,t)    = kappa / X - X
         sigma(X,t) = sigma
     """
 
     def __init__(self):
-        super().__init__(has_exact_density=False)
+        super().__init__(has_constant_diffusion=True)
 
     def drift(self, x: Union[float, np.ndarray], t: float) -> Union[float, np.ndarray]:
         return self._params[0] / x - x
 
     def diffusion(self, x: Union[float, np.ndarray], t: float) -> Union[float, np.ndarray]:
         return self._params[1]
```

### Comparing `pymle-diffusion-0.0.8/pymle/models/Threehalf.py` & `pymle-diffusion-0.0.9/pymle/models/Threehalf.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/models/__init__.py` & `pymle-diffusion-0.0.9/pymle/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/sim/Simulator1D.py` & `pymle-diffusion-0.0.9/pymle/sim/Simulator1D.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle/sim/Stepper.py` & `pymle-diffusion-0.0.9/pymle/sim/Stepper.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/pymle_diffusion.egg-info/SOURCES.txt` & `pymle-diffusion-0.0.9/pymle_diffusion.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,27 @@
+.gitignore
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
 setup.cfg
 setup.py
+examples/Example_CIR_MLE.py
+examples/Example_TimeDependent_MLE.py
+examples/RealDataExample_CIR_Fit_Interest.py
+examples/RealDataExample_CKLS_Fit_Interest.py
 pymle/__init__.py
 pymle/core/Model.py
 pymle/core/TransitionDensity.py
 pymle/core/__init__.py
 pymle/ctmc/CTMCEstimator.py
 pymle/ctmc/Generator1D.py
 pymle/ctmc/StateSpace.py
 pymle/ctmc/__init__.py
+pymle/ctmc/utility/__init__.py
 pymle/data/10yrCMrate.csv
 pymle/data/FX_EUR_USD.csv
 pymle/data/VIX.csv
 pymle/data/__init__.py
 pymle/data/loader.py
 pymle/fit/AnalyticalMLE.py
 pymle/fit/Estimator.py
```

### Comparing `pymle-diffusion-0.0.8/setup.py` & `pymle-diffusion-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name='pymle-diffusion',
-      version='0.0.8',
+      version='0.0.9',
       description='Maximum Likelihood Estimation (MLE) and simulation for SDE',
       long_description='Maximum Likelihood Estimation (MLE) and simulation for '
                        'Stochastic Differential Equations (SDE)',
       classifiers=[
           'Development Status :: 3 - Alpha',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3.7',
```

### Comparing `pymle-diffusion-0.0.8/tests/fit/Test_AnalyticalMLE.py` & `pymle-diffusion-0.0.9/tests/fit/Test_AnalyticalMLE.py`

 * *Files identical despite different names*

### Comparing `pymle-diffusion-0.0.8/tests/models/Test_CEV.py` & `pymle-diffusion-0.0.9/tests/models/Test_CEV.py`

 * *Files identical despite different names*

