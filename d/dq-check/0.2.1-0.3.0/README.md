# Comparing `tmp/dq_check-0.2.1.tar.gz` & `tmp/dq_check-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dq_check-0.2.1.tar", last modified: Wed May  8 05:25:43 2024, max compression
+gzip compressed data, was "dq_check-0.3.0.tar", last modified: Sun May 12 21:43:43 2024, max compression
```

## Comparing `dq_check-0.2.1.tar` & `dq_check-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-08 05:25:43.609782 dq_check-0.2.1/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2458 2024-05-08 05:25:43.609299 dq_check-0.2.1/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2219 2024-05-08 05:16:24.000000 dq_check-0.2.1/README.md
--rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-08 05:25:17.000000 dq_check-0.2.1/pyproject.toml
--rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-08 05:25:43.610562 dq_check-0.2.1/setup.cfg
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-08 05:25:43.601623 dq_check-0.2.1/src/
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-08 05:25:43.604221 dq_check-0.2.1/src/dq_check/
--rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.2.1/src/dq_check/__init__.py
--rw-r--r--   0 rohan.goel   (502) staff       (20)    10899 2024-05-08 05:23:41.000000 dq_check-0.2.1/src/dq_check/dq_check.py
-drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-08 05:25:43.608493 dq_check-0.2.1/src/dq_check.egg-info/
--rw-r--r--   0 rohan.goel   (502) staff       (20)     2458 2024-05-08 05:25:43.000000 dq_check-0.2.1/src/dq_check.egg-info/PKG-INFO
--rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-08 05:25:43.000000 dq_check-0.2.1/src/dq_check.egg-info/SOURCES.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-08 05:25:43.000000 dq_check-0.2.1/src/dq_check.egg-info/dependency_links.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-08 05:25:43.000000 dq_check-0.2.1/src/dq_check.egg-info/requires.txt
--rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-08 05:25:43.000000 dq_check-0.2.1/src/dq_check.egg-info/top_level.txt
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-12 21:43:43.257844 dq_check-0.3.0/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-12 21:43:43.257516 dq_check-0.3.0/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2440 2024-05-12 21:16:29.000000 dq_check-0.3.0/README.md
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      327 2024-05-12 21:28:43.000000 dq_check-0.3.0/pyproject.toml
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      131 2024-05-12 21:43:43.258822 dq_check-0.3.0/setup.cfg
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-12 21:43:43.248422 dq_check-0.3.0/src/
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-12 21:43:43.251700 dq_check-0.3.0/src/dq_check/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       29 2024-05-05 04:45:50.000000 dq_check-0.3.0/src/dq_check/__init__.py
+-rw-r--r--   0 rohan.goel   (502) staff       (20)    15105 2024-05-12 21:16:57.000000 dq_check-0.3.0/src/dq_check/dq_check.py
+drwxr-xr-x   0 rohan.goel   (502) staff       (20)        0 2024-05-12 21:43:43.256485 dq_check-0.3.0/src/dq_check.egg-info/
+-rw-r--r--   0 rohan.goel   (502) staff       (20)     2679 2024-05-12 21:43:43.000000 dq_check-0.3.0/src/dq_check.egg-info/PKG-INFO
+-rw-r--r--   0 rohan.goel   (502) staff       (20)      263 2024-05-12 21:43:43.000000 dq_check-0.3.0/src/dq_check.egg-info/SOURCES.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        1 2024-05-12 21:43:43.000000 dq_check-0.3.0/src/dq_check.egg-info/dependency_links.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)       15 2024-05-12 21:43:43.000000 dq_check-0.3.0/src/dq_check.egg-info/requires.txt
+-rw-r--r--   0 rohan.goel   (502) staff       (20)        9 2024-05-12 21:43:43.000000 dq_check-0.3.0/src/dq_check.egg-info/top_level.txt
```

### Comparing `dq_check-0.2.1/PKG-INFO` & `dq_check-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: dq_check
-Version: 0.2.1
-Summary: A data quality check module for Spark
-Author-email: rohan goel <rohan.goel@databricks.com>
-Description-Content-Type: text/markdown
-Requires-Dist: pyspark
-Requires-Dist: pandas
-
 ## dq_check
 
 
 ## Overview
 
 `dq_check` is a Python package that provides a data quality check function encapsulated in the `DQCheck` class. It allows you to perform data quality checks on tables using SQL queries and save the results into a Delta table for auditing purposes.
 
@@ -39,15 +30,23 @@
 from dq_check import DQCheck
 
 ## Initialize Spark session
 spark = SparkSession.builder.appName("DQCheckExample").getOrCreate()
 
 ## Create an instance of DQCheck
 
-dq_checker = DQCheck(spark,audit_table) #audit table name should have catalog and schema.
+dq_checker = DQCheck(spark,audit_table_name) #audit table name should have catalog and schema.
+
+spark (SparkSession): The Spark session.
+
+audit_table_name (str):Default is audit_log. The name of the Delta table to store audit logs.
+
+azure_sql_client:Default is None. This is required for asql,create azure_sql_client by providing scope and secret with AzureSQLClient
+            
+run_id:Default is -999 , run_id for the ADF pipeline
 
 ## Define the data quality check parameters
 
 table_type = "delta"  # Type of the table ('delta' or 'asql')
 
 table_name = "your_table_name"  # Name of the table, should have catalog/schema for delta and schema for asql.
 
@@ -62,23 +61,19 @@
 
     table_name,
 
     primary_keys,
 
     sql_query,
 
