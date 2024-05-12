# Comparing `tmp/missing_mga-0.4.1-py3-none-any.whl.zip` & `tmp/missing_mga-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7796 bytes, number of entries: 7
--rw-r--r--  2.0 unx       44 b- defN 24-May-12 13:01 missing_mga/__init__.py
+Zip file size: 7800 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       55 b- defN 24-May-12 15:18 missing_mga/__init__.py
 -rw-r--r--  2.0 unx    18749 b- defN 24-May-12 14:40 missing_mga/missing_methods.py
--rw-r--r--  2.0 unx     1069 b- defN 24-May-12 15:04 missing_mga-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     6026 b- defN 24-May-12 15:04 missing_mga-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 15:04 missing_mga-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-May-12 15:04 missing_mga-0.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      572 b- defN 24-May-12 15:04 missing_mga-0.4.1.dist-info/RECORD
-7 files, 26564 bytes uncompressed, 6778 bytes compressed:  74.5%
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-12 15:20 missing_mga-0.4.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6026 b- defN 24-May-12 15:20 missing_mga-0.4.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 15:20 missing_mga-0.4.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-12 15:20 missing_mga-0.4.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      572 b- defN 24-May-12 15:20 missing_mga-0.4.2.dist-info/RECORD
+7 files, 26575 bytes uncompressed, 6782 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: missing_mga/__init__.py
 Comment: 
 
 Filename: missing_mga/missing_methods.py
 Comment: 
 
-Filename: missing_mga-0.4.1.dist-info/LICENSE
+Filename: missing_mga-0.4.2.dist-info/LICENSE
 Comment: 
 
-Filename: missing_mga-0.4.1.dist-info/METADATA
+Filename: missing_mga-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: missing_mga-0.4.1.dist-info/WHEEL
+Filename: missing_mga-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: missing_mga-0.4.1.dist-info/top_level.txt
+Filename: missing_mga-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: missing_mga-0.4.1.dist-info/RECORD
+Filename: missing_mga-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## missing_mga/__init__.py

```diff
@@ -1 +1 @@
-from .missing_methods import MissingMethods
+from .missing_methods import MissingMethods as missing
```

## Comparing `missing_mga-0.4.1.dist-info/LICENSE` & `missing_mga-0.4.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `missing_mga-0.4.1.dist-info/METADATA` & `missing_mga-0.4.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: missing_mga
-Version: 0.4.1
+Version: 0.4.2
 Summary: A package for handling missing values in datasets.
 Home-page: https://github.com/Mgobeaalcoba/missing_mga
 Author: Mariano Gobea Alcoba
 Author-email: gobeamariano@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `missing_mga-0.4.1.dist-info/RECORD` & `missing_mga-0.4.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-missing_mga/__init__.py,sha256=xJDGSbh4zgyoAA9gdcX7BmaOiM9IJNtlBRlUx76Bcvs,44
+missing_mga/__init__.py,sha256=Y0Ira_Y7QTTvTUT0W1SLMPHDGn6mNtJrIkZ7K1_msiQ,55
 missing_mga/missing_methods.py,sha256=iVPaikKO_Ua9xPE2e6Bsc_kaRaN8XT4WUty1VvY6HbQ,18749
-missing_mga-0.4.1.dist-info/LICENSE,sha256=Ldmia3atdQGph82A3xxsshdEdvlvCHs8sB-VTmn2W1E,1069
-missing_mga-0.4.1.dist-info/METADATA,sha256=ynQZHIUZatoMuwQukcjs5DALzQ02Lw3XYjshdnnSyzk,6026
-missing_mga-0.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-missing_mga-0.4.1.dist-info/top_level.txt,sha256=3TGq-rFYvXfUzKjxu7Y8BFIvwuN3QvnZIX2WKRQNVBA,12
-missing_mga-0.4.1.dist-info/RECORD,,
+missing_mga-0.4.2.dist-info/LICENSE,sha256=Ldmia3atdQGph82A3xxsshdEdvlvCHs8sB-VTmn2W1E,1069
+missing_mga-0.4.2.dist-info/METADATA,sha256=tveo4GNLVaZa7R19PrK-CnGVEEEVaFpyIYSbFr-v90Y,6026
+missing_mga-0.4.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+missing_mga-0.4.2.dist-info/top_level.txt,sha256=3TGq-rFYvXfUzKjxu7Y8BFIvwuN3QvnZIX2WKRQNVBA,12
+missing_mga-0.4.2.dist-info/RECORD,,
```

