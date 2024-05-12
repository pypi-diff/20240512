# Comparing `tmp/omopsurvey-0.0.4.tar.gz` & `tmp/omopsurvey-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omopsurvey-0.0.4.tar", max compression
+gzip compressed data, was "omopsurvey-0.0.5.tar", max compression
```

## Comparing `omopsurvey-0.0.4.tar` & `omopsurvey-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     5369 2024-05-10 04:47:09.981340 omopsurvey-0.0.4/README.md
--rw-r--r--   0        0        0      308 2024-05-10 04:21:01.287198 omopsurvey-0.0.4/omopsurvey/__init__.py
--rw-r--r--   0        0        0     3699 2024-05-10 04:36:24.494077 omopsurvey-0.0.4/omopsurvey/codebook.py
--rw-r--r--   0        0        0     2216 2024-05-10 14:38:36.819420 omopsurvey-0.0.4/omopsurvey/pivot_data.py
--rw-r--r--   0        0        0      887 2024-05-09 23:16:46.718345 omopsurvey-0.0.4/omopsurvey/recode_missing.py
--rw-r--r--   0        0        0     3686 2024-05-10 04:36:24.488122 omopsurvey-0.0.4/omopsurvey/response_set.py
--rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omopsurvey-0.0.4/omopsurvey/survey_key.csv
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.840855 omopsurvey-0.0.4/omopsurvey/tests/codebook_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.844331 omopsurvey-0.0.4/omopsurvey/tests/map_responses_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.847047 omopsurvey-0.0.4/omopsurvey/tests/pivot_data_test.py
--rw-r--r--   0        0        0      194 2024-05-01 01:54:49.831523 omopsurvey-0.0.4/omopsurvey/tests/recode_missing_test.py
--rw-r--r--   0        0        0      615 2024-05-01 01:53:42.049881 omopsurvey-0.0.4/omopsurvey/vignettes/example_basics.ipynb
--rw-r--r--   0        0        0      615 2024-05-01 01:53:00.463035 omopsurvey-0.0.4/omopsurvey/vignettes/example_healthcare.ipynb
--rw-r--r--   0        0        0      615 2024-05-01 01:53:25.889124 omopsurvey-0.0.4/omopsurvey/vignettes/example_sdoh.ipynb
--rw-r--r--   0        0        0      722 2024-05-10 14:38:36.824745 omopsurvey-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 omopsurvey-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5369 2024-05-10 04:47:09.981340 omopsurvey-0.0.5/README.md
+-rw-r--r--   0        0        0      258 2024-05-11 22:40:02.259765 omopsurvey-0.0.5/omopsurvey/__init__.py
+-rw-r--r--   0        0        0     3921 2024-05-12 03:53:34.300366 omopsurvey-0.0.5/omopsurvey/codebooks.py
+-rw-r--r--   0        0        0     1566 2024-05-12 03:58:00.406974 omopsurvey-0.0.5/omopsurvey/pivot_data.py
+-rw-r--r--   0        0        0      872 2024-05-11 22:10:49.324160 omopsurvey-0.0.5/omopsurvey/recode_missing.py
+-rw-r--r--   0        0        0     4581 2024-05-11 22:35:34.376582 omopsurvey-0.0.5/omopsurvey/response_set.py
+-rw-r--r--   0        0        0  1172489 2024-05-10 03:42:23.460428 omopsurvey-0.0.5/omopsurvey/survey_key.csv
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.840855 omopsurvey-0.0.5/omopsurvey/tests/codebook_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.844331 omopsurvey-0.0.5/omopsurvey/tests/map_responses_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.847047 omopsurvey-0.0.5/omopsurvey/tests/pivot_data_test.py
+-rw-r--r--   0        0        0      194 2024-05-01 01:54:49.831523 omopsurvey-0.0.5/omopsurvey/tests/recode_missing_test.py
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:42.049881 omopsurvey-0.0.5/omopsurvey/vignettes/example_basics.ipynb
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:00.463035 omopsurvey-0.0.5/omopsurvey/vignettes/example_healthcare.ipynb
+-rw-r--r--   0        0        0      615 2024-05-01 01:53:25.889124 omopsurvey-0.0.5/omopsurvey/vignettes/example_sdoh.ipynb
+-rw-r--r--   0        0        0      722 2024-05-12 04:24:32.235654 omopsurvey-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6384 1970-01-01 00:00:00.000000 omopsurvey-0.0.5/PKG-INFO
```

### Comparing `omopsurvey-0.0.4/README.md` & `omopsurvey-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.4/omopsurvey/codebook.py` & `omopsurvey-0.0.5/omopsurvey/codebooks.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import pandas as pd
+from IPython.display import display, FileLink
+import os
 
 
 def load_data(source):
     if isinstance(source, pd.DataFrame):
         return source
     elif isinstance(source, str):
         if source.endswith('.csv'):
