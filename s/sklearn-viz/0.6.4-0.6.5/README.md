# Comparing `tmp/sklearn_viz-0.6.4.tar.gz` & `tmp/sklearn_viz-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.6.4.tar", max compression
+gzip compressed data, was "sklearn_viz-0.6.5.tar", max compression
```

## Comparing `sklearn_viz-0.6.4.tar` & `sklearn_viz-0.6.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2024-05-11 06:16:51.563821 sklearn_viz-0.6.4/LICENSE
--rw-r--r--   0        0        0      354 2024-05-11 06:16:51.563821 sklearn_viz-0.6.4/README.md
--rw-r--r--   0        0        0      165 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0        0 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/components/__init__.py
--rw-r--r--   0        0        0     5912 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/components/estimators.py
--rw-r--r--   0        0        0      811 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/components/kfold.py
--rw-r--r--   0        0        0      329 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     8306 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4633 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2403 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16590 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      643 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      129 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0    12455 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/cross_validation.py
--rw-r--r--   0        0        0     6079 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1572 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    13742 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2497 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      508 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       21 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     4377 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0      544 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/utils/file.py
--rw-r--r--   0        0        0     3033 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/utils/plotly.py
--rw-r--r--   0        0        0     3111 2024-05-11 06:16:51.567821 sklearn_viz-0.6.4/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0      977 2024-05-11 06:16:51.571821 sklearn_viz-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 sklearn_viz-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-12 00:10:09.595038 sklearn_viz-0.6.5/LICENSE
+-rw-r--r--   0        0        0      354 2024-05-12 00:10:09.595038 sklearn_viz-0.6.5/README.md
+-rw-r--r--   0        0        0      165 2024-05-12 00:10:09.595038 sklearn_viz-0.6.5/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 00:10:09.595038 sklearn_viz-0.6.5/elphick/sklearn_viz/components/__init__.py
+-rw-r--r--   0        0        0     5912 2024-05-12 00:10:09.595038 sklearn_viz-0.6.5/elphick/sklearn_viz/components/estimators.py
+-rw-r--r--   0        0        0      811 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/components/kfold.py
+-rw-r--r--   0        0        0      329 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     8306 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4633 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2403 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16590 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      643 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      129 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0    12454 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/cross_validation.py
+-rw-r--r--   0        0        0    14149 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1572 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    13742 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2497 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      508 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       21 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     4377 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0      544 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/utils/file.py
+-rw-r--r--   0        0        0     3033 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/utils/plotly.py
+-rw-r--r--   0        0        0     3111 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0      977 2024-05-12 00:10:09.599038 sklearn_viz-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 sklearn_viz-0.6.5/PKG-INFO
```

### Comparing `sklearn_viz-0.6.4/LICENSE` & `sklearn_viz-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/components/estimators.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/components/estimators.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/components/kfold.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/components/kfold.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/features/importance.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/features/importance.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/features/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/features/principal_components.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/cross_validation.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/cross_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,20 +232,20 @@
         by_group_metric_chunks: list = []
         for grp in self.group.unique():
             grp_index: pd.Index = self.group.loc[self.group == grp].index
             x: pd.DataFrame = self.datasets[dataset][self.features_in].loc[grp_index]
             y: pd.DataFrame = self.datasets[dataset][self.target].loc[grp_index]
             if self.pre_processor:
                 x = self.pre_processor.set_output(transform="pandas").fit_transform(X=x)
+            cv = self.cv
             if isinstance(self.cv, int):
                 cv = KFold(n_splits=self.cv, random_state=self.random_state, shuffle=True)
-            else:
-                cv = self.cv
+
             res = cross_validate(self.estimators[estimator], x, y, cv=cv, scoring=self.scorer, return_estimator=True,
-                                 return_indices=True)
+                                 return_indices=True, n_jobs=self.n_jobs)
             by_group_score_chunks.append(pd.Series(res['test_score'], name=grp))
             if self.metrics is not None:
                 res['metrics'], _ = self.calculate_metrics(x=x, y=y,
                                                            estimators=res['estimator'],
                                                            indices=res['indices'],
                                                            group=None)
             results[grp] = res
```

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/metrics.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/model_selection.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/model_selection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/model_selection/models.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/residuals/error.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/residuals/error.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/utils/file.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/utils/file.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/utils/plotly.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/utils/plotly.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.6.5/elphick/sklearn_viz/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.6.4/pyproject.toml` & `sklearn_viz-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sklearn-viz"
-version = "0.6.4"
+version = "0.6.5"
 description = ""
 authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "elphick/sklearn_viz" }]
 
 [[tool.poetry.source]]
 name = "PyPI"
```

### Comparing `sklearn_viz-0.6.4/PKG-INFO` & `sklearn_viz-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.6.4
+Version: 0.6.5
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

