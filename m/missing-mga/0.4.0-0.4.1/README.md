# Comparing `tmp/missing_mga-0.4.0-py3-none-any.whl.zip` & `tmp/missing_mga-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7605 bytes, number of entries: 7
+Zip file size: 7796 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       44 b- defN 24-May-12 13:01 missing_mga/__init__.py
 -rw-r--r--  2.0 unx    18749 b- defN 24-May-12 14:40 missing_mga/missing_methods.py
--rw-r--r--  2.0 unx     1069 b- defN 24-May-12 14:55 missing_mga-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5124 b- defN 24-May-12 14:55 missing_mga-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 14:55 missing_mga-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-12 14:55 missing_mga-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      572 b- defN 24-May-12 14:55 missing_mga-0.4.0.dist-info/RECORD
-7 files, 25662 bytes uncompressed, 6587 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-12 15:04 missing_mga-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6026 b- defN 24-May-12 15:04 missing_mga-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 15:04 missing_mga-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-12 15:04 missing_mga-0.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      572 b- defN 24-May-12 15:04 missing_mga-0.4.1.dist-info/RECORD
+7 files, 26564 bytes uncompressed, 6778 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: missing_mga/__init__.py
 Comment: 
 
 Filename: missing_mga/missing_methods.py
 Comment: 
 
-Filename: missing_mga-0.4.0.dist-info/LICENSE
+Filename: missing_mga-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: missing_mga-0.4.0.dist-info/METADATA
+Filename: missing_mga-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: missing_mga-0.4.0.dist-info/WHEEL
+Filename: missing_mga-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: missing_mga-0.4.0.dist-info/top_level.txt
+Filename: missing_mga-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: missing_mga-0.4.0.dist-info/RECORD
+Filename: missing_mga-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `missing_mga-0.4.0.dist-info/LICENSE` & `missing_mga-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `missing_mga-0.4.0.dist-info/METADATA` & `missing_mga-0.4.1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missing_mga
-Version: 0.4.0
+Version: 0.4.1
 Summary: A package for handling missing values in datasets.
 Home-page: https://github.com/Mgobeaalcoba/missing_mga
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -23,28 +23,36 @@
 
 This class provides several methods for handling missing values in a DataFrame. Here's a brief explanation of each method:
 
 1. **number_missing**: Returns the total number of missing values in the DataFrame.
 2. **number_missing_by_column**: Returns the number of missing values for each column.
 3. **number_complete**: Returns the total number of complete (non-missing) values in the DataFrame.
 4. **number_complete_by_column**: Returns the number of complete values for each column.
-5. **missing_variable_summary**: Generates a summary table showing the count and percentage of missing values for each variable (column).
-6. **missing_case_summary**: Generates a summary table showing the count and percentage of missing values for each case (row).
-7. **missing_variable_table**: Generates a table showing the distribution of missing values across variables.
-8. **missing_case_table**: Generates a table showing the distribution of missing values across cases.
-9. **missing_variable_span**: Analyzes the missing values in a variable over a specified span and returns a DataFrame summarizing the percentage of missing and complete values.
-10. **missing_variable_run**: Identifies runs of missing and complete values in a specified variable and returns a DataFrame summarizing their lengths.
-11. **sort_variables_by_missingness**: Sorts the DataFrame columns based on the number of missing values in each column.
-12. **create_shadow_matrix**: Creates a shadow matrix indicating missing values with a specified string.
-13. **bind_shadow_matrix**: Binds the original DataFrame with its shadow matrix indicating missing values.
-14. **missing_scan_count**: Counts occurrences of specified values in the DataFrame and returns the counts per variable.
-15. **missing_variable_plot**: Plots a horizontal bar chart showing the number of missing values for each variable.
-16. **missing_case_plot**: Plots a histogram showing the distribution of missing values across cases.
-17. **missing_variable_span_plot**: Plots a stacked bar chart showing the percentage of missing and complete values over a repeating span for a specified variable.
-18. **missing_upsetplot**: Generates an UpSet plot to visualize the combinations of missing values across variables.
+5. **impute_mean** Input a value in the missing values of the DataFrame using the mean of each column.
+6. **impute_median** Input a value in the missing values of the DataFrame using the median of each column.
+7. **impute_mode** Input a value in the missing values of the DataFrame using the mode of each column.
+8. **impute_knn(n_neighbors=5)** Input a value in the missing values of the DataFrame using the K-Nearest Neighbors algorithm.
+9. **missing_value_heatmap** Generates a heatmap showing the distribution of missing values in the DataFrame.
+10. **missing_value_pattern** Generates a pattern showing the distribution of missing values in the DataFrame.
+11. **drop_missing_rows(thresh=0.5)** Deletes the rows that contain missing values above the specified percentage.
+12. **drop_missing_columns(thresh=0.5)** Deletes the columns that contain missing values above the specified percentage.
+13. **missing_variable_summary**: Generates a summary table showing the count and percentage of missing values for each variable (column).
+14. **missing_case_summary**: Generates a summary table showing the count and percentage of missing values for each case (row).
+15. **missing_variable_table**: Generates a table showing the distribution of missing values across variables.
+16. **missing_case_table**: Generates a table showing the distribution of missing values across cases.
+17. **missing_variable_span**: Analyzes the missing values in a variable over a specified span and returns a DataFrame summarizing the percentage of missing and complete values.
+18. **missing_variable_run**: Identifies runs of missing and complete values in a specified variable and returns a DataFrame summarizing their lengths.
+19. **sort_variables_by_missingness**: Sorts the DataFrame columns based on the number of missing values in each column.
+20. **create_shadow_matrix**: Creates a shadow matrix indicating missing values with a specified string.
+21. **bind_shadow_matrix**: Binds the original DataFrame with its shadow matrix indicating missing values.
+22. **missing_scan_count**: Counts occurrences of specified values in the DataFrame and returns the counts per variable.
+23. **missing_variable_plot**: Plots a horizontal bar chart showing the number of missing values for each variable.
+24. **missing_case_plot**: Plots a histogram showing the distribution of missing values across cases.
+25. **missing_variable_span_plot**: Plots a stacked bar chart showing the percentage of missing and complete values over a repeating span for a specified variable.
+26. **missing_upsetplot**: Generates an UpSet plot to visualize the combinations of missing values across variables.
 
 These methods provide comprehensive tools for analyzing and visualizing missing values in a DataFrame. They can be used to gain insights into the patterns and distribution of missing values, as well as to inform data cleaning and imputation strategies.
 
 ## Installation
 
 To install the package, you can use pip:
```

