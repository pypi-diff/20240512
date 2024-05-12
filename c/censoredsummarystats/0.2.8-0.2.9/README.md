# Comparing `tmp/censoredsummarystats-0.2.8.tar.gz` & `tmp/censoredsummarystats-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censoredsummarystats-0.2.8.tar", max compression
+gzip compressed data, was "censoredsummarystats-0.2.9.tar", max compression
```

## Comparing `censoredsummarystats-0.2.8.tar` & `censoredsummarystats-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       58 2023-06-21 09:23:06.539217 censoredsummarystats-0.2.8/censoredsummarystats/__init__.py
--rw-r--r--   0        0        0     7707 2023-06-24 22:57:00.053048 censoredsummarystats-0.2.8/censoredsummarystats/interval_to_result.py
--rw-r--r--   0        0        0     3347 2023-06-24 15:44:48.413793 censoredsummarystats-0.2.8/censoredsummarystats/merge_count_info.py
--rw-r--r--   0        0        0     5009 2023-06-24 15:44:48.419795 censoredsummarystats-0.2.8/censoredsummarystats/percent_exceedance.py
--rw-r--r--   0        0        0     2466 2023-06-24 15:44:48.428794 censoredsummarystats-0.2.8/censoredsummarystats/precision.py
--rw-r--r--   0        0        0    15228 2023-06-24 15:44:48.435796 censoredsummarystats-0.2.8/censoredsummarystats/stat_interval_aggregation.py
--rw-r--r--   0        0        0    14298 2023-06-24 22:57:00.060493 censoredsummarystats-0.2.8/censoredsummarystats/statistics.py
--rw-r--r--   0        0        0     6055 2023-06-24 15:44:48.450797 censoredsummarystats-0.2.8/censoredsummarystats/validation.py
--rw-r--r--   0        0        0    11558 2023-06-21 07:54:57.796594 censoredsummarystats-0.2.8/LICENSE
--rw-r--r--   0        0        0      575 2023-06-24 23:04:34.640492 censoredsummarystats-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     8600 2023-06-24 15:44:48.385792 censoredsummarystats-0.2.8/README.md
--rw-r--r--   0        0        0     9265 1970-01-01 00:00:00.000000 censoredsummarystats-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-06-21 09:23:06.539217 censoredsummarystats-0.2.9/censoredsummarystats/__init__.py
+-rw-r--r--   0        0        0     7459 2023-08-13 11:21:53.642793 censoredsummarystats-0.2.9/censoredsummarystats/interval_to_result.py
+-rw-r--r--   0        0        0     3347 2023-06-24 15:44:48.413793 censoredsummarystats-0.2.9/censoredsummarystats/merge_count_info.py
+-rw-r--r--   0        0        0     5020 2023-08-13 11:21:53.657794 censoredsummarystats-0.2.9/censoredsummarystats/percent_exceedance.py
+-rw-r--r--   0        0        0     2531 2023-08-13 11:21:53.668794 censoredsummarystats-0.2.9/censoredsummarystats/precision.py
+-rw-r--r--   0        0        0    15501 2023-08-13 11:21:53.694795 censoredsummarystats-0.2.9/censoredsummarystats/stat_interval_aggregation.py
+-rw-r--r--   0        0        0    25218 2023-08-13 11:21:53.717797 censoredsummarystats-0.2.9/censoredsummarystats/statistics.py
+-rw-r--r--   0        0        0     5892 2023-08-13 11:21:53.733800 censoredsummarystats-0.2.9/censoredsummarystats/validation.py
+-rw-r--r--   0        0        0    11558 2023-06-21 07:54:57.796594 censoredsummarystats-0.2.9/LICENSE
+-rw-r--r--   0        0        0      575 2023-08-13 11:21:53.754800 censoredsummarystats-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    10498 2023-08-13 11:21:53.628790 censoredsummarystats-0.2.9/README.md
+-rw-r--r--   0        0        0    11124 1970-01-01 00:00:00.000000 censoredsummarystats-0.2.9/PKG-INFO
```

### Comparing `censoredsummarystats-0.2.8/censoredsummarystats/interval_to_result.py` & `censoredsummarystats-0.2.9/censoredsummarystats/interval_to_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,61 +15,55 @@
     df = stat_data.copy()
     
     # Determine the left boundary symbol
     df[cdf.interval_col] = (
         np.where(df[cdf.left_boundary_col] == 'Open','(','['))
     
     # Incorporate left and right bounds
-    if cdf.precision_rounding:
-        df[cdf.interval_col] += (
-            df[cdf.left_bound_col].apply(_string_precision) + ', ' + 
-            df[cdf.right_bound_col].apply(_string_precision)
-            )
-    else:
-        df[cdf.interval_col] += (
-            df[cdf.left_bound_col].astype(str) + ', ' + 
-            df[cdf.right_bound_col].astype(str)
-            )
+    df[cdf.interval_col] += (
+        df[cdf.left_bound_col].astype(str) + ', ' + 
+        df[cdf.right_bound_col].astype(str)
+        )
     
     # Determine the right boundary symbol
     df[cdf.interval_col] += (
         np.where(df[cdf.right_boundary_col] == 'Open',')',']'))
     
     return df
 
 def _components_from_interval(cdf, stat_data, focus_high_potential):
     
     # Create a copy of the data
     df = stat_data.copy()
     
     # Determine the midpoint for the interval if finite interval
