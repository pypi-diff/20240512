# Comparing `tmp/plum_dispatch-2.3.5.tar.gz` & `tmp/plum_dispatch-2.3.6.tar.gz`

## Comparing `plum_dispatch-2.3.5.tar` & `plum_dispatch-2.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/_version.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/alias.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/autoreload.py
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/dispatcher.py
--rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/function.py
--rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/method.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/overload.py
--rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/parametric.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/promotion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/py.typed
--rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/repr.py
--rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/resolver.py
--rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/signature.py
--rw-r--r--   0        0        0     9721 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/type.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/typing.py
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/plum/util.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/LICENCE.txt
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/README.md
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/pyproject.toml
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 plum_dispatch-2.3.5/PKG-INFO
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/_version.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/alias.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/autoreload.py
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/dispatcher.py
+-rw-r--r--   0        0        0    17779 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/function.py
+-rw-r--r--   0        0        0     6904 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/method.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/overload.py
+-rw-r--r--   0        0        0    23461 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/parametric.py
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/promotion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/py.typed
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/repr.py
+-rw-r--r--   0        0        0    12283 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/resolver.py
+-rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/signature.py
+-rw-r--r--   0        0        0     9721 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/type.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/typing.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/plum/util.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/LICENCE.txt
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/README.md
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 plum_dispatch-2.3.6/PKG-INFO
```

### Comparing `plum_dispatch-2.3.5/plum/__init__.py` & `plum_dispatch-2.3.6/plum/__init__.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/alias.py` & `plum_dispatch-2.3.6/plum/alias.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/autoreload.py` & `plum_dispatch-2.3.6/plum/autoreload.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/dispatcher.py` & `plum_dispatch-2.3.6/plum/dispatcher.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/function.py` & `plum_dispatch-2.3.6/plum/function.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/method.py` & `plum_dispatch-2.3.6/plum/method.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/parametric.py` & `plum_dispatch-2.3.6/plum/parametric.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .type import resolve_type_hint
 from .util import TypeHint
 
 __all__ = [
     "CovariantMeta",
     "parametric",
     "type_parameter",
+    "type_nonparametric",
     "type_unparametrized",
     "kind",
     "Kind",
     "Val",
 ]
 
 T = TypeVar("T")
