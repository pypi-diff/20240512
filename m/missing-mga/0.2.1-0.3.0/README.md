# Comparing `tmp/missing_mga-0.2.1-py3-none-any.whl.zip` & `tmp/missing_mga-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7086 bytes, number of entries: 7
+Zip file size: 7085 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       44 b- defN 24-May-12 13:01 missing_mga/__init__.py
 -rw-r--r--  2.0 unx    16310 b- defN 24-May-12 12:50 missing_mga/missing_methods.py
--rw-r--r--  2.0 unx     1069 b- defN 24-May-12 13:35 missing_mga-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5105 b- defN 24-May-12 13:35 missing_mga-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 13:35 missing_mga-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-12 13:35 missing_mga-0.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      572 b- defN 24-May-12 13:35 missing_mga-0.2.1.dist-info/RECORD
-7 files, 23204 bytes uncompressed, 6068 bytes compressed:  73.8%
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-12 13:43 missing_mga-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5096 b- defN 24-May-12 13:43 missing_mga-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 13:43 missing_mga-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-12 13:43 missing_mga-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      572 b- defN 24-May-12 13:43 missing_mga-0.3.0.dist-info/RECORD
+7 files, 23195 bytes uncompressed, 6067 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: missing_mga/__init__.py
 Comment: 
 
 Filename: missing_mga/missing_methods.py
 Comment: 
 
-Filename: missing_mga-0.2.1.dist-info/LICENSE
+Filename: missing_mga-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: missing_mga-0.2.1.dist-info/METADATA
+Filename: missing_mga-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: missing_mga-0.2.1.dist-info/WHEEL
+Filename: missing_mga-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: missing_mga-0.2.1.dist-info/top_level.txt
+Filename: missing_mga-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: missing_mga-0.2.1.dist-info/RECORD
+Filename: missing_mga-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `missing_mga-0.2.1.dist-info/LICENSE` & `missing_mga-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `missing_mga-0.2.1.dist-info/METADATA` & `missing_mga-0.3.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missing-mga
-Version: 0.2.1
+Version: 0.3.0
 Summary: A package for handling missing values in datasets.
 Home-page: https://github.com/Mgobeaalcoba/missing_mga
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -52,15 +52,15 @@
 ```
 
 ## Usage
 
 To use the package, you need to import the MissingMethods class from the pandas_missing module:
 
 ```python
-from missing-mga import MissingMethods
+import missing_mga as missing
 ```
 
 Then, you can create a DataFrame and use the missing method to access the missing value handling methods:
 
 ```python
 import pandas as pd
```

