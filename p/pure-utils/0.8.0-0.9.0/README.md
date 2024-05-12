# Comparing `tmp/pure_utils-0.8.0.tar.gz` & `tmp/pure_utils-0.9.0.tar.gz`

## Comparing `pure_utils-0.8.0.tar` & `pure_utils-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 pure_utils-0.8.0/Makefile
--rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/Makefile
--rwxr-xr-x   0        0        0     1412 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/conf.py
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/source/changelog.rst
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/source/commands.rst
--rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/source/index.rst
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/source/license.rst
--rwxr-xr-x   0        0        0      158 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/source/refs/index.rst
--rwxr-xr-x   0        0        0     8643 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/templates/page.html
--rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.docs/templates/autosummary/module.rst
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/common.py
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/containers.py
--rw-r--r--   0        0        0     7296 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/debug.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/profiler.py
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/repeaters.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/strings.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/system.py
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/times.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/_internal/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/_internal/_profile_stats.py
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pure_utils/_internal/_profile_stats_serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_common.py
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_containers.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_debug.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_profiler.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_repeaters.py
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_strings.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_system.py
--rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 pure_utils-0.8.0/tests/test_times.py
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pure_utils-0.8.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pure_utils-0.8.0/LICENSE
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 pure_utils-0.8.0/README.md
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pure_utils-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8803 2020-02-02 00:00:00.000000 pure_utils-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 pure_utils-0.9.0/Makefile
+-rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.docs/Makefile
+-rwxr-xr-x   0        0        0     1363 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.docs/conf.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.docs/source/changelog.rst
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.docs/source/commands.rst
+-rwxr-xr-x   0        0        0      742 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.docs/source/index.rst
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.docs/source/license.rst
+-rwxr-xr-x   0        0        0      269 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.docs/source/refs/index.rst
+-rwxr-xr-x   0        0        0     8643 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.docs/templates/page.html
+-rwxr-xr-x   0        0        0      762 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.docs/templates/autosummary/module.rst
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/__init__.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/common.py
+-rw-r--r--   0        0        0     7932 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/containers.py
+-rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/debug.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/profiler.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/repeaters.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/strings.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/system.py
+-rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/times.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/types.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/_internal/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/_internal/_profile_stats.py
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pure_utils/_internal/_profile_stats_serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pure_utils-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 pure_utils-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pure_utils-0.9.0/tests/test_common.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 pure_utils-0.9.0/tests/test_containers.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 pure_utils-0.9.0/tests/test_debug.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 pure_utils-0.9.0/tests/test_profiler.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 pure_utils-0.9.0/tests/test_repeaters.py
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 pure_utils-0.9.0/tests/test_strings.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pure_utils-0.9.0/tests/test_system.py
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 pure_utils-0.9.0/tests/test_times.py
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 pure_utils-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pure_utils-0.9.0/LICENSE
+-rw-r--r--   0        0        0     6951 2020-02-02 00:00:00.000000 pure_utils-0.9.0/README.md
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pure_utils-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 pure_utils-0.9.0/PKG-INFO
```

### Comparing `pure_utils-0.8.0/Makefile` & `pure_utils-0.9.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 	python -m pytest --cov pure_utils --cov-report html
 
 tests-cov-json:
 	python -m pytest --cov pure_utils --cov-report json
 
 cleanup:
 	rm -rf .pytest_cache/ .mypy_cache/ junit/ build/ dist/ coverage_report/
-	find . -not -path './.venv*' -path '*/__pycache__*' -delete
-	find . -not -path './.venv*' -path '*/*.egg-info*' -delete
+	find . -not -path 'venv*' -path '*/__pycache__*' -delete
+	find . -not -path 'venv*' -path '*/*.egg-info*' -delete
 
 help:
 	echo
 	echo "Usage:"
 	echo "--------------------------------------------------------------------------------"
 	echo "help\t\tShow this message."
 	echo
@@ -81,9 +81,9 @@
 	echo
 	echo "tests\t\tRun tests with coverage measure (output to terminal)."
 	echo "tests-cov-json\tRun tests with coverage measure (output to json [coverage.json])."
 	echo "tests-cov-html\tRun tests with coverage measure (output to html [coverage_report/])."
 	echo
 	echo "cleanup\t\tClean up python temporary files and caches."
 	echo "format\t\tFromat the code (by black and isort)."
-	echo "lint\t\tCheck code style and types (by flake8, pydocstyle and mypy)."
+	echo "lint\t\tCheck code style, docstring style and types (by flake8, pydocstyle and mypy)."
 	echo
```

### Comparing `pure_utils-0.8.0/.docs/Makefile` & `pure_utils-0.9.0/.docs/Makefile`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/.docs/conf.py` & `pure_utils-0.9.0/.docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 import sys
 from pathlib import Path
 
-sys.path.insert(0, os.path.abspath("../pure_utils"))
-
-autodoc_mock_imports = ["pure_utils"]
+sys.path.insert(0, os.path.abspath("../"))
 
 DOCS_ROOT_DIR = Path(__file__).resolve(strict=True).parent
 
 project = html_title = "pure-utils"
 copyright = "Peter Bro <p3t3rbr0@gmail.com || peter@peterbro.su>"
 
 extensions = [
```

### Comparing `pure_utils-0.8.0/.docs/source/changelog.rst` & `pure_utils-0.9.0/.docs/source/changelog.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+v0.9.0 - [2024-05-12]
+---------------------
+* Add ``types`` module.
+* Fix "cleanup" make command.
+* Fix modules short descriptions.
+* Fix make commands short description.
+* Fix relative imports errors into docs.
+* Rewrite examples of usage into docstrings.
+* Replace AssertionError to ValueError with messages.
+
 v0.8.0 - [2024-05-06]
 ---------------------
 * Add new module - ``system`` (system purpose utilities).
 * Update development dependencies.
 * Use dynamic version into pyproject.toml.
 * Fix project short description.
```

### Comparing `pure_utils-0.8.0/.docs/source/commands.rst` & `pure_utils-0.9.0/.docs/source/commands.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 - ``make deps`` - Install all dependencies.
 
 Distributing
 ------------
 - ``make build-sdist`` - Build a source distrib.
 - ``make build-wheel`` - Build a pure python wheel distrib.
 - ``make build`` - Build both distribs (source and wheel).
