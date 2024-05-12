# Comparing `tmp/bw_graph_tools-0.3.tar.gz` & `tmp/bw_graph_tools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_graph_tools-0.3.tar", last modified: Sun Nov 12 12:39:40 2023, max compression
+gzip compressed data, was "bw_graph_tools-0.3.1.tar", last modified: Sun May 12 02:21:12 2024, max compression
```

## Comparing `bw_graph_tools-0.3.tar` & `bw_graph_tools-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,27 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-11-12 12:39:40.283840 bw_graph_tools-0.3/
--rw-r--r--   0 cmutel     (501) staff       (20)     1456 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)       31 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     4979 2023-11-12 12:39:40.283774 bw_graph_tools-0.3/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     3493 2023-08-08 09:54:02.000000 bw_graph_tools-0.3/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-11-12 12:39:40.281481 bw_graph_tools-0.3/bw_graph_tools/
--rw-r--r--   0 cmutel     (501) staff       (20)        4 2023-11-12 12:38:48.000000 bw_graph_tools-0.3/bw_graph_tools/VERSION
--rw-r--r--   0 cmutel     (501) staff       (20)      652 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/bw_graph_tools/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)      123 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/bw_graph_tools/errors.py
--rw-r--r--   0 cmutel     (501) staff       (20)    25895 2023-08-08 08:44:43.000000 bw_graph_tools-0.3/bw_graph_tools/graph_traversal.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2077 2023-11-12 12:38:48.000000 bw_graph_tools-0.3/bw_graph_tools/graph_traversal_utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)     8742 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/bw_graph_tools/matrix_tools.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7924 2023-11-12 12:38:48.000000 bw_graph_tools-0.3/bw_graph_tools/shortest_path.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1265 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/bw_graph_tools/testing.py
--rw-r--r--   0 cmutel     (501) staff       (20)      349 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/bw_graph_tools/utils.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-11-12 12:39:40.282335 bw_graph_tools-0.3/bw_graph_tools.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     4979 2023-11-12 12:39:40.000000 bw_graph_tools-0.3/bw_graph_tools.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      962 2023-11-12 12:39:40.000000 bw_graph_tools-0.3/bw_graph_tools.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-11-12 12:39:40.000000 bw_graph_tools-0.3/bw_graph_tools.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2023-08-08 08:54:24.000000 bw_graph_tools-0.3/bw_graph_tools.egg-info/not-zip-safe
--rw-r--r--   0 cmutel     (501) staff       (20)      174 2023-11-12 12:39:40.000000 bw_graph_tools-0.3/bw_graph_tools.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       35 2023-11-12 12:39:40.000000 bw_graph_tools-0.3/bw_graph_tools.egg-info/top_level.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-11-12 12:39:40.280343 bw_graph_tools-0.3/docs/
--rw-r--r--   0 cmutel     (501) staff       (20)     2261 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/docs/conf.py
--rw-r--r--   0 cmutel     (501) staff       (20)       87 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/pyproject.toml
--rw-r--r--   0 cmutel     (501) staff       (20)     1701 2023-11-12 12:39:40.284199 bw_graph_tools-0.3/setup.cfg
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-11-12 12:39:40.283133 bw_graph_tools-0.3/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)     5819 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/tests/test_first_heuristic.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2494 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/tests/test_get_path_from_matrix.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1176 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/tests/test_matrix_utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4782 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/tests/test_second_heuristic.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3670 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/tests/test_third_heuristic.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2023-11-12 12:39:40.281321 bw_graph_tools-0.3/tests/traversal/
--rw-r--r--   0 cmutel     (501) staff       (20)     5256 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/tests/traversal/test_marc_vd_meide.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7103 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/tests/traversal/test_negative_production.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7095 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/tests/traversal/test_nonunitary_production_with_recursion.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4550 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/tests/traversal/test_only_one_layer.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7254 2023-08-08 08:41:58.000000 bw_graph_tools-0.3/tests/traversal/test_separate_production.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 02:21:12.876002 bw_graph_tools-0.3.1/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1456 2024-05-12 00:14:28.000000 bw_graph_tools-0.3.1/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2024-05-12 00:14:20.000000 bw_graph_tools-0.3.1/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     4881 2024-05-12 02:21:12.875817 bw_graph_tools-0.3.1/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     3201 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 02:21:12.872735 bw_graph_tools-0.3.1/bw_graph_tools/
+-rw-r--r--   0 cmutel     (501) staff       (20)      603 2024-05-12 01:52:38.000000 bw_graph_tools-0.3.1/bw_graph_tools/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      123 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/bw_graph_tools/errors.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    25946 2024-05-12 02:13:01.000000 bw_graph_tools-0.3.1/bw_graph_tools/graph_traversal.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2077 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/bw_graph_tools/graph_traversal_utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     9280 2024-05-12 01:31:09.000000 bw_graph_tools-0.3.1/bw_graph_tools/matrix_tools.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     7924 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/bw_graph_tools/shortest_path.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1295 2024-05-12 02:11:22.000000 bw_graph_tools-0.3.1/bw_graph_tools/testing.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 02:21:12.875157 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     4881 2024-05-12 02:21:12.000000 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      601 2024-05-12 02:21:12.000000 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-12 02:21:12.000000 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      205 2024-05-12 02:21:12.000000 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       15 2024-05-12 02:21:12.000000 bw_graph_tools-0.3.1/bw_graph_tools.egg-info/top_level.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)     2478 2024-05-12 02:00:32.000000 bw_graph_tools-0.3.1/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)       38 2024-05-12 02:21:12.876048 bw_graph_tools-0.3.1/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 02:21:12.874764 bw_graph_tools-0.3.1/tests/
+-rw-r--r--   0 cmutel     (501) staff       (20)     7001 2024-05-12 01:36:14.000000 bw_graph_tools-0.3.1/tests/test_first_heuristic.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2494 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/tests/test_get_path_from_matrix.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1176 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/tests/test_matrix_utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4782 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/tests/test_second_heuristic.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3670 2024-05-11 23:47:54.000000 bw_graph_tools-0.3.1/tests/test_third_heuristic.py
```

### Comparing `bw_graph_tools-0.3/LICENSE` & `bw_graph_tools-0.3.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2023 Chris Mutel
+Copyright 2024 Chris Mutel
 
 Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
 2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