-    df['__MidPoint__'] = (
+    df[cdf._midpoint_col] = (
         np.where((df[cdf.left_bound_col] > -np.inf) & 
                  (df[cdf.right_bound_col] < np.inf),
             0.5 * (df[cdf.left_bound_col] + df[cdf.right_bound_col]),
             np.nan
             )
         )
     
     # Start with the conditions that produce an uncensored result
     conditions = [
         # If the bounds are equal, then the result is uncensored
         (df[cdf.left_bound_col] == df[cdf.right_bound_col]) |
         # If the bounds are finite and the interval is within the 
         # precision tolerance, then the result is uncensored
-        ((df[cdf.right_bound_col] - df['__MidPoint__']) <= 
-            df['__MidPoint__'] * cdf.precision_tolerance_to_drop_censor)
+        ((df[cdf.right_bound_col] - df[cdf._midpoint_col]) <= 
+            df[cdf._midpoint_col] * cdf.precision_tolerance_to_drop_censor)
         ]
     
     censor_results = [
         ''
         ]
     
     numeric_results =[
-        df['__MidPoint__']
+        df[cdf._midpoint_col]
         ]
     
     # If focused on the highest potential result
     if focus_high_potential:
         # Set censor and numeric components for each condition
         conditions += [
             # If there is an infinite right bound,
@@ -131,19 +125,19 @@
                 (df[cdf.left_bound_col] == lower_bound) & 
                 (df[cdf.right_bound_col] < np.inf) & 
                 (df[cdf.right_boundary_col] == 'Closed')
             ),
             # Otherwise, the result is right censored
             # where closed boundary indicates potential equality
             (
-                (df[cdf.left_bound_col] > lower_bound) &
+                (df[cdf.left_bound_col] > -np.inf) &
                 (df[cdf.left_boundary_col] == 'Open')
             ),
             (
-                (df[cdf.left_bound_col] > lower_bound) &
+                (df[cdf.left_bound_col] > -np.inf) &
                 (df[cdf.left_boundary_col] == 'Closed')
             )
             ]
         
         censor_results += [
             '<',
             '≤',
@@ -162,15 +156,15 @@
     # If no condition is met, default to <> and NaN
     df[cdf.censor_col] = np.select(conditions, censor_results, '<>')
     df[cdf.numeric_col] = np.select(conditions, numeric_results, np.nan)
     if cdf.precision_rounding:
         df[cdf.numeric_col] = df[cdf.numeric_col].apply(_numeric_precision)
     
     # Drop working columns
-    df = df.drop(df.filter(regex='__').columns, axis=1)
+    df = df.drop([cdf._midpoint_col], axis=1)
     
     return df
     
 def _result_from_components(cdf, stat_data):
     
     # Create a copy of the data
     df = stat_data.copy()
```

### Comparing `censoredsummarystats-0.2.8/censoredsummarystats/merge_count_info.py` & `censoredsummarystats-0.2.9/censoredsummarystats/merge_count_info.py`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.8/censoredsummarystats/percent_exceedance.py` & `censoredsummarystats-0.2.9/censoredsummarystats/percent_exceedance.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,28 +91,28 @@
                          round_to):
     
     # Within groups, count exceedances, determinate values, and all values
     # including indeterminate
     df = (df.groupby(groupby_cols)
           .agg(**{
               cdf.exceedances_col: (cdf.exceedances_col,'sum'),
-              '__DeterminedCount__': (cdf.exceedances_col,'count'),
-              '__TotalCount__': (cdf.exceedances_col,'size')
+              cdf._determined_col: (cdf.exceedances_col,'count'),
+              cdf._totalcount_col: (cdf.exceedances_col,'size')
             })
         )
     
     # Determine counts of non-exceedances and ignored/dropped values
     df[cdf.non_exceedances_col] = (
-        df['__DeterminedCount__'] - df[cdf.exceedances_col]
+        df[cdf._determined_col] - df[cdf.exceedances_col]
         )
-    df[cdf.ignored_col] = df['__TotalCount__'] - df['__DeterminedCount__']
+    df[cdf.ignored_col] = df[cdf._totalcount_col] - df[cdf._determined_col]
     
     # Calculate percentage and round
     df[cdf.numeric_col] = (
-        round(df[cdf.exceedances_col] / df['__DeterminedCount__'] * 100,
+        round(df[cdf.exceedances_col] / df[cdf._determined_col] * 100,
               round_to)
         )
     # Create result and included count of dropped values
     df[cdf.result_col] = df[cdf.numeric_col].astype(str) + '%'
     df.loc[df[cdf.ignored_col] > 0, cdf.result_col] = (
         df[cdf.result_col] +
         ' (' + df[cdf.ignored_col].astype(str) + ' value(s) ignored)'
@@ -123,12 +123,12 @@
     if threshold_is_exceedance:
         df[cdf.threshold_col] = '<' + df[cdf.threshold_col]
     
     # Reset index
     df = df.reset_index()
     
     # Drop working columns
-    df = df.drop(df.filter(regex='__').columns, axis=1)
+    df = df.drop([cdf._determined_col, cdf._totalcount_col], axis=1)
     
     return df
```

### Comparing `censoredsummarystats-0.2.8/censoredsummarystats/precision.py` & `censoredsummarystats-0.2.9/censoredsummarystats/precision.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,33 +24,36 @@
     Returns
     -------
     string : string
         The rounded value expressed as a string to the appropriate precision.
 
     '''
     
+    # Calculate the absolute value
+    abs_value = abs(value)
+    
     # Check for infinite values
-    if abs(value) == np.inf:
+    if abs_value == np.inf:
         string = str(value)
     # Values above 100 or are rounded to 100 should be rounded to 3 significant digits
-    elif round(abs(value),1) >= 100:
+    elif round(abs_value,1) >= 100:
         string = f'{value:.3g}'
         # Include thousands separator, depending on input
         if thousands_comma:
             string = f'{int(float(string)):,}'
         else:
             string = str(int(float(string)))
     # Values above 10 or are rounded to 10 should be rounded to 1 decimal place
-    elif round(abs(value),2) >= 10:
+    elif round(abs_value,2) >= 10:
         string = f'{value:.1f}'
     # Values above 0.2 or are rounded to 0.2 should be rounded to 2 decimal places
-    elif round(abs(value),3) >= 0.2:
+    elif round(abs_value,3) >= 0.2:
         string = f'{value:.2f}'
     # Values above 0.1 or are rounded to 0.1 should be rounded to 3 decimal places
-    elif round(abs(value),3) >= 0.1:
+    elif round(abs_value,3) >= 0.1:
         string = f'{value:.3f}'
     # Values below 0.1 should be rounded to 2 significant digits
     else:
         string = f'{value:.2g}'
 
     return string
```

### Comparing `censoredsummarystats-0.2.8/censoredsummarystats/stat_interval_aggregation.py` & `censoredsummarystats-0.2.9/censoredsummarystats/stat_interval_aggregation.py`

 * *Files 9% similar despite different names*

```diff
@@ -156,45 +156,45 @@
     # the bound mean/sum, then the resulting mean/sum should be open
     # Determine the min and max of the bounds to correct situations where
     # the bound is infinite
     df = (
         df.groupby(groupby_cols + [cdf.stat_col])
             .agg(**{
                 cdf.left_boundary_col: (cdf.left_boundary_col, 'max'),
-                '__Minimum__': (cdf.left_bound_col, 'min'),
+                cdf._minimum_col: (cdf.left_bound_col, 'min'),
                 cdf.left_bound_col: (cdf.left_bound_col, stat),
                 cdf.right_bound_col: (cdf.right_bound_col, stat),
-                '__Maximum__': (cdf.right_bound_col, 'max'),
+                cdf._maximum_col: (cdf.right_bound_col, 'max'),
                 cdf.right_boundary_col: (cdf.right_boundary_col, 'max')
                 })
         )
     
     # Replace integers with text for boundaries
     df[[cdf.left_boundary_col, cdf.right_boundary_col]] = (
         df[[cdf.left_boundary_col, cdf.right_boundary_col]]
             .replace([0,1], ['Closed','Open']))
     
     # Means/sums with infinite values produce nan values rather than 
     # np.inf values. Convert nan to inf only if infinite values are
     # included in the mean/sum
     df[cdf.left_bound_col] = (
-        np.where(df['__Minimum__'] == -np.inf,
+        np.where(df[cdf._minimum_col] == -np.inf,
                  -np.inf,
                  df[cdf.left_bound_col]
                  )
         )
     df[cdf.right_bound_col] = (
-        np.where(df['__Maximum__'] == np.inf,
+        np.where(df[cdf._maximum_col] == np.inf,
                  np.inf,
                  df[cdf.right_bound_col]
                  )
         )
     
     # Drop working columns
-    df = df.drop(df.filter(regex='__').columns, axis=1)
+    df = df.drop([cdf._minimum_col, cdf._maximum_col], axis=1)
     
     # Reset index
     df = df.reset_index()
     
     return df
 
 def _mean_interval(cdf, data, groupby_cols, stat_name='Mean'):
@@ -235,32 +235,32 @@
     # https://en.wikipedia.org/wiki/Percentile
     C = method_dict[method]
     
     # Convert percentile to be between 0 and 1
     percentile = percentile/100
     
     # Create column for the size of each group
-    df['__Size__'] = (df.groupby(groupby_cols + [cdf.stat_col])
+    df[cdf._size_col] = (df.groupby(groupby_cols + [cdf.stat_col])
                         .transform('size'))
     
     # Determine the rank in each group for the percentile
     # Use rounding at 8 decimals to prevent artificial decimals
-    df['__Rank__'] = round(C + percentile*(df['__Size__'] + 1 - 2*C), 8)
+    df[cdf._rank_col] = round(C + percentile*(df[cdf._size_col] + 1 - 2*C), 8)
     
     # Create warning column to flag if the percentile rank is outside
     # the range of possible values. If rank is less than 1, the minimum will
     # be returned for the percentile; if the rank is greater than the size
     # of the group, the maximum will be returned.
     df[cdf.warning_col] = ''
-    max_condition = (df['__Rank__'] > df['__Size__'])
-    min_condition = (df['__Rank__'] < 1)
+    max_condition = (df[cdf._rank_col] > df[cdf._size_col])
+    min_condition = (df[cdf._rank_col] < 1)
     df.loc[max_condition, cdf.warning_col] = '(low count, used max)'
     df.loc[min_condition, cdf.warning_col] = '(low count, used min)'
-    df.loc[max_condition, '__Rank__'] = df['__Size__']
-    df.loc[min_condition, '__Rank__'] = 1
+    df.loc[max_condition, cdf._rank_col] = df[cdf._size_col]
+    df.loc[min_condition, cdf._rank_col] = 1
     
     # For the left bound, change notation of Closed and Open boundaries to 0
     # and 1, respectively. Use 0 for Closed to ensure that Closed boundaries
     # are sorted smaller than Open boundaries when the left bound is tied
     df[cdf.left_boundary_col] = (
         df[cdf.left_boundary_col].replace(['Closed','Open'], [0,1]))
     
@@ -270,122 +270,124 @@
     df[cdf.right_boundary_col] = (
         df[cdf.right_boundary_col].replace(['Closed','Open'], [1,0]))
     
     # Sort the left and right bounds
     # Reduce working dataframes to relevant columns
     left = (
         df.copy()[groupby_cols + [cdf.stat_col] +
-                  ['__Size__', '__Rank__', cdf.warning_col] +
+                  [cdf._size_col, cdf._rank_col, cdf.warning_col] +
                   [cdf.left_boundary_col, cdf.left_bound_col]]
             .sort_values(
                 by = [cdf.left_bound_col, cdf.left_boundary_col]
                 )
         )
     right = (
         df.copy()[groupby_cols + [cdf.stat_col] +
-                  ['__Size__', '__Rank__', cdf.warning_col] +
+                  [cdf._size_col, cdf._rank_col, cdf.warning_col] +
                   [cdf.right_boundary_col, cdf.right_bound_col]]
             .sort_values(
                 by = [cdf.right_bound_col, cdf.right_boundary_col]
                 )
         )
     
     # Add index for each group
-    left['__Index__'] = (left.groupby(groupby_cols + [cdf.stat_col])
+    left[cdf._index_col] = (left.groupby(groupby_cols + [cdf.stat_col])
                              .cumcount() + 1)
-    right['__Index__'] = (right.groupby(groupby_cols + [cdf.stat_col])
+    right[cdf._index_col] = (right.groupby(groupby_cols + [cdf.stat_col])
                                .cumcount() + 1)
     
     def find_values_within_one_of_rank(df):
         
         # Determine proximity of each result to percentile rank using the index
         
         # Set default as 0
-        df['__Proximity__'] = 0
+        df[cdf._proximity_col] = 0
         
         condition_set = [
             # If the percentile rank is a whole number,
             # then use that index result
-            (df['__Rank__'] == df['__Index__']),
+            (df[cdf._rank_col] == df[cdf._index_col]),
             # If the percentile rank is less than 1 above the index value,
             # then assign the appropriate contribution to that index value
-            ((df['__Rank__'] - df['__Index__'])
+            ((df[cdf._rank_col] - df[cdf._index_col])
                                          .between(0,1,inclusive='neither')),
             # If the percentile rank is less than 1 below the index value,
             # then assign the appropriate contribution to that index value
-            ((df['__Index__'] - df['__Rank__'])
+            ((df[cdf._index_col] - df[cdf._rank_col])
                                          .between(0,1,inclusive='neither'))
             ]
         
         proximities = [
             1,
-            1 - (df['__Rank__'] - df['__Index__']),
-            1 - (df['__Index__'] - df['__Rank__'])
+            1 - (df[cdf._rank_col] - df[cdf._index_col]),
+            1 - (df[cdf._index_col] - df[cdf._rank_col])
             ]
         
         # Set proximity of each result to rank
-        df['__Proximity__'] = np.select(condition_set, proximities, np.nan)
+        df[cdf._proximity_col] = np.select(condition_set, proximities, np.nan)
         
         # Drop non-contributing rows
-        df = df[df['__Proximity__'] > 0]
+        df = df[df[cdf._proximity_col] > 0]
         
         return df
     
     left = find_values_within_one_of_rank(left)
     right = find_values_within_one_of_rank(right)
     
     # Calculate contribution for using proximity to rank
-    left['__Contribution__'] = (
-        left['__Proximity__'] * left[cdf.left_bound_col])
-    right['__Contribution__'] = (
-        right['__Proximity__'] * right[cdf.right_bound_col])
+    left[cdf._contribution_col] = (
+        left[cdf._proximity_col] * left[cdf.left_bound_col])
+    right[cdf._contribution_col] = (
+        right[cdf._proximity_col] * right[cdf.right_bound_col])
     
     # Determine bound and boundary using the sum of the contributions
     # and an open boundary if any of the contributing values is open
     # Replace nan sums with infinite bound
     left = (
         left.groupby(groupby_cols + [cdf.stat_col, cdf.warning_col])
             .agg(**{
                 cdf.left_boundary_col: (cdf.left_boundary_col, 'max'),
-                cdf.left_bound_col: ('__Contribution__', 'sum'),
-                '__Minimum__': ('__Contribution__', 'min')
+                cdf.left_bound_col: (cdf._contribution_col, 'sum'),
+                cdf._minimum_col: (cdf._contribution_col, 'min')
                 }))
     right = (
         right.groupby(groupby_cols + [cdf.stat_col, cdf.warning_col])
             .agg(**{
-                cdf.right_bound_col: ('__Contribution__', 'sum'),
+                cdf.right_bound_col: (cdf._contribution_col, 'sum'),
                 cdf.right_boundary_col: (cdf.right_boundary_col, 'min'),
-                '__Maximum__': ('__Contribution__', 'max')
+                cdf._maximum_col: (cdf._contribution_col, 'max')
                 }))
     
     # Replace the numeric value for the boundary
     left[cdf.left_boundary_col] = (
         left[cdf.left_boundary_col].replace([0,1], ['Closed','Open']))
     right[cdf.right_boundary_col] = (
         right[cdf.right_boundary_col].replace([1,0], ['Closed','Open']))
     
     # Replace nan bounds with infinite bound
     left[cdf.left_bound_col] = (
-        np.where(left['__Minimum__'] == -np.inf, -np.inf,
+        np.where(left[cdf._minimum_col] == -np.inf, -np.inf,
                  left[cdf.left_bound_col]))
     right[cdf.right_bound_col] = (
-        np.where(right['__Maximum__'] == np.inf, np.inf,
+        np.where(right[cdf._maximum_col] == np.inf, np.inf,
                  right[cdf.right_bound_col]))
     
     
     # Merge the two boundaries to create the interval for the percentile
     # Check that the merge is 1-to-1
     df = left.merge(right,
                     how = 'outer',
                     on = groupby_cols + [cdf.stat_col, cdf.warning_col],
                     validate = '1:1'
                     )
     
     # Drop working columns
-    df = df.drop(df.filter(regex='__').columns, axis=1)
+    df = df.drop([cdf._minimum_col, cdf._maximum_col,
+                  cdf._size_col, cdf._rank_col, cdf._index_col,
+                  cdf._proximity_col, cdf._contribution_col], axis=1)
     
     # Reset index
     df = df.reset_index()
     
     return df
 
 def _median_interval(cdf, data, groupby_cols, stat_name='Median'):
```

### Comparing `censoredsummarystats-0.2.8/censoredsummarystats/validation.py` & `censoredsummarystats-0.2.9/censoredsummarystats/validation.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,38 +24,48 @@
     
     if cdf.value_col not in cdf.data.columns:
         raise ValueError('The value column supplied to CensoredData() '
             'was not found as a column in the data. Columns include '
             f'{cdf.data.columns.to_list()} which does not include '
             f'{repr(cdf.value_col)}.')
     
-    #%% Check the four stat settings
+    #%% Check the stat settings
+    
+    # Check the true/false settings
     
     boolean_settings = ['include_negative_interval',
                         'focus_high_potential',
                         'precision_rounding',
                         'thousands_comma',
                         'output_interval']
     
     for setting in boolean_settings:
         setting_mode = getattr(cdf, setting)
         if not isinstance(setting_mode, bool):
             raise ValueError(f'The value supplied to {setting} must be '
                 'True or False. Instead, the value supplied was '
                 f'{repr(setting_mode)}.')
     
+    # Check precision_tolerance_to_drop_censor is numeric
     # True or False are considered integer types so check for boolean too
     if ((isinstance(cdf.precision_tolerance_to_drop_censor, bool)) |
         (not isinstance(cdf.precision_tolerance_to_drop_censor,
                        (int, float)))):
         raise ValueError(f'The value supplied to '
             'precision_tolerance_to_drop_censor must be numeric. Instead, '
             'the value supplied was '
             f'{repr(cdf.precision_tolerance_to_drop_censor)}.')
     
+    # Check precision_tolerance_to_drop_censor is non-negative
+    if cdf.precision_tolerance_to_drop_censor < 0:
+        raise ValueError(f'The value supplied to '
+            'precision_tolerance_to_drop_censor must be non-negative. '
+            'The value supplied was '
+            f'{repr(cdf.precision_tolerance_to_drop_censor)}.')
+    
     #%% Check column names for conflicts
     
     # Check that columns created within methods don't conflict with column
     # names in provided data
     # Check that new column names are string values
     
     # Create list of column names that may be created
@@ -79,21 +89,14 @@
                 f'{col} when initialising CensoredDataFrame.')
         
         if not isinstance(col_name, str):
             raise ValueError('Text values are required for column names. '
                 f'The column name {col_name} should be changed to a text '
                 f'value for {col}.')
     
-    # Check that the data has no columns starting with double underscore
-    dunder_cols = [col for col in cdf.data if col.startswith('__')]
-    if len(dunder_cols) != 0:
-        raise ValueError('Columns starting with "__" are used within '
-            'the stat methods. Rename the following columns: '
-            f'{dunder_cols}')
-    
     #%% Check that there are no nan values or empty strings
     if ((cdf.data[cdf.value_col].isnull().any()) |
         (cdf.data[cdf.value_col].astype(str).str.len().min() == 0)):
         raise ValueError('Missing values need to be removed from the data '
             'before it can be analysed.')
 
 #%% Groupby validation
@@ -127,26 +130,7 @@
                     f'groups: {errors}')
         
         # Check for null values in groupby columns
         if cdf.data[groupby_cols[0]].isnull().values.any():
             raise ValueError('Null values found in one of the columns used '
                 'for grouping.')
             
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-            
-
```

### Comparing `censoredsummarystats-0.2.8/LICENSE` & `censoredsummarystats-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `censoredsummarystats-0.2.8/pyproject.toml` & `censoredsummarystats-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "censoredsummarystats"
-version = "0.2.8"
+version = "0.2.9"
 description = "A python package for calculating summary stats on censored data (data that contains < and > symbols)."
 authors = ["Kurt van Ness <vanness.kurt@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/kurtvanness/CensoredSummaryStats"
 license = "Apache-2.0"
 packages = [{include = "censoredsummarystats"}]
```

### Comparing `censoredsummarystats-0.2.8/README.md` & `censoredsummarystats-0.2.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 - **censor_col**: (default 'CensorComponent') This column contains the censor component for statistical results.
 - **numeric_col**: (default 'NumericComponent') This column contains the numeric component for statistical results.
 - **interval_col**: (default 'Interval') This column contains the possible range of the statistical result when considering all possibilities of censored values.
 - **threshold_col**: (default 'Threshold') This column contains the threshold supplied by the user for the percent_exceedances method.
 - **exceedances_col**: (default 'Exceedances') This column contains the number of exceedances resulting from the percent_exceedances method.
 - **non_exceedances_col**: (default 'NonExceedances') This column contains the number of non-exceedances resulting from the percent_exceedances method.
 - **ignored_col**: (default 'Ignored') This column contains the number of values that couldn't be assessed for the percent_exceedances method. For example, a value of '<2' cannot be determined as being above or below 1. Users should manually adjust values to be above or below the supplied threshold if they need to be considered.
+- **warning_col**: (default 'Warning') This column is only generated for percentiles under certain situations.
 
 ## Precision Rounding approach:
 
 There is a built in rounding option that is based on common water quality reporting measurement precision. 
 
 | NumericComponent  | Rounding process |
 | ------------- | ------------- |
@@ -70,14 +71,18 @@
 Many of the methods above have similar input parameters. Those are:
 
 - **groupby_cols**: (default None) These are the columns that should be used to define the groups. Multiple groupings can be provided for some functions. This is useful to even weight data over sites or time periods. For example, a potential input for could be [['Year','Month','Day'], ['Year','Month'], ['Year']]. This would ensure that all days are evenly weighted within the month and that all months are evenly weighted within the year for a stat such as mean or median.
 - **count_cols**: (default None) Supplying a list of strings here will cause methods to return value counts. There should be the same number of strings as there are groupings in groupby_cols. Using the same example for groupby_cols, a user could supply ['Samples', 'Days Sampled', 'Months Sampled'] to get value counts for each grouping.
 - **stat_name**: (default is statistic) The text to use to describe the stat ('Minimum', 'Median', etc.)
 - **filters**: (default None) A dictionary of column names with values to filter for. This allows some simple filtering without recreating CensoredData objects.
 
+The percentile function has the following additional input parameters:
+- **percentile**: The percentile that should be determined. The supplied value needs to be between 0 and 100.
+- **method**: (default hazen) The percentile method to use. Options include: 'weibull', 'tukey', 'blom', 'hazen', 'excel'.
+
 ## Dependencies
 
 For the installation of `censoredsummarystats`, the following packages are required:
 - [numpy >= 1.24](https://www.numpy.org/)
 
 ## Installation
 
@@ -85,52 +90,86 @@
 
 ```python
 pip install censoredsummarystats
 ```
 
 ## Usage
 
-A quick example of `censoredsummarystats` usage is given below.
+An example of `censoredsummarystats` usage is given below.
 
 ```python
 import pandas as pd
 import censoredsummarystats as css
 
 # Create DataFrame
-df = pd.DataFrame([['Set1',1.5],['Set1','2'],['Set1','>2.5'],['Set2',2],['Set2','<3'],['Set2',7.0]],columns=['Groups','Results'])
-
-Groups Results
-0   Set1     1.5
-1   Set1       2
-2   Set1    >2.5
-3   Set2       2
-4   Set2      <3
-5   Set2     7.0
+df = pd.DataFrame([
+    ['Site1','E. coli', 2021, '<1'],
+    ['Site1','E. coli', 2021, '<1'],
+    ['Site1','E. coli', 2022, 455],
+    ['Site1','E. coli', 2022, '>2420'],
+    ['Site1','E. coli', 2022, 257],
+    ['Site2','E. coli', 2021, 5],
+    ['Site2','E. coli', 2021, '>2420'],
+    ['Site2','E. coli', 2022, '<10'],
+    ['Site2','E. coli', 2022, 17000],
+    ['Site2','Temperature', 2022, 12.4]
+    ],
+    columns=['SiteID','Parameter','Year','Result'])
+
+  SiteID    Parameter  Year Result
+0  Site1      E. coli  2021     <1
+1  Site1      E. coli  2021     <1
+2  Site1      E. coli  2022    455
+3  Site1      E. coli  2022  >2420
+4  Site1      E. coli  2022    257
+5  Site2      E. coli  2021      5
+6  Site2      E. coli  2021  >2420
+7  Site2      E. coli  2022    <10
+8  Site2      E. coli  2022  17000
+9  Site2  Temperature  2022   12.4
 
 # Create CensoredData object from dataframe
-cdf = css.CensoredData(data=df,value_col='Results')
-
-# Calculate minimums, averages, and medians for the data
-minimums = cdf.minimum(groupby_cols=['Groups'])
+cdf = css.CensoredData(data=df,value_col='Result')
 
-averages = cdf.mean(groupby_cols=['Groups'])
+# Calculate annual maximums
+annual_maximums = cdf.maximum(groupby_cols=[['SiteID','Parameter','Year']],
+                                count_cols=['Samples'],
+                                stat_name='Annual Maximum')
+
+# Calculate the maximum concentrations of E. coli measured at each site
+site_ecoli_maximums = cdf.maximum(groupby_cols=[['SiteID','Year'],['SiteID']],
+                                count_cols=['Samples','YearsSampled'],
+                                stat_name='Site Maximum',
+                                filters = {'Parameter':['E. coli']})
+
+# Calculate the annual averages
+annual_averages = cdf.average(groupby_cols=[['SiteID','Parameter','Year']],
+                                count_cols=['Samples'],
+                                stat_name='Annual Average')
 
-medians = cdf.median(groupby_cols=['Groups'])
 ```
-Output are like this:
+Outputs are like this:
 ```python
-print(minimums)
-  Groups Statistic Result CensorComponent  NumericComponent      Interval
-0   Set1   Minimum   1.50                               1.5  [1.50, 1.50]
-1   Set2   Minimum  ≤2.00               ≤               2.0     [0, 2.00]
-
-print(averages)
-  Groups Statistic Result CensorComponent  NumericComponent      Interval
-0   Set1      Mean  >2.00               >               2.0   (2.00, inf)
-1   Set2      Mean   3.50                               3.5  [3.00, 4.00)
-
-print(medians)
-  Groups Statistic Result CensorComponent  NumericComponent      Interval
-0   Set1    Median   2.00                               2.0  [2.00, 2.00]
-1   Set2    Median   2.50                               2.5  [2.00, 3.00)
+print(annual_maximums)
+	SiteID	Parameter	Year	Statistic	Result	Interval	Samples
+0	Site1	E. coli	        2021	Annual Maximum	<1	[0, 1)	        2
+1	Site1	E. coli	        2022	Annual Maximum	>2420	(2420, inf)	3
+2	Site2	E. coli	        2021	Annual Maximum	>2420	(2420, inf)	2
+3	Site2	E. coli	        2022	Annual Maximum	17000	[17000, 17000]	2
+4	Site2	Temperature	2022	Annual Maximum	12.4    [12.4, 12.4]	1
+
+
+print(site_ecoli_maximums)
+	SiteID	Statistic	Result	Interval	Samples	YearsSampled
+0	Site1	Site Maximum	>2420	(2420, inf)	5	2
+1	Site2	Site Maximum	≥17000	[17000, inf)	4	2
+
+
+print(annual_averages)
+	SiteID	Parameter	Year	Statistic	Result	Interval	Samples
+0	Site1	E. coli	        2021	Annual Average	<1	[0, 1)	        2
+1	Site1	E. coli	        2022	Annual Average	>1040	(1044, inf)	3
+2	Site2	E. coli	        2021	Annual Average	>1210	(1212.5, inf)	2
+3	Site2	E. coli	        2022	Annual Average	8500	[8500, 8505)	2
+4	Site2	Temperature	2022	Annual Average	12.4	[12.4, 12.4]	1
 ```
```

### Comparing `censoredsummarystats-0.2.8/PKG-INFO` & `censoredsummarystats-0.2.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censoredsummarystats
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python package for calculating summary stats on censored data (data that contains < and > symbols).
 Home-page: https://github.com/kurtvanness/CensoredSummaryStats
 License: Apache-2.0
 Author: Kurt van Ness
 Author-email: vanness.kurt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -45,14 +45,15 @@
 - **censor_col**: (default 'CensorComponent') This column contains the censor component for statistical results.
 - **numeric_col**: (default 'NumericComponent') This column contains the numeric component for statistical results.
 - **interval_col**: (default 'Interval') This column contains the possible range of the statistical result when considering all possibilities of censored values.
 - **threshold_col**: (default 'Threshold') This column contains the threshold supplied by the user for the percent_exceedances method.
 - **exceedances_col**: (default 'Exceedances') This column contains the number of exceedances resulting from the percent_exceedances method.
 - **non_exceedances_col**: (default 'NonExceedances') This column contains the number of non-exceedances resulting from the percent_exceedances method.
 - **ignored_col**: (default 'Ignored') This column contains the number of values that couldn't be assessed for the percent_exceedances method. For example, a value of '<2' cannot be determined as being above or below 1. Users should manually adjust values to be above or below the supplied threshold if they need to be considered.
+- **warning_col**: (default 'Warning') This column is only generated for percentiles under certain situations.
 
 ## Precision Rounding approach:
 
 There is a built in rounding option that is based on common water quality reporting measurement precision. 
 
 | NumericComponent  | Rounding process |
 | ------------- | ------------- |
@@ -89,14 +90,18 @@
 Many of the methods above have similar input parameters. Those are:
 
 - **groupby_cols**: (default None) These are the columns that should be used to define the groups. Multiple groupings can be provided for some functions. This is useful to even weight data over sites or time periods. For example, a potential input for could be [['Year','Month','Day'], ['Year','Month'], ['Year']]. This would ensure that all days are evenly weighted within the month and that all months are evenly weighted within the year for a stat such as mean or median.
 - **count_cols**: (default None) Supplying a list of strings here will cause methods to return value counts. There should be the same number of strings as there are groupings in groupby_cols. Using the same example for groupby_cols, a user could supply ['Samples', 'Days Sampled', 'Months Sampled'] to get value counts for each grouping.
 - **stat_name**: (default is statistic) The text to use to describe the stat ('Minimum', 'Median', etc.)
 - **filters**: (default None) A dictionary of column names with values to filter for. This allows some simple filtering without recreating CensoredData objects.
 
+The percentile function has the following additional input parameters:
+- **percentile**: The percentile that should be determined. The supplied value needs to be between 0 and 100.
+- **method**: (default hazen) The percentile method to use. Options include: 'weibull', 'tukey', 'blom', 'hazen', 'excel'.
+
 ## Dependencies
 
 For the installation of `censoredsummarystats`, the following packages are required:
 - [numpy >= 1.24](https://www.numpy.org/)
 
 ## Installation
 
@@ -104,53 +109,87 @@
 
 ```python
 pip install censoredsummarystats
 ```
 
 ## Usage
 
-A quick example of `censoredsummarystats` usage is given below.
+An example of `censoredsummarystats` usage is given below.
 
 ```python
 import pandas as pd
 import censoredsummarystats as css
 
 # Create DataFrame
-df = pd.DataFrame([['Set1',1.5],['Set1','2'],['Set1','>2.5'],['Set2',2],['Set2','<3'],['Set2',7.0]],columns=['Groups','Results'])
-
-Groups Results
-0   Set1     1.5
-1   Set1       2
-2   Set1    >2.5
-3   Set2       2
-4   Set2      <3
-5   Set2     7.0
+df = pd.DataFrame([
+    ['Site1','E. coli', 2021, '<1'],
+    ['Site1','E. coli', 2021, '<1'],
+    ['Site1','E. coli', 2022, 455],
+    ['Site1','E. coli', 2022, '>2420'],
+    ['Site1','E. coli', 2022, 257],
+    ['Site2','E. coli', 2021, 5],
+    ['Site2','E. coli', 2021, '>2420'],
+    ['Site2','E. coli', 2022, '<10'],
+    ['Site2','E. coli', 2022, 17000],
+    ['Site2','Temperature', 2022, 12.4]
+    ],
+    columns=['SiteID','Parameter','Year','Result'])
+
+  SiteID    Parameter  Year Result
+0  Site1      E. coli  2021     <1
+1  Site1      E. coli  2021     <1
+2  Site1      E. coli  2022    455
+3  Site1      E. coli  2022  >2420
+4  Site1      E. coli  2022    257
+5  Site2      E. coli  2021      5
+6  Site2      E. coli  2021  >2420
+7  Site2      E. coli  2022    <10
+8  Site2      E. coli  2022  17000
+9  Site2  Temperature  2022   12.4
 
 # Create CensoredData object from dataframe
-cdf = css.CensoredData(data=df,value_col='Results')
-
-# Calculate minimums, averages, and medians for the data
-minimums = cdf.minimum(groupby_cols=['Groups'])
+cdf = css.CensoredData(data=df,value_col='Result')
 
-averages = cdf.mean(groupby_cols=['Groups'])
+# Calculate annual maximums
+annual_maximums = cdf.maximum(groupby_cols=[['SiteID','Parameter','Year']],
+                                count_cols=['Samples'],
+                                stat_name='Annual Maximum')
+
+# Calculate the maximum concentrations of E. coli measured at each site
+site_ecoli_maximums = cdf.maximum(groupby_cols=[['SiteID','Year'],['SiteID']],
+                                count_cols=['Samples','YearsSampled'],
+                                stat_name='Site Maximum',
+                                filters = {'Parameter':['E. coli']})
+
+# Calculate the annual averages
+annual_averages = cdf.average(groupby_cols=[['SiteID','Parameter','Year']],
+                                count_cols=['Samples'],
+                                stat_name='Annual Average')
 
-medians = cdf.median(groupby_cols=['Groups'])
 ```
-Output are like this:
+Outputs are like this:
 ```python
-print(minimums)
-  Groups Statistic Result CensorComponent  NumericComponent      Interval
-0   Set1   Minimum   1.50                               1.5  [1.50, 1.50]
-1   Set2   Minimum  ≤2.00               ≤               2.0     [0, 2.00]
-
-print(averages)
-  Groups Statistic Result CensorComponent  NumericComponent      Interval
-0   Set1      Mean  >2.00               >               2.0   (2.00, inf)
-1   Set2      Mean   3.50                               3.5  [3.00, 4.00)
-
-print(medians)
-  Groups Statistic Result CensorComponent  NumericComponent      Interval
-0   Set1    Median   2.00                               2.0  [2.00, 2.00]
-1   Set2    Median   2.50                               2.5  [2.00, 3.00)
+print(annual_maximums)
+	SiteID	Parameter	Year	Statistic	Result	Interval	Samples
+0	Site1	E. coli	        2021	Annual Maximum	<1	[0, 1)	        2
+1	Site1	E. coli	        2022	Annual Maximum	>2420	(2420, inf)	3
+2	Site2	E. coli	        2021	Annual Maximum	>2420	(2420, inf)	2
+3	Site2	E. coli	        2022	Annual Maximum	17000	[17000, 17000]	2
+4	Site2	Temperature	2022	Annual Maximum	12.4    [12.4, 12.4]	1
+
+
+print(site_ecoli_maximums)
+	SiteID	Statistic	Result	Interval	Samples	YearsSampled
+0	Site1	Site Maximum	>2420	(2420, inf)	5	2
+1	Site2	Site Maximum	≥17000	[17000, inf)	4	2
+
+
+print(annual_averages)
+	SiteID	Parameter	Year	Statistic	Result	Interval	Samples
+0	Site1	E. coli	        2021	Annual Average	<1	[0, 1)	        2
+1	Site1	E. coli	        2022	Annual Average	>1040	(1044, inf)	3
+2	Site2	E. coli	        2021	Annual Average	>1210	(1212.5, inf)	2
+3	Site2	E. coli	        2022	Annual Average	8500	[8500, 8505)	2
+4	Site2	Temperature	2022	Annual Average	12.4	[12.4, 12.4]	1
 ```
```