-- ``make upload`` - Upload built packages to PyPI..
+- ``make upload`` - Upload built packages to PyPI.
 
 Development
 -----------
 - ``make cleanup`` - Clean up python temporary files and caches.
 - ``make format`` - Fromat the code (by black and isort).
-- ``make lint`` - Check code style and types (by flake8, pydocstyle and mypy).
+- ``make lint`` - Check code style, docstring style and types (by flake8, pydocstyle and mypy).
 - ``make tests`` - Run tests with coverage measure (output to terminal).
 - ``make tests-cov-json`` - Run tests with coverage measure (output to json [coverage.json]).
 - ``make tests-cov-html`` - Run tests with coverage measure (output to html [coverage_report/]).
```

### Comparing `pure_utils-0.8.0/.docs/source/index.rst` & `pure_utils-0.9.0/.docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/.docs/source/license.rst` & `pure_utils-0.9.0/.docs/source/license.rst`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/.docs/templates/page.html` & `pure_utils-0.9.0/.docs/templates/page.html`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/.docs/templates/autosummary/module.rst` & `pure_utils-0.9.0/.docs/templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/.github/workflows/ci.yaml` & `pure_utils-0.9.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/pure_utils/containers.py` & `pure_utils-0.9.0/pure_utils/containers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,112 +1,105 @@
-"""Utilities for working with data containers (lists, dictionaries, tuples, sets, etc.)."""
+"""Utilities for working with data containers (lists, dicts, tuples, sets, etc.)."""
 
-from typing import (
-    Any,
-    Generator,
-    KeysView,
-    Mapping,
-    Optional,
-    Sequence,
-    TypeAlias,
-    TypeVar,
-)
+from typing import Any, Generator, Mapping, Optional, Sequence
+
+from .types import KeysT, T
 
 __all__ = [
     "bisect",
     "first",
     "flatten",
     "get_or_else",
     "omit",
     "paginate",
     "pick",
     "symmdiff",
     "unpack",
 ]
 
-T = TypeVar("T")
-KeysT: TypeAlias = Sequence[T] | KeysView[T]
-
 
 def bisect(collection: list[T], /) -> tuple[list[T], list[T]]:
     """Bisect the list into two parts/halves based on the number of elements.
 
     The function does not change the original collection.
 
     Args:
         collection: Source collection.
 
     Returns:
         A two-element tuple containing two lists: the first list represents the first half of the
         original collection, and the second list is the second half.
 
     Raises:
-        AssertionError: If collection is empty.
+        ValueError: If collection is empty.
 
-    Example::
+    Usage:
 
-        from pure_utils.containers import bisect
+    >>> from pure_utils import bisect
 
-        l = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
+    >>> l = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
 
-        first_half, second_half = bisect(l)
-        print(first_half, second_half)
-        >>> [1, 2, 3, 4, 5] [6, 7, 8, 9, 10, 11]
+    >>> first_half, second_half = bisect(l)
+    >>> print(first_half, second_half)
+    [1, 2, 3, 4, 5] [6, 7, 8, 9, 10, 11]
     """
-    assert collection
     length = len(collection)
