# Comparing `tmp/phylo2vec-0.1.2.tar.gz` & `tmp/phylo2vec-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phylo2vec-0.1.2.tar", last modified: Wed Mar 13 12:27:33 2024, max compression
+gzip compressed data, was "phylo2vec-0.1.3.tar", last modified: Sun May 12 16:53:16 2024, max compression
```

## Comparing `phylo2vec-0.1.2.tar` & `phylo2vec-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     7651 2023-11-10 11:05:51.000000 phylo2vec-0.1.2/LICENSE
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     3198 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/PKG-INFO
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     2442 2024-03-13 12:14:51.000000 phylo2vec-0.1.2/README.md
-drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/phylo2vec/
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)        0 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/__init__.py
-drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/phylo2vec/base/
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      228 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/base/__init__.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     5431 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/base/to_newick.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     4545 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/base/to_vector.py
-drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/phylo2vec/datasets/
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      152 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/datasets/__init__.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     2576 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/datasets/_base.py
-drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/phylo2vec/datasets/data/
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)        0 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/datasets/data/__init__.py
-drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/phylo2vec/datasets/descr/
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)        0 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/datasets/descr/__init__.py
-drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/phylo2vec/opt/
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      170 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/opt/__init__.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     2424 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/opt/_base.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     7571 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/opt/_hc.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     3675 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/opt/_hc_losses.py
-drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/phylo2vec/tests/
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)        0 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/tests/__init__.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      278 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/tests/config.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      987 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/tests/test_utils.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     3137 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/tests/test_v2newick2v.py
-drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/phylo2vec/utils/
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      548 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/utils/__init__.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     3120 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/utils/newick.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      589 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/utils/random.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      400 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/utils/validation.py
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     6135 2023-11-10 11:05:36.000000 phylo2vec-0.1.2/phylo2vec/utils/vector.py
-drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/phylo2vec.egg-info/
--rw-r--r--   0 nclow23   (1002) nclow23   (1002)     3198 2024-03-13 12:27:33.000000 phylo2vec-0.1.2/phylo2vec.egg-info/PKG-INFO
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      795 2024-03-13 12:27:33.000000 phylo2vec-0.1.2/phylo2vec.egg-info/SOURCES.txt
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)        1 2024-03-13 12:27:33.000000 phylo2vec-0.1.2/phylo2vec.egg-info/dependency_links.txt
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)       60 2024-03-13 12:27:33.000000 phylo2vec-0.1.2/phylo2vec.egg-info/requires.txt
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)       10 2024-03-13 12:27:33.000000 phylo2vec-0.1.2/phylo2vec.egg-info/top_level.txt
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      216 2023-11-10 11:06:11.000000 phylo2vec-0.1.2/pyproject.toml
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)       38 2024-03-13 12:27:33.204603 phylo2vec-0.1.2/setup.cfg
--rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     1260 2024-03-13 12:26:38.000000 phylo2vec-0.1.2/setup.py
+drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-05-12 16:53:16.686331 phylo2vec-0.1.3/
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     7651 2023-11-10 11:05:51.000000 phylo2vec-0.1.3/LICENSE
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     3244 2024-05-12 16:53:16.686331 phylo2vec-0.1.3/PKG-INFO
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     2442 2024-03-13 12:14:51.000000 phylo2vec-0.1.3/README.md
+drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-05-12 16:53:16.682331 phylo2vec-0.1.3/phylo2vec/
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)        0 2023-11-10 11:05:36.000000 phylo2vec-0.1.3/phylo2vec/__init__.py
+drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-05-12 16:53:16.682331 phylo2vec-0.1.3/phylo2vec/base/
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      228 2023-11-10 11:05:36.000000 phylo2vec-0.1.3/phylo2vec/base/__init__.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     5407 2024-05-12 16:17:14.000000 phylo2vec-0.1.3/phylo2vec/base/to_newick.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     4579 2024-05-12 16:20:06.000000 phylo2vec-0.1.3/phylo2vec/base/to_vector.py
+drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-05-12 16:53:16.682331 phylo2vec-0.1.3/phylo2vec/datasets/
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      152 2023-11-10 11:05:36.000000 phylo2vec-0.1.3/phylo2vec/datasets/__init__.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     2577 2024-05-12 16:20:29.000000 phylo2vec-0.1.3/phylo2vec/datasets/_base.py
+drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-05-12 16:53:16.682331 phylo2vec-0.1.3/phylo2vec/datasets/data/
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)        0 2023-11-10 11:05:36.000000 phylo2vec-0.1.3/phylo2vec/datasets/data/__init__.py
+drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-05-12 16:53:16.682331 phylo2vec-0.1.3/phylo2vec/datasets/descr/
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)        0 2023-11-10 11:05:36.000000 phylo2vec-0.1.3/phylo2vec/datasets/descr/__init__.py
+drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-05-12 16:53:16.682331 phylo2vec-0.1.3/phylo2vec/opt/
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      170 2023-11-10 11:05:36.000000 phylo2vec-0.1.3/phylo2vec/opt/__init__.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     2425 2024-05-12 16:21:06.000000 phylo2vec-0.1.3/phylo2vec/opt/_base.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     7571 2023-11-10 11:05:36.000000 phylo2vec-0.1.3/phylo2vec/opt/_hc.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     3675 2023-11-10 11:05:36.000000 phylo2vec-0.1.3/phylo2vec/opt/_hc_losses.py
+drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-05-12 16:53:16.686331 phylo2vec-0.1.3/phylo2vec/tests/
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)        0 2023-11-10 11:05:36.000000 phylo2vec-0.1.3/phylo2vec/tests/__init__.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      278 2023-11-10 11:05:36.000000 phylo2vec-0.1.3/phylo2vec/tests/config.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     1714 2024-05-12 16:49:41.000000 phylo2vec-0.1.3/phylo2vec/tests/test_utils.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     3138 2024-05-12 16:23:41.000000 phylo2vec-0.1.3/phylo2vec/tests/test_v2newick2v.py
+drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-05-12 16:53:16.686331 phylo2vec-0.1.3/phylo2vec/utils/
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      607 2024-05-12 16:50:05.000000 phylo2vec-0.1.3/phylo2vec/utils/__init__.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     3121 2024-05-12 16:24:07.000000 phylo2vec-0.1.3/phylo2vec/utils/newick.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      621 2024-05-12 16:24:34.000000 phylo2vec-0.1.3/phylo2vec/utils/random.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      401 2024-05-12 16:50:24.000000 phylo2vec-0.1.3/phylo2vec/utils/validation.py
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     9442 2024-05-12 16:47:55.000000 phylo2vec-0.1.3/phylo2vec/utils/vector.py
+drwxrwxr-x   0 nclow23   (1002) nclow23   (1002)        0 2024-05-12 16:53:16.682331 phylo2vec-0.1.3/phylo2vec.egg-info/
+-rw-r--r--   0 nclow23   (1002) nclow23   (1002)     3244 2024-05-12 16:53:16.000000 phylo2vec-0.1.3/phylo2vec.egg-info/PKG-INFO
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      795 2024-05-12 16:53:16.000000 phylo2vec-0.1.3/phylo2vec.egg-info/SOURCES.txt
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)        1 2024-05-12 16:53:16.000000 phylo2vec-0.1.3/phylo2vec.egg-info/dependency_links.txt
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)       60 2024-05-12 16:53:16.000000 phylo2vec-0.1.3/phylo2vec.egg-info/requires.txt
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)       10 2024-05-12 16:53:16.000000 phylo2vec-0.1.3/phylo2vec.egg-info/top_level.txt
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)      216 2023-11-10 11:06:11.000000 phylo2vec-0.1.3/pyproject.toml
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)       38 2024-05-12 16:53:16.686331 phylo2vec-0.1.3/setup.cfg
+-rw-rw-r--   0 nclow23   (1002) nclow23   (1002)     1305 2024-05-12 16:40:29.000000 phylo2vec-0.1.3/setup.py
```

### Comparing `phylo2vec-0.1.2/LICENSE` & `phylo2vec-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phylo2vec-0.1.2/PKG-INFO` & `phylo2vec-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: phylo2vec
-Version: 0.1.2
+Version: 0.1.3
 Summary: Phylo2Vec: integer vector representation of binary (phylogenetic) trees
 Home-page: https://github.com/Neclow/phylo2vec
 Author: Neil Scheidwasser
 Author-email: neil.clow@sund.ku.dk
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `phylo2vec-0.1.2/README.md` & `phylo2vec-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `phylo2vec-0.1.2/phylo2vec/base/to_newick.py` & `phylo2vec-0.1.3/phylo2vec/base/to_newick.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Methods to convert a Phylo2Vec vector to a Newick-format string.
 """
+
 import numba as nb
 import numpy as np
 
 
 @nb.njit(cache=True)
 def _get_ancestry(v):
     """
