# Comparing `tmp/d42-1.7.0.tar.gz` & `tmp/d42-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d42-1.7.0.tar", last modified: Sun Aug 27 12:38:07 2023, max compression
+gzip compressed data, was "d42-1.7.1.tar", last modified: Sun May 12 15:54:11 2024, max compression
```

## Comparing `d42-1.7.0.tar` & `d42-1.7.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 12:38:07.282477 d42-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (999)    11357 2023-08-27 12:37:50.000000 d42-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     2113 2023-08-27 12:38:07.282477 d42-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1437 2023-08-27 12:37:50.000000 d42-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 12:38:07.278477 d42-1.7.0/d42/
--rw-r--r--   0 runner    (1001) docker     (999)      832 2023-08-27 12:37:50.000000 d42-1.7.0/d42/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 12:38:07.282477 d42-1.7.0/d42/custom_type/
--rw-r--r--   0 runner    (1001) docker     (999)      340 2023-08-27 12:37:50.000000 d42-1.7.0/d42/custom_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2052 2023-08-27 12:37:50.000000 d42-1.7.0/d42/custom_type/_custom_type.py
--rw-r--r--   0 runner    (1001) docker     (999)      307 2023-08-27 12:37:50.000000 d42-1.7.0/d42/custom_type/errors.py
--rw-r--r--   0 runner    (1001) docker     (999)      231 2023-08-27 12:37:50.000000 d42-1.7.0/d42/custom_type/utils.py
--rw-r--r--   0 runner    (1001) docker     (999)      207 2023-08-27 12:37:50.000000 d42-1.7.0/d42/custom_type/visitors.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-27 12:37:50.000000 d42-1.7.0/d42/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 12:38:07.282477 d42-1.7.0/d42.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2113 2023-08-27 12:38:07.000000 d42-1.7.0/d42.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      386 2023-08-27 12:38:07.000000 d42-1.7.0/d42.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-27 12:38:07.000000 d42-1.7.0/d42.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)      105 2023-08-27 12:38:07.000000 d42-1.7.0/d42.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-08-27 12:38:07.000000 d42-1.7.0/d42.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      710 2023-08-27 12:38:07.282477 d42-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1218 2023-08-27 12:37:50.000000 d42-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-27 12:38:07.282477 d42-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (999)     4454 2023-08-27 12:37:50.000000 d42-1.7.0/tests/test_custom_type.py
--rw-r--r--   0 runner    (1001) docker     (999)     1148 2023-08-27 12:37:50.000000 d42-1.7.0/tests/test_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:54:11.230851 d42-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 15:53:58.000000 d42-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-12 15:54:11.230851 d42-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-12 15:53:58.000000 d42-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:54:11.230851 d42-1.7.1/d42/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-12 15:53:58.000000 d42-1.7.1/d42/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:54:11.230851 d42-1.7.1/d42/custom_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-12 15:53:58.000000 d42-1.7.1/d42/custom_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-12 15:53:58.000000 d42-1.7.1/d42/custom_type/_custom_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-12 15:53:58.000000 d42-1.7.1/d42/custom_type/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-12 15:53:58.000000 d42-1.7.1/d42/custom_type/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-12 15:53:58.000000 d42-1.7.1/d42/custom_type/visitors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:53:58.000000 d42-1.7.1/d42/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:54:11.230851 d42-1.7.1/d42.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-12 15:54:11.000000 d42-1.7.1/d42.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-12 15:54:11.000000 d42-1.7.1/d42.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:54:11.000000 d42-1.7.1/d42.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-12 15:54:11.000000 d42-1.7.1/d42.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-12 15:54:11.000000 d42-1.7.1/d42.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-12 15:54:11.230851 d42-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-12 15:53:58.000000 d42-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:54:11.230851 d42-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-12 15:53:58.000000 d42-1.7.1/tests/test_custom_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-12 15:53:58.000000 d42-1.7.1/tests/test_imports.py
```

### Comparing `d42-1.7.0/LICENSE` & `d42-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `d42-1.7.0/PKG-INFO` & `d42-1.7.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 Metadata-Version: 2.1
 Name: d42
-Version: 1.7.0
+Version: 1.7.1
 Summary: One package for district42 ecosystem
-Home-page: https://github.com/tsv1/d42
+Home-page: https://github.com/d42-schemas/d42
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
-Project-URL: Docs, https://d42.vedro.io
-Project-URL: GitHub, https://github.com/tsv1/d42
+Project-URL: Docs, https://d42.sh
+Project-URL: GitHub, https://github.com/d42-schemas/d42
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: district42<1.8,>=1.7
+Requires-Dist: blahblah<1.8,>=1.7
+Requires-Dist: valera<1.8,>=1.7
+Requires-Dist: revolt<1.8,>=1.7
+Requires-Dist: niltype<2.0,>=0.3
+Requires-Dist: th<1.0,>=0.3
 
 # d42
 
 [![PyPI](https://img.shields.io/pypi/v/d42.svg?style=flat-square)](https://pypi.python.org/pypi/d42/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/d42?style=flat-square)](https://pypi.python.org/pypi/d42/)
 [![Python Version](https://img.shields.io/pypi/pyversions/d42.svg?style=flat-square)](https://pypi.python.org/pypi/d42/)
 
-`d42` package offers several tools to define, generate, validate, and substitute data based on models defined using the district42 data description language.
+The `d42` package is a comprehensive toolkit for data modeling, which includes functionalities for definition, generation, validation, and substitution of data models using a robust data description language.
 
 ## Installation
 
 ```shell
 $ pip3 install d42
 ```
 
-## Components
-
-The [d42](https://pypi.org/project/d42/) package comprises the following components:
-- [district42](https://pypi.org/project/district42/) — a data description language for defining data models
-- [blahblah](https://pypi.org/project/blahblah/) — a fake data generator tailored for the district42 schema
-- [valera](https://pypi.org/project/valera/) — a validator designed for the district42 schema
-- [revolt](https://pypi.org/project/revolt/) — a value substitutor compatible with the district42 schema
-
-## Usage
+## Usage Example
 
 ```python
 from d42 import schema, fake, validate_or_fail
 