+
+    if not length:
+        raise ValueError("The source collection must not be empty")
+
     return (collection[: length // 2], collection[length // 2 :])
 
 
 def first(collection: Sequence[T], /) -> Optional[T]:
     """Get the value of the first element from a subscriptable collection.
 
     Args:
         collection: Subscriptable collection.
 
     Returns:
         The value of the first element of the collection, or None if there is none.
 
-    Example::
+    Usage:
 
-        from pure_utils.containers import first
+    >>> from pure_utils import first
 
-        seq = (1, 2, 3)
-        print(first(seq))
-        >>> 1
+    >>> seq = (1, 2, 3)
+    >>> print(first(seq))
+    1
 
-        seq = []
-        print(first(seq))
-        >>> None
+    >>> seq = []
+    >>> print(first(seq))
+    None
     """
     return next((_ for _ in collection), None)
 
 
 def flatten(collection: Sequence[T], /) -> Generator[Sequence[T] | T, None, None]:
     """Make the subscriptable collection a flat (single nesting level).
 
     Args:
         collection: Subscriptable collection to flatten.
 
     Returns:
         Generator of the flatten function.
 
-    Example::
+    Usage:
 
-        from pure_utils.containers import flatten
+    >>> from pure_utils import flatten
 
-        seq = [[1], [2], [3], [4], [5]]
-        result = list(flatten(seq))
-        print(result)
-        >>> [1, 2, 3, 4, 5]
-
-        seq = [[[[[[1]]]]], [[[[[2]]]]], [[[[[3]]]]], [[[[[4]]]]], [[[[[5]]]]]]
-        result = list(flatten(seq))
-        print(result)
-        >>> [1, 2, 3, 4, 5]
+    >>> seq = [[1], [2], [3], [4], [5]]
+    >>> result = list(flatten(seq))
+    >>> print(result)
+    [1, 2, 3, 4, 5]
+
+    >>> seq = [[[[[[1]]]]], [[[[[2]]]]], [[[[[3]]]]], [[[[[4]]]]], [[[[[5]]]]]]
+    >>> result = list(flatten(seq))
+    >>> print(result)
+    [1, 2, 3, 4, 5]
     """
     if isinstance(collection, (list, tuple, set)):
         for _ in collection:
             yield from flatten(_)
     else:
         yield collection
 
@@ -121,79 +114,77 @@
         index: Index of the collection element to get the value.
         default: Optional default value, returned when no element at the specified index.
 
     Returns:
         The value of the sequence element at the specified index,
         or default value, when no element by this index.
 
-    Example::
+    Usage:
 
-        from pure_utils.containers import get_or_else
+    >>> from pure_utils import get_or_else
 
-        seq = (1, 2, 3)
-        print(get_or_else(seq, 0))
-        >>> 1
-        print(get_or_else(seq, 3))
-        >>> None
-        print(get_or_else(seq, 3, -1))
-        >>> -1
-
-        seq = ["a", "b", "c"]
-        print(get_or_else(seq, 3, "does not exists"))
-        >>> does not exists
+    >>> seq = (1, 2, 3)
+    >>> print(get_or_else(seq, 0))
+    1
+    >>> print(get_or_else(seq, 3))
+    None
+    >>> print(get_or_else(seq, 3, -1))
+    -1
+    >>> print(get_or_else(seq, 3, "does not exists"))
+    does not exists
     """
     try:
         return collection[index]
     except IndexError:
         return default
 
 
-def symmdiff(s1: KeysT, s2: KeysT, /) -> Sequence[T]:
+def symmdiff(collection1: KeysT, collection2: KeysT, /) -> Sequence[T]:
     """Obtain the symmetric difference of two sequences.
 
     Args:
-        s1: The first sequence to form a set on the LEFT.
-        s2: The second sequence to form a set on the RIGHT.
+        collection1: The first sequence to form a set on the LEFT.
+        collection2: The second sequence to form a set on the RIGHT.
 
     Returns:
         The symmetric difference of two sequences as a list.
 
-    Example::
+    Usage:
 
-         from pure_utils.containers import symmdiff
+    >>> from pure_utils import symmdiff
 
-         s1 = ["a", "b", "c"]
-         s2 = ["e", "b", "a"]
-         result = symmdiff(s1, s2)
-         print(result)
-         >>> ["c", "e"]
+    >>> collection1 = ["a", "b", "c"]
+    >>> collection2 = ["e", "b", "a"]
+    >>> result = symmdiff(collection1, collection2)
+    >>> print(result)
+    ["c", "e"]
     """
-    return list(set(s1).symmetric_difference(set(s2)))
+    return list(set(collection1).symmetric_difference(set(collection2)))
 
 
 def omit(container: Mapping[str, Any], keys: KeysT, /) -> Mapping[str, Any]:
     """Omit key-value pairs from the source dictionary, by keys sequence.
 
     The function does not modify the original collection.
 
     Args:
         container: Source data container.
         keys: A sequence of strings or keys() for omitted pairs in the source data container.
 
     Returns:
         A data container without omitted key-value pairs.
 
-    Example::
+    Usage:
 
-        from pure_utils.containers import omit
+    >>> from pure_utils import omit
 
-        container = {"key1": "val1", "key2": "val2", "key3": "val3", "key4": "val4"}
-        result = omit(container, ["key2", "key4"] )
-        print(result)
-        >>> {"key1": "val1", "key3": "val3"}
+    >>> container = {"key1": "val1", "key2": "val2", "key3": "val3", "key4": "val4"}
+    >>> result = omit(container, ["key2", "key4"] )
+    >>> print(result)
+    {"key1": "val1", "key3": "val3"}
     """
     keys_diff: KeysT = symmdiff(container.keys(), keys)
     return {_: container[_] for _ in keys_diff if _ in container}
 
 
 def paginate(collection: Sequence[T], /, *, size: int) -> Sequence[Sequence[T]]:
     """Split the collection into page(s), limited by size.
@@ -204,26 +195,28 @@
         collection: Collection of homogeneous elements.
         size: Page size of elements in one page.
 
     Returns:
         A collection with elements splitted into pages (nested collections).
 
     Raises:
-        AssertionError: If size is less than zero.
+        ValueError: If page size is less than zero.
 
-    Example::
+    Usage:
 
-        from pure_utils.containers import paginate
+    >>> from pure_utils import paginate
 
-        a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
-        pages = paginate(a, size=3)
-        print(pages)
-        >>> [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10]]
+    >>> a = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
+    >>> pages = paginate(a, size=3)
+    >>> print(pages)
+    [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10]]
     """
-    assert size > 0
+    if size <= 0:
+        raise ValueError("Page size must be a positive integer")
+
     return [collection[start : start + size] for start in range(0, len(collection), size)]
 
 
 def pick(container: Mapping[str, Any], keys: KeysT, /) -> Mapping[str, Any]:
     """Pick key-value pairs from the source dictionary, by keys sequence.
 
     All other dictionary values will be omitted.
@@ -233,62 +226,61 @@
     Args:
         container: Source data container.
         keys: A sequence of strings or keys() for pick pairs in the source data container.
 
     Returns:
         A new data container with picked key-value pairs.
 
-    Example::
+    Usage:
 
-        from pure_utils.containers import pick
+    >>> from pure_utils import pick
 
-        container = {"key1": "val1", "key2": "val2", "key3": "val3"}
-        result = pick(container, ["key2", "key3"])
-        print(result)
-        >>> {"key2": "val2", "key3": "val3"}
+    >>> container = {"key1": "val1", "key2": "val2", "key3": "val3"}
+    >>> result = pick(container, ["key2", "key3"])
+    >>> print(result)
+    {"key2": "val2", "key3": "val3"}
     """
     return {_: container[_] for _ in keys if _ in container}
 
 
 def unpack(container: Mapping[str, Any], attributes: KeysT, /) -> tuple[Any, ...]:
     """Unpack the values of container object into separate variables.
 
     Args:
         container: Source data container.
         attributes: A sequence of strings or keys() whose values need to be unpacked.
 
     Returns:
         A tuple of unpacked values of the specified attributes.
 
-    Example::
+    Usage:
 
-        from pure_utils.containers import unpack
+    >>> from pure_utils import unpack
 
-        # Unpack existent attributes
-        d = {"a": 1, "b": True, "c": {"d": "test"}}
-        a, b = unpack(d, ("a", "b"))
-        print(a, b, sep=", ")
-        >>> 1, True
-
-        # Unpack non-existent attributes
-        e, f = print(unpack(d, ("e", "f")))
-        print(e, f, sep=", ")
-        >>> None, None
-
-        class A:
-            def __init__(self):
-                self.a = 100
-                self.b = 200
-                self.c = 300
-
-        # Unpack object attributes
-        obj = A()
-        a, b, c = unpack(obj, ("a", "b", "c"))
-        print(a, b, c, sep=", ")
-        >>> 100, 200, 300
+    >>> # Unpack existent attributes
+    >>> d = {"a": 1, "b": True, "c": {"d": "test"}}
+    >>> a, b = unpack(d, ("a", "b"))
+    >>> print(a, b, sep=", ")
+    1, True
+
+    >>> # Unpack non-existent attributes
+    >>> e, f = print(unpack(d, ("e", "f")))
+    >>> print(e, f, sep=", ")
+    None, None
+
+    >>> class A:
+    ...     def __init__(self):
+    ...         self.a = 100
+    ...         self.b = 200
+    ...         self.c = 300
+    >>> # Unpack object attributes
+    >>> obj = A()
+    >>> a, b, c = unpack(obj, ("a", "b", "c"))
+    >>> print(a, b, c, sep=", ")
+    100, 200, 300
     """
     if isinstance(container, dict):
         return tuple(container.get(attr) for attr in attributes)
 
     unpacked_values = []
 
     for attr in attributes:
```

### Comparing `pure_utils-0.8.0/pure_utils/debug.py` & `pure_utils-0.9.0/pure_utils/debug.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Utilities for debugging and development."""
 
 from copy import deepcopy
 from functools import wraps
 from inspect import stack
 from logging import Logger
 from time import time