+    Get the "ancestry" of v (see "Returns" paragraph)
 
-    New get ancestry, but with a MUCH clearer interpretation of what v[i] is.
     v[i] = which BRANCH we do the pairing from
 
-
     The initial situation looks like this:
                       R
                       |
                       | --> branch 2
                     // \\
       branch 0 <-- //   \\  --> branch 1
                    0     1
@@ -64,15 +64,15 @@
             # which is deeper than the branch v[i]
             pairs.insert(
                 v[i] - len(pairs), (pairs[v[i] - len(pairs) - 1][0], next_leaf)
             )
 
     # We have our pairs, we can now build our ancestry
     # Matrix with 3 columns: child1, child2, parent
-    ancestry = np.zeros((len(pairs), 3), dtype=np.int32)
+    ancestry = np.zeros((len(pairs), 3), dtype=np.int16)
 
     # Dictionary to keep track of the following relationship: child->highest parent
     parents = nb.typed.Dict.empty(key_type=nb.types.int64, value_type=nb.types.int64)
 
     # Dictionary to keep track of siblings (i.e., sister nodes)
     siblings = nb.typed.Dict.empty(key_type=nb.types.int64, value_type=nb.types.int64)
```

### Comparing `phylo2vec-0.1.2/phylo2vec/base/to_vector.py` & `phylo2vec-0.1.3/phylo2vec/base/to_vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Methods to convert a Newick to a Phylo2Vec vector.
 
 Two main methods:
     - to_vector for a Newick with parent labels
     - to_vector_no_parents for a Newick without parent labels
 """
+
 import numba as nb
 import numpy as np
 
 
 def _reduce(newick):
     ancestry = []
 
@@ -29,15 +30,15 @@
                 )
                 newick = newick[: open_idx - 1] + newick[i + 1 :]
 
                 return do_reduce(ancestry, newick)
 
     do_reduce(ancestry, newick[:-1])
 
-    return np.array(ancestry)
+    return np.array(ancestry, dtype=np.int16)
 
 
 def _reduce_no_parents(newick):
     ancestry = []
 
     def do_reduce(ancestry, newick):
         for i, char in enumerate(newick):
@@ -55,23 +56,23 @@
                     newick[open_idx - 1 : i + 1], f"{min(child1, child2)}"
                 )
 
                 return do_reduce(ancestry, newick)
 
     do_reduce(ancestry, newick[:-1])
 
-    return np.array(ancestry)
+    return np.array(ancestry, dtype=np.int16)
 
 
 @nb.njit(cache=True)
 def _find_cherries(ancestry):
     ancestry_sorted = ancestry[np.argsort(ancestry[:, -1]), :]
 
     small_children = nb.typed.Dict.empty(
-        key_type=nb.types.int64, value_type=nb.types.int64
+        key_type=nb.types.int16, value_type=nb.types.int16
     )
 
     for i, row in enumerate(ancestry_sorted):
         c1, c2, p = row
 
         parent_c1, parent_c2 = small_children.get(c1, c1), small_children.get(c2, c2)
 
@@ -122,15 +123,15 @@
     cherries_ = cherries_[cherries_[:, -1].argsort()]
 
     return cherries_[:, :-1]
 
 
 @nb.njit(cache=True)
 def _build_vector(cherries):
-    v_res = np.zeros((cherries.shape[0],), dtype=np.int16)
+    v_res = np.zeros((cherries.shape[0],), dtype=np.uint16)
     for i in range(cherries.shape[0] - 1, -1, -1):
         c1, c2, _ = cherries[i]
 
         c_max = max(c1, c2)
 
         subset = cherries[cherries[:, -1] <= c_max][:, :-1]
 
@@ -141,15 +142,15 @@
         else:
             v_res[c_max - 1] = c_max - 1 + idx
 
     return v_res
 
 
 def to_vector(newick):
-    """Convert a newick string with parent labels to a vector
+    """Convert a Newick string with parent labels to a vector
 
     Parameters
     ----------
     newick : str
         Newick string for a tree
 
     Returns
@@ -163,15 +164,15 @@
 
     v = _build_vector(cherries)
 
     return v
 
 
 def to_vector_no_parents(newick_no_parents):
-    """Convert a newick string without parent labels to a vector
+    """Convert a Newick string without parent labels to a vector
 
     Parameters
     ----------
     newick_no_parents : str
         Newick string for a tree
 
     Returns
```

### Comparing `phylo2vec-0.1.2/phylo2vec/datasets/_base.py` & `phylo2vec-0.1.3/phylo2vec/datasets/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base IO code for all datasets."""
+
 from importlib import resources
 
 from Bio import SeqIO
 
 DATA_MODULE = "phylo2vec.datasets.data"
 DESCR_MODULE = "phylo2vec.datasets.descr"
