# Comparing `tmp/bw_aggregation-1.0.tar.gz` & `tmp/bw_aggregation-1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_aggregation-1.0.tar", last modified: Sun May 12 15:30:47 2024, max compression
+gzip compressed data, was "bw_aggregation-1.0rc1.tar", last modified: Sat May 11 20:25:26 2024, max compression
```

## Comparing `bw_aggregation-1.0.tar` & `bw_aggregation-1.0rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 15:30:47.143775 bw_aggregation-1.0/
--rw-r--r--   0 cmutel     (501) staff       (20)     1070 2024-05-09 15:12:25.000000 bw_aggregation-1.0/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2024-05-09 15:12:25.000000 bw_aggregation-1.0/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     9147 2024-05-12 15:30:47.143263 bw_aggregation-1.0/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     7437 2024-05-12 10:18:03.000000 bw_aggregation-1.0/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 15:30:47.140592 bw_aggregation-1.0/bw_aggregation/
--rw-r--r--   0 cmutel     (501) staff       (20)      578 2024-05-12 10:12:37.000000 bw_aggregation-1.0/bw_aggregation/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4597 2024-05-11 11:29:50.000000 bw_aggregation-1.0/bw_aggregation/calculator.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1881 2024-05-12 09:38:25.000000 bw_aggregation-1.0/bw_aggregation/estimator.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7931 2024-05-12 09:27:35.000000 bw_aggregation-1.0/bw_aggregation/main.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1625 2024-05-09 16:51:23.000000 bw_aggregation-1.0/bw_aggregation/override.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 15:30:47.142527 bw_aggregation-1.0/bw_aggregation.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     9147 2024-05-12 15:30:47.000000 bw_aggregation-1.0/bw_aggregation.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      434 2024-05-12 15:30:47.000000 bw_aggregation-1.0/bw_aggregation.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-12 15:30:47.000000 bw_aggregation-1.0/bw_aggregation.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      236 2024-05-12 15:30:47.000000 bw_aggregation-1.0/bw_aggregation.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       15 2024-05-12 15:30:47.000000 bw_aggregation-1.0/bw_aggregation.egg-info/top_level.txt
--rw-r--r--   0 cmutel     (501) staff       (20)     2603 2024-05-12 10:13:46.000000 bw_aggregation-1.0/pyproject.toml
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2024-05-12 15:30:47.143828 bw_aggregation-1.0/setup.cfg
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-12 15:30:47.142159 bw_aggregation-1.0/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)      298 2024-05-12 09:39:24.000000 bw_aggregation-1.0/tests/test_estimation.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7741 2024-05-12 10:06:47.000000 bw_aggregation-1.0/tests/test_main.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1983 2024-05-09 16:58:44.000000 bw_aggregation-1.0/tests/test_override.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-11 20:25:26.256236 bw_aggregation-1.0rc1/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1070 2024-05-09 15:12:25.000000 bw_aggregation-1.0rc1/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2024-05-09 15:12:25.000000 bw_aggregation-1.0rc1/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     8403 2024-05-11 20:25:26.256014 bw_aggregation-1.0rc1/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     6712 2024-05-11 11:08:34.000000 bw_aggregation-1.0rc1/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-11 20:25:26.253610 bw_aggregation-1.0rc1/bw_aggregation/
+-rw-r--r--   0 cmutel     (501) staff       (20)      582 2024-05-11 20:25:19.000000 bw_aggregation-1.0rc1/bw_aggregation/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4597 2024-05-11 11:29:50.000000 bw_aggregation-1.0rc1/bw_aggregation/calculator.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1827 2024-05-11 12:21:39.000000 bw_aggregation-1.0rc1/bw_aggregation/estimator.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     7930 2024-05-11 12:19:09.000000 bw_aggregation-1.0rc1/bw_aggregation/main.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1625 2024-05-09 16:51:23.000000 bw_aggregation-1.0rc1/bw_aggregation/override.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-11 20:25:26.255386 bw_aggregation-1.0rc1/bw_aggregation.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     8403 2024-05-11 20:25:26.000000 bw_aggregation-1.0rc1/bw_aggregation.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      434 2024-05-11 20:25:26.000000 bw_aggregation-1.0rc1/bw_aggregation.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-11 20:25:26.000000 bw_aggregation-1.0rc1/bw_aggregation.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      214 2024-05-11 20:25:26.000000 bw_aggregation-1.0rc1/bw_aggregation.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       15 2024-05-11 20:25:26.000000 bw_aggregation-1.0rc1/bw_aggregation.egg-info/top_level.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)     2581 2024-05-11 09:44:51.000000 bw_aggregation-1.0rc1/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)       38 2024-05-11 20:25:26.256291 bw_aggregation-1.0rc1/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-11 20:25:26.255094 bw_aggregation-1.0rc1/tests/
+-rw-r--r--   0 cmutel     (501) staff       (20)      238 2024-05-11 12:23:14.000000 bw_aggregation-1.0rc1/tests/test_estimation.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     7628 2024-05-11 11:30:42.000000 bw_aggregation-1.0rc1/tests/test_main.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1983 2024-05-09 16:58:44.000000 bw_aggregation-1.0rc1/tests/test_override.py
```

### Comparing `bw_aggregation-1.0/LICENSE` & `bw_aggregation-1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_aggregation-1.0/PKG-INFO` & `bw_aggregation-1.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_aggregation
-Version: 1.0
+Version: 1.0rc1
 Summary: Use aggregated processes for quicker calculations
 Author-email: bw_aggregation <cmutel@gmail.com>
 Maintainer-email: bw_aggregation <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/bw_aggregation
 Project-URL: homepage, https://github.com/brightway-lca/bw_aggregation
 Project-URL: tracker, https://github.com/brightway-lca/bw_aggregation/issues
 Classifier: Development Status :: 4 - Beta
