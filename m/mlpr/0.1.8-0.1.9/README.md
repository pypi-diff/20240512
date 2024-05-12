# Comparing `tmp/mlpr-0.1.8.tar.gz` & `tmp/mlpr-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpr-0.1.8.tar", max compression
+gzip compressed data, was "mlpr-0.1.9.tar", max compression
```

## Comparing `mlpr-0.1.8.tar` & `mlpr-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.8/LICENSE
--rw-r--r--   0        0        0    30200 2024-05-11 16:06:30.324399 mlpr-0.1.8/README.md
--rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.8/SECURITY.md
--rw-r--r--   0        0        0     2502 2024-05-11 16:49:47.333980 mlpr-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       70 2024-05-11 16:49:50.565708 mlpr-0.1.8/src/mlpr/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.8/src/mlpr/ml/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.8/src/mlpr/ml/supervisioned/__init__.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/__init__.py
--rw-r--r--   0        0        0    13901 2024-05-11 16:38:36.531053 mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/metrics.py
--rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/uncertainty.py
--rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/utils.py
--rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.8/src/mlpr/ml/supervisioned/forecasting/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.8/src/mlpr/ml/supervisioned/regression/__init__.py
--rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.8/src/mlpr/ml/supervisioned/regression/metrics.py
--rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.8/src/mlpr/ml/supervisioned/regression/plots.py
--rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.8/src/mlpr/ml/supervisioned/tunning/__init__.py
--rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.8/src/mlpr/ml/supervisioned/tunning/grid_search.py
--rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.8/src/mlpr/reports/__init__.py
--rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.8/src/mlpr/reports/create.py
--rw-r--r--   0        0        0    32161 1970-01-01 00:00:00.000000 mlpr-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      289 2024-05-11 02:18:39.159292 mlpr-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2024-04-27 16:49:57.314542 mlpr-0.1.9/LICENSE
+-rw-r--r--   0        0        0    30292 2024-05-11 17:07:25.245570 mlpr-0.1.9/README.md
+-rw-r--r--   0        0        0      256 2024-05-11 02:24:23.791737 mlpr-0.1.9/SECURITY.md
+-rw-r--r--   0        0        0     2502 2024-05-11 17:20:09.628879 mlpr-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       70 2024-05-11 17:20:13.684801 mlpr-0.1.9/src/mlpr/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.9/src/mlpr/ml/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:27:54.717513 mlpr-0.1.9/src/mlpr/ml/supervisioned/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:38.701333 mlpr-0.1.9/src/mlpr/ml/supervisioned/classification/__init__.py
+-rw-r--r--   0        0        0    13901 2024-05-11 16:38:36.531053 mlpr-0.1.9/src/mlpr/ml/supervisioned/classification/metrics.py
+-rw-r--r--   0        0        0     5103 2024-05-11 02:06:39.037536 mlpr-0.1.9/src/mlpr/ml/supervisioned/classification/uncertainty.py
+-rw-r--r--   0        0        0     2242 2024-05-11 01:58:21.065745 mlpr-0.1.9/src/mlpr/ml/supervisioned/classification/utils.py
+-rw-r--r--   0        0        0        0 2024-04-27 18:28:52.537279 mlpr-0.1.9/src/mlpr/ml/supervisioned/forecasting/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:35:52.450714 mlpr-0.1.9/src/mlpr/ml/supervisioned/regression/__init__.py
+-rw-r--r--   0        0        0    18436 2024-05-05 00:35:48.981115 mlpr-0.1.9/src/mlpr/ml/supervisioned/regression/metrics.py
+-rw-r--r--   0        0        0    18464 2024-05-05 00:20:45.686332 mlpr-0.1.9/src/mlpr/ml/supervisioned/regression/plots.py
+-rw-r--r--   0        0        0        0 2024-04-27 16:52:49.073225 mlpr-0.1.9/src/mlpr/ml/supervisioned/tunning/__init__.py
+-rw-r--r--   0        0        0     6314 2024-05-10 23:01:04.220209 mlpr-0.1.9/src/mlpr/ml/supervisioned/tunning/grid_search.py
+-rw-r--r--   0        0        0       62 2024-04-27 21:43:09.387068 mlpr-0.1.9/src/mlpr/reports/__init__.py
+-rw-r--r--   0        0        0     1742 2024-05-04 23:35:34.703861 mlpr-0.1.9/src/mlpr/reports/create.py
+-rw-r--r--   0        0        0    32253 1970-01-01 00:00:00.000000 mlpr-0.1.9/PKG-INFO
```

### Comparing `mlpr-0.1.8/LICENSE` & `mlpr-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.8/README.md` & `mlpr-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -442,24 +442,25 @@
 for i, k in enumerate(np.unique(y)):
   ax.scatter(X[:, 0][y == k], X[:, 1][y == k], marker=markers[i % len(markers)], color=colors[i], label=f"c{i}")
 
 ax.set_title("Dataset")
 ax.set_frame_on(False)
 ax.set_xticks([])
 ax.set_yticks([])
