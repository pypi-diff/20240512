# Comparing `tmp/missing_mga-0.3.0-py3-none-any.whl.zip` & `tmp/missing_mga-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7085 bytes, number of entries: 7
+Zip file size: 7605 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       44 b- defN 24-May-12 13:01 missing_mga/__init__.py
--rw-r--r--  2.0 unx    16310 b- defN 24-May-12 12:50 missing_mga/missing_methods.py
--rw-r--r--  2.0 unx     1069 b- defN 24-May-12 13:43 missing_mga-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5096 b- defN 24-May-12 13:43 missing_mga-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 13:43 missing_mga-0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-12 13:43 missing_mga-0.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      572 b- defN 24-May-12 13:43 missing_mga-0.3.0.dist-info/RECORD
-7 files, 23195 bytes uncompressed, 6067 bytes compressed:  73.8%
+-rw-r--r--  2.0 unx    18749 b- defN 24-May-12 14:40 missing_mga/missing_methods.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-12 14:55 missing_mga-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5124 b- defN 24-May-12 14:55 missing_mga-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 14:55 missing_mga-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-12 14:55 missing_mga-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      572 b- defN 24-May-12 14:55 missing_mga-0.4.0.dist-info/RECORD
+7 files, 25662 bytes uncompressed, 6587 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: missing_mga/__init__.py
 Comment: 
 
 Filename: missing_mga/missing_methods.py
 Comment: 
 
-Filename: missing_mga-0.3.0.dist-info/LICENSE
+Filename: missing_mga-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: missing_mga-0.3.0.dist-info/METADATA
+Filename: missing_mga-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: missing_mga-0.3.0.dist-info/WHEEL
+Filename: missing_mga-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: missing_mga-0.3.0.dist-info/top_level.txt
+Filename: missing_mga-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: missing_mga-0.3.0.dist-info/RECORD
+Filename: missing_mga-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## missing_mga/missing_methods.py

```diff
@@ -1,13 +1,15 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 import itertools
 import upsetplot
+from sklearn.impute import KNNImputer
+
 
 @pd.api.extensions.register_dataframe_accessor("missing")
 class MissingMethods:
     def __init__(self, pandas_obj):
         self._obj = pandas_obj
 
     def number_missing(self):
@@ -66,14 +68,77 @@
             >>> df.missing.number_complete_by_column()
             A    2
             B    2
             dtype: int64
         """
         return self._obj.count()
 
+    def impute_mean(self):
+        """
+        Imputes missing values using the mean of each column.
+        Returns a new DataFrame with missing values imputed.
+        """
+        return self._obj.fillna(self._obj.mean())
+
+    def impute_median(self):
+        """
+        Imputes missing values using the median of each column.
+        Returns a new DataFrame with missing values imputed.
+        """
+        return self._obj.fillna(self._obj.median())
+
+    def impute_mode(self):
+        """
+        Imputes missing values using the mode of each column.
+        Returns a new DataFrame with missing values imputed.
+        """
+        return self._obj.fillna(self._obj.mode().iloc[0])
+
+    def impute_knn(self, n_neighbors=5):
+        """
+        Imputes missing values using KNN (K-Nearest Neighbors).
+        Returns a new DataFrame with missing values imputed.
+        """
+        imputer = KNNImputer(n_neighbors=n_neighbors)
+        return pd.DataFrame(imputer.fit_transform(self._obj), columns=self._obj.columns)
+
+    # Analysis and Visualization of Missing Values
+    def missing_value_heatmap(self):
+        """
+        Creates a heatmap to visualize the distribution of missing values in the dataset.
+        """
+        plt.figure(figsize=(10, 6))
+        sns.heatmap(self._obj.isnull(), cmap='viridis', cbar=False)
+        plt.title('Missing Values Heatmap')
+        plt.show()
+
+    def missing_value_pattern(self):
+        """
+        Identifies patterns and correlations in missing values in the dataset.
+        Returns a DataFrame with information about missing value patterns.
+        """
+        missing_values = self._obj.isnull()
+        missing_patterns = missing_values.groupby((missing_values != missing_values.shift()).cumsum()).cumsum()
+        return missing_patterns
+
+    # Filtering and Dropping Missing Values
+    def drop_missing_rows(self, thresh=0.5):
+        """
+        Drops rows containing missing values above the specified percentage.
+        Returns a new DataFrame with dropped rows.
+        """
+        return self._obj.dropna(thresh=int(thresh * len(self._obj.columns)))
+
+    def drop_missing_columns(self, thresh=0.5):
+        """
+        Drops columns containing missing values above the specified percentage.
+        Returns a new DataFrame with dropped columns.
+        """
+        return self._obj.dropna(axis=1, thresh=int(thresh * len(self._obj)))
+
     def missing_variable_summary(self) -> pd.DataFrame:
         """
         Generates a summary of missing values for each variable (column).
 
         Returns:
             pandas.DataFrame: A DataFrame summarizing the count and percentage of missing values for each variable.
```

## Comparing `missing_mga-0.3.0.dist-info/LICENSE` & `missing_mga-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `missing_mga-0.3.0.dist-info/METADATA` & `missing_mga-0.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
-Name: missing-mga
-Version: 0.3.0
+Name: missing_mga
+Version: 0.4.0
 Summary: A package for handling missing values in datasets.
 Home-page: https://github.com/Mgobeaalcoba/missing_mga
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
 Requires-Dist: upsetplot
+Requires-Dist: scikit-learn
 
 # Extends Pandas DataFrame with a new method to work with missing values
 
 ## Introduction
 
 This package extends the Pandas DataFrame with a new methods to work with missing values. The new method lives in the extension class MissingMethods and is called missing. This methods allows to work with missing values in a more intuitive way.
```