@@ -13,27 +15,27 @@
             return pd.read_excel(source)
         else:
             raise ValueError("Unsupported file type provided.")
     else:
         raise TypeError("Input source must be a pandas DataFrame or a filepath as a string.")
 
 
-def create_codebook(dataframe):
+def create_codebook(input_data):
 
     required_columns = ['question_concept_id', 'question']
     response_columns = ['answer_concept_id', 'answer', 'answer_text', 'answer_numeric']
 
-    response_columns = [col for col in response_columns if col in dataframe.columns]
+    response_columns = [col for col in response_columns if col in input_data.columns]
 
-    if not all(col in dataframe.columns for col in required_columns):
+    if not all(col in input_data.columns for col in required_columns):
         raise ValueError("Dataframe must contain the necessary columns: 'question_concept_id' and 'question'.")
 
-    dataframe['question_concept_id'] = dataframe['question_concept_id'].astype(str)
+    input_data['question_concept_id'] = input_data['question_concept_id'].astype(str)
 
-    grouped = dataframe.groupby(required_columns).apply(
+    grouped = input_data.groupby(required_columns).apply(
         lambda x: x[response_columns].drop_duplicates().reset_index(drop=True)
     )
 
     codebook_df = grouped.reset_index(drop=False)
 
     codebook_df = codebook_df[required_columns + response_columns].drop_duplicates()
 
@@ -68,22 +70,22 @@
     except ImportError:
         print("Tabulate module not installed, using default print.")
         print(codebook_df)
     except Exception as e:
         print(f"Error: {e}")
 
 
-def create_formatted_codebook(dataframe):
+def codebook(input_data):
 
-    dataframe['question'] = dataframe['question'].str.strip().str.lower()
-    dataframe['answer'] = dataframe['answer'].str.strip().str.lower()
+    input_data['question'] = input_data['question'].str.strip().str.lower()
+    input_data['answer'] = input_data['answer'].str.strip().str.lower()
 
-    dataframe = dataframe.drop_duplicates(subset=['question_concept_id', 'question', 'answer_concept_id'])
+    input_data = input_data.drop_duplicates(subset=['question_concept_id', 'question', 'answer_concept_id'])
 
-    grouped = dataframe.groupby(['question_concept_id', 'question'], sort=False)
+    grouped = input_data.groupby(['question_concept_id', 'question'], sort=False)
 
     formatted_data = []
 
     for (question_concept_id, question), group in grouped:
         is_first = True
 
         for idx, row in group.iterrows():
@@ -105,8 +107,13 @@
                     'answer_concept_id recoded as answer_numeric': row['answer_numeric'],
                     'answer': row['answer'],
                     'answer recoded as answer_text': row['answer_text']
                 })
 
     formatted_codebook_df = pd.DataFrame(formatted_data)
 
-    return formatted_codebook_df.to_html(index=False, escape=False)
+    file_name = 'codebook.html'
+    file_path = os.path.join(os.getcwd(), file_name)
+    with open(file_path, 'w') as f:
+        f.write(formatted_codebook_df.to_html(index=False, escape=False))
+
+    return display(FileLink(file_path))
```

### Comparing `omopsurvey-0.0.4/omopsurvey/pivot_data.py` & `omopsurvey-0.0.5/omopsurvey/pivot_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,37 @@
 import pandas as pd
 import os
 import subprocess
 
 
