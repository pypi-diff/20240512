# Comparing `tmp/missing_mga-0.4.3-py3-none-any.whl.zip` & `tmp/missing_mga-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7711 bytes, number of entries: 7
+Zip file size: 7725 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       55 b- defN 24-May-12 15:18 missing_mga/__init__.py
--rw-r--r--  2.0 unx    18353 b- defN 24-May-12 16:23 missing_mga/missing_methods.py
--rw-r--r--  2.0 unx     1069 b- defN 24-May-12 16:25 missing_mga-0.4.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     5915 b- defN 24-May-12 16:25 missing_mga-0.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 16:25 missing_mga-0.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-12 16:25 missing_mga-0.4.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      572 b- defN 24-May-12 16:25 missing_mga-0.4.3.dist-info/RECORD
-7 files, 26068 bytes uncompressed, 6693 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    18439 b- defN 24-May-12 17:46 missing_mga/missing_methods.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-12 17:52 missing_mga-1.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5915 b- defN 24-May-12 17:52 missing_mga-1.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 17:52 missing_mga-1.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-12 17:52 missing_mga-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      572 b- defN 24-May-12 17:52 missing_mga-1.0.0.dist-info/RECORD
+7 files, 26154 bytes uncompressed, 6707 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: missing_mga/__init__.py
 Comment: 
 
 Filename: missing_mga/missing_methods.py
 Comment: 
 
-Filename: missing_mga-0.4.3.dist-info/LICENSE
+Filename: missing_mga-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: missing_mga-0.4.3.dist-info/METADATA
+Filename: missing_mga-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: missing_mga-0.4.3.dist-info/WHEEL
+Filename: missing_mga-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: missing_mga-0.4.3.dist-info/top_level.txt
+Filename: missing_mga-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: missing_mga-0.4.3.dist-info/RECORD
+Filename: missing_mga-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## missing_mga/missing_methods.py

```diff
@@ -189,15 +189,15 @@
             0                       1            2           50.0
             1                       0            1           50.0
         """
         return (
             self._obj.missing.missing_variable_summary()
             .value_counts("n_missing")
             .reset_index()
-            .rename(columns={"n_missing": "n_missing_in_variable", 0: "n_variables"})
+            .rename(columns={"n_missing": "n_missing_in_variable", "count": "n_variables"})
             .assign(
                 pct_variables=lambda df: df.n_variables / df.n_variables.sum() * 100
             )
             .sort_values("pct_variables", ascending=False)
         )
 
     def missing_case_table(self) -> pd.DataFrame:
@@ -214,15 +214,15 @@
             0                    1        2      66.7
             1                    0        1      33.3
         """
         return (
             self._obj.missing.missing_case_summary()
             .value_counts("n_missing")
             .reset_index()
-            .rename(columns={"n_missing": "n_missing_in_case", 0: "n_cases"})
+            .rename(columns={"n_missing": "n_missing_in_case", "count": "n_cases"})
             .assign(pct_case=lambda df: df.n_cases / df.n_cases.sum() * 100)
             .sort_values("pct_case", ascending=False)
         )
 
     def missing_variable_span(self, variable: str, span_every: int) -> pd.DataFrame:
         """
         Generates a summary of missing values over a repeating span for a specified variable.
@@ -432,23 +432,24 @@
         plt.grid(axis="y")
 
         plt.xlabel("Number missing")
         plt.ylabel("Variable")
 
     def missing_case_plot(self):
         """
-        Plots a histogram showing the distribution of missing values across cases.
+        Plots a bar plot showing the distribution of missing values across cases.
 
         Example:
             >>> df = pd.DataFrame({'A': [1, 2, np.nan], 'B': [4, np.nan, 6]})
             >>> df.missing.missing_case_plot()
         """
-        df = self._obj.missing.missing_case_summary()
+        df = self._obj.missing.missing_case_summary().value_counts("n_missing")
+        df = pd.DataFrame(df).reset_index()
 
-        sns.displot(data=df, x="n_missing", binwidth=1, color="black")
+        sns.barplot(data=df_test2, x="n_missing", y="count", color="black")
 
         plt.grid(axis="x")
         plt.xlabel("Number of missings in case")
         plt.ylabel("Number of cases")
 
     def missing_variable_span_plot(
             self, variable: str, span_every: int, rot: int = 0, figsize=None
```

## Comparing `missing_mga-0.4.3.dist-info/LICENSE` & `missing_mga-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `missing_mga-0.4.3.dist-info/METADATA` & `missing_mga-1.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missing_mga
-Version: 0.4.3
+Version: 1.0.0
 Summary: A package for handling missing values in datasets.
 Home-page: https://github.com/Mgobeaalcoba/missing_mga
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