```

### Comparing `phylo2vec-0.1.2/phylo2vec/opt/_base.py` & `phylo2vec-0.1.3/phylo2vec/opt/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base class for all optimisation methods in Phylo2Vec."""
+
 import random
 
 import numba as nb
 
 from phylo2vec.datasets import read_fasta
 from phylo2vec.utils import sample, seed_everything
```

### Comparing `phylo2vec-0.1.2/phylo2vec/opt/_hc.py` & `phylo2vec-0.1.3/phylo2vec/opt/_hc.py`

 * *Files identical despite different names*

### Comparing `phylo2vec-0.1.2/phylo2vec/opt/_hc_losses.py` & `phylo2vec-0.1.3/phylo2vec/opt/_hc_losses.py`

 * *Files identical despite different names*

### Comparing `phylo2vec-0.1.2/phylo2vec/tests/test_utils.py` & `phylo2vec-0.1.3/phylo2vec/tests/test_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 """Tests for utility functions."""
+
+import random
+
+import numpy as np
 import pytest
 
 from phylo2vec.tests.config import MIN_N_LEAVES, MAX_N_LEAVES, N_REPEATS
-from phylo2vec.base.to_newick import to_newick
+from phylo2vec.base import to_newick
 from phylo2vec.utils import (
+    add_leaf,
     check_v,
+    remove_leaf,
     sample,
     find_num_leaves,
 )
 
 
 @pytest.mark.parametrize("n_leaves", range(MIN_N_LEAVES, MAX_N_LEAVES + 1))
 def test_sample(n_leaves):
@@ -35,9 +41,37 @@
     """
     for _ in range(N_REPEATS):
         v = sample(n_leaves)
         newick = to_newick(v)
         assert find_num_leaves(newick) == n_leaves
 
 
