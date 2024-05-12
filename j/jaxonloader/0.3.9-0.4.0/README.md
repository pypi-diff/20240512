# Comparing `tmp/jaxonloader-0.3.9.tar.gz` & `tmp/jaxonloader-0.4.0.tar.gz`

## Comparing `jaxonloader-0.3.9.tar` & `jaxonloader-0.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/mkdocs.yml
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/docs/images/performance.png
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/__init__.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/boto_client.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/config.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/dataloader.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/dataset.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/utils.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/datasets/__init__.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/datasets/_datasets.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/jaxonloader/datasets/download.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/tests/test_mnist.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/tests/test_slicing.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/LICENSE
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/README.md
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 jaxonloader-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/docs/future.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/docs/images/performance.png
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/__init__.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/boto_client.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/config.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/utils.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/datasets/__init__.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/datasets/_datasets.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/jaxonloader/datasets/download.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/tests/test_mnist.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/tests/test_slicing.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 jaxonloader-0.4.0/PKG-INFO
```

### Comparing `jaxonloader-0.3.9/.github/workflows/nox.yaml` & `jaxonloader-0.4.0/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/docs/getting-started.md` & `jaxonloader-0.4.0/docs/getting-started.md`

 * *Files 19% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 6. Profit!
 
 Here's an example:
 
 ```python
 
 import pandas as pd
-from jaxonloader import make, from_dataframe
+from jaxonloader import JaxonDataLoader, SingleArrayDataset
 
 # Step 1
 df = pd.read_csv('data.csv')
 
 # Step 2
 df['column'] = df['column'].apply(lambda x: x + 1)
 
 # Step 3
-jaxon_dataset = from_dataframe(df)
+jaxon_dataset = SingleArrayDataset(df.to_numpy())
 
 # Step 4
 jaxon_dataloader = JaxonDataLoader(
-    jaxon_dataset, batch_size=64, shuffle=True, key=subkey, jit=True
+    jaxon_dataset, batch_size=64, shuffle=True
 )
 
 # Step 5
 for x in jaxon_dataloader:
     pass
 
 # Step 6
```

### Comparing `jaxonloader-0.3.9/docs/index.md` & `jaxonloader-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/docs/images/performance.png` & `jaxonloader-0.4.0/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/jaxonloader/config.py` & `jaxonloader-0.4.0/jaxonloader/config.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/jaxonloader/dataloader.py` & `jaxonloader-0.4.0/jaxonloader/dataloader.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/jaxonloader/dataset.py` & `jaxonloader-0.4.0/jaxonloader/dataset.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/jaxonloader/utils.py` & `jaxonloader-0.4.0/jaxonloader/utils.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/jaxonloader/datasets/_datasets.py` & `jaxonloader-0.4.0/jaxonloader/datasets/_datasets.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/jaxonloader/datasets/download.py` & `jaxonloader-0.4.0/jaxonloader/datasets/download.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/tests/test_tinyshakespeare.py` & `jaxonloader-0.4.0/tests/test_tinyshakespeare.py`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/.gitignore` & `jaxonloader-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/LICENSE` & `jaxonloader-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.3.9/README.md` & `jaxonloader-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,14 @@
 # these are JaxonDatasets
 
 train_loader = JaxonDataLoader(
     train,
     batch_size=4,
     shuffle=True,
     drop_last=True,
-    key=key,
-    jit=True
 )
 for x in train_loader:
     pass
 ```
 
 ## Philosophy
```

### Comparing `jaxonloader-0.3.9/pyproject.toml` & `jaxonloader-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "jaxonloader"
-version = "0.3.9"
-description = "A dataloader, but for JAX"
+version = "0.4.0"
+description = "A dataloader, but for JAX/Numpy"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
 dependencies=[
```

### Comparing `jaxonloader-0.3.9/PKG-INFO` & `jaxonloader-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.3.9
-Summary: A dataloader, but for JAX
+Version: 0.4.0
+Summary: A dataloader, but for JAX/Numpy
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -75,16 +75,14 @@
 # these are JaxonDatasets
 
 train_loader = JaxonDataLoader(
     train,
     batch_size=4,
     shuffle=True,
     drop_last=True,
-    key=key,
-    jit=True
 )
 for x in train_loader:
     pass
 ```
 
 ## Philosophy
```