```

### Comparing `bw_graph_tools-0.3/PKG-INFO` & `bw_graph_tools-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: bw_graph_tools
-Version: 0.3
+Version: 0.3.1
 Summary: Graph traversal class and utilities
-Home-page: https://github.com/brightway-lca/bw_graph_tools
-Author: Chris Mutel
-Author-email: <cmutel@gmail.com>
-Maintainer: Chris Mutel
-Maintainer-email: <cmutel@gmail.com>
-License: BSD-3-Clause
+Author-email: Chris Mutel <cmutel@gmail.com>
+Maintainer-email: Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/bw_graph_tools
 Project-URL: homepage, https://github.com/brightway-lca/bw_graph_tools
 Project-URL: tracker, https://github.com/brightway-lca/bw_graph_tools/issues
-Keywords: "brightway","development"
-Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bw2calc>=2.0.dev13
+Requires-Dist: bw_processing
 Requires-Dist: matrix_utils
-Requires-Dist: numpy
+Requires-Dist: numpy<2
 Requires-Dist: scipy
-Requires-Dist: bw_processing
 Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: bw_graph_tools; extra == "testing"
+Requires-Dist: bw2data; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: bw2data>=4.0.dev18; extra == "testing"
+Requires-Dist: python-coveralls; extra == "testing"
 Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: myst_parser; extra == "docs"
