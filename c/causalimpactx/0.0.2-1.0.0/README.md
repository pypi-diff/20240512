# Comparing `tmp/causalimpactx-0.0.2.tar.gz` & `tmp/causalimpactx-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causalimpactx-0.0.2.tar", last modified: Thu Apr  4 16:01:08 2024, max compression
+gzip compressed data, was "causalimpactx-1.0.0.tar", last modified: Sun May 12 19:36:06 2024, max compression
```

## Comparing `causalimpactx-0.0.2.tar` & `causalimpactx-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-04 16:01:08.767597 causalimpactx-0.0.2/
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)       99 2024-03-31 13:45:19.000000 causalimpactx-0.0.2/AUTHORS.md
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)    10947 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/LICENSE.md
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2723 2024-04-04 16:01:08.767597 causalimpactx-0.0.2/PKG-INFO
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2001 2024-03-31 19:14:32.000000 causalimpactx-0.0.2/README.md
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)      785 2024-04-04 15:59:58.000000 causalimpactx-0.0.2/pyproject.toml
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)       38 2024-04-04 16:01:08.767597 causalimpactx-0.0.2/setup.cfg
-drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-04 16:01:08.765597 causalimpactx-0.0.2/src/
-drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-04 16:01:08.765597 causalimpactx-0.0.2/src/causalimpactx/
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)      864 2024-04-02 19:50:56.000000 causalimpactx-0.0.2/src/causalimpactx/__init__.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)    37197 2024-04-03 23:52:23.000000 causalimpactx-0.0.2/src/causalimpactx/analysis.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     4870 2024-04-03 19:25:15.000000 causalimpactx-0.0.2/src/causalimpactx/inferences.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     1936 2024-04-02 19:51:47.000000 causalimpactx-0.0.2/src/causalimpactx/misc.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     7780 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/src/causalimpactx/model.py
-drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-04 16:01:08.766597 causalimpactx-0.0.2/src/causalimpactx.egg-info/
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2723 2024-04-04 16:01:08.000000 causalimpactx-0.0.2/src/causalimpactx.egg-info/PKG-INFO
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)      482 2024-04-04 16:01:08.000000 causalimpactx-0.0.2/src/causalimpactx.egg-info/SOURCES.txt
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)        1 2024-04-04 16:01:08.000000 causalimpactx-0.0.2/src/causalimpactx.egg-info/dependency_links.txt
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)       45 2024-04-04 16:01:08.000000 causalimpactx-0.0.2/src/causalimpactx.egg-info/requires.txt
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)       14 2024-04-04 16:01:08.000000 causalimpactx-0.0.2/src/causalimpactx.egg-info/top_level.txt
-drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-04-04 16:01:08.766597 causalimpactx-0.0.2/tests/
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)    35198 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/tests/test_analysis.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)    10560 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/tests/test_inferences.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2540 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/tests/test_misc.py
--rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2728 2024-03-29 08:05:54.000000 causalimpactx-0.0.2/tests/test_model.py
+drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-05-12 19:36:06.414349 causalimpactx-1.0.0/
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)       99 2024-03-31 13:45:19.000000 causalimpactx-1.0.0/AUTHORS.md
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)    10947 2024-03-29 08:05:54.000000 causalimpactx-1.0.0/LICENSE.md
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2723 2024-05-12 19:36:06.413349 causalimpactx-1.0.0/PKG-INFO
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2001 2024-03-31 19:14:32.000000 causalimpactx-1.0.0/README.md
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)      785 2024-05-12 19:29:09.000000 causalimpactx-1.0.0/pyproject.toml
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)       38 2024-05-12 19:36:06.414349 causalimpactx-1.0.0/setup.cfg
+drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-05-12 19:36:06.404349 causalimpactx-1.0.0/src/
+drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-05-12 19:36:06.410349 causalimpactx-1.0.0/src/causalimpactx/
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)      864 2024-04-02 19:50:56.000000 causalimpactx-1.0.0/src/causalimpactx/__init__.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)    37203 2024-04-10 21:53:25.000000 causalimpactx-1.0.0/src/causalimpactx/analysis.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     4870 2024-04-03 19:25:15.000000 causalimpactx-1.0.0/src/causalimpactx/inferences.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     1946 2024-05-12 19:15:47.000000 causalimpactx-1.0.0/src/causalimpactx/misc.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     7780 2024-03-29 08:05:54.000000 causalimpactx-1.0.0/src/causalimpactx/model.py
+drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-05-12 19:36:06.412349 causalimpactx-1.0.0/src/causalimpactx.egg-info/
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2723 2024-05-12 19:36:06.000000 causalimpactx-1.0.0/src/causalimpactx.egg-info/PKG-INFO
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)      482 2024-05-12 19:36:06.000000 causalimpactx-1.0.0/src/causalimpactx.egg-info/SOURCES.txt
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)        1 2024-05-12 19:36:06.000000 causalimpactx-1.0.0/src/causalimpactx.egg-info/dependency_links.txt
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)       45 2024-05-12 19:36:06.000000 causalimpactx-1.0.0/src/causalimpactx.egg-info/requires.txt
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)       14 2024-05-12 19:36:06.000000 causalimpactx-1.0.0/src/causalimpactx.egg-info/top_level.txt
+drwxr-xr-x   0 yaseen    (1000) yaseen    (1000)        0 2024-05-12 19:36:06.411349 causalimpactx-1.0.0/tests/
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)    35198 2024-03-29 08:05:54.000000 causalimpactx-1.0.0/tests/test_analysis.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)    10560 2024-03-29 08:05:54.000000 causalimpactx-1.0.0/tests/test_inferences.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2540 2024-03-29 08:05:54.000000 causalimpactx-1.0.0/tests/test_misc.py
+-rw-r--r--   0 yaseen    (1000) yaseen    (1000)     2728 2024-03-29 08:05:54.000000 causalimpactx-1.0.0/tests/test_model.py
```

### Comparing `causalimpactx-0.0.2/LICENSE.md` & `causalimpactx-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.2/PKG-INFO` & `causalimpactx-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalimpactx
-Version: 0.0.2
+Version: 1.0.0
 Summary: A clone of R version CausalImpact developed by Google
 Author-email: Yaseen Esmaeelpour <yaseenes@gmail.com>
 Project-URL: Homepage, https://github.com/yaseenesmaeelpour/causalimpactx
 Project-URL: Issues, https://github.com/yaseenesmaeelpour/causalimpactx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `causalimpactx-0.0.2/README.md` & `causalimpactx-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.2/pyproject.toml` & `causalimpactx-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # AVOID CHANGING REQUIRES: IT WILL BE UPDATED BY PYSCAFFOLD!
 requires = ["setuptools>=46.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "causalimpactx"
-version = "0.0.2"
+version = "1.0.0"
 authors = [
   { name="Yaseen Esmaeelpour", email="yaseenes@gmail.com" },
 ]
 description = "A clone of R version CausalImpact developed by Google"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `causalimpactx-0.0.2/src/causalimpactx/__init__.py` & `causalimpactx-1.0.0/src/causalimpactx/__init__.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.2/src/causalimpactx/analysis.py` & `causalimpactx-1.0.0/src/causalimpactx/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -880,16 +880,16 @@
             data_inter = pd.Timestamp(data_inter)
 
         inferences = self.inferences.iloc[1:, :]
 
         # Observation and regression components
         if "original" in panels:
             ax1 = plt.subplot(3, 1, 1)
-            plt.plot(inferences.point_pred, "r--", linewidth=2, label="model")
-            plt.plot(inferences.response, "k", linewidth=2, label="endog")
+            plt.plot(inferences.point_pred, "r--", linewidth=2, label="Prediction")
+            plt.plot(inferences.response, "k", linewidth=2, label="Actual")
 
             plt.axvline(data_inter, c="k", linestyle="--")
 
             plt.fill_between(
                 inferences.index,
                 inferences.point_pred_lower,
                 inferences.point_pred_upper,
```

### Comparing `causalimpactx-0.0.2/src/causalimpactx/inferences.py` & `causalimpactx-1.0.0/src/causalimpactx/inferences.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.2/src/causalimpactx/misc.py` & `causalimpactx-1.0.0/src/causalimpactx/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
     data_mu = data.loc[pre_period[0] : pre_period[1], :].mean(skipna=True)
     data_sd = data.loc[pre_period[0] : pre_period[1], :].std(skipna=True, ddof=0)
     data = data - data_mu
     data_sd = data_sd.fillna(1)
 
     data[data != 0] = data[data != 0] / data_sd
-    y_mu = data_mu[0]
-    y_sd = data_sd[0]
+    y_mu = data_mu.iloc[0]
+    y_sd = data_sd.iloc[0]
 
     data_pre = data.loc[pre_period[0] : pre_period[1], :]
     data_post = data.loc[post_period[0] : post_period[1], :]
 
     return {
         "data_pre": data_pre,
         "data_post": data_post,
```

### Comparing `causalimpactx-0.0.2/src/causalimpactx/model.py` & `causalimpactx-1.0.0/src/causalimpactx/model.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.2/src/causalimpactx.egg-info/PKG-INFO` & `causalimpactx-1.0.0/src/causalimpactx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causalimpactx
-Version: 0.0.2
+Version: 1.0.0
 Summary: A clone of R version CausalImpact developed by Google
 Author-email: Yaseen Esmaeelpour <yaseenes@gmail.com>
 Project-URL: Homepage, https://github.com/yaseenesmaeelpour/causalimpactx
 Project-URL: Issues, https://github.com/yaseenesmaeelpour/causalimpactx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `causalimpactx-0.0.2/tests/test_analysis.py` & `causalimpactx-1.0.0/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.2/tests/test_inferences.py` & `causalimpactx-1.0.0/tests/test_inferences.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.2/tests/test_misc.py` & `causalimpactx-1.0.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `causalimpactx-0.0.2/tests/test_model.py` & `causalimpactx-1.0.0/tests/test_model.py`

 * *Files identical despite different names*