-from typing import Any, Callable, Optional, TypeAlias
+from typing import Any, Callable, Optional
 
 from pure_utils._internal._profile_stats_serializers import (
     ProfileStatsStringSerializer,
     SerializedProfileStatsT,
 )
 from pure_utils.profiler import Profiler
 
+from .types import CallableAnyT
+
 __all__ = ["around", "caller", "deltatime", "profileit"]
 
-AnyCallableT: TypeAlias = Callable[[Any], Any]
 
 DEFAULT_STACK_SIZE: int = 20
 DEFAULT_STACK_FRAME: int = 2
 
 
 def around(*, before: Optional[Callable] = None, after: Optional[Callable] = None) -> Callable:
     """Add additional behavior before and after execution of decorated function.
@@ -35,50 +36,53 @@
 
     This memory is transferred in the form of additional parameter ("_pipe")
     in the kwargs named argument dictionary.
 
     Raises:
         ValueError: If one of the handlers (`before`, `after`) is not specified.
 
-    Example::
+    Usage:
 
-        from pure_utils.debug import around
+    >>> from pure_utils import around
 
-        def before_handler(*args, **kwargs):
-            kwargs["_pipe"]["key"] = "some data (from before to after handlers)"
-            print("before!")
-
-        def after_handler(*args, **kwargs):
-            print(f"after: {kwargs['_pipe']['key']} !")
-
-        @around(before=before_handler, after=after_handler)
-        def func():
-            print("in da func")
-
-        func()
-        >>> before!
-        >>> in da func
-        >>> after: some data (from before to after handlers) !
-
-        # !!! Use around with only BEFORE handler !!!
-        @around(before=before_handler)
-        def func2():
-            print("in da func2")
-        >>> before!
-        >>> in da func2
-
-        # !!! Use around with only AFTER handler !!!
-        @around(after=after_handler)
-        def func3():
-            print("in da func3")
-        >>> after!
-        >>> in da func3
+    >>> def before_handler(*args, **kwargs):
+    ...     kwargs["_pipe"]["key"] = "some data (from before to after handlers)"
+    ...     print("before!")
+
+    >>> def after_handler(*args, **kwargs):
+    ...     print(f"after: {kwargs['_pipe']['key']} !")
+
+    >>> @around(before=before_handler, after=after_handler)
+    ... def func():
+    ...     print("in da func")
+    >>> func()
+    before!
+    in da func
+    after: some data (from before to after handlers) !
+
+    Use around with only BEFORE handler:
+
+    >>> @around(before=before_handler)
+    ... def func2():
+    ...     print("in da func2")
+    >>> func2()
+    before!
+    in da func2
+
+    Use around with only AFTER handler:
+
+    >>> @around(after=after_handler)
+    ... def func3():
+    ...     print("in da func3")
+    >>> func3()
+    after!
+    in da func3
     """
 
-    def decorate(func) -> AnyCallableT:
+    def decorate(func) -> CallableAnyT:
         @wraps(func)
         def wrapper(*args, **kwargs):
             if not before and not after:
                 raise ValueError(
                     "One of the handlers (`before`, `after`) is not specified. Read the doc - "
                     "https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.around"
                 )
@@ -107,64 +111,65 @@
     Args:
         at_frame: The frame index number on the call stack (default 2).
                   Need increased with each wrap to decorator.
 
     Returns:
         The name of calling function/method.
 
-    Example::
+    Usage:
 
-        from pure_utils.debug import caller
+    >>> from pure_utils import caller
 
-        def func1(*args, **kwargs):
-            print(f"I'am 'func1', '{caller()}' called me.")
+    >>> def func1(*args, **kwargs):
+    ...     print(f"I'am 'func1', '{caller()}' called me.")
 
-        def func2(*args, **kwargs):
-            return func1()
+    >>> def func2(*args, **kwargs):
+    ...     return func1()
 
-        func2()
-        >>> I'am 'func1', 'func2' called me.
+    >>> func2()
+    I'am 'func1', 'func2' called me.
     """
     return str(stack()[at_frame].function)
 
 
 def deltatime(*, logger: Optional[Logger] = None) -> Callable:
     """Measure execution time of decorated function and print it to log.
 
     Args:
         logger: Optional logger object for printing execution time to file.
 
-    Example::
+    Usage:
 
-        from pure_utils.debug import deltatime
+    >>> from pure_utils import deltatime
 
-        @deltatime()
-        def aim_func():
-            for _ in range(1, 1000_000):
-                ...
+    >>> @deltatime()
+    ... def aim_func():
+    ...     for _ in range(1, 1000_000):
+    ...         pass
 
-        result, delta = aim_func()
-        print(f"Execution time of aim_func: {delta} sec.")
-        >>> Execution time of aim_func: 0.025 sec.
+    >>> result, delta = aim_func()
+    >>> print(f"Execution time of aim_func: {delta} sec.")
+    Execution time of aim_func: 0.025 sec.
 
-        # !!! Or use decorator with logger (side effect) !!!
+    Or use decorator with logger (side effect):
 
-        from logging import getLogger, DEBUG, basicConfig
-        basicConfig(level=DEBUG)
+    >>> from logging import getLogger, DEBUG, basicConfig
+    >>> basicConfig(level=DEBUG)
+    >>> root_logger = getLogger()
 
-        @deltatime(logger=getLogger())
-        def aim_func2():
-            for _ in range(1, 1000_000):
-                ...
+    >>> @deltatime(logger=root_logger)
+    ... def aim_func2():
+    ...     for _ in range(1, 1000_000):
+    ...         pass
 
