# Comparing `tmp/remla2024_team9_lib_ml-0.1.0.tar.gz` & `tmp/remla2024_team9_lib_ml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla2024_team9_lib_ml-0.1.0.tar", max compression
+gzip compressed data, was "remla2024_team9_lib_ml-0.1.1.tar", max compression
```

## Comparing `remla2024_team9_lib_ml-0.1.0.tar` & `remla2024_team9_lib_ml-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      445 2024-05-12 13:05:01.974275 remla2024_team9_lib_ml-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       89 2024-05-12 11:49:36.334190 remla2024_team9_lib_ml-0.1.0/remla2024_team9_lib_ml/__init__.py
--rw-r--r--   0        0        0      317 2024-05-12 11:49:36.336191 remla2024_team9_lib_ml-0.1.0/remla2024_team9_lib_ml/data_split.py
--rw-r--r--   0        0        0      617 2024-05-12 11:49:36.337192 remla2024_team9_lib_ml-0.1.0/remla2024_team9_lib_ml/encode_labels.py
--rw-r--r--   0        0        0     1145 2024-05-12 11:49:36.339194 remla2024_team9_lib_ml-0.1.0/remla2024_team9_lib_ml/tokenize_features.py
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 remla2024_team9_lib_ml-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      427 2024-05-12 14:38:45.864277 remla2024_team9_lib_ml-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-12 14:38:45.864277 remla2024_team9_lib_ml-0.1.1/remla2024_team9_lib_ml/__init__.py
+-rw-r--r--   0        0        0      307 2024-05-12 14:38:45.864277 remla2024_team9_lib_ml-0.1.1/remla2024_team9_lib_ml/data_split.py
+-rw-r--r--   0        0        0      602 2024-05-12 14:38:45.864277 remla2024_team9_lib_ml-0.1.1/remla2024_team9_lib_ml/encode_labels.py
+-rw-r--r--   0        0        0     1121 2024-05-12 14:38:45.864277 remla2024_team9_lib_ml-0.1.1/remla2024_team9_lib_ml/tokenize_features.py
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 remla2024_team9_lib_ml-0.1.1/PKG-INFO
```

### Comparing `remla2024_team9_lib_ml-0.1.0/remla2024_team9_lib_ml/encode_labels.py` & `remla2024_team9_lib_ml-0.1.1/remla2024_team9_lib_ml/encode_labels.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from sklearn.preprocessing import LabelEncoder
-
-def encode_labels(train_labels, val_labels, test_labels):
-    """
-    Encodes labels using sklearn LabelEncoder and returns numpy arrays of encoded labels.
-    """
-
-    encoder = LabelEncoder()
-
-    # Transform labels
-    train_labels_encoded = encoder.fit_transform([label.strip() for label in train_labels])
-    val_labels_encoded = encoder.transform([label.strip() for label in val_labels])
-    test_labels_encoded = encoder.transform([label.strip() for label in test_labels])
-
-    return train_labels_encoded, val_labels_encoded, test_labels_encoded
+from sklearn.preprocessing import LabelEncoder
+
+def encode_labels(train_labels, val_labels, test_labels):
+    """
+    Encodes labels using sklearn LabelEncoder and returns numpy arrays of encoded labels.
+    """
+
+    encoder = LabelEncoder()
+
+    # Transform labels
+    train_labels_encoded = encoder.fit_transform([label.strip() for label in train_labels])
+    val_labels_encoded = encoder.transform([label.strip() for label in val_labels])
+    test_labels_encoded = encoder.transform([label.strip() for label in test_labels])
+
+    return train_labels_encoded, val_labels_encoded, test_labels_encoded
```

### Comparing `remla2024_team9_lib_ml-0.1.0/remla2024_team9_lib_ml/tokenize_features.py` & `remla2024_team9_lib_ml-0.1.1/remla2024_team9_lib_ml/tokenize_features.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from tensorflow.keras.preprocessing.text import Tokenizer
-from tensorflow.keras.preprocessing.sequence import pad_sequences
-
-def tokenize_features(train_features, val_features, test_features, sequence_length=200):
-    """
-    Tokenizes the given features using a pre-loaded tokenizer and returns the tokenized features.
-    """
-    # Initialize tokenizer
-    tokenizer = Tokenizer(lower=True, char_level=True, oov_token='-n-')
-    tokenizer.fit_on_texts(train_features + val_features + test_features)
-
-    # Tokenize and pad sequences
-    x_train = pad_sequences(tokenizer.texts_to_sequences(train_features), maxlen=sequence_length)
-    x_val = pad_sequences(tokenizer.texts_to_sequences(val_features), maxlen=sequence_length)
-    x_test = pad_sequences(tokenizer.texts_to_sequences(test_features), maxlen=sequence_length)
-
-    return x_train, x_val, x_test, tokenizer
-
-def tokenize_url(tokenizer, url, sequence_length=200):
-    """
-    Tokenizes the given url using a pre-loaded tokenizer and returns the tokenized sequence.
-    """
-    return pad_sequences(tokenizer.texts_to_sequences([url]), maxlen=sequence_length)
-
+from tensorflow.keras.preprocessing.text import Tokenizer
+from tensorflow.keras.preprocessing.sequence import pad_sequences
+
+def tokenize_features(train_features, val_features, test_features, sequence_length=200):
+    """
+    Tokenizes the given features using a pre-loaded tokenizer and returns the tokenized features.
+    """
+    # Initialize tokenizer
+    tokenizer = Tokenizer(lower=True, char_level=True, oov_token='-n-')
+    tokenizer.fit_on_texts(train_features + val_features + test_features)
+
+    # Tokenize and pad sequences
+    x_train = pad_sequences(tokenizer.texts_to_sequences(train_features), maxlen=sequence_length)
+    x_val = pad_sequences(tokenizer.texts_to_sequences(val_features), maxlen=sequence_length)
+    x_test = pad_sequences(tokenizer.texts_to_sequences(test_features), maxlen=sequence_length)
+
+    return x_train, x_val, x_test, tokenizer
+
+def tokenize_url(tokenizer, url, sequence_length=200):
+    """
+    Tokenizes the given url using a pre-loaded tokenizer and returns the tokenized sequence.
+    """
+    return pad_sequences(tokenizer.texts_to_sequences([url]), maxlen=sequence_length)
+
```