+@pytest.mark.parametrize("n_leaves", range(MIN_N_LEAVES, MAX_N_LEAVES + 1))
+def test_remove_and_add(n_leaves):
+    """Test removing and adding a node to a vector
+
+    Sample a v, remove a random leaf and add it back
+    Test if we recover the same v
+
+    Parameters
+    ----------
+    n_leaves : int
+        Number of leaves
+    """
+    for _ in range(N_REPEATS):
+        v = sample(n_leaves)
+
+        leaf = random.randint(0, n_leaves - 1)
+
+        v_sub, sis = remove_leaf(v, leaf)
+
+        # To deal with increment when removing a leaf
+        if sis >= leaf:
+            sis -= 1
+
+        v_add = add_leaf(v_sub, leaf, sis)
+
+        assert np.array_equal(v, v_add)
+
+
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `phylo2vec-0.1.2/phylo2vec/tests/test_v2newick2v.py` & `phylo2vec-0.1.3/phylo2vec/tests/test_v2newick2v.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test conversion from v to newick and back to v"""
+
 import numpy as np
 import pytest
 
 from ete3 import Tree
 
 from phylo2vec.tests.config import MIN_N_LEAVES, MAX_N_LEAVES, N_REPEATS
 from phylo2vec.base import to_newick, to_vector, to_vector_no_parents
```