-for center, color in zip(centers, colors):
-  ax.scatter(
-    center[0],
-    center[1],
-    color="white",
-    linewidths=3,
-    marker="o",
-    edgecolor="black",
-    s=120
-  )
+for i, (center, color) in enumerate(zip(centers, colors)):
+    ax.scatter(
+        center[0],
+        center[1],
+        color="white",
+        linewidths=3,
+        marker="o",
+        edgecolor="black",
+        s=120,
+        label="center" if i == 0 else None
+    )
 plt.legend()
 fig.tight_layout()
 ```
 
 [![fig1](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/classification_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/classification_scatter.png)
```

#### html2text {}

```diff
@@ -119,39 +119,39 @@
 dataset for experiments, using blobs from scikit-learn. ```python X, y =
 make_blobs( **params ) ``` ## Plot the dataset Behavior of the dataset used in
 the experiment. ```python markers = ['o', 'v', '^'] fig, ax = plt.subplots(1,
 1, figsize=(14, 6)) colors = generate_colors("FF4B3E", "1C2127", len(np.unique
 (y))) for i, k in enumerate(np.unique(y)): ax.scatter(X[:, 0][y == k], X[:, 1]
 [y == k], marker=markers[i % len(markers)], color=colors[i], label=f"c{i}")
 ax.set_title("Dataset") ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks(
-[]) for center, color in zip(centers, colors): ax.scatter( center[0], center
-[1], color="white", linewidths=3, marker="o", edgecolor="black", s=120 )
-plt.legend() fig.tight_layout() ``` [![fig1](https://raw.githack.com/Manuelfjr/
-mlpr/develop/assets/classification_scatter.png)](https://raw.githack.com/
-Manuelfjr/mlpr/develop/assets/classification_scatter.png) ## Cross-validation
-```python models: dict[BaseEstimator, dict] = { RandomForestClassifier:
-{ 'n_estimators': [10, 50, 100, 200], 'max_depth': [None, 5, 10, 15],
-'min_samples_split': [2, 5, 10], 'min_samples_leaf': [1, 2, 4], 'random_state':
-[random_state] }, GradientBoostingClassifier: { 'n_estimators': [50, 100, 200],
-'learning_rate': [0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0],
-'random_state': [random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0,
-10.0], 'penalty': ['l1', 'l2'], 'solver': ['liblinear', 'saga'],
-'random_state': [random_state], 'max_iter': [10000] }, GaussianNB:
-{ 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6, 1e-5] }, SVC: { 'C': [0.01, 0.1,
-1.0, 10.0], 'kernel': ['linear', 'poly', 'rbf', 'sigmoid'], 'degree': [2, 3,
-4], 'gamma': ['scale', 'auto'], 'probability': [True], 'random_state':
-[random_state] }, DecisionTreeClassifier: { 'criterion': ['gini', 'entropy'],
-'splitter': ['best', 'random'], 'max_depth': [None, 5, 10, 15],
-'min_samples_split': [2, 5, 10], 'min_samples_leaf': [1, 2, 4], 'random_state':
-[random_state] } } ``` ```python grid_search = GridSearch( X, y,
-params_split=params_split, models_params=models, normalize=True,
-params_norm=params_norm, scoring='accuracy', metrics=model_metrics )
-grid_search.search(cv=cv, n_jobs=-1) best_model, best_params = \ grid_search \
-.get_best_model() ``` ```python results: pd.DataFrame = pd.DataFrame
-(grid_search._metrics).T results ```
+[]) for i, (center, color) in enumerate(zip(centers, colors)): ax.scatter
+( center[0], center[1], color="white", linewidths=3, marker="o",
+edgecolor="black", s=120, label="center" if i == 0 else None ) plt.legend()
+fig.tight_layout() ``` [![fig1](https://raw.githack.com/Manuelfjr/mlpr/develop/
+assets/classification_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/
+develop/assets/classification_scatter.png) ## Cross-validation ```python
+models: dict[BaseEstimator, dict] = { RandomForestClassifier: { 'n_estimators':
+[10, 50, 100, 200], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5,
+10], 'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] },
+GradientBoostingClassifier: { 'n_estimators': [50, 100, 200], 'learning_rate':
+[0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0], 'random_state':
+[random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0, 10.0], 'penalty':
+['l1', 'l2'], 'solver': ['liblinear', 'saga'], 'random_state': [random_state],
+'max_iter': [10000] }, GaussianNB: { 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6,
+1e-5] }, SVC: { 'C': [0.01, 0.1, 1.0, 10.0], 'kernel': ['linear', 'poly',
+'rbf', 'sigmoid'], 'degree': [2, 3, 4], 'gamma': ['scale', 'auto'],
+'probability': [True], 'random_state': [random_state] },
+DecisionTreeClassifier: { 'criterion': ['gini', 'entropy'], 'splitter':
+['best', 'random'], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5,
+10], 'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] } } ```
+```python grid_search = GridSearch( X, y, params_split=params_split,
+models_params=models, normalize=True, params_norm=params_norm,
+scoring='accuracy', metrics=model_metrics ) grid_search.search(cv=cv, n_jobs=-
+1) best_model, best_params = \ grid_search \ .get_best_model() ``` ```python
+results: pd.DataFrame = pd.DataFrame(grid_search._metrics).T results ```
                            ccuussttoomm__aaccccuurraaccyy aaccccuurraaccyy pprreecciissiioonn rreeccaallll   kkaappppaa    ff11
 RandomForestClassifier     222.0           0.888    0.883566  0.885902 0.831666 0.882724
 GradientBoostingClassifier 221.0           0.884    0.878830  0.881207 0.825583 0.878421
 LogisticRegression         230.0           0.920    0.915170  0.916987 0.879457 0.915662
 GaussianNB                 231.0           0.924    0.919375  0.921682 0.885539 0.920046
 SVC                        230.0           0.920    0.915170  0.916987 0.879457 0.915662
 DecisionTreeClassifier     214.0           0.856    0.848155  0.845622 0.782325 0.846414
```

### Comparing `mlpr-0.1.8/pyproject.toml` & `mlpr-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlpr"
-version = "0.1.8"
+version = "0.1.9"
 authors = ["Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"]
 description = "A library for machine learning pipeline and creation of reports."
 readme = "README.md"
 maintainers = [
     "Manuel Ferreira Junior <ferreira.jr.ufpb@gmail.com>"
 ]
 classifiers=[
```

### Comparing `mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/metrics.py` & `mlpr-0.1.9/src/mlpr/ml/supervisioned/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/uncertainty.py` & `mlpr-0.1.9/src/mlpr/ml/supervisioned/classification/uncertainty.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.8/src/mlpr/ml/supervisioned/classification/utils.py` & `mlpr-0.1.9/src/mlpr/ml/supervisioned/classification/utils.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.8/src/mlpr/ml/supervisioned/regression/metrics.py` & `mlpr-0.1.9/src/mlpr/ml/supervisioned/regression/metrics.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.8/src/mlpr/ml/supervisioned/regression/plots.py` & `mlpr-0.1.9/src/mlpr/ml/supervisioned/regression/plots.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.8/src/mlpr/ml/supervisioned/tunning/grid_search.py` & `mlpr-0.1.9/src/mlpr/ml/supervisioned/tunning/grid_search.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.8/src/mlpr/reports/create.py` & `mlpr-0.1.9/src/mlpr/reports/create.py`

 * *Files identical despite different names*

### Comparing `mlpr-0.1.8/PKG-INFO` & `mlpr-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpr
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for machine learning pipeline and creation of reports.
 Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com
 Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com
 Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
@@ -485,24 +485,25 @@
 for i, k in enumerate(np.unique(y)):
   ax.scatter(X[:, 0][y == k], X[:, 1][y == k], marker=markers[i % len(markers)], color=colors[i], label=f"c{i}")
 
 ax.set_title("Dataset")
 ax.set_frame_on(False)
 ax.set_xticks([])
 ax.set_yticks([])
-for center, color in zip(centers, colors):
-  ax.scatter(
-    center[0],
-    center[1],
-    color="white",
-    linewidths=3,
-    marker="o",
-    edgecolor="black",
-    s=120
-  )
+for i, (center, color) in enumerate(zip(centers, colors)):
+    ax.scatter(
+        center[0],
+        center[1],
+        color="white",
+        linewidths=3,
+        marker="o",
+        edgecolor="black",
+        s=120,
+        label="center" if i == 0 else None
+    )
 plt.legend()
 fig.tight_layout()
 ```
 
 [![fig1](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/classification_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/develop/assets/classification_scatter.png)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mlpr Version: 0.1.8 Summary: A library for machine
+Metadata-Version: 2.1 Name: mlpr Version: 0.1.9 Summary: A library for machine
 learning pipeline and creation of reports. Author: Manuel Ferreira Junior
 Author-email: ferreira.jr.ufpb@gmail.com Maintainer: Manuel Ferreira Junior
 Maintainer-email: ferreira.jr.ufpb@gmail.com Requires-Python: >=3.9 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: MacOS Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: Unix
@@ -145,39 +145,39 @@
 dataset for experiments, using blobs from scikit-learn. ```python X, y =
 make_blobs( **params ) ``` ## Plot the dataset Behavior of the dataset used in
 the experiment. ```python markers = ['o', 'v', '^'] fig, ax = plt.subplots(1,
 1, figsize=(14, 6)) colors = generate_colors("FF4B3E", "1C2127", len(np.unique
 (y))) for i, k in enumerate(np.unique(y)): ax.scatter(X[:, 0][y == k], X[:, 1]
 [y == k], marker=markers[i % len(markers)], color=colors[i], label=f"c{i}")
 ax.set_title("Dataset") ax.set_frame_on(False) ax.set_xticks([]) ax.set_yticks(
-[]) for center, color in zip(centers, colors): ax.scatter( center[0], center
-[1], color="white", linewidths=3, marker="o", edgecolor="black", s=120 )
-plt.legend() fig.tight_layout() ``` [![fig1](https://raw.githack.com/Manuelfjr/
-mlpr/develop/assets/classification_scatter.png)](https://raw.githack.com/
-Manuelfjr/mlpr/develop/assets/classification_scatter.png) ## Cross-validation
-```python models: dict[BaseEstimator, dict] = { RandomForestClassifier:
-{ 'n_estimators': [10, 50, 100, 200], 'max_depth': [None, 5, 10, 15],
-'min_samples_split': [2, 5, 10], 'min_samples_leaf': [1, 2, 4], 'random_state':
-[random_state] }, GradientBoostingClassifier: { 'n_estimators': [50, 100, 200],
-'learning_rate': [0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0],
-'random_state': [random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0,
-10.0], 'penalty': ['l1', 'l2'], 'solver': ['liblinear', 'saga'],
-'random_state': [random_state], 'max_iter': [10000] }, GaussianNB:
-{ 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6, 1e-5] }, SVC: { 'C': [0.01, 0.1,
-1.0, 10.0], 'kernel': ['linear', 'poly', 'rbf', 'sigmoid'], 'degree': [2, 3,
-4], 'gamma': ['scale', 'auto'], 'probability': [True], 'random_state':
-[random_state] }, DecisionTreeClassifier: { 'criterion': ['gini', 'entropy'],
-'splitter': ['best', 'random'], 'max_depth': [None, 5, 10, 15],
-'min_samples_split': [2, 5, 10], 'min_samples_leaf': [1, 2, 4], 'random_state':
-[random_state] } } ``` ```python grid_search = GridSearch( X, y,
-params_split=params_split, models_params=models, normalize=True,
-params_norm=params_norm, scoring='accuracy', metrics=model_metrics )
-grid_search.search(cv=cv, n_jobs=-1) best_model, best_params = \ grid_search \
-.get_best_model() ``` ```python results: pd.DataFrame = pd.DataFrame
-(grid_search._metrics).T results ```
+[]) for i, (center, color) in enumerate(zip(centers, colors)): ax.scatter
+( center[0], center[1], color="white", linewidths=3, marker="o",
+edgecolor="black", s=120, label="center" if i == 0 else None ) plt.legend()
+fig.tight_layout() ``` [![fig1](https://raw.githack.com/Manuelfjr/mlpr/develop/
+assets/classification_scatter.png)](https://raw.githack.com/Manuelfjr/mlpr/
+develop/assets/classification_scatter.png) ## Cross-validation ```python
+models: dict[BaseEstimator, dict] = { RandomForestClassifier: { 'n_estimators':
+[10, 50, 100, 200], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5,
+10], 'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] },
+GradientBoostingClassifier: { 'n_estimators': [50, 100, 200], 'learning_rate':
+[0.1, 0.05, 0.01, 0.005], 'subsample': [0.5, 0.8, 1.0], 'random_state':
+[random_state] }, LogisticRegression: { 'C': [0.01, 0.1, 1.0, 10.0], 'penalty':
+['l1', 'l2'], 'solver': ['liblinear', 'saga'], 'random_state': [random_state],
+'max_iter': [10000] }, GaussianNB: { 'var_smoothing': [1e-9, 1e-8, 1e-7, 1e-6,
+1e-5] }, SVC: { 'C': [0.01, 0.1, 1.0, 10.0], 'kernel': ['linear', 'poly',
+'rbf', 'sigmoid'], 'degree': [2, 3, 4], 'gamma': ['scale', 'auto'],
+'probability': [True], 'random_state': [random_state] },
+DecisionTreeClassifier: { 'criterion': ['gini', 'entropy'], 'splitter':
+['best', 'random'], 'max_depth': [None, 5, 10, 15], 'min_samples_split': [2, 5,
+10], 'min_samples_leaf': [1, 2, 4], 'random_state': [random_state] } } ```
+```python grid_search = GridSearch( X, y, params_split=params_split,
+models_params=models, normalize=True, params_norm=params_norm,
+scoring='accuracy', metrics=model_metrics ) grid_search.search(cv=cv, n_jobs=-
+1) best_model, best_params = \ grid_search \ .get_best_model() ``` ```python
+results: pd.DataFrame = pd.DataFrame(grid_search._metrics).T results ```
                            ccuussttoomm__aaccccuurraaccyy aaccccuurraaccyy pprreecciissiioonn rreeccaallll   kkaappppaa    ff11
 RandomForestClassifier     222.0           0.888    0.883566  0.885902 0.831666 0.882724
 GradientBoostingClassifier 221.0           0.884    0.878830  0.881207 0.825583 0.878421
 LogisticRegression         230.0           0.920    0.915170  0.916987 0.879457 0.915662
 GaussianNB                 231.0           0.924    0.919375  0.921682 0.885539 0.920046
 SVC                        230.0           0.920    0.915170  0.916987 0.879457 0.915662
 DecisionTreeClassifier     214.0           0.856    0.848155  0.845622 0.782325 0.846414
```