-# Define a schema with a string "banana"
+# Define a schema for a string containing "banana"
 sch = schema.str("banana")
 
 # Generate a fake value based on the schema and validate it
 assert validate_or_fail(sch, fake(sch))
 ```
 
-For a more comprehensive guide and detailed information, check out the [official documentation](https://d42.vedro.io/).
+## Documentation
+
+For detailed documentation, visit the [official d42 documentation](https://d42.sh).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `d42-1.7.0/README.md` & `d42-1.7.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 # d42
 
 [![PyPI](https://img.shields.io/pypi/v/d42.svg?style=flat-square)](https://pypi.python.org/pypi/d42/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/d42?style=flat-square)](https://pypi.python.org/pypi/d42/)
 [![Python Version](https://img.shields.io/pypi/pyversions/d42.svg?style=flat-square)](https://pypi.python.org/pypi/d42/)
 
-`d42` package offers several tools to define, generate, validate, and substitute data based on models defined using the district42 data description language.
+The `d42` package is a comprehensive toolkit for data modeling, which includes functionalities for definition, generation, validation, and substitution of data models using a robust data description language.
 
 ## Installation
 
 ```shell
 $ pip3 install d42
 ```
 
-## Components
-
-The [d42](https://pypi.org/project/d42/) package comprises the following components:
-- [district42](https://pypi.org/project/district42/) — a data description language for defining data models
-- [blahblah](https://pypi.org/project/blahblah/) — a fake data generator tailored for the district42 schema
-- [valera](https://pypi.org/project/valera/) — a validator designed for the district42 schema
-- [revolt](https://pypi.org/project/revolt/) — a value substitutor compatible with the district42 schema
-
-## Usage
+## Usage Example
 
 ```python
 from d42 import schema, fake, validate_or_fail
 
-# Define a schema with a string "banana"
+# Define a schema for a string containing "banana"
 sch = schema.str("banana")
 
 # Generate a fake value based on the schema and validate it
 assert validate_or_fail(sch, fake(sch))
 ```
 
-For a more comprehensive guide and detailed information, check out the [official documentation](https://d42.vedro.io/).
+## Documentation
+
+For detailed documentation, visit the [official d42 documentation](https://d42.sh).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `d42-1.7.0/d42/__init__.py` & `d42-1.7.1/d42/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 try:
     make_required = district42.make_required
 except AttributeError:
     from typing import Any
 
     def make_required(schema: Any, keys: Any = None) -> Any:
-        raise ValueError("make_required is not available in district42 < 1.7.0")
+        raise ValueError("make_required is not available in district42 < 1.7.1")
 
 schema = district42.schema
 optional = district42.optional
 from_native = district42.from_native
 register_type = district42.register_type
 
 fake = blahblah.fake
@@ -26,8 +26,8 @@
 
 __all__ = (
     "schema", "optional", "from_native", "register_type", "make_required",
     "fake",
     "validate", "validate_or_fail", "ValidationException",
     "substitute",
 )
-__version__ = "1.7.0"
+__version__ = "1.7.1"
```

### Comparing `d42-1.7.0/d42/custom_type/_custom_type.py` & `d42-1.7.1/d42/custom_type/_custom_type.py`

 * *Files identical despite different names*

### Comparing `d42-1.7.0/d42.egg-info/PKG-INFO` & `d42-1.7.1/d42.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 Metadata-Version: 2.1
 Name: d42
-Version: 1.7.0
+Version: 1.7.1
 Summary: One package for district42 ecosystem
-Home-page: https://github.com/tsv1/d42
+Home-page: https://github.com/d42-schemas/d42
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
-Project-URL: Docs, https://d42.vedro.io
-Project-URL: GitHub, https://github.com/tsv1/d42
+Project-URL: Docs, https://d42.sh
+Project-URL: GitHub, https://github.com/d42-schemas/d42
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: district42<1.8,>=1.7
+Requires-Dist: blahblah<1.8,>=1.7
+Requires-Dist: valera<1.8,>=1.7
+Requires-Dist: revolt<1.8,>=1.7
+Requires-Dist: niltype<2.0,>=0.3
+Requires-Dist: th<1.0,>=0.3
 
 # d42
 
 [![PyPI](https://img.shields.io/pypi/v/d42.svg?style=flat-square)](https://pypi.python.org/pypi/d42/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/d42?style=flat-square)](https://pypi.python.org/pypi/d42/)
 [![Python Version](https://img.shields.io/pypi/pyversions/d42.svg?style=flat-square)](https://pypi.python.org/pypi/d42/)
 
-`d42` package offers several tools to define, generate, validate, and substitute data based on models defined using the district42 data description language.
+The `d42` package is a comprehensive toolkit for data modeling, which includes functionalities for definition, generation, validation, and substitution of data models using a robust data description language.
 
 ## Installation
 
 ```shell
 $ pip3 install d42
 ```
 
-## Components
-
-The [d42](https://pypi.org/project/d42/) package comprises the following components:
-- [district42](https://pypi.org/project/district42/) — a data description language for defining data models
-- [blahblah](https://pypi.org/project/blahblah/) — a fake data generator tailored for the district42 schema
-- [valera](https://pypi.org/project/valera/) — a validator designed for the district42 schema
-- [revolt](https://pypi.org/project/revolt/) — a value substitutor compatible with the district42 schema
-
-## Usage
+## Usage Example
 
 ```python
 from d42 import schema, fake, validate_or_fail
 
-# Define a schema with a string "banana"
+# Define a schema for a string containing "banana"
 sch = schema.str("banana")
 
 # Generate a fake value based on the schema and validate it
 assert validate_or_fail(sch, fake(sch))
 ```
 
-For a more comprehensive guide and detailed information, check out the [official documentation](https://d42.vedro.io/).
+## Documentation
+
+For detailed documentation, visit the [official d42 documentation](https://d42.sh).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `d42-1.7.0/setup.cfg` & `d42-1.7.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.7.0
+current_version = 1.7.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `d42-1.7.0/setup.py` & `d42-1.7.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,33 +9,34 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="d42",
-    version="1.7.0",
+    version="1.7.1",
     description="One package for district42 ecosystem",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
-    url="https://github.com/tsv1/d42",
+    url="https://github.com/d42-schemas/d42",
     project_urls={
-        "Docs": "https://d42.vedro.io",
-        "GitHub": "https://github.com/tsv1/d42",
+        "Docs": "https://d42.sh",
+        "GitHub": "https://github.com/d42-schemas/d42",
     },
     license="Apache-2.0",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"d42": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
     ],
 )
```

### Comparing `d42-1.7.0/tests/test_custom_type.py` & `d42-1.7.1/tests/test_custom_type.py`

 * *Files identical despite different names*

### Comparing `d42-1.7.0/tests/test_imports.py` & `d42-1.7.1/tests/test_imports.py`

 * *Files identical despite different names*