@@ -277,73 +278,111 @@
             cls.__new__ = class_new
         super(original_class, cls).__init_subclass__(**kw_args)
 
     def __class_nonparametric__(cls):
         """Return the non-parametric type of an object.
 
         :mod:`plum.parametric` produces parametric subtypes of classes. This
-        method can be used to get the non-parametric type of an object.
+        method can be used to get the original non-parametric type of an object.
+
+        See Also
+        --------
+        :func:`plum.type_nonparametric`
+            The more-user-friendly function equivalent of this method.
+        :func:`plum.type_unparametrized`
+            A function that returns the non-concrete, but still parametric, type
+            of an object.
 
         Examples
         --------
+        In this example we will demonstrate how to retrieve the original
+        non-parametric class from a :func:`plum.parametric` decorated class.
+
+        :func:`plum.parametric` defines a parametric class of the same name as
+        the original class, and then creates a subclass of the original class
+        with the type parameter inferred from the arguments of the constructor.
+
         >>> from plum import parametric
-        >>> @parametric
-        ... class Obj:
+        >>> class Obj:
         ...     @classmethod
         ...     def __infer_type_parameter__(cls, *arg):
         ...         return type(arg[0])
         ...     def __init__(self, x):
         ...         self.x = x
         ...     def __repr__(self):
         ...         return f"Obj({self.x})"
+        >>> PObj = parametric(Obj)
 
-        >>> obj = Obj(1)
-        >>> obj
-        Obj(1)
+        >>> PObj.mro()
+        [<class 'plum.parametric.Obj'>, <class 'plum.parametric.Obj'>,
+         <class 'object'>]
+
+        Note that the class `Obj` appears twice in the MRO. The first one is the
+        parametric class, and the second one is the non-parametric class. The
+        non-parametric class is the original class that was passed to the
+        ``parametric`` decorator.
 
-        >>> type(obj).mro()
-        [Obj[int], Obj, object]
+        Rather than navigating the MRO, we can get the non-parametric class of
+        an object by calling the ``__class_nonparametric__`` method.
 
-        >>> obj.__class_nonparametric__().mro()
-        [Obj, object]
+        >>> PObj(1).__class_nonparametric__() is Obj
+        True
         """
         return original_class
 
     def __class_unparametrized__(cls):
         """Return the unparametrized type of an object.
 
         :mod:`plum.parametric` produces parametric subtypes of classes. This
         method can be used to get the un-parametrized type of an object.
 
+        See Also
+        --------
+        :func:`plum.type_unparametrized`
+            The more-user-friendly function equivalent of this method.
+        :func:`plum.type_nonparametric`
+            A function to get the non-parametric type of an object.
+
         Examples
         --------
+        In this example we will demonstrate how to retrieve the original
+        non-parametric class from a :func:`plum.parametric` decorated class.
+
+        :func:`plum.parametric` defines a parametric class of the same name as
+        the original class, and then creates a subclass of the original class
+        with the type parameter inferred from the arguments of the constructor.
+
         >>> from plum import parametric
-        >>> @parametric
-        ... class Obj:
+        >>> class Obj:
         ...     @classmethod
         ...     def __infer_type_parameter__(cls, *arg):
         ...         return type(arg[0])
         ...     def __init__(self, x):
         ...         self.x = x
         ...     def __repr__(self):
         ...         return f"Obj({self.x})"
+        >>> PObj = parametric(Obj)
 
-        >>> obj = Obj(1)
-        >>> obj
-        Obj(1)
-
-        >>> type(obj).__name__
-        Obj[int]
-
-        >>> obj.__class_unparametrized__().mro()
-        [Obj, Obj, object]
-
-        Note that this is still NOT the 'original' non-`parametric`-wrapped
-        type.  This is the type that is wrapped by :mod:`plum.parametric`, but
-        without the inferred type parameter(s).
+        >>> PObj.mro()
+        [<class 'plum.parametric.Obj'>, <class 'plum.parametric.Obj'>,
+         <class 'object'>]
+
+        Note that the class `Obj` appears twice in the MRO. The first one is the
+        non-concrete parametric class, and the second one is the non-parametric
+        class. Rather than navigating the MRO, we can get the non-concrete
+        parametric class of an object by calling the
+        ``__class_unparametrized__`` method.
+
+        >>> PObj(1).__class_unparametrized__() is PObj
+        True
+
+        Note that this is still NOT the 'original'
+        non-:func:`plum.parametric`-wrapped type.  This is the type that is
+        wrapped by :mod:`plum.parametric`, but without the inferred type
+        parameter(s).
         """
         return parametric_class
 
     # Create parametric class.
     parametric_class = meta(
         original_class.__name__,
         (original_class,),
@@ -426,47 +465,141 @@
         return t.type_parameter
     raise ValueError(
         f"`{x}` is not a concrete parametric type or an instance of a"
         f" concrete parametric type."
     )
 
 
+def type_nonparametric(q: T) -> Type[T]:
+    """Return the non-parametric type of an object.
+
+    :mod:`plum.parametric` produces parametric subtypes of classes. This method
+    can be used to get the original non-parametric type of an object.
+
+    See Also
+    --------
+    :func:`plum.type_unparametrized`
+        A function that returns the non-concrete, but still parametric, type of
+        an object.
+
+    Examples
+    --------
+    In this example we will demonstrate how to retrieve the original
+    non-parametric class from a :func:`plum.parametric` decorated class.
+
+    :func:`plum.parametric` defines a parametric class of the same name as the
+    original class, and then creates a subclass of the original class with the
+    type parameter inferred from the arguments of the constructor.
+
+    >>> from plum import parametric
+    >>> class Obj:
+    ...     @classmethod
+    ...     def __infer_type_parameter__(cls, *arg):
+    ...         return type(arg[0])
+    ...     def __init__(self, x):
+    ...         self.x = x
+    ...     def __repr__(self):
+    ...         return f"Obj({self.x})"
+    >>> PObj = parametric(Obj)
+    >>> pobj = PObj(1)
+
+    >>> type(pobj).mro()
+    [<class 'plum.parametric.Obj[int]'>, <class 'plum.parametric.Obj'>,
+     <class 'plum.parametric.Obj'>, <class 'object'>]
+
+    Note that the class `Obj` appears twice in the MRO. The first one is the
+    parametric class, and the second one is the non-parametric class. The
+    non-parametric class is the original class that was passed to the
+    ``parametric`` decorator.
+
+    Rather than navigating the MRO, we can get the non-parametric class of an
+    object by calling ``type_nonparametric`` function.
+
+    >>> type(pobj) is PObj[int]
+    True
+    >>> type(pobj) is PObj
+    False
+    >>> type(pobj) is Obj
+    False
+
+    >>> type_nonparametric(pobj) is PObj[int]
+    False
+    >>> type_nonparametric(pobj) is PObj
+    False
+    >>> type_nonparametric(pobj) is Obj
+    True
+    """
+    return (
+        q.__class_nonparametric__()
+        if isinstance(type(q), ParametricTypeMeta)
+        else type(q)
+    )
+
+
 def type_unparametrized(q: T) -> Type[T]:
     """Return the unparametrized type of an object.
 
     :mod:`plum.parametric` produces parametric subtypes of classes.  This
     function can be used to get the un-parametrized type of an object.
     This function also works for normal, :mod:`plum.parametric`-wrapped classes.
 
+    See Also
+    --------
+    :func:`plum.type_nonparametric`
+        A function to get the non-parametric type of an object.
+
     Examples
     --------
+    In this example we will demonstrate how to retrieve the original
+    non-parametric class from a :func:`plum.parametric` decorated class.
+
+    :func:`plum.parametric` defines a parametric class of the same name as
+    the original class, and then creates a subclass of the original class
+    with the type parameter inferred from the arguments of the constructor.
+
     >>> from plum import parametric
-    >>> @parametric
-    ... class Obj:
+    >>> class Obj:
     ...     @classmethod
     ...     def __infer_type_parameter__(cls, *arg):
     ...         return type(arg[0])
     ...     def __init__(self, x):
     ...         self.x = x
     ...     def __repr__(self):
     ...         return f"Obj({self.x})"
+    >>> PObj = parametric(Obj)
+    >>> pobj = PObj(1)
 
-    >>> obj = Obj(1)
-    >>> obj
-    Obj(1)
-
-    >>> type(obj).__name__
-    Obj[int]
-
-    >>> type_unparametrized(obj).__name__
-    Obj
-
-    Note that this is still NOT the 'original' non-`parametric`-wrapped type.
-    This is the type that is wrapped by :mod:`plum.parametric`, but without the
-    inferred type parameter(s).
+    >>> type(pobj).mro()
+    [<class 'plum.parametric.Obj[int]'>, <class 'plum.parametric.Obj'>,
+     <class 'plum.parametric.Obj'>, <class 'object'>]
+
+    Note that the class `Obj` appears twice in the MRO. The first one is the
+    non-concrete parametric class, and the second one is the non-parametric
+    class. Rather than navigating the MRO, we can get the non-concrete
+    parametric class of an object by calling the
+    ``type_unparametrized`` function.
+
+    >>> type(pobj) is PObj[int]
+    True
+    >>> type(pobj) is PObj
+    False
+    >>> type(pobj) is Obj
+    False
+
+    >>> type_unparametrized(pobj) is PObj[int]
+    False
+    >>> type_unparametrized(pobj) is PObj
+    True
+    >>> type_unparametrized(pobj) is Obj
+    False
+
+    Note that this is still NOT the 'original'
+    non-:func:`plum.parametric`-wrapped type.  This is the type that is
+    wrapped by :mod:`plum.parametric`, but without the inferred type
+    parameter(s).
     """
     typ = type(q)
     return q.__class_unparametrized__() if isinstance(typ, ParametricTypeMeta) else typ
 
 
 def kind(SuperClass=object):
     """Create a parametric wrapper type for dispatch purposes.
```

### Comparing `plum_dispatch-2.3.5/plum/promotion.py` & `plum_dispatch-2.3.6/plum/promotion.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/repr.py` & `plum_dispatch-2.3.6/plum/repr.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/resolver.py` & `plum_dispatch-2.3.6/plum/resolver.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/signature.py` & `plum_dispatch-2.3.6/plum/signature.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/type.py` & `plum_dispatch-2.3.6/plum/type.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/typing.py` & `plum_dispatch-2.3.6/plum/typing.py`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/plum/util.py` & `plum_dispatch-2.3.6/plum/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,16 +118,18 @@
         bool: Whether `f` is part of a class.
     """
     parts = f.__qualname__.split(".")
     return len(parts) >= 2 and parts[-2] != "<locals>"
 
 
 def _split_parts(f: Callable) -> List[str]:
-    qualified_name = f.__module__ + "." + f.__qualname__
-    return qualified_name.split(".")
+    # Under edge cases, `f.__module__` can be `None`. In this case we skip it.
+    # Otherwise, the fully-qualified name is the module.qual.name.
+    fqn = ("" if f.__module__ is None else f.__module__ + ".") + f.__qualname__
+    return fqn.split(".")
 
 
 def get_class(f: Callable) -> str:
     """Assuming that `f` is part of a class, get the fully qualified name of the
     class.
 
     Args:
```

### Comparing `plum_dispatch-2.3.5/LICENCE.txt` & `plum_dispatch-2.3.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/README.md` & `plum_dispatch-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `plum_dispatch-2.3.5/pyproject.toml` & `plum_dispatch-2.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     "ghp-import",
     "wheel",
     "build",
     "tox",
     "jupyter-book",
     "mypy",
     "pyright>=1.1.331",
-    "ruff==0.1.0"
+    "ruff==0.1.0",
+    "sybil",
 ]
 
 [project.urls]
 repository = "https://github.com/beartype/plum"
 
 [tool.hatch.build]
 include = ["plum*"]
@@ -58,17 +59,20 @@
 # Development tools
 [tool.coverage.run]
 branch = true
 command_line = "-m pytest --verbose test"
 source = ["plum"]
 
 [tool.pytest.ini_options]
-testpaths = [
-    "tests",
+testpaths = ["tests/", "plum", "docs"]
+addopts = [
+    "-ra",
+    "-p no:doctest",
 ]
+minversion = "6.0"
 
 # Formatting tools
 [tool.black]
 line-length = 88
 target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 exclude = '''
```

### Comparing `plum_dispatch-2.3.5/PKG-INFO` & `plum_dispatch-2.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: plum-dispatch
-Version: 2.3.5
+Version: 2.3.6
 Summary: Multiple dispatch in Python
 Project-URL: repository, https://github.com/beartype/plum
 Author-email: Wessel Bruinsma <wessel.p.bruinsma@gmail.com>
 License: MIT
 License-File: LICENCE.txt
 Keywords: multiple dispatch
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,14 +23,15 @@
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: numpy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pyright>=1.1.331; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Requires-Dist: ruff==0.1.0; extra == 'dev'
+Requires-Dist: sybil; extra == 'dev'
 Requires-Dist: tox; extra == 'dev'
 Requires-Dist: wheel; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # [Plum: Multiple Dispatch in Python](https://github.com/beartype/plum)
 
 [![DOI](https://zenodo.org/badge/110279931.svg)](https://zenodo.org/badge/latestdoi/110279931)
```