@@ -17,20 +17,20 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bw2calc>1.99
-Requires-Dist: bw2data>=4.0.dev36
-Requires-Dist: bw_graph_tools>=0.3.1
-Requires-Dist: bw_processing>=0.9.3
+Requires-Dist: bw2data>3.99
+Requires-Dist: bw_graph_tools
+Requires-Dist: bw_processing
 Requires-Dist: fs
 Requires-Dist: matrix_utils
-Requires-Dist: numpy<2
+Requires-Dist: numpy
 Provides-Extra: testing
 Requires-Dist: bw_aggregation; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: python-coveralls; extra == "testing"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
@@ -93,37 +93,25 @@
 ```python
 import bw_aggregated as bwa
 bwa.AggregatedDatabase.estimate_speedup("<database label>")
 ```
 
 That will return something like:
 
-```python
-Speedup(
-    database_name='ecoinvent-3.10-cutoff', 
-    time_with_aggregation=4.297600030899048, 
-    time_without_aggregation=2.22904896736145, 
-    time_difference_absolute=2.0685510635375977, 
-    time_difference_relative=1.9279971386120622
-)
-```
-
-The times reported include `LCA` object creation, data loading, matrix construcion, and inventory calculations.
-
-As you can see, creating aggregated activities to avoid solving linear systems will not always lead to faster calculations, as the linear algebra libraries we use are pretty fast, and loading lots of data into the biosphere can take a lot of time. Please check on potential speedups before deciding to aggregate background databases.
+TBD
 
 If you want to convert that database, you can with:
 
 ```python
 bwa.AggregatedDatabase.convert_existing("<database label>")
 ```
 
 From now on, calling `bw2data.Database("<database label>")` will return an instance of `AggregatedDatabase`. You can do everything you normally would with this database, including making changes.
 
-> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` class instances.
+> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` object references.
 
 The conversion command will also set the default to use the aggregated values during calculations. You can change the default back to using unit process data with:
 
 ```python
 import bw2data as bd
 bd.Database("<database label>").use_aggregated(False)
 ```
