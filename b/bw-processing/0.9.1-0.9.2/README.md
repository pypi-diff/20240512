# Comparing `tmp/bw_processing-0.9.1.tar.gz` & `tmp/bw_processing-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_processing-0.9.1.tar", last modified: Fri May 10 20:45:23 2024, max compression
+gzip compressed data, was "bw_processing-0.9.2.tar", last modified: Sat May 11 22:57:16 2024, max compression
```

## Comparing `bw_processing-0.9.1.tar` & `bw_processing-0.9.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.027037 bw_processing-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-10 20:45:19.000000 bw_processing-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-10 20:45:19.000000 bw_processing-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-05-10 20:45:23.027037 bw_processing-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-05-10 20:45:19.000000 bw_processing-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.023037 bw_processing-0.9.1/bw_processing/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/array_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    44619 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/datapackage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.027037 bw_processing-0.9.1/bw_processing/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/examples/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/examples/parquet_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/examples/simple.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/io_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/io_parquet_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/io_pyarrow_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/merging.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/unique_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-10 20:45:19.000000 bw_processing-0.9.1/bw_processing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.027037 bw_processing-0.9.1/bw_processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-05-10 20:45:23.000000 bw_processing-0.9.1/bw_processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-10 20:45:23.000000 bw_processing-0.9.1/bw_processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:45:23.000000 bw_processing-0.9.1/bw_processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:45:22.000000 bw_processing-0.9.1/bw_processing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-10 20:45:23.000000 bw_processing-0.9.1/bw_processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 20:45:23.000000 bw_processing-0.9.1/bw_processing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.023037 bw_processing-0.9.1/dev/
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-10 20:45:19.000000 bw_processing-0.9.1/dev/calculation_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-10 20:45:19.000000 bw_processing-0.9.1/dev/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-10 20:45:19.000000 bw_processing-0.9.1/dev/processed_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-10 20:45:19.000000 bw_processing-0.9.1/dev/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-10 20:45:19.000000 bw_processing-0.9.1/dev/speed_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.023037 bw_processing-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-10 20:45:19.000000 bw_processing-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 20:45:19.000000 bw_processing-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-10 20:45:23.027037 bw_processing-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.027037 bw_processing-0.9.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.023037 bw_processing-0.9.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 20:45:19.000000 bw_processing-0.9.1/tests/fixtures/basic_arrays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:45:23.023037 bw_processing-0.9.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-10 20:45:19.000000 bw_processing-0.9.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-10 20:45:19.000000 bw_processing-0.9.1/tests/helpers/basic_array_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-10 20:45:19.000000 bw_processing-0.9.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:57:16.369112 bw_processing-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-11 22:57:12.000000 bw_processing-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-11 22:57:12.000000 bw_processing-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-05-11 22:57:16.369112 bw_processing-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2024-05-11 22:57:12.000000 bw_processing-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:57:16.365112 bw_processing-0.9.2/bw_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/array_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44620 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/datapackage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:57:16.369112 bw_processing-0.9.2/bw_processing/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/examples/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/examples/parquet_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/examples/simple.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/io_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/io_parquet_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/io_pyarrow_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/merging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/unique_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-11 22:57:12.000000 bw_processing-0.9.2/bw_processing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:57:16.369112 bw_processing-0.9.2/bw_processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16378 2024-05-11 22:57:16.000000 bw_processing-0.9.2/bw_processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-11 22:57:16.000000 bw_processing-0.9.2/bw_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:57:16.000000 bw_processing-0.9.2/bw_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:57:16.000000 bw_processing-0.9.2/bw_processing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-11 22:57:16.000000 bw_processing-0.9.2/bw_processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-11 22:57:16.000000 bw_processing-0.9.2/bw_processing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:57:16.365112 bw_processing-0.9.2/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-05-11 22:57:12.000000 bw_processing-0.9.2/dev/calculation_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-11 22:57:12.000000 bw_processing-0.9.2/dev/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-05-11 22:57:12.000000 bw_processing-0.9.2/dev/processed_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-11 22:57:12.000000 bw_processing-0.9.2/dev/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-11 22:57:12.000000 bw_processing-0.9.2/dev/speed_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:57:16.365112 bw_processing-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-11 22:57:12.000000 bw_processing-0.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 22:57:12.000000 bw_processing-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-11 22:57:16.373112 bw_processing-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:57:16.369112 bw_processing-0.9.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:57:16.369112 bw_processing-0.9.2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-11 22:57:12.000000 bw_processing-0.9.2/tests/fixtures/basic_arrays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:57:16.369112 bw_processing-0.9.2/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-11 22:57:12.000000 bw_processing-0.9.2/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-11 22:57:12.000000 bw_processing-0.9.2/tests/helpers/basic_array_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6824 2024-05-11 22:57:12.000000 bw_processing-0.9.2/tests/test_utils.py
```

### Comparing `bw_processing-0.9.1/LICENSE` & `bw_processing-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/PKG-INFO` & `bw_processing-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-processing
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tools to create structured arrays in a common format
 Home-page: https://github.com/brightway-lca/bw_processing
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_processing-0.9.1/README.md` & `bw_processing-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/__init__.py` & `bw_processing-0.9.2/bw_processing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "reset_index",
     "safe_filename",
     "simple_graph",
     "UNCERTAINTY_DTYPE",
     "UndefinedInterface",
 )
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 
 from .array_creation import create_array, create_structured_array
 from .constants import (
     DEFAULT_LICENSES,
     INDICES_DTYPE,
     UNCERTAINTY_DTYPE,
```

### Comparing `bw_processing-0.9.1/bw_processing/array_creation.py` & `bw_processing-0.9.2/bw_processing/array_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,16 @@
 
 
 def create_structured_array(iterable, dtype, nrows=None, sort=False, sort_fields=None):
     """Create a numpy `structured array <https://docs.scipy.org/doc/numpy/user/basics.rec.html>`__ for data ``iterable``. Returns a filepath of a created file (if ``filepath`` is provided, or the array.
 
     ``iterable`` can be data already in memory, or a generator.
 
-    ``nrows`` can be supplied, if known. If ``iterable`` has a length, it will be determined automatically. If ``nrows`` is not known, this function generates chunked arrays until ``iterable`` is exhausted, and concatenates them."""
+    ``nrows`` can be supplied, if known. If ``iterable`` has a length, it will be determined automatically. If ``nrows`` is not known, this function generates chunked arrays until ``iterable`` is exhausted, and concatenates them.
+    """
     if nrows or hasattr(iterable, "__len__"):
         if not nrows:
             nrows = len(iterable)
         array = np.zeros(nrows, dtype=dtype)
         for i, row in enumerate(iterable):
             if i > (nrows - 1):
                 raise ValueError("More rows than `nrows`")
```

### Comparing `bw_processing-0.9.1/bw_processing/constants.py` & `bw_processing-0.9.2/bw_processing/constants.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/datapackage.py` & `bw_processing-0.9.2/bw_processing/datapackage.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     PotentialInconsistency,
     ShapeMismatch,
     WrongDatatype,
 )
 from .filesystem import clean_datapackage_name
 from .io_helpers import file_reader, file_writer
 from .proxies import Proxy, UndefinedInterface
-from .utils import check_name, check_suffix, load_bytes, resolve_dict_iterator
+from .utils import check_name, check_suffix, load_bytes, resolve_dict_iterator, utc_now
 
 
 class DatapackageBase(ABC):
     """Base class for datapackages. Not for normal use - you should use either `Datapackage` or `FilteredDatapackage`."""
 
     def __init__(self):
         # This is the global serialization format used for numpy.ndarray for the whole object.
@@ -123,15 +123,16 @@
 
         del self.resources[index]
         del self.data[index]
 
     def del_resource_group(self, name: str) -> None:
         """Remove a resource group, and delete its data files, if any.
 
-        Use ``exclude_resource_group`` if you want to keep the underlying resource in the filesystem."""
+        Use ``exclude_resource_group`` if you want to keep the underlying resource in the filesystem.
+        """
         if self._modified:
             raise PotentialInconsistency(
                 "Datapackage is modified; save modifications or reload"
             )
 
         indices = [
             i
@@ -177,15 +178,16 @@
         return self.data[index], self.resources[index]
 
     def filter_by_attribute(self, key: str, value: Any) -> "FilteredDatapackage":
         """Create a new ``FilteredDatapackage`` which satisfies the filter ``resource[key] == value``.
 
         All included objects are the same as in the original data package, i.e. no copies are made. No checks are made to ensure consistency with modifications to the original datapackage after the creation of this filtered datapackage.
 
-        This method was introduced to allow for the efficient construction of matrices; each datapackage can have data for multiple matrices, and we can then create filtered datapackages which exclusively have data for the matrix of interest. As such, they should be considered read-only, though this is not enforced."""
+        This method was introduced to allow for the efficient construction of matrices; each datapackage can have data for multiple matrices, and we can then create filtered datapackages which exclusively have data for the matrix of interest. As such, they should be considered read-only, though this is not enforced.
+        """
         fdp = FilteredDatapackage()
         fdp.fs = self.fs
         fdp.metadata = {k: v for k, v in self.metadata.items() if k != "resources"}
         fdp.metadata["resources"] = []
         to_include = [
             i for i, resource in enumerate(self.resources) if resource.get(key) == value
         ]
@@ -365,15 +367,15 @@
 
         self.metadata = {
             "profile": "data-package",
             "name": name,
             "id": id_ or uuid.uuid4().hex,
             "licenses": (metadata or {}).get("licenses", DEFAULT_LICENSES),
             "resources": [],
-            "created": datetime.datetime.now(datetime.UTC).isoformat("T") + "Z",
+            "created": utc_now().isoformat("T") + "Z",
             "combinatorial": combinatorial,
             "sequential": sequential,
             "seed": seed,
             "sum_intra_duplicates": sum_intra_duplicates,
             "sum_inter_duplicates": sum_inter_duplicates,
             "matrix_serialize_format_type": matrix_serialize_format_type.value,
         }
@@ -1111,24 +1113,24 @@
         obj = fs_or_obj
     else:
         obj = Datapackage()
         obj._load(fs=fs_or_obj, mmap_mode=mmap_mode, proxy=proxy)
     return obj
 
 
-def simple_graph(data: dict, fs: Optional[FS] = None, **metadata)->Datapackage:
+def simple_graph(data: dict, fs: Optional[FS] = None, **metadata) -> Datapackage:
     """Easy creation of simple datapackages with only persistent vectors.
 
     Args:
         * data: is a dictionary.
             The data dictionary has the form::
 
                 {
-                    matrix_name: [ 
-                    (row_id, col_id, value, flip) 
+                    matrix_name: [
+                    (row_id, col_id, value, flip)
                     ]
                 }
 
 
             Where `row_id` and `col_id are an `int` s, value is a `float` and flip is a `bool`  (False by default).
 
         * fs: is a filesystem.
```

### Comparing `bw_processing-0.9.1/bw_processing/errors.py` & `bw_processing-0.9.2/bw_processing/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
     pass
 
 
 class InvalidName(BrightwayProcessingError):
     """Name fails datapackage requirements:
 
-    A short url-usable (and preferably human-readable) name of the package. This MUST be lower-case and contain only alphanumeric characters along with ".", "_" or "-" characters."""
+    A short url-usable (and preferably human-readable) name of the package. This MUST be lower-case and contain only alphanumeric characters along with ".", "_" or "-" characters.
+    """
 
     pass
 
 
 class FileIntegrityError(BrightwayProcessingError):
     """MD5 hash does not agree with file contents"""
```

### Comparing `bw_processing-0.9.1/bw_processing/examples/interfaces.py` & `bw_processing-0.9.2/bw_processing/examples/interfaces.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/examples/parquet_files.py` & `bw_processing-0.9.2/bw_processing/examples/parquet_files.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/examples/simple.zip` & `bw_processing-0.9.2/bw_processing/examples/simple.zip`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/filesystem.py` & `bw_processing-0.9.2/bw_processing/filesystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 def safe_filename(
     string: Union[str, bytes], add_hash: bool = True, full: bool = False
 ) -> str:
     """Convert arbitrary strings to make them safe for filenames. Substitutes strange characters, and uses unicode normalization.
 
     if `add_hash`, appends hash of `string` to avoid name collisions.
 
-    From http://stackoverflow.com/questions/295135/turn-a-string-into-a-valid-filename-in-python"""
+    From http://stackoverflow.com/questions/295135/turn-a-string-into-a-valid-filename-in-python
+    """
     safe = re.sub(
         r"[-\s]+",
         "-",
         str(re_slugify.sub("", unicodedata.normalize("NFKD", str(string))).strip()),
     )
     if add_hash:
         if isinstance(string, str):
```

### Comparing `bw_processing-0.9.1/bw_processing/indexing.py` & `bw_processing-0.9.2/bw_processing/indexing.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/io_helpers.py` & `bw_processing-0.9.2/bw_processing/io_helpers.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/io_parquet_helpers.py` & `bw_processing-0.9.2/bw_processing/io_parquet_helpers.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/io_pyarrow_helpers.py` & `bw_processing-0.9.2/bw_processing/io_pyarrow_helpers.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/merging.py` & `bw_processing-0.9.2/bw_processing/merging.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/unique_fields.py` & `bw_processing-0.9.2/bw_processing/unique_fields.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/bw_processing/utils.py` & `bw_processing-0.9.2/bw_processing/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from datetime import datetime
 from io import BytesIO
 from pathlib import Path
 from typing import Any, Union
 
 import numpy as np
 from numpy.lib.recfunctions import repack_fields
 
@@ -94,7 +95,15 @@
                     "maximum",
                     "negative",
                 ]
             ]
         ),
         array["flip"],
     )
+
+
+def utc_now() -> datetime:
+    """Get current datetime compatible with Py 3.8 to 3.12"""
+    if hasattr(datetime, "UTC"):
+        return datetime.now(datetime.UTC)
+    else:
+        return datetime.utcnow()
```

### Comparing `bw_processing-0.9.1/bw_processing.egg-info/PKG-INFO` & `bw_processing-0.9.2/bw_processing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw-processing
-Version: 0.9.1
+Version: 0.9.2
 Summary: Tools to create structured arrays in a common format
 Home-page: https://github.com/brightway-lca/bw_processing
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_processing-0.9.1/bw_processing.egg-info/SOURCES.txt` & `bw_processing-0.9.2/bw_processing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/dev/calculation_package.py` & `bw_processing-0.9.2/dev/calculation_package.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/dev/loading.py` & `bw_processing-0.9.2/dev/loading.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/dev/processed_package.py` & `bw_processing-0.9.2/dev/processed_package.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/dev/resources.py` & `bw_processing-0.9.2/dev/resources.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/dev/speed_tests.py` & `bw_processing-0.9.2/dev/speed_tests.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/docs/conf.py` & `bw_processing-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/setup.cfg` & `bw_processing-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/tests/fixtures/basic_arrays.py` & `bw_processing-0.9.2/tests/fixtures/basic_arrays.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/tests/helpers/basic_array_helpers.py` & `bw_processing-0.9.2/tests/helpers/basic_array_helpers.py`

 * *Files identical despite different names*

### Comparing `bw_processing-0.9.1/tests/test_utils.py` & `bw_processing-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