-        result, _ = aim_func2()
-        >>> DEBUG:root:[DELTATIME]: 'aim_func2' (0.025 sec.)
+    >>> result, _ = aim_func2()
+    DEBUG:root:[DELTATIME]: 'aim_func2' (0.025 sec.)
     """
 
-    def decorate(func) -> AnyCallableT:
+    def decorate(func) -> CallableAnyT:
         @wraps(func)
         def wrapper(*args, **kwargs) -> tuple[Any, float]:
             t0 = time()
             retval = func(*args, **kwargs)
             delta = float(f"{time() - t0:.3f}")
             if logger:
                 logger.log(
@@ -181,57 +186,64 @@
 def profileit(*, logger: Optional[Logger] = None, stack_size: int = DEFAULT_STACK_SIZE) -> Callable:
     """Profile decorated function being with 'cProfile'.
 
     Args:
         logger: Optional logger object for printing execution time to file.
         stack_size: Stack size limit for profiler results.
 
-    Example::
-
-        from pure_utils.debug import profileit
-
-        def func1():
-            ...
-
-        def func2():
-            func1()
-
-        def func3():
-            func2()
-
-        @profileit()
-        def func4():
-            func3()
-
-        _, profile_info = func4()
-        print(profile_info)
-
-        5 function calls in 0.000 seconds
-           Ordered by: cumulative time, function name
-           ncalls  tottime  percall  cumtime  percall filename:lineno(function)
-              1    0.000    0.000    0.000    0.000 {method 'disable' of '_lsprof.Profiler' objects}
-              1    0.000    0.000    0.000    0.000 scriptname.py:13(func4)
-              1    0.000    0.000    0.000    0.000 scriptname.py:10(func3)
-              1    0.000    0.000    0.000    0.000 scriptname.py:7(func2)
-              1    0.000    0.000    0.000    0.000 scriptname.py:4(func1)
-        <pstats.Stats object at 0x10cf1a390>
-
-        # !!! Or use decorator with logger (side effect) !!!
-
-        from logging import getLogger, DEBUG, basicConfig
-        basicConfig(level=DEBUG)
+    Usage:
 
-        @profileit(logger=getLogger())
-        def func4():
-            func3()
+    >>> from pure_utils import profileit
 
-        func4()
+    >>> def func1():
+    ...     pass
+    >>> def func2():
+    ...     func1()
+    >>> def func3():
+    ...     func2()
+
+    >>> @profileit()
+    ... def func4():
+    ...     func3()
+
+    >>> _, profile_info = func4()
+    >>> print(profile_info)
+    5 function calls in 0.000 seconds
+       Ordered by: cumulative time, function name
+       ncalls  tottime  percall  cumtime  percall filename:lineno(function)
+          1    0.000    0.000    0.000    0.000 {method 'disable' of '_lsprof.Profiler' objects}
+          1    0.000    0.000    0.000    0.000 scriptname.py:13(func4)
+          1    0.000    0.000    0.000    0.000 scriptname.py:10(func3)
+          1    0.000    0.000    0.000    0.000 scriptname.py:7(func2)
+          1    0.000    0.000    0.000    0.000 scriptname.py:4(func1)
+    <pstats.Stats object at 0x10cf1a390>
+
+    Or use decorator with logger (side effect):
+
+    >>> from logging import getLogger, DEBUG, basicConfig
+    >>> basicConfig(level=DEBUG)
+    >>> root_logger = getlogger()
+
+    >>> @profileit(logger=root_logger)
+    ... def func4():
+    ...     func3()
+
+    >>> func4()
+    DEBUG:root: 5 function calls in 0.000 seconds
+       Ordered by: cumulative time, function name
+       ncalls  tottime  percall  cumtime  percall filename:lineno(function)
+          1    0.000    0.000    0.000    0.000 {method 'disable' of '_lsprof.Profiler' objects}
+          1    0.000    0.000    0.000    0.000 scriptname.py:13(func4)
+          1    0.000    0.000    0.000    0.000 scriptname.py:10(func3)
+          1    0.000    0.000    0.000    0.000 scriptname.py:7(func2)
+          1    0.000    0.000    0.000    0.000 scriptname.py:4(func1)
+    <pstats.Stats object at 0x10cf1a390>
     """
 
-    def decorate(func) -> AnyCallableT:
+    def decorate(func) -> CallableAnyT:
         @wraps(func)
         def wrapper(*args, **kwargs) -> tuple[Any, SerializedProfileStatsT]:
             retval = None
             profiler = Profiler()
 
             try:
                 retval = profiler.profile(func, *args, **kwargs)
```

### Comparing `pure_utils-0.8.0/pure_utils/profiler.py` & `pure_utils-0.9.0/pure_utils/profiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """Helper classes for working with the cProfile."""
 
 from cProfile import Profile
-from typing import Callable, ParamSpec, Type, TypeVar
+from typing import Callable, Type
 
-from pure_utils._internal._profile_stats import ProfileStats
-from pure_utils._internal._profile_stats_serializers import (
+from ._internal._profile_stats import ProfileStats
+from ._internal._profile_stats_serializers import (
     ProfileStatsSerializer,
     SerializedProfileStatsT,
 )
+from .types import P, T
 
 __all__ = ["Profiler"]
 
 
-T = TypeVar("T")
-P = ParamSpec("P")
-
-
 class Profiler:
     """A class provides a simple interface for profiling code.
 
-    Example::
+    Usage:
+
+    >>> from pure_utils import Profiler
+
+    >>> profiler = Profiler()
+    >>> some_function_retval = profiler.profile(some_func, *func_args, **func_kwargs)
+    >>> serialize_profile_result = profiler.serialize_result(SomeProfilerStatsSerializer)
 
-        from pure_utils.profiler import Profiler
+    Usage with string serializer:
 
-        profiler = Profiler()
-        some_function_retval = profiler.profile(some_func, *func_args, **func_kwargs)
-        profile_result = profiler.serialize_result(SomeProfilerStatsSerializer)
+    >>> from pure_utils._internal._profile_stats_serializers import ProfileStatsStringSerializer
+    >>> profile_result_as_string = profiler.serialize_result(ProfileStatsStringSerializer)
     """
 
     __slots__ = ("_profile", "__weakref__")
 
     def __init__(self) -> None:
         """Initialize profiler object."""
         self._profile = Profile()
```

### Comparing `pure_utils-0.8.0/pure_utils/repeaters.py` & `pure_utils-0.9.0/pure_utils/repeaters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,48 @@
 """Utilities for repeatedly execute custom logic.
 
-Example of usage exception based repeater::
+Example of usage exception based repeater:
 