@@ -173,17 +161,17 @@
 ## Implementation
 
 This library gets the possibility of using both aggregated and unit process data by overriding the `.datapackage` method, and loading one or two different datapackages depending on the current context. This approach is compatiable with both manual loading of datapackages, and with the `bw2data` function `prepare_lca_inputs`. The `.datapackage` method of an `AggregatedDatabase` is roughly:
 
 ```
 if global_context is True:
     load_aggregated()
-elif local_context(this_database) is True:
+elif local_context(me) is True:
     load_aggregated()
-elif this_database.prefer_aggregated is True:
+elif me.perfer_aggregated is True:
     load_aggregated()
 else:
     load_unit_process()
 ```
 
 ## Contributing
```

### Comparing `bw_aggregation-1.0/README.md` & `bw_aggregation-1.0rc1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -50,37 +50,25 @@
 ```python
 import bw_aggregated as bwa
 bwa.AggregatedDatabase.estimate_speedup("<database label>")
 ```
 
 That will return something like:
 
-```python
-Speedup(
-    database_name='ecoinvent-3.10-cutoff', 
-    time_with_aggregation=4.297600030899048, 
-    time_without_aggregation=2.22904896736145, 
-    time_difference_absolute=2.0685510635375977, 
-    time_difference_relative=1.9279971386120622
-)
-```
-
-The times reported include `LCA` object creation, data loading, matrix construcion, and inventory calculations.
-
-As you can see, creating aggregated activities to avoid solving linear systems will not always lead to faster calculations, as the linear algebra libraries we use are pretty fast, and loading lots of data into the biosphere can take a lot of time. Please check on potential speedups before deciding to aggregate background databases.
+TBD
 
 If you want to convert that database, you can with:
 
 ```python
 bwa.AggregatedDatabase.convert_existing("<database label>")
 ```
 
 From now on, calling `bw2data.Database("<database label>")` will return an instance of `AggregatedDatabase`. You can do everything you normally would with this database, including making changes.
 
-> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` class instances.
+> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` object references.
 
 The conversion command will also set the default to use the aggregated values during calculations. You can change the default back to using unit process data with:
 
 ```python
 import bw2data as bd
 bd.Database("<database label>").use_aggregated(False)
 ```
@@ -130,17 +118,17 @@
 ## Implementation
 
 This library gets the possibility of using both aggregated and unit process data by overriding the `.datapackage` method, and loading one or two different datapackages depending on the current context. This approach is compatiable with both manual loading of datapackages, and with the `bw2data` function `prepare_lca_inputs`. The `.datapackage` method of an `AggregatedDatabase` is roughly:
 
 ```
 if global_context is True:
     load_aggregated()
-elif local_context(this_database) is True:
+elif local_context(me) is True:
     load_aggregated()
-elif this_database.prefer_aggregated is True:
+elif me.perfer_aggregated is True:
     load_aggregated()
 else:
     load_unit_process()
 ```
 
 ## Contributing
```

### Comparing `bw_aggregation-1.0/bw_aggregation/__init__.py` & `bw_aggregation-1.0rc1/bw_aggregation/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     "__version__",
     "AggregatedDatabase",
     "AggregationContext",
     "ObsoleteAggregatedDatapackage",
     "Speedup",
 )
 
-__version__ = "1.0"
+__version__ = "1.0.RC1"
 
 
 from bw2data.backends import Activity
 from bw2data.subclass_mapping import (
     DATABASE_BACKEND_MAPPING,
     NODE_PROCESS_CLASS_MAPPING,
 )
 
-from .estimator import Speedup
 from .main import AggregatedDatabase, ObsoleteAggregatedDatapackage
 from .override import AggregationContext
+from .estimator import Speedup
 
 DATABASE_BACKEND_MAPPING["aggregated"] = AggregatedDatabase
 NODE_PROCESS_CLASS_MAPPING["aggregated"] = Activity
```

### Comparing `bw_aggregation-1.0/bw_aggregation/calculator.py` & `bw_aggregation-1.0rc1/bw_aggregation/calculator.py`

 * *Files identical despite different names*

### Comparing `bw_aggregation-1.0/bw_aggregation/estimator.py` & `bw_aggregation-1.0rc1/bw_aggregation/estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from dataclasses import dataclass
 from time import time
 
 from bw2calc import LCA