-    scope=None,# Optional, required for asql only
-
-    secret=None, # Optional, required for asql only
-
-    data_batch_identifier_name=None,  # Optional batch identifier name
+    where_clause=None, # Optional where clause for sample data
 
-    data_batch_identifier_value=None,  # Optional batch identifier value
+    quality_threshold_percentage=5,  # Optional Quality threshold percentage
 
-    quality_threshold_percentage=5,  # Quality threshold percentage
+    chunk_size=200, #Optional chunk size for pks list
 )
 
 
 ## Configuration
 
 Adjust the parameters passed to the perform_dq_check method based on your requirements.
 
@@ -91,8 +86,8 @@
 
 Contributions are welcome! Please feel free to submit issues and pull requests on the GitHub repository.
 
 ## License
 None.
 
 ## Contact
-For any questions or feedback, open a github issue
+For any questions or feedback, open a github issue
```

### Comparing `dq_check-0.2.1/README.md` & `dq_check-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: dq_check
+Version: 0.3.0
+Summary: A data quality check module for Spark
+Author-email: rohan goel <rohan.goel@databricks.com>
+Description-Content-Type: text/markdown
+Requires-Dist: pyspark
+Requires-Dist: pandas
+
 ## dq_check
 
 
 ## Overview
 
 `dq_check` is a Python package that provides a data quality check function encapsulated in the `DQCheck` class. It allows you to perform data quality checks on tables using SQL queries and save the results into a Delta table for auditing purposes.
 
@@ -30,15 +39,23 @@
 from dq_check import DQCheck
 
 ## Initialize Spark session
 spark = SparkSession.builder.appName("DQCheckExample").getOrCreate()
 
 ## Create an instance of DQCheck
 
-dq_checker = DQCheck(spark,audit_table) #audit table name should have catalog and schema.
+dq_checker = DQCheck(spark,audit_table_name) #audit table name should have catalog and schema.
+
+spark (SparkSession): The Spark session.
+
+audit_table_name (str):Default is audit_log. The name of the Delta table to store audit logs.
+
+azure_sql_client:Default is None. This is required for asql,create azure_sql_client by providing scope and secret with AzureSQLClient
+            
+run_id:Default is -999 , run_id for the ADF pipeline
 
 ## Define the data quality check parameters
 
 table_type = "delta"  # Type of the table ('delta' or 'asql')
 
 table_name = "your_table_name"  # Name of the table, should have catalog/schema for delta and schema for asql.
 
@@ -53,23 +70,19 @@
 
     table_name,
 
     primary_keys,
 
     sql_query,
 
-    scope=None,# Optional, required for asql only
-
-    secret=None, # Optional, required for asql only
-
-    data_batch_identifier_name=None,  # Optional batch identifier name
+    where_clause=None, # Optional where clause for sample data
 
-    data_batch_identifier_value=None,  # Optional batch identifier value
+    quality_threshold_percentage=5,  # Optional Quality threshold percentage
 
-    quality_threshold_percentage=5,  # Quality threshold percentage
+    chunk_size=200, #Optional chunk size for pks list
 )
 
 
 ## Configuration
 
 Adjust the parameters passed to the perform_dq_check method based on your requirements.
 
@@ -82,8 +95,8 @@
 
 Contributions are welcome! Please feel free to submit issues and pull requests on the GitHub repository.
 
 ## License
 None.
 
 ## Contact
-For any questions or feedback, open a github issue
+For any questions or feedback, open a github issue
```

### Comparing `dq_check-0.2.1/src/dq_check.egg-info/PKG-INFO` & `dq_check-0.3.0/src/dq_check.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dq_check
-Version: 0.2.1
+Version: 0.3.0
 Summary: A data quality check module for Spark
 Author-email: rohan goel <rohan.goel@databricks.com>
 Description-Content-Type: text/markdown
 Requires-Dist: pyspark
 Requires-Dist: pandas
 
 ## dq_check
@@ -39,15 +39,23 @@
 from dq_check import DQCheck
 
 ## Initialize Spark session
 spark = SparkSession.builder.appName("DQCheckExample").getOrCreate()
 
 ## Create an instance of DQCheck
 
-dq_checker = DQCheck(spark,audit_table) #audit table name should have catalog and schema.
+dq_checker = DQCheck(spark,audit_table_name) #audit table name should have catalog and schema.
+
+spark (SparkSession): The Spark session.
+
+audit_table_name (str):Default is audit_log. The name of the Delta table to store audit logs.
+
+azure_sql_client:Default is None. This is required for asql,create azure_sql_client by providing scope and secret with AzureSQLClient
+            
+run_id:Default is -999 , run_id for the ADF pipeline
 
 ## Define the data quality check parameters
 
 table_type = "delta"  # Type of the table ('delta' or 'asql')
 
 table_name = "your_table_name"  # Name of the table, should have catalog/schema for delta and schema for asql.
 
@@ -62,23 +70,19 @@
 
     table_name,
 
     primary_keys,
 
     sql_query,
 
-    scope=None,# Optional, required for asql only
-
-    secret=None, # Optional, required for asql only
-
-    data_batch_identifier_name=None,  # Optional batch identifier name
+    where_clause=None, # Optional where clause for sample data
 
-    data_batch_identifier_value=None,  # Optional batch identifier value
+    quality_threshold_percentage=5,  # Optional Quality threshold percentage
 
-    quality_threshold_percentage=5,  # Quality threshold percentage
+    chunk_size=200, #Optional chunk size for pks list
 )
 
 
 ## Configuration
 
 Adjust the parameters passed to the perform_dq_check method based on your requirements.
```