-    from pure_utils.repeaters import ExceptionBasedRepeater, repeat
-
-    repeater = ExceptionBasedRepeater(
-        exceptions=(RuntimeError,),
-        attempts=5,
-        interval=2,
-        logger=getLogger()
-    )
-
-    @repeat(repeater)
-    def some_func(*args, **kwargs)
-        if some_negative_statement:
-             rise RuntimeError
-
-
-Example of usage predicate based repeater::
-
-    from pure_utils.repeaters import PredicateBasedRepeater, repeat
-
-    repeater = PredicateBasedRepeater(
-        predicate=lambda x: x != 0 ,
-        attempts=5,
-        interval=2,
-        logger=getLogger()
-    )
-
-    @repeat(repeater)
-    def some_func(*args, **kwargs)
-        return 0
+>>> from pure_utils import ExceptionBasedRepeater, repeat
 
+>>> repeater = ExceptionBasedRepeater(
+...     exceptions=(RuntimeError,),
+...     attempts=5,
+...     interval=2,
+...     logger=getLogger()
+... )
+
+>>> @repeat(repeater)
+... def some_func(*args, **kwargs)
+...     if some_negative_statement:
+...         rise RuntimeError
+
+Example of usage predicate based repeater:
+
+>>> from pure_utils import PredicateBasedRepeater, repeat
+
+>>> repeater = PredicateBasedRepeater(
+...     predicate=lambda x: x != 0,
+...     attempts=5,
+...     interval=2,
+...     logger=getLogger()
+... )
+
+>>> @repeat(repeater)
+... def some_func(*args, **kwargs)
+...     return 0
 """
 
 from abc import ABC, abstractmethod
 from functools import wraps
 from logging import Logger
 from time import sleep
-from typing import Any, Callable, Optional, ParamSpec, Type, TypeVar
-
-T = TypeVar("T")
-P = ParamSpec("P")
-ExceptionT = Type[BaseException]
+from typing import Any, Callable, Optional
 
+from .types import ExceptionT, P, T
 
 __all__ = ["Repeater", "ExceptionBasedRepeater", "PredicateBasedRepeater", "repeat"]
 
 DEFAULT_ATTEMPTS: int = 3
 DEFAULT_INTERVAL: int = 1
```

### Comparing `pure_utils-0.8.0/pure_utils/strings.py` & `pure_utils-0.9.0/pure_utils/strings.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     Args:
         length: The length of generated string.
         is_uppercase: If enable, generate string in uppercase.
 
     Returns:
         Generated ASCII-string with random letters.
 
-    Example::
+    Usage:
 
-        from pure_utils.strings import genstr
+    >>> from pure_utils import genstr
 
-        dummy = genstr(20)
-        print(dummy)
-        >>> otvqydcprjtpcuboumbs
+    >>> dummy = genstr(20)
+    >>> print(dummy)
+    otvqydcprjtpcuboumbs
 
-        dummy = genstr(20, is_uppercase=True)
-        print(dummy)
-        >>> POXDVZCMDWXBPVVRXWHN
+    >>> dummy = genstr(20, is_uppercase=True)
+    >>> print(dummy)
+    POXDVZCMDWXBPVVRXWHN
     """
     string_generator = ascii_uppercase if is_uppercase else ascii_lowercase
     return "".join(choices(string_generator, k=length))
 
 
 def gzip(string: str | bytes, /, *, level: int = 9) -> bytes:
     """Compress string (or bytes string) with gzip compression level.
@@ -41,40 +41,40 @@
         level: Compression level (numbers from 1 to 9) (default: 9).
                1 - fastest compression but big result size;
                9 - slowest compression but small result size (max compression).
 
     Returns:
         Compressed string in bytes.
 
-    Example::
+    Usage:
 
-        from pure_utils.strings import gzip
+    >>> from pure_utils import gzip
 
-        big_string = "abc" * 100500
-        print(len(big_string))
-        >>> 301500
+    >>> big_string = "abc" * 100500
+    >>> print(len(big_string))
+    301500
 
-        compressed_string = gzip(big_string)
-        print(len(compressed_string))
-        >>> 319
+    >>> compressed_string = gzip(big_string)
+    >>> print(len(compressed_string))
+    319
     """
     return compress(string if isinstance(string, bytes) else string.encode(), level=level)
 
 
 def gunzip(compressed_string: bytes, /) -> str:
     """Decompress bytes (earlier compressed with gzip) to string.
 
     Args:
         compressed_string: Bytes for decompression to string.
 
     Returns:
         Decompressed string from bytes.
 
-    Example::
+    Usage:
 
-        from pure_utils.strings import gzip, gunzip
+    >>> from pure_utils import gzip, gunzip
 
-        compressed_string = gzip("sample string")
-        print(gunzip(compressed_string))
-        >>> sample string
+    >>> compressed_string = gzip("sample string")
+    >>> print(gunzip(compressed_string))
+    sample string
     """
     return decompress(compressed_string).decode()
```

### Comparing `pure_utils-0.8.0/pure_utils/system.py` & `pure_utils-0.9.0/pure_utils/system.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,17 @@
         input: A data string that should be sent to input stream of command.
         timeout: Command completion timeout (30 seconds by default).
         *kwargs: Additional options for subprocess.run.
 
     Returns:
         Two-element tuple with data from standard streams: stdout and stderr.
 
-    Example::
+    Usage:
 
-        from pure_utils.system import execute
+    >>> from pure_utils import execute
 