-from bw2data import Database, prepare_lca_inputs
+from bw2data import prepare_lca_inputs, Database
 
+from .calculator import AggregationCalculator
 from .override import AggregationContext
 
 
 @dataclass
 class Speedup:
     database_name: str
     time_with_aggregation: float
@@ -22,16 +23,15 @@
         self.db = Database(database_name)
 
     def difference(self) -> Speedup:
         without = self.calculate_without_speedup()
         with_ = self.calculate_with_speedup()
         return Speedup(
             database_name=self.name,
-            # Timer on Windows is coarse, could be zero for small databases
-            time_difference_relative=(with_ / without if without > 0 else 0),
+            time_difference_relative=with_ / without,
             time_difference_absolute=with_ - without,
             time_with_aggregation=with_,
             time_without_aggregation=without,
         )
 
     def calculate_with_speedup(self):
         from .main import AggregatedDatabase
```

### Comparing `bw_aggregation-1.0/bw_aggregation/main.py` & `bw_aggregation-1.0rc1/bw_aggregation/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     create_datapackage,
     load_datapackage,
     safe_filename,
 )
 from fs.zipfs import ZipFS
 
 from .calculator import AggregationCalculator
-from .estimator import CalculationDifferenceEstimator
 from .override import AggregationContext, aggregation_override
+from .estimator import CalculationDifferenceEstimator
 
 
 class ObsoleteAggregatedDatapackage(Exception):
     """The results from this aggregated datapackage are obsolete"""
 
     pass
 
@@ -196,8 +196,8 @@
         dp.add_persistent_vector_from_iterator(
             matrix="technosphere_matrix",
             name=clean_datapackage_name(self.name + " technosphere matrix"),
             dict_iterator=calculator.technosphere_iterator,
         )
         if not in_memory:
             dp.finalize_serialization()
-        return dp
+        return dp
```

### Comparing `bw_aggregation-1.0/bw_aggregation/override.py` & `bw_aggregation-1.0rc1/bw_aggregation/override.py`

 * *Files identical despite different names*

### Comparing `bw_aggregation-1.0/bw_aggregation.egg-info/PKG-INFO` & `bw_aggregation-1.0rc1/bw_aggregation.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_aggregation
-Version: 1.0
+Version: 1.0rc1
 Summary: Use aggregated processes for quicker calculations
 Author-email: bw_aggregation <cmutel@gmail.com>
 Maintainer-email: bw_aggregation <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/bw_aggregation
 Project-URL: homepage, https://github.com/brightway-lca/bw_aggregation
 Project-URL: tracker, https://github.com/brightway-lca/bw_aggregation/issues
 Classifier: Development Status :: 4 - Beta
@@ -17,20 +17,20 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bw2calc>1.99
-Requires-Dist: bw2data>=4.0.dev36
-Requires-Dist: bw_graph_tools>=0.3.1
-Requires-Dist: bw_processing>=0.9.3
+Requires-Dist: bw2data>3.99
+Requires-Dist: bw_graph_tools
+Requires-Dist: bw_processing
 Requires-Dist: fs
 Requires-Dist: matrix_utils
-Requires-Dist: numpy<2
+Requires-Dist: numpy
 Provides-Extra: testing
 Requires-Dist: bw_aggregation; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: python-coveralls; extra == "testing"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
@@ -93,37 +93,25 @@
 ```python
 import bw_aggregated as bwa
 bwa.AggregatedDatabase.estimate_speedup("<database label>")
 ```
 
 That will return something like:
 