-Requires-Dist: furo; extra == "docs"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-randomly; extra == "dev"
+Requires-Dist: setuptools; extra == "dev"
 
 # bw_graph_tools
 
 [![PyPI](https://img.shields.io/pypi/v/bw_graph_tools.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/bw_graph_tools.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/bw_graph_tools)][pypi status]
 [![License](https://img.shields.io/pypi/l/bw_graph_tools)][license]
@@ -81,15 +82,14 @@
 * Distinguishing between different paths to the same object
 
 * Convolving temporal distributions
 
 If we add temporal information using `bw_temporalis`, then the same node can occur at different times depending on how the temporal dynamics its preceding path. For example:
 
 
-
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
 
@@ -99,19 +99,13 @@
 ## Issues
 
 If you encounter any problems,
 please [file an issue] along with a detailed description.
 
 ## Documentation
 
-1. Install the `sphinx-furo` conda environment from the file `.docs/environment.yml`.
-2. Build the documentation locally by running
+1. Install the conda environment from the file `.docs/environment.yml`
+2. Build the documentation locally by running:
 
-```
+```bash
 sphinx-autobuild docs _build/html -a -j auto --open-browser
 ```
-
-<!-- github-only -->
-
-[command-line reference]: https://bw_graph_tools.readthedocs.io/en/latest/usage.html
-[license]: https://github.com/brightway-lca/bw_graph_tools/blob/main/LICENSE
-[contributor guide]: https://github.com/brightway-lca/bw_graph_tools/blob/main/CONTRIBUTING.md
```

### Comparing `bw_graph_tools-0.3/README.md` & `bw_graph_tools-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 * Distinguishing between different paths to the same object
 
 * Convolving temporal distributions
 
 If we add temporal information using `bw_temporalis`, then the same node can occur at different times depending on how the temporal dynamics its preceding path. For example:
 
 
-
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
 
@@ -58,19 +57,13 @@
 ## Issues
 
 If you encounter any problems,
 please [file an issue] along with a detailed description.
 
 ## Documentation
 
-1. Install the `sphinx-furo` conda environment from the file `.docs/environment.yml`.
-2. Build the documentation locally by running
+1. Install the conda environment from the file `.docs/environment.yml`
+2. Build the documentation locally by running:
 
-```
+```bash
 sphinx-autobuild docs _build/html -a -j auto --open-browser
-```
-
-<!-- github-only -->
-
-[command-line reference]: https://bw_graph_tools.readthedocs.io/en/latest/usage.html
-[license]: https://github.com/brightway-lca/bw_graph_tools/blob/main/LICENSE
-[contributor guide]: https://github.com/brightway-lca/bw_graph_tools/blob/main/CONTRIBUTING.md
+```
```

### Comparing `bw_graph_tools-0.3/bw_graph_tools/__init__.py` & `bw_graph_tools-0.3.1/bw_graph_tools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,18 @@
     "guess_production_exchanges",
     "NewNodeEachVisitGraphTraversal",
     "Node",
     "path_as_brightway_objects",
     "to_normalized_adjacency_matrix",
 )
 
+__version__ = "0.3.1"
+
 from .graph_traversal_utils import get_path_from_matrix, path_as_brightway_objects
 from .matrix_tools import guess_production_exchanges, to_normalized_adjacency_matrix
-from .utils import get_version_tuple
 from .graph_traversal import (
     AssumedDiagonalGraphTraversal,
     Edge,
     Flow,
     NewNodeEachVisitGraphTraversal,
     Node,
 )
-
-__version__ = get_version_tuple()
```

### Comparing `bw_graph_tools-0.3/bw_graph_tools/graph_traversal.py` & `bw_graph_tools-0.3.1/bw_graph_tools/graph_traversal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 from dataclasses import dataclass
 from functools import lru_cache
 from heapq import heappop, heappush
+from typing import Optional
 
 from bw2calc import LCA
 from scipy.sparse import spmatrix
 import matrix_utils as mu
 import numpy as np
 
 try:
@@ -172,21 +173,21 @@
 
     """
 
     @classmethod
     def calculate(
         cls,
         lca_object: LCA,
-        cutoff: float | None = 5e-3,
-        biosphere_cutoff: float | None = 1e-4,
-        max_calc: int | None = 1e5,
-        skip_coproducts: bool | None = False,
-        separate_biosphere_flows: bool | None = True,
-        static_activity_indices: set[int] | None = set(),
-        functional_unit_unique_id: int | None = -1,
+        cutoff: Optional[float] = 5e-3,
+        biosphere_cutoff: Optional[float] = 1e-4,
+        max_calc: Optional[int] = 10000,
+        skip_coproducts: Optional[bool] = False,
+        separate_biosphere_flows: Optional[bool] = True,
+        static_activity_indices: Optional[set[int]] = set(),
+        functional_unit_unique_id: Optional[int] = -1,
     ) -> dict:
         """
         Priority-first traversal (i.e. follow the past of highest score) of the supply chain graph. This class unrolls
         the graph, i.e. every time it arrives at a given activity, it treats
         it as a separate node in the graph.
 
         In contrast with previous graph traversal implementations, we do not assume reference production exchanges are on the diagonal. It should also correctly handle the following:
@@ -236,16 +237,16 @@
             Add separate `Flow` nodes for important individual biosphere
             emissions
         static_activity_indices : set
             A set of activity matrix indices which we don't want the graph to
             traverse
         functional_unit_unique_id : int
             An integer id we can use for the functional unit virtual activity.
-            Shouldn't overlap any other activity ids. Don't change unless you r
-            eally know what you are doing.
+            Shouldn't overlap any other activity ids. Don't change unless you 
+            really know what you are doing.
 
         Returns
         -------
         dict
             Dictionary with keys `nodes`, `edges`, `flows`, `calculation_counter`
 
         """
```

### Comparing `bw_graph_tools-0.3/bw_graph_tools/graph_traversal_utils.py` & `bw_graph_tools-0.3.1/bw_graph_tools/graph_traversal_utils.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3/bw_graph_tools/matrix_tools.py` & `bw_graph_tools-0.3.1/bw_graph_tools/matrix_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,16 +63,27 @@
         group: mu.ResourceGroup,
     ) -> Tuple[np.ndarray, np.ndarray]:
         indices = group.get_indices_data()
 
         # Need to check the original input values, not after mapping when they are
         # normalized to [0, X] range.
         ident_mask = indices["row"] == indices["col"]
-        row_mapped = group.row_mapper.map_array(indices["row"][ident_mask])
-        col_mapped = group.col_mapper.map_array(indices["col"][ident_mask])
+
+        # In theory these values should be on the diagonal, as the input row and col
+        # values are the same. However, we don't have a strong guarantee that this is
+        # true. So to eliminate duplicate values we combine to a (X, 2) array, and get
+        # unique rows.
+        # Note that `unique` also does sorting, see 
+        # https://stackoverflow.com/questions/16970982/find-unique-rows-in-numpy-array
+        combined = np.unique(np.vstack((
+            group.row_mapper.map_array(indices["row"][ident_mask]),
+            group.col_mapper.map_array(indices["col"][ident_mask])
+        )), axis=1)
+        row_mapped = combined[0, :]
+        col_mapped = combined[1, :]
 
         if (row_mapped == -1).sum() or (col_mapped == -1).sum():
             ERROR = """
 Found unmapped values in technosphere matrix generator, but that should be impossible.
 
 {} unmapped values in the row indices: {}
 {} unmapped values in the column indices: {}
```

### Comparing `bw_graph_tools-0.3/bw_graph_tools/shortest_path.py` & `bw_graph_tools-0.3.1/bw_graph_tools/shortest_path.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3/bw_graph_tools/testing.py` & `bw_graph_tools-0.3.1/bw_graph_tools/testing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from numbers import Number
+from typing import Union
 import numpy as np
 
 from . import Node, Edge, Flow
 
 
-def equal_dict(a: Node | Edge | Flow, b: dict, fields: list[str]):
+def equal_dict(a: Union[Node, Edge, Flow], b: dict, fields: list[str]):
     for field in fields:
         if field in b:
             if isinstance(b[field], Number):
                 assert np.allclose(getattr(a, field), b[field])
             else:
                 assert getattr(a, field) == b[field]
```

### Comparing `bw_graph_tools-0.3/bw_graph_tools.egg-info/PKG-INFO` & `bw_graph_tools-0.3.1/bw_graph_tools.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
-Name: bw-graph-tools
-Version: 0.3
+Name: bw_graph_tools
+Version: 0.3.1
 Summary: Graph traversal class and utilities
-Home-page: https://github.com/brightway-lca/bw_graph_tools
-Author: Chris Mutel
-Author-email: <cmutel@gmail.com>
-Maintainer: Chris Mutel
-Maintainer-email: <cmutel@gmail.com>
-License: BSD-3-Clause
+Author-email: Chris Mutel <cmutel@gmail.com>
+Maintainer-email: Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/bw_graph_tools
 Project-URL: homepage, https://github.com/brightway-lca/bw_graph_tools
 Project-URL: tracker, https://github.com/brightway-lca/bw_graph_tools/issues
-Keywords: "brightway","development"
-Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bw2calc>=2.0.dev13
+Requires-Dist: bw_processing
 Requires-Dist: matrix_utils
-Requires-Dist: numpy
+Requires-Dist: numpy<2
 Requires-Dist: scipy
-Requires-Dist: bw_processing
 Provides-Extra: testing
-Requires-Dist: setuptools; extra == "testing"
+Requires-Dist: bw_graph_tools; extra == "testing"
+Requires-Dist: bw2data; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: bw2data>=4.0.dev18; extra == "testing"
+Requires-Dist: python-coveralls; extra == "testing"
 Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
-Provides-Extra: docs
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: myst_parser; extra == "docs"
-Requires-Dist: furo; extra == "docs"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-randomly; extra == "dev"
+Requires-Dist: setuptools; extra == "dev"
 
 # bw_graph_tools
 
 [![PyPI](https://img.shields.io/pypi/v/bw_graph_tools.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/bw_graph_tools.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/bw_graph_tools)][pypi status]
 [![License](https://img.shields.io/pypi/l/bw_graph_tools)][license]
@@ -81,15 +82,14 @@
 * Distinguishing between different paths to the same object
 
 * Convolving temporal distributions
 
 If we add temporal information using `bw_temporalis`, then the same node can occur at different times depending on how the temporal dynamics its preceding path. For example:
 
 
-
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
 
@@ -99,19 +99,13 @@
 ## Issues
 
 If you encounter any problems,
 please [file an issue] along with a detailed description.
 
 ## Documentation
 
-1. Install the `sphinx-furo` conda environment from the file `.docs/environment.yml`.
-2. Build the documentation locally by running
+1. Install the conda environment from the file `.docs/environment.yml`
+2. Build the documentation locally by running:
 
-```
+```bash
 sphinx-autobuild docs _build/html -a -j auto --open-browser
 ```
-
-<!-- github-only -->
-
-[command-line reference]: https://bw_graph_tools.readthedocs.io/en/latest/usage.html
-[license]: https://github.com/brightway-lca/bw_graph_tools/blob/main/LICENSE
-[contributor guide]: https://github.com/brightway-lca/bw_graph_tools/blob/main/CONTRIBUTING.md
```

### Comparing `bw_graph_tools-0.3/tests/test_first_heuristic.py` & `bw_graph_tools-0.3.1/tests/test_first_heuristic.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,16 +92,16 @@
         data_array=data,
     )
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
     row, col = gpe_first_heuristic(mm)
-    assert np.array_equal(np.array([1, 0]), row)
-    assert np.array_equal(np.array([1, 0]), col)
+    assert np.array_equal(np.array([0, 1]), row)
+    assert np.array_equal(np.array([0, 1]), col)
 
 
 def test_gpe_first_heuristic_multiple_dp():
     dp1 = bwp.create_datapackage()
     data = np.array([1, 2])
     indices = np.array(
         [
@@ -166,16 +166,16 @@
         data_array=data,
     )
     mm = mu.MappedMatrix(
         packages=[dp1, dp2],
         matrix="test",
     )
     row, col = gpe_first_heuristic(mm)
-    assert np.array_equal(np.array([1, 0]), row)
-    assert np.array_equal(np.array([1, 0]), col)
+    assert np.array_equal(np.array([0, 1]), row)
+    assert np.array_equal(np.array([0, 1]), col)
 
 
 def test_gpe_first_heuristic_mix_product_no_product():
     dp1 = bwp.create_datapackage()
     data = np.array([1, 2, 3, 4])
     indices = np.array(
         [
@@ -224,7 +224,59 @@
     mm = mu.MappedMatrix(
         packages=[dp1],
         matrix="test",
     )
     row, col = gpe_first_heuristic(mm)
     assert row.shape == (0,)
     assert col.shape == (0,)
+
+
+def test_gpe_first_heuristic_same_but_not_diagonal_in_matrix():
+    dp1 = bwp.create_datapackage()
+    data = np.array([1, -0.05, 1])
+    indices = np.array(
+        [
+            (10, 10),
+            (10, 10),
+            (0, 21),
+        ],
+        dtype=bwp.INDICES_DTYPE,
+    )
+    dp1.add_persistent_vector(
+        matrix="test",
+        indices_array=indices,
+        name="foo",
+        data_array=data,
+    )
+    mm = mu.MappedMatrix(
+        packages=[dp1],
+        matrix="test",
+    )
+    row, col = gpe_first_heuristic(mm)
+    assert np.allclose(row, [1])
+    assert np.allclose(col, [0])
+
+
+def test_gpe_first_heuristic_self_consumption():
+    dp1 = bwp.create_datapackage()
+    data = np.array([1, -0.05, 1])
+    indices = np.array(
+        [
+            (1, 1),
+            (1, 1),
+            (2, 2),
+        ],
+        dtype=bwp.INDICES_DTYPE,
+    )
+    dp1.add_persistent_vector(
+        matrix="test",
+        indices_array=indices,
+        name="foo",
+        data_array=data,
+    )
+    mm = mu.MappedMatrix(
+        packages=[dp1],
+        matrix="test",
+    )
+    row, col = gpe_first_heuristic(mm)
+    assert row.shape == (2,)
+    assert col.shape == (2,)
```

### Comparing `bw_graph_tools-0.3/tests/test_get_path_from_matrix.py` & `bw_graph_tools-0.3.1/tests/test_get_path_from_matrix.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3/tests/test_matrix_utils.py` & `bw_graph_tools-0.3.1/tests/test_matrix_utils.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3/tests/test_second_heuristic.py` & `bw_graph_tools-0.3.1/tests/test_second_heuristic.py`

 * *Files identical despite different names*

### Comparing `bw_graph_tools-0.3/tests/test_third_heuristic.py` & `bw_graph_tools-0.3.1/tests/test_third_heuristic.py`

 * *Files identical despite different names*