-# def pivot_data_numeric(data):
-#
-#     pivot_df = data.pivot_table(index='person_id',
-#                                 columns='question_concept_id',
-#                                 values='answer_numeric',
-#                                 aggfunc='first')
-#
-#     pivot_df.columns = ['q' + str(col) for col in pivot_df.columns]
-#     dir_name = os.path.dirname(data)
-#     new_filename = 'pivot_n_' + os.path.basename(data)
-#     new_filepath = os.path.join(dir_name, new_filename)
-#     pivot_df.to_csv(new_filepath)
-#
-#     print(f"Pivoted dataset with numeric values saved as: {new_filepath}")
-
-
-def pivot_data_text(data, file_name='pivot_t.csv'):
+def pivot_text(data, file_name='pivot_t.csv'):
     pivot_df = data.pivot_table(index='person_id',
                                 columns='question_concept_id',
                                 values='answer_text',
                                 aggfunc='first')
 
     pivot_df.columns = ['q' + str(col) for col in pivot_df.columns]
-    pivot_df.to_csv(file_name, index=False)
+    pivot_df.to_csv(file_name)
     my_bucket = os.getenv('WORKSPACE_BUCKET')
     args = ["gsutil", "cp", f"./{file_name}", f"{my_bucket}/data/"]
     output = subprocess.run(args, capture_output=True)
     if output.returncode == 0:
         print(f"Pivoted dataset with text values saved and uploaded successfully to: {my_bucket}/data/{file_name}")
     else:
         print("Failed to upload the file:", output.stderr.decode())
 
 
-def pivot_data_numeric(data, file_name='pivot_n.csv'):
+def pivot(data, file_name='pivot_n.csv'):
     pivot_df = data.pivot_table(index='person_id',
                                 columns='question_concept_id',
                                 values='answer_numeric',
                                 aggfunc='first')
 
     pivot_df.columns = ['q' + str(col) for col in pivot_df.columns]
-    pivot_df.to_csv(file_name, index=False)
+    pivot_df.to_csv(file_name)
     my_bucket = os.getenv('WORKSPACE_BUCKET')
     args = ["gsutil", "cp", f"./{file_name}", f"{my_bucket}/data/"]
     output = subprocess.run(args, capture_output=True)
     if output.returncode == 0:
         print(f"Pivoted dataset with text values saved and uploaded successfully to: {my_bucket}/data/{file_name}")
     else:
         print("Failed to upload the file:", output.stderr.decode())
-
```

### Comparing `omopsurvey-0.0.4/omopsurvey/recode_missing.py` & `omopsurvey-0.0.5/omopsurvey/recode_missing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 
 
-def recode_missing_values(input_data):
+def recode(input_data):
     missing_values = [-999, -998, -997, -996, -995, -994, -993, -992, -991, -990,
                       -989, -988, -987, -986, -985, -984, -983, -982, -981, -980]
 
     if isinstance(input_data, str):
         if input_data.endswith('.csv') or input_data.endswith('.txt'):
             return pd.read_csv(input_data, na_values=missing_values)
         elif input_data.endswith(('.xlsx', '.xls')):
```

### Comparing `omopsurvey-0.0.4/omopsurvey/survey_key.csv` & `omopsurvey-0.0.5/omopsurvey/survey_key.csv`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.4/omopsurvey/vignettes/example_basics.ipynb` & `omopsurvey-0.0.5/omopsurvey/vignettes/example_basics.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.4/omopsurvey/vignettes/example_healthcare.ipynb` & `omopsurvey-0.0.5/omopsurvey/vignettes/example_healthcare.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.4/omopsurvey/vignettes/example_sdoh.ipynb` & `omopsurvey-0.0.5/omopsurvey/vignettes/example_sdoh.ipynb`

 * *Files identical despite different names*

### Comparing `omopsurvey-0.0.4/pyproject.toml` & `omopsurvey-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omopsurvey"
-version = "0.0.4"
+version = "0.0.5"
 description = "The 'omopsurvey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis."
 authors = ["Elif Dede Yildirim <elifdy@auburn.edu>"]
 repository = "https://github.com/elifdy/omopsurvey.git"
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `omopsurvey-0.0.4/PKG-INFO` & `omopsurvey-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omopsurvey
-Version: 0.0.4
+Version: 0.0.5
 Summary: The 'omopsurvey' Python package transforms standardized response codes from the OMOP CDM survey variables into numeric values and simplifies data preparation by providing functionalities for mapping and converting response codes, as well as handling missing data, facilitating easier and more reliable data analysis.
 Home-page: https://github.com/elifdy/omopsurvey.git
 License: MIT
 Author: Elif Dede Yildirim
 Author-email: elifdy@auburn.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

