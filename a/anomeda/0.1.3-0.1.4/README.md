# Comparing `tmp/anomeda-0.1.3.tar.gz` & `tmp/anomeda-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomeda-0.1.3.tar", last modified: Sun Apr 14 18:39:32 2024, max compression
+gzip compressed data, was "anomeda-0.1.4.tar", last modified: Sun May 12 12:05:30 2024, max compression
```

## Comparing `anomeda-0.1.3.tar` & `anomeda-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 18:39:32.113075 anomeda-0.1.3/
--rw-rw-rw-   0        0        0     1094 2023-12-21 17:57:18.000000 anomeda-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     8784 2024-04-14 18:39:32.107657 anomeda-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     8138 2024-04-14 15:40:52.000000 anomeda-0.1.3/README.md
--rw-rw-rw-   0        0        0      722 2024-04-14 18:23:01.000000 anomeda-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-14 18:39:32.114073 anomeda-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-14 18:39:32.019031 anomeda-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-14 18:39:32.041745 anomeda-0.1.3/src/anomeda/
--rw-rw-rw-   0        0        0    24164 2024-04-14 15:40:38.000000 anomeda-0.1.3/src/anomeda/DataFrame.py
--rw-rw-rw-   0        0        0     1455 2024-02-23 19:24:49.000000 anomeda-0.1.3/src/anomeda/__init__.py
--rw-rw-rw-   0        0        0    65024 2024-04-14 18:36:54.000000 anomeda-0.1.3/src/anomeda/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-14 18:39:32.104452 anomeda-0.1.3/src/anomeda.egg-info/
--rw-rw-rw-   0        0        0     8784 2024-04-14 18:39:31.000000 anomeda-0.1.3/src/anomeda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-04-14 18:39:32.000000 anomeda-0.1.3/src/anomeda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 18:39:31.000000 anomeda-0.1.3/src/anomeda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-14 18:39:31.000000 anomeda-0.1.3/src/anomeda.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-14 18:39:32.099616 anomeda-0.1.3/tests/
--rw-rw-rw-   0        0        0    13469 2024-04-14 15:40:52.000000 anomeda-0.1.3/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:05:30.135594 anomeda-0.1.4/
+-rw-rw-rw-   0        0        0     1094 2023-12-21 17:57:18.000000 anomeda-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     8784 2024-05-12 12:05:30.127081 anomeda-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8138 2024-04-14 15:40:52.000000 anomeda-0.1.4/README.md
+-rw-rw-rw-   0        0        0      722 2024-05-12 12:03:51.000000 anomeda-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 12:05:30.136630 anomeda-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 12:05:30.030592 anomeda-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 12:05:30.065408 anomeda-0.1.4/src/anomeda/
+-rw-rw-rw-   0        0        0    24295 2024-05-12 11:45:59.000000 anomeda-0.1.4/src/anomeda/DataFrame.py
+-rw-rw-rw-   0        0        0     1455 2024-02-23 19:24:49.000000 anomeda-0.1.4/src/anomeda/__init__.py
+-rw-rw-rw-   0        0        0    65885 2024-05-12 12:04:52.000000 anomeda-0.1.4/src/anomeda/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:05:30.124325 anomeda-0.1.4/src/anomeda.egg-info/
+-rw-rw-rw-   0        0        0     8784 2024-05-12 12:05:29.000000 anomeda-0.1.4/src/anomeda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-05-12 12:05:30.000000 anomeda-0.1.4/src/anomeda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 12:05:29.000000 anomeda-0.1.4/src/anomeda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-12 12:05:29.000000 anomeda-0.1.4/src/anomeda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 12:05:30.118986 anomeda-0.1.4/tests/
+-rw-rw-rw-   0        0        0    14140 2024-05-12 11:45:34.000000 anomeda-0.1.4/tests/test_main.py
```

### Comparing `anomeda-0.1.3/LICENSE` & `anomeda-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anomeda-0.1.3/PKG-INFO` & `anomeda-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomeda
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package which helps to identify important metric changes and quickly find clusters in data which changed the trend of the metric or caused the anomaly
 Author-email: Anton Saroka <anton.soroka.1313@gmail.com>
 Project-URL: Homepage, https://github.com/AntonSarr/anomeda
 Project-URL: Issues, https://github.com/AntonSarr/anomeda/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anomeda-0.1.3/README.md` & `anomeda-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `anomeda-0.1.3/pyproject.toml` & `anomeda-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "anomeda"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Anton Saroka", email="anton.soroka.1313@gmail.com" },
 ]
 description = "Python package which helps to identify important metric changes and quickly find clusters in data which changed the trend of the metric or caused the anomaly"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `anomeda-0.1.3/src/anomeda/DataFrame.py` & `anomeda-0.1.4/src/anomeda/DataFrame.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,29 +220,29 @@
             self.set_index(index_name, inplace=True)
         
         measures_names = kwargs.get('measures_names')
         if measures_names is None:
             measures_names = []
         self.set_measures_names(measures_names)
         
-        measures_types = kwargs.get('measures_types')
-        if measures_types is None:
-            measures_types = {}
-        self.set_measures_types(measures_types)
-        
         discretized_measures = kwargs.get('discretized_measures')
         discretized_measures_mapping = kwargs.get('discretized_measures_mapping')
 
         if discretized_measures is not None and discretized_measures != {}\
               and discretized_measures_mapping is not None and discretized_measures_mapping != {}:
-            raise NotImplementedError('As for now "discretized_measures" and "discretized_measures_mapping" cannot be passed at the same time. Please choose either mapping or measures.')
+            raise NotImplementedError('As for now, "discretized_measures" and "discretized_measures_mapping" cannot be passed at the same time. Please choose either mapping or measures.')
         
         self.set_discretized_measures(discretized_measures)
         self.set_discretization_mapping(discretized_measures_mapping)
         
+        measures_types = kwargs.get('measures_types')
+        if measures_types is None:
+            measures_types = {}
+        self.set_measures_types(measures_types)
+        
         metric_name = kwargs.get('metric_name')
         self.set_metric_name(metric_name)
         
         agg_func = kwargs.get('agg_func')
         if agg_func is None:
             agg_func = 'sum'
         self.set_agg_func(agg_func)
@@ -360,14 +360,16 @@
                 1: [[0.5, 0.94999]] # may correspond to "normal" values; 94999 is an excluding bound
             }
         })
         ```
         """
         if discretized_measures_mapping is not None:
             self._discretized_measures_mapping = discretized_measures_mapping.copy()
+        else:
+            self._discretized_measures_mapping = {}
 
         if discretized_measures_mapping is not None and recalculate_measures:
             self._discretized_measures = {}
             for measure in discretized_measures_mapping.keys():
                 tmp_measure_values = self[measure].copy()
                 mapped_measure_values = pd.Series([None for i in range(tmp_measure_values.shape[0])], index=tmp_measure_values.index)
                 for discrete_value in discretized_measures_mapping[measure].keys():
@@ -415,34 +417,37 @@
         ```python
         anmd_df.set_measures_types({
             'continous': ['numeric_measure_1'],
             'categorical': ['measure_1']
         })
         ```
         """