-        result, _ = execute(["uname", "-o"])
-        print(result.decode())
-        >>> Darwin
+    >>> result, _ = execute(["uname", "-o"])
+    >>> print(result.decode())
+    Darwin
     """
     process = run(args, stdout=PIPE, stderr=PIPE, input=input, timeout=timeout, **kwargs)
     return process.stdout, process.stderr
```

### Comparing `pure_utils-0.8.0/pure_utils/times.py` & `pure_utils-0.9.0/pure_utils/times.py`

 * *Files 20% similar despite different names*

```diff
@@ -31,81 +31,81 @@
     Args:
         dt: Source datetime object.
         tz: Name of timezone for correction (UTC by default).
 
     Returns:
         A new datetime object in specified timezone.
 
-    Example::
+    Usage:
 
-        from datetime import datetime, UTC
-        from pure_utils.times import apply_tz
+    >>> from datetime import datetime, UTC
+    >>> from pure_utils import apply_tz
 
-        datetime_with_tz_context = apply_tz(datetime.now(UTC), "Europe/Moscow")
+    >>> datetime_with_tz_context = apply_tz(datetime.now(UTC), "Europe/Moscow")
     """
     return dt.astimezone(ZoneInfo(tz))
 
 
 def iso2format(isostr: str, fmt: str, /) -> str:
     """Convert ISO-8601 datetime string into a string of specified format.
 
     Args:
         isostr: ISO-8601 datetime string.
         fmt: New datetime format.
 
     Returns:
         Datetime string in specified format.
 
-    Example::
+    Usage:
 
-        from pure_utils.times import iso2format, YMD
+    >>> from pure_utils import iso2format, YMD
 
-        formatted_dt = iso2format("2005-08-09T18:31:42/P3Y6M4DT12H30M17S", YMD)
-        print(formatted_dt)
-        >>> 2005-08-09
+    >>> formatted_dt = iso2format("2005-08-09T18:31:42/P3Y6M4DT12H30M17S", YMD)
+    >>> print(formatted_dt)
+    2005-08-09
     """
     return datetime.fromisoformat(isostr).strftime(fmt)
 
 
 def iso2dmy(isostr: str, /) -> str:
     """Convert ISO-8601 datetime string into a string of DMY (DD.MM.YYYY) format.
 
     Args:
         isostr: ISO-8601 datetime string.
 
     Returns:
         Datetime string in DMY format (DD.MM.YYYY).
 
-    Example::
+    Usage:
 
-        from pure_utils.times import iso2dmy
+    >>> from pure_utils import iso2dmy
 
-        formatted_dt = iso2dmy("2005-08-09T18:31:42")
-        print(formatted_dt)
-        >>> 09.08.2005
+    >>> formatted_dt = iso2dmy("2005-08-09T18:31:42")
+    >>> print(formatted_dt)
+    09.08.2005
     """
     return iso2format(isostr, DMY)
 
 
 def iso2ymd(isostr: str, /) -> str:
     """Convert ISO-8601 datetime string into a string of YMD (YYYY-MM-DD) format.
 
     Args:
         isostr: ISO-8601 datetime string.
 
     Returns:
         Datetime string in YMD format (YYYY-MM-DD).
 
-    Example::
+    Usage:
 
-        from pure_utils.times import iso2ymd
+    >>> from pure_utils import iso2ymd
 
-        formatted_dt = iso2ymd("20080809T183142+0")
-        print(formatted_dt)
-        >>> 2008-08-09
+    >>> formatted_dt = iso2ymd("20080809T183142+0")
+    >>> print(formatted_dt)
+    2008-08-09
     """
     return iso2format(isostr, YMD)
 
 
 def round_by(dt: datetime, /, *, boundary: str) -> datetime:
     """Round datetime, discarding excessive precision.
 
@@ -116,26 +116,26 @@
 
     Returns:
         Rounded datetime object.
 
     Raises:
         ValueError: If `boundary` is invalid.
 
-    Example::
+    Usage:
 
-        from datetime import datetime
-        from pure_utils.times import round_by
+    >>> from datetime import datetime
+    >>> from pure_utils import round_by
 
-        exact_datatime = datetime.now()
-        print(exact_datatime)
-        >>> 2024-02-03 17:54:37.472482
-
-        rounded_datetime = round_by(exact_datatime, boundary="hour")
-        print(rounded_datetime)
-        >>> 2024-02-03 17:00:00
+    >>> exact_datatime = datetime.now()
+    >>> print(exact_datatime)
+    2024-02-03 17:54:37.472482
+
+    >>> rounded_datetime = round_by(exact_datatime, boundary="hour")
+    >>> print(rounded_datetime)
+    2024-02-03 17:00:00
     """
     replace = {}
 
     match boundary:
         case RoundByEnum.DAY.value:
             for _ in ("hour", "minute", "second", "microsecond"):
                 replace[_] = 0
```

### Comparing `pure_utils-0.8.0/pure_utils/_internal/_profile_stats.py` & `pure_utils-0.9.0/pure_utils/_internal/_profile_stats.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/pure_utils/_internal/_profile_stats_serializers.py` & `pure_utils-0.9.0/pure_utils/_internal/_profile_stats_serializers.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/tests/test_containers.py` & `pure_utils-0.9.0/tests/test_containers.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,22 +17,23 @@
     def test_on_non_empty_list(self):
         source_list = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
         a, b = bisect(source_list)
 
         assert a == [1, 2, 3, 4, 5]
         assert b == [6, 7, 8, 9, 10, 11]
 