-```python
-Speedup(
-    database_name='ecoinvent-3.10-cutoff', 
-    time_with_aggregation=4.297600030899048, 
-    time_without_aggregation=2.22904896736145, 
-    time_difference_absolute=2.0685510635375977, 
-    time_difference_relative=1.9279971386120622
-)
-```
-
-The times reported include `LCA` object creation, data loading, matrix construcion, and inventory calculations.
-
-As you can see, creating aggregated activities to avoid solving linear systems will not always lead to faster calculations, as the linear algebra libraries we use are pretty fast, and loading lots of data into the biosphere can take a lot of time. Please check on potential speedups before deciding to aggregate background databases.
+TBD
 
 If you want to convert that database, you can with:
 
 ```python
 bwa.AggregatedDatabase.convert_existing("<database label>")
 ```
 
 From now on, calling `bw2data.Database("<database label>")` will return an instance of `AggregatedDatabase`. You can do everything you normally would with this database, including making changes.
 
-> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` class instances.
+> :warning: Any **existing `Database("<database label>")` reference is out of date**: You need to create new `Database` object references.
 
 The conversion command will also set the default to use the aggregated values during calculations. You can change the default back to using unit process data with:
 
 ```python
 import bw2data as bd
 bd.Database("<database label>").use_aggregated(False)
 ```
@@ -173,17 +161,17 @@
 ## Implementation
 
 This library gets the possibility of using both aggregated and unit process data by overriding the `.datapackage` method, and loading one or two different datapackages depending on the current context. This approach is compatiable with both manual loading of datapackages, and with the `bw2data` function `prepare_lca_inputs`. The `.datapackage` method of an `AggregatedDatabase` is roughly:
 
 ```
 if global_context is True:
     load_aggregated()
-elif local_context(this_database) is True:
+elif local_context(me) is True:
     load_aggregated()
-elif this_database.prefer_aggregated is True:
+elif me.perfer_aggregated is True:
     load_aggregated()
 else:
     load_unit_process()
 ```
 
 ## Contributing
```

### Comparing `bw_aggregation-1.0/pyproject.toml` & `bw_aggregation-1.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     "Topic :: Scientific/Engineering"
 ]
 requires-python = ">=3.9"
 dependencies = [
     # dependencies as strings with quotes, e.g. "foo"
     # You can add version requirements like "foo>2.0"
     "bw2calc>1.99",
-    "bw2data>=4.0.dev36",
-    "bw_graph_tools>=0.3.1",
-    "bw_processing>=0.9.3",
+    "bw2data>3.99",
+    "bw_graph_tools",
+    "bw_processing",
     "fs",
     "matrix_utils",
-    "numpy<2",
+    "numpy",
 ]
 
 [project.urls]
 source = "https://github.com/brightway-lca/bw_aggregation"
 homepage = "https://github.com/brightway-lca/bw_aggregation"
 tracker = "https://github.com/brightway-lca/bw_aggregation/issues"
```

### Comparing `bw_aggregation-1.0/tests/test_main.py` & `bw_aggregation-1.0rc1/tests/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import sys
-
 import numpy as np
 import pytest
 from bw2calc import LCA
 from bw2data import Database, databases, get_node
 from bw2data.backends import SQLiteBackend
 
 from bw_aggregation import AggregatedDatabase, ObsoleteAggregatedDatapackage
@@ -51,17 +49,14 @@
     assert lca.technosphere_matrix[:, lca.dicts.activity[node.id]].sum() == 1
 
     rows, _ = lca.biosphere_matrix[:, lca.dicts.activity[node.id]].nonzero()
     assert rows.shape == (2,)
     assert lca.biosphere_matrix[:, lca.dicts.activity[node.id]].sum() != 7
 
 
-@pytest.mark.skipif(
-    sys.platform.startswith("win"), reason="Error on cleanup deleting tmpdir"
-)
 def test_convert_existing(background):
     AggregatedDatabase.convert_existing("a")
     assert databases["a"]["backend"] == "aggregated"
     assert databases["a"]["aggregation_calculation_time"]
     assert databases["a"]["aggregation_calculation_timestamp"]
     assert databases["a"]["aggregation_use_in_calculation"]
```

### Comparing `bw_aggregation-1.0/tests/test_override.py` & `bw_aggregation-1.0rc1/tests/test_override.py`

 * *Files identical despite different names*