+        
         self._measures_types = measures_types
-        if measures_types is not None:    
-            if 'continuous' in measures_types:
-                if not hasattr(self, '_discretized_measures') or self._discretized_measures is None:
-                    self._discretized_measures = {}
-                    self._discretized_measures_mapping = {}
-                for measure in measures_types['continuous']:
-                    if measure not in self._discretized_measures:
-                        n_samples = self[measure].values.shape[0]
-                        if n_samples >= 2:
-                            self._discretized_measures[measure], \
-                            self._discretized_measures_mapping[measure] = _to_discrete_values(self[measure].values)
-                        elif n_samples == 1:
-                            self._discretized_measures[measure] = [0]
-                            self._discretized_measures_mapping[measure] = {
-                                0: [[self[measure].values[0], self[measure].values[0]]]
-                            }
-                        else:
-                            self._discretized_measures[measure] = []
-                            self._discretized_measures_mapping[measure] = {}
+        
+        if not hasattr(self, '_discretized_measures') or self._discretized_measures is None:
+            self._discretized_measures = {}
+            self._discretized_measures_mapping = {}
+
+            if measures_types is not None:    
+                if 'continuous' in measures_types:
+                    for measure in measures_types['continuous']:
+                        if measure not in self._discretized_measures:
+                            n_samples = self[measure].values.shape[0]
+                            if n_samples >= 2:
+                                self._discretized_measures[measure], \
+                                self._discretized_measures_mapping[measure] = _to_discrete_values(self[measure].values)
+                            elif n_samples == 1:
+                                self._discretized_measures[measure] = [0]
+                                self._discretized_measures_mapping[measure] = {
+                                    0: [[self[measure].values[0], self[measure].values[0]]]
+                                }
+                            else:
+                                self._discretized_measures[measure] = []
+                                self._discretized_measures_mapping[measure] = {}
 
     def get_discretized_measures(self):
         """Return discretized versions of continous measures."""
         return self._discretized_measures.copy()
     
     def set_discretized_measures(self, discretized_measures : 'dict'):
         """Set custom discretization for continous measures.
```

### Comparing `anomeda-0.1.3/src/anomeda/__init__.py` & `anomeda-0.1.4/src/anomeda/__init__.py`

 * *Files identical despite different names*

### Comparing `anomeda-0.1.3/src/anomeda/utils.py` & `anomeda-0.1.4/src/anomeda/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -641,15 +641,18 @@
             y_fitted = y_fitted[sorted_ind]
 
             
             if len(ydata) == 1:
                 outliers = np.array([False])
             else:
                 clusterizator = LocalOutlierFactor(n_neighbors=max(min(len(ydata) - 1, n_neighbors), 1), novelty=False)
-                outliers = clusterizator.fit_predict(y_diff.reshape(-1, 1)) == -1
+                try:
+                    outliers = clusterizator.fit_predict(y_diff.reshape(-1, 1)) == -1
+                except ValueError:
+                    raise ValueError("Something is wrong with the metric values. It may contain NaN or other values which caused errors while fitting trends.")
 
             # Remove inliers, i.e. isolated points not from the left or right tail of values range
             # We want to keep only the largest or the lowest differences
             # We also keep only % of anomalies defined by p_low and p_large
             indeces_sorted_by_y_diff = np.argsort(y_diff)
             not_outliers_indeces = np.where(outliers[indeces_sorted_by_y_diff] == False)[0]
             outliers[indeces_sorted_by_y_diff[np.min(not_outliers_indeces): np.max(not_outliers_indeces)]] = False
@@ -741,15 +744,18 @@
         y_diff = y_diff[sorted_ind]
         y_fitted = y_fitted[sorted_ind]
 
         if len(ydata) == 1:
             outliers = np.array([False])
         else:
             clusterizator = LocalOutlierFactor(n_neighbors=max(min(len(ydata) - 1, n_neighbors), 1), novelty=False)
-            outliers = clusterizator.fit_predict(y_diff.reshape(-1, 1)) == -1
+            try:
+                outliers = clusterizator.fit_predict(y_diff.reshape(-1, 1)) == -1
+            except ValueError:
+                raise ValueError("Something is wrong with the metric values. It may contain NaN or other values which caused errors while fitting trends.")
 
         # Remove inliers, i.e. isolated points not from the left or right tail of values range
         # We want to keep only the largest or the lowest differences
         # We also keep only % of anomalies defined by p_low and p_large
         indeces_sorted_by_y_diff = np.argsort(y_diff)
         not_outliers_indeces = np.where(outliers[indeces_sorted_by_y_diff] == False)[0]
         outliers[indeces_sorted_by_y_diff[np.min(not_outliers_indeces): np.max(not_outliers_indeces)]] = False
@@ -794,15 +800,16 @@
         raise TypeError('Data parameter must be either anomeda.DataFrame or (numpy.ndarray[int], numpy.ndarray[float]) tuple')
         
 
 def plot_trends(
     data: 'anomeda.DataFrame | pandas.DataFrame returned from anomeda.fit_trends()', 
     breakdowns : "'no' | 'all' | list[str] | list[list[str]]" = 'no',
     show_metric=True,
-    colors : 'dict' = None
+    colors : 'dict' = None,
+    ax : 'matplotlib.axes.Axes' = None
 ):
     """Plot fitted trends.
     
     Plot trends either from anomeda.DataFrame instance or using a response from anomeda.fit_trends().
     
     Parameters
     ----------