### Comparing `phylo2vec-0.1.2/phylo2vec/utils/newick.py` & `phylo2vec-0.1.3/phylo2vec/utils/newick.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Newick string manipulation functions"""
+
 import re
 
 
 # Pattern of an integer label on the left of a pair
 LEFT_NODE_PATTERN = re.compile(r"\(\b\d+\b")
 # Pattern of an integer label on the right of a pair
 RIGHT_NODE_PATTERN = re.compile(r",\b\d+\b")
```

### Comparing `phylo2vec-0.1.2/phylo2vec/utils/random.py` & `phylo2vec-0.1.3/phylo2vec/utils/random.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Random utility functions: sampling and seeding."""
+
 import os
 import random
 import numpy as np
 
 
 def sample(n_leaves):
     """Sample a random tree via Phylo2Vec
 
     Returns
     -------
     numpy.ndarray
         Phylo2Vec vector where v_i in {0, 1, ..., 2*i}
     """
-    return np.array([random.randint(0, 2 * i) for i in range(n_leaves - 1)])
+    return np.array(
+        [random.randint(0, 2 * i) for i in range(n_leaves - 1)], dtype=np.uint16
+    )
 
 
 def seed_everything(seed):
     """Seed random, the Python hash seed, numpy
 
     Parameters
     ----------
```

### Comparing `phylo2vec-0.1.2/phylo2vec.egg-info/PKG-INFO` & `phylo2vec-0.1.3/phylo2vec.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: phylo2vec
-Version: 0.1.2
+Version: 0.1.3
 Summary: Phylo2Vec: integer vector representation of binary (phylogenetic) trees
 Home-page: https://github.com/Neclow/phylo2vec
 Author: Neil Scheidwasser
 Author-email: neil.clow@sund.ku.dk
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `phylo2vec-0.1.2/phylo2vec.egg-info/SOURCES.txt` & `phylo2vec-0.1.3/phylo2vec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phylo2vec-0.1.2/setup.py` & `phylo2vec-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="phylo2vec",
-    version="0.1.2",
+    version="0.1.3",
     description="Phylo2Vec: integer vector representation of binary (phylogenetic) trees",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",  # This is important!
     author="Neil Scheidwasser",
     author_email="neil.clow@sund.ku.dk",
     url="https://github.com/Neclow/phylo2vec",
     packages=find_packages(),
@@ -23,17 +23,18 @@
     install_requires=[
         "numba==0.56.4",
         "numpy==1.23.5",
         "biopython==1.80.0",
         "joblib==1.1.1",
     ],
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Alpha",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
     ],
 )
```

