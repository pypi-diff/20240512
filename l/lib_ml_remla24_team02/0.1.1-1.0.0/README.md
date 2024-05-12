# Comparing `tmp/lib_ml_remla24_team02-0.1.1.tar.gz` & `tmp/lib_ml_remla24_team02-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_ml_remla24_team02-0.1.1.tar", max compression
+gzip compressed data, was "lib_ml_remla24_team02-1.0.0.tar", max compression
```

## Comparing `lib_ml_remla24_team02-0.1.1.tar` & `lib_ml_remla24_team02-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0       69 2024-05-12 14:22:02.864868 lib_ml_remla24_team02-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-12 14:22:02.864868 lib_ml_remla24_team02-0.1.1/lib_ml_remla24_team02/__init__.py
--rw-r--r--   0        0        0     3483 2024-05-12 14:22:02.864868 lib_ml_remla24_team02-0.1.1/lib_ml_remla24_team02/data_preprocessing.py
--rw-r--r--   0        0        0      423 2024-05-12 14:22:15.889165 lib_ml_remla24_team02-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 lib_ml_remla24_team02-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       69 2024-05-12 14:58:21.825878 lib_ml_remla24_team02-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-12 14:58:21.825878 lib_ml_remla24_team02-1.0.0/lib_ml_remla24_team02/__init__.py
+-rw-r--r--   0        0        0      444 2024-05-12 14:58:21.825878 lib_ml_remla24_team02-1.0.0/lib_ml_remla24_team02/data/char_index.joblib
+-rw-r--r--   0        0        0      407 2024-05-12 14:58:21.825878 lib_ml_remla24_team02-1.0.0/lib_ml_remla24_team02/data/label_encoder.joblib
+-rw-r--r--   0        0        0     3954 2024-05-12 14:58:21.825878 lib_ml_remla24_team02-1.0.0/lib_ml_remla24_team02/data_preprocessing.py
+-rw-r--r--   0        0        0      473 2024-05-12 14:58:35.221823 lib_ml_remla24_team02-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 lib_ml_remla24_team02-1.0.0/PKG-INFO
```

### Comparing `lib_ml_remla24_team02-0.1.1/lib_ml_remla24_team02/data_preprocessing.py` & `lib_ml_remla24_team02-1.0.0/lib_ml_remla24_team02/data_preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Preprocess the data to be trained by the learning algorithm.
 """
 import os, sys, logging
+import importlib.resources as pkg_resources
 from sklearn.preprocessing import LabelEncoder
 from tensorflow.keras.preprocessing.text import Tokenizer  # type: ignore
 from tensorflow.keras.preprocessing.sequence import pad_sequences  # type: ignore
 from joblib import dump, load
 
 
 def load_data(data_dir):
@@ -61,49 +62,61 @@
 
     encoder = LabelEncoder()
 
     y_train = encoder.fit_transform(raw_y_train)
     y_val = encoder.transform(raw_y_val)
     y_test = encoder.transform(raw_y_test)
 
-    return y_train, y_val, y_test
+    return y_train, y_val, y_test, encoder
 
 
 def preprocess(data_dir, output_dir):
     """
     Preprocessing the data for training.
     """
     raw_x, raw_y = load_data(data_dir)
     x_train, x_val, x_test, char_index = tokenize_data(raw_x)
-    y_train, y_val, y_test = encode_data(raw_y)
+    y_train, y_val, y_test, encoder = encode_data(raw_y)
 
     os.makedirs(output_dir, exist_ok=True)
 
     # Dumping the data
     dump(x_train, os.path.join(output_dir, 'preprocessed_x_train.joblib'))
     dump(x_val, os.path.join(output_dir, 'preprocessed_x_val.joblib'))
     dump(x_test, os.path.join(output_dir, 'preprocessed_x_test.joblib'))
     dump(char_index, os.path.join(output_dir, 'char_index.joblib'))
 
     dump(y_train, os.path.join(output_dir, 'preprocessed_y_train.joblib'))
     dump(y_val, os.path.join(output_dir, 'preprocessed_y_val.joblib'))
     dump(y_test, os.path.join(output_dir, 'preprocessed_y_test.joblib'))
+    dump(encoder, os.path.join(output_dir, 'label_encoder.joblib'))
 
-def preprocess_single(url, char_index_path):
+
+def preprocess_single(url):
     """
     Preprocess a single URL.
     """
     sequence_length = 200
-    char_index = load(char_index_path)
+    with pkg_resources.path('lib_ml_remla24_team02.data', 'char_index.joblib') as model_path:
+        char_index = load(model_path)
+
+        sequence = []
+        for char in url:
+            sequence.append(char_index.get(char, char_index.get('-n-', 1)))
+
+        return pad_sequences([sequence], maxlen=sequence_length)
 
-    sequence = []
-    for char in url:
-        sequence.append(char_index.get(char, char_index.get('-n-', 1)))
 
-    return pad_sequences([sequence], maxlen=sequence_length)
+def decode_label(labels):
+    """
+    Decode labels.
+    """
+    with pkg_resources.path('lib_ml_remla24_team02.data', 'label_encoder.joblib') as encoder_path:
+        encoder = load(encoder_path)
+        return encoder.inverse_transform(labels)
 
 
 if __name__ == '__main__':
     if len(sys.argv) < 3:
         logging.error("Incorrect arguments. Usage: python data_preprocessing.py <data_dir> <output_dir>")
         sys.exit(1)
```

### Comparing `lib_ml_remla24_team02-0.1.1/PKG-INFO` & `lib_ml_remla24_team02-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib_ml_remla24_team02
-Version: 0.1.1
+Version: 1.0.0
 Summary: A package for pre-processing ML data for the REMLA course at the TU Delft.
 Author: REMLA 24 Team 02
 Author-email: team02@remla24.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: joblib (>=1.4.2,<2.0.0)
```