@@ -811,24 +818,29 @@
     breakdowns : 'no' | 'all' | list[str], default 'no'
         If 'no', the metric is grouped by date points only. 
         If 'all', all combinations of measures are used to extract and plot clusters. 
         If list[str], then only specific clusters specified in the list are plotted. 
         If list[list[str]] then each internal list is a list of measures used to extract clusters.
     show_metric : bool, default True
         Indicator if to show actual metric on plots.
+    ax : matplotlib.axes.Axes, default None
+        Axes to use for plotting. If None, a new Axes is created.
         
     Returns
     -------
     None
 
     Examples
     --------
     >>> anomeda.fit_trends(data)
     >>> anomeda.plot_trends(data)
     """
+    if ax is None:
+        fig, ax = plt.subplots()
+    
     if type(data) == DataFrame:
         if hasattr(data, '_trends'):
             df = data._trends.copy()
         if not hasattr(data, '_trends') or not hasattr(data, '_clusters'):
             raise NotFittedError('The anomeda.DataFrame instance has no fitted trends or clusters. Run anomeda.fit_trends() with save_trends=True and prefered parameters first')
     
         if df is None or len(df) == 0:
@@ -965,30 +977,31 @@
             y_trend = x * t['slope'] + t['intercept']
             
             x_cluster.append(x_axis)
             y_trend_cluster.append(y_trend)
         
         x_cluster = np.concatenate(x_cluster)
         y_trend_cluster = np.concatenate(y_trend_cluster)
-        plt.plot(x_cluster, y_trend_cluster, label=cluster, color=cluster_c[cluster], linestyle=(0, (5, 2)))
+        ax.plot(x_cluster, y_trend_cluster, label=cluster, color=cluster_c[cluster], linestyle=(0, (5, 2)))
         
         if show_metric and type(data) == DataFrame:
             cluster_info = data._clusters[c]
-            plt.plot(cluster_info['index'], cluster_info['values'], color=cluster_c[cluster])
+            ax.plot(cluster_info['index'], cluster_info['values'], color=cluster_c[cluster])
         
-    plt.legend()
+    ax.legend()
 
 
 def plot_clusters(
     data : 'anomeda.DataFrame', 
     breakdowns : "'no' | 'all' | list[str] | list[list[str]]" = 'no',
     metric_propagate : '"zeros" | "ffil" | None' = None,
     min_cluster_size : 'int | None' = None,
     max_cluster_size : 'int | None' = None,
-    colors : 'dict' = None
+    colors : 'dict' = None,
+    ax : 'matplotlib.axes.Axes' = None
 ):
     """Plot metric in clusters.
     
     Plot metric extracted from clusters from anomeda.DataFrame instance.
     
     Parameters
     ----------