-        # Source list not changed.
+        # Source list is not changed
         assert source_list == [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
 
     def test_on_empty_list(self):
         source_list = []
 
-        with pytest.raises(AssertionError):
+        with pytest.raises(ValueError) as excinfo:
             bisect(source_list)
+            assert excinfo.value.error == "The source collection must not be empty"
 
         assert source_list == []
 
 
 class TestFirst:
     def test_on_non_empty_list(self):
         assert first([1, 2, 3]) == 1
@@ -162,20 +163,22 @@
         pages = paginate(source_list, size=5)
         assert pages == [[1]]
 
     def test_on_empty_list(self):
         assert paginate([], size=2) == []
 
     def test_on_zero_size(self):
-        with pytest.raises(AssertionError):
+        with pytest.raises(ValueError) as excinfo:
             paginate([1, 2], size=0)
+            assert excinfo.value.error == "Page size must be a positive integer"
 
     def test_on_negative_size(self):
-        with pytest.raises(AssertionError):
+        with pytest.raises(ValueError) as excinfo:
             paginate([1, 2], size=-1)
+            assert excinfo.value.error == "Page size must be a positive integer"
 
     def test_on_tuple(self):
         source_tuple = (1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
         pages = paginate(source_tuple, size=5)
         assert pages == [(1, 2, 3, 4, 5), (6, 7, 8, 9, 10)]
```

### Comparing `pure_utils-0.8.0/tests/test_debug.py` & `pure_utils-0.9.0/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/tests/test_profiler.py` & `pure_utils-0.9.0/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/tests/test_repeaters.py` & `pure_utils-0.9.0/tests/test_repeaters.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/tests/test_strings.py` & `pure_utils-0.9.0/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/tests/test_system.py` & `pure_utils-0.9.0/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/tests/test_times.py` & `pure_utils-0.9.0/tests/test_times.py`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/LICENSE` & `pure_utils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/README.md` & `pure_utils-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 5. Full test coverage.
 
 **For detail information read the [doc](https://p3t3rbr0.github.io/py3-pure-utils/)**.
 
 # Available utilities
 
 * [common](https://p3t3rbr0.github.io/py3-pure-utils/refs/common.html) - The common purpose utilities.
-  * [Singleton](https://p3t3rbr0.github.io/py3-pure-utils/refs/common.html#common.Singleton) - A metaclass that implements the singleton pattern for inheritors.
-* [containers](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html) - Utilities for working with data containers (lists, dictionaries, tuples, sets, etc.).
+  * [Singleton](https://p3t3rbr0.github.io/py3-pure-utils/refs/common.html#common.Singleton) - A metaclass, implements the singleton pattern for inheritors.
+* [containers](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html) - Utilities for working with data containers (lists, dicts, tuples, sets, etc.).
   * [bisect](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.bisect)(collection, /) - Bisect the list into two parts/halves based on the number of elements.
   * [first](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.first)(collection, /) - Get the value of the first element from a homogeneous collection.
   * [flatten](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.flatten)(collection, /) - Make the iterated collection a flat (single nesting level).
   * [get_or_else](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.bisect)(collection, index[, default]) - Get value of element, and if it is missing, return the default value.
   * [omit](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.omit)(container, keys, /) - Omit key-value pairs from the source dictionary, by keys sequence.
   * [paginate](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.paginate)(collection, /, *, size) - Split the collection into page(s) according to the specified limit.
   * [pick](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.pick)(container, keys, /) - Pick key-value pairs from the source dictionary, by keys sequence.
-  * [symmdiff](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.symmdiff)(s1, s2, /) - Obtain the symmetric difference of two sequences.
+  * [symmdiff](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.symmdiff)(collection1, collection2, /) - Obtain the symmetric difference of two sequences.
   * [unpack](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.unpack)(container, attributes, /) - Unpack the values of container object into separate variables.
 * [debug](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html) - Utilities for debugging and development.
   * [around](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.around)(*[, before, after]) - Add additional behavior before and after execution of decorated function.
   * [caller](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.caller)(*[, at_frame]) - Get the name of calling function/method (from current function/method context).
   * [deltatime](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.deltatime)(*[, logger]) - Measure execution time of decorated function and print it to log.
   * [profileit](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.profileit)(*[, logger, stack_size]) - Profile decorated function being with 'cProfile'.
 * [profiler](https://p3t3rbr0.github.io/py3-pure-utils/refs/profiler.html) - Helper classes for working with the cProfile.
```

### Comparing `pure_utils-0.8.0/pyproject.toml` & `pure_utils-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pure_utils-0.8.0/PKG-INFO` & `pure_utils-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-utils
-Version: 0.8.0
+Version: 0.9.0
 Summary: Yet another python utilities, with the goal of collecting useful bicycles and crutches in one place.
 Project-URL: Homepage, https://github.com/p3t3rbr0/py3-pure-utils
 Project-URL: Documentation, https://p3t3rbr0.github.io/py3-pure-utils/
 Project-URL: Repository, https://github.com/p3t3rbr0/py3-pure-utils.git
 Project-URL: Issues, https://github.com/p3t3rbr0/py3-pure-utils/issues
 Project-URL: Changelog, https://github.com/p3t3rbr0/py3-pure-utils/blob/master/.docs/source/changelog.rst
 Author-email: Peter Bro <p3t3rbr0@gmail.com>
@@ -58,24 +58,24 @@
 5. Full test coverage.
 
 **For detail information read the [doc](https://p3t3rbr0.github.io/py3-pure-utils/)**.
 
 # Available utilities
 
 * [common](https://p3t3rbr0.github.io/py3-pure-utils/refs/common.html) - The common purpose utilities.
-  * [Singleton](https://p3t3rbr0.github.io/py3-pure-utils/refs/common.html#common.Singleton) - A metaclass that implements the singleton pattern for inheritors.
-* [containers](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html) - Utilities for working with data containers (lists, dictionaries, tuples, sets, etc.).
+  * [Singleton](https://p3t3rbr0.github.io/py3-pure-utils/refs/common.html#common.Singleton) - A metaclass, implements the singleton pattern for inheritors.
+* [containers](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html) - Utilities for working with data containers (lists, dicts, tuples, sets, etc.).
   * [bisect](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.bisect)(collection, /) - Bisect the list into two parts/halves based on the number of elements.
   * [first](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.first)(collection, /) - Get the value of the first element from a homogeneous collection.
   * [flatten](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.flatten)(collection, /) - Make the iterated collection a flat (single nesting level).
   * [get_or_else](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.bisect)(collection, index[, default]) - Get value of element, and if it is missing, return the default value.
   * [omit](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.omit)(container, keys, /) - Omit key-value pairs from the source dictionary, by keys sequence.
   * [paginate](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.paginate)(collection, /, *, size) - Split the collection into page(s) according to the specified limit.
   * [pick](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.pick)(container, keys, /) - Pick key-value pairs from the source dictionary, by keys sequence.
-  * [symmdiff](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.symmdiff)(s1, s2, /) - Obtain the symmetric difference of two sequences.
+  * [symmdiff](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.symmdiff)(collection1, collection2, /) - Obtain the symmetric difference of two sequences.
   * [unpack](https://p3t3rbr0.github.io/py3-pure-utils/refs/containers.html#containers.unpack)(container, attributes, /) - Unpack the values of container object into separate variables.
 * [debug](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html) - Utilities for debugging and development.
   * [around](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.around)(*[, before, after]) - Add additional behavior before and after execution of decorated function.
   * [caller](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.caller)(*[, at_frame]) - Get the name of calling function/method (from current function/method context).
   * [deltatime](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.deltatime)(*[, logger]) - Measure execution time of decorated function and print it to log.
   * [profileit](https://p3t3rbr0.github.io/py3-pure-utils/refs/debug.html#debug.profileit)(*[, logger, stack_size]) - Profile decorated function being with 'cProfile'.
 * [profiler](https://p3t3rbr0.github.io/py3-pure-utils/refs/profiler.html) - Helper classes for working with the cProfile.
```