@@ -1021,14 +1034,16 @@
             Use only present metric and index values.
     min_cluster_size : int, default None
         Skip clusters whose total size among all date points is less than the value.
     max_cluster_size : int, default None
         Skip clusters whose total size among all date points is more than the value.
     colors : dict, default None
         Dictionary with a mapping between clusters and colors used in matplotlib.
+    ax : matplotlib.axes.Axes, default None
+        Axes to use for plotting. If None, a new object is created.
         
     Returns
     -------
     None
 
     Examples
     --------
@@ -1043,14 +1058,17 @@
     >>> )
 
     >>> anomeda.plot_clusters(
     >>>     data, # anomeda.DataFrame
     >>>     breakdowns='no' # plot a metric grouped by index values only
     >>> )
     """
+    if ax is None:
+        fig, ax = plt.subplots()
+        
     if type(data) == DataFrame:
         pass
     else:
         raise ValueError('"data" argument must be an anomeda.DataFrame instance')
     
     if data is None or len(data) == 0:
         return None
@@ -1139,17 +1157,17 @@
             yindex = yseries.index.values
             ydata = yseries.values
             
             if metric_propagate is not None:
                 freq = data._index_freq
                 yindex, _, ydata = _propagate_metric(yindex, ydata, strategy=metric_propagate, freq=freq)
             
-            plt.plot(yindex, ydata, label=query, color=cluster_c[query])
+            ax.plot(yindex, ydata, label=query, color=cluster_c[query])
     if len(clusters) > 0:
-        plt.legend()
+        ax.legend()
 
 
 def fit_trends(
     data : 'anomeda.DataFrame | (numpy.ndarray[int], numpy.ndarray[float]) | (pandas.DatetimeIndex, numpy.ndarray[float])', 
     trend_fitting_conf : 'dict' = {'max_trends': 'auto', 'min_var_reduction': 0.75},
     save_trends : 'bool' = True,
     breakdowns : "'no' | 'all' | list[str] | list[list[str]]" = 'no',
```

### Comparing `anomeda-0.1.3/src/anomeda.egg-info/PKG-INFO` & `anomeda-0.1.4/src/anomeda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anomeda
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python package which helps to identify important metric changes and quickly find clusters in data which changed the trend of the metric or caused the anomaly
 Author-email: Anton Saroka <anton.soroka.1313@gmail.com>
 Project-URL: Homepage, https://github.com/AntonSarr/anomeda
 Project-URL: Issues, https://github.com/AntonSarr/anomeda/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `anomeda-0.1.3/tests/test_main.py` & `anomeda-0.1.4/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,17 +315,32 @@
         measures_types=measures_types,
         index_name=index_name,
         metric_name=metric_name,
         agg_func=agg_func
     )
 
     res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"')
-
     res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"', breakdowns=['total'])
-
+    res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"', breakdowns=['`a`==20'])
+    
+    index_name = 'dt'
+    metric_name = 'metric'
+    agg_func = 'sum'
+    measures_names = ['a', 'b']
+    
+    anmd_df = anomeda.DataFrame(
+        dummy_df,
+        measures_names=measures_names,
+        index_name=index_name,
+        metric_name=metric_name,
+        agg_func=agg_func
+    )
+    
+    res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"')
+    res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"', breakdowns=['total'])
     res = anomeda.compare_clusters(anmd_df, period1='dt < "2024-01-01"', period2='dt >= "2024-01-01"', breakdowns=['`a`==20'])
 
 
 def test_empty_df():
 
     dummy_df = pd.DataFrame({'dt': [], 'a': [], 'b': [], 'metric': []})
```

