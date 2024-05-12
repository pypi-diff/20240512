# Comparing `tmp/omymodels-0.8.4.tar.gz` & `tmp/omymodels-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omymodels-0.8.4.tar", last modified: Sun Jul 18 14:31:07 2021, max compression
+gzip compressed data, was "omymodels-0.9.0.tar", last modified: Sat Aug 14 22:26:50 2021, max compression
```

## Comparing `omymodels-0.8.4.tar` & `omymodels-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0     1093 2021-03-07 15:01:11.136907 omymodels-0.8.4/LICENSE
--rw-r--r--   0        0        0    10965 2021-07-18 14:31:06.510336 omymodels-0.8.4/docs/README.rst
--rw-r--r--   0        0        0       73 2021-07-18 08:31:53.169445 omymodels-0.8.4/omymodels/__init__.py
--rw-r--r--   0        0        0     2125 2021-07-18 08:31:56.204996 omymodels-0.8.4/omymodels/cli.py
--rw-r--r--   0        0        0     5053 2021-07-18 14:23:47.451216 omymodels-0.8.4/omymodels/common.py
--rw-r--r--   0        0        0     5971 2021-07-18 08:31:56.208179 omymodels-0.8.4/omymodels/dataclass/core.py
--rw-r--r--   0        0        0       26 2021-07-18 08:31:56.209773 omymodels-0.8.4/omymodels/dataclass/dataclass.jinja2
--rw-r--r--   0        0        0      632 2021-07-18 08:31:56.211797 omymodels-0.8.4/omymodels/dataclass/templates.py
--rw-r--r--   0        0        0      674 2021-07-18 08:31:56.213453 omymodels-0.8.4/omymodels/dataclass/types.py
--rw-r--r--   0        0        0      277 2021-07-18 14:23:47.237657 omymodels-0.8.4/omymodels/errors.py
--rw-r--r--   0        0        0     4738 2021-07-18 14:30:44.403175 omymodels-0.8.4/omymodels/gino/core.py
--rw-r--r--   0        0        0       48 2021-07-18 08:31:56.216318 omymodels-0.8.4/omymodels/gino/gino.jinja2
--rw-r--r--   0        0        0     1386 2021-07-18 08:31:56.218021 omymodels-0.8.4/omymodels/gino/templates.py
--rw-r--r--   0        0        0      764 2021-07-18 12:56:35.999483 omymodels-0.8.4/omymodels/gino/types.py
--rw-r--r--   0        0        0     3362 2021-07-18 14:23:47.406195 omymodels-0.8.4/omymodels/logic.py
--rw-r--r--   0        0        0     1187 2021-07-18 08:31:56.220806 omymodels-0.8.4/omymodels/meta_model.py
--rw-r--r--   0        0        0     5403 2021-07-18 08:31:56.222199 omymodels-0.8.4/omymodels/pydantic/core.py
--rw-r--r--   0        0        0       26 2021-07-18 08:31:56.223033 omymodels-0.8.4/omymodels/pydantic/pydantic.jinja2
--rw-r--r--   0        0        0      601 2021-07-18 08:31:56.224568 omymodels-0.8.4/omymodels/pydantic/templates.py
--rw-r--r--   0        0        0      648 2021-07-18 08:31:56.226385 omymodels-0.8.4/omymodels/pydantic/types.py
--rw-r--r--   0        0        0      350 2021-05-23 09:54:52.857494 omymodels-0.8.4/omymodels/sqlalchemy/Untitled.code-workspace
--rw-r--r--   0        0        0     4497 2021-07-18 14:29:52.121772 omymodels-0.8.4/omymodels/sqlalchemy/core.py
--rw-r--r--   0        0        0      133 2021-07-18 08:31:56.229571 omymodels-0.8.4/omymodels/sqlalchemy/sqlalchemy.jinja2
--rw-r--r--   0        0        0     1490 2021-07-18 14:02:10.488891 omymodels-0.8.4/omymodels/sqlalchemy/templates.py
--rw-r--r--   0        0        0      877 2021-07-18 08:31:56.232424 omymodels-0.8.4/omymodels/sqlalchemy/types.py
--rw-r--r--   0        0        0    10408 2021-07-18 08:31:56.234055 omymodels-0.8.4/omymodels/sqlalchemy_core/core.py
--rw-r--r--   0        0        0      121 2021-07-18 08:31:56.235750 omymodels-0.8.4/omymodels/sqlalchemy_core/sqlalchemy_core.jinja2
--rw-r--r--   0        0        0     1234 2021-07-18 08:31:56.237422 omymodels-0.8.4/omymodels/sqlalchemy_core/templates.py
--rw-r--r--   0        0        0      877 2021-07-18 08:31:56.238719 omymodels-0.8.4/omymodels/sqlalchemy_core/types.py
--rw-r--r--   0        0        0      445 2021-07-18 14:23:47.340582 omymodels-0.8.4/omymodels/test.py
--rw-r--r--   0        0        0     3419 2021-07-18 14:30:37.532697 omymodels-0.8.4/omymodels/types.py
--rw-r--r--   0        0        0     1769 2021-07-18 08:31:56.240700 omymodels-0.8.4/omymodels/utils.py
--rw-r--r--   0        0        0     1142 2021-07-18 14:31:05.335686 omymodels-0.8.4/pyproject.toml
--rw-r--r--   0        0        0    12498 2021-07-18 14:31:07.428557 omymodels-0.8.4/setup.py
--rw-r--r--   0        0        0    12208 2021-07-18 14:31:07.429622 omymodels-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2021-03-07 15:01:11.136907 omymodels-0.9.0/LICENSE
+-rw-r--r--   0        0        0    11869 2021-08-14 22:26:50.103695 omymodels-0.9.0/docs/README.rst
+-rw-r--r--   0        0        0      138 2021-08-14 17:43:21.743345 omymodels-0.9.0/omymodels/__init__.py
+-rw-r--r--   0        0        0     2125 2021-07-18 08:31:56.204996 omymodels-0.9.0/omymodels/cli.py
+-rw-r--r--   0        0        0     5147 2021-08-14 22:10:55.625588 omymodels-0.9.0/omymodels/common.py
+-rw-r--r--   0        0        0     1918 2021-08-14 22:26:36.756317 omymodels-0.9.0/omymodels/converter.py
+-rw-r--r--   0        0        0     5998 2021-08-14 21:35:43.727195 omymodels-0.9.0/omymodels/dataclass/core.py
+-rw-r--r--   0        0        0       26 2021-07-18 08:31:56.209773 omymodels-0.9.0/omymodels/dataclass/dataclass.jinja2
+-rw-r--r--   0        0        0      632 2021-07-18 08:31:56.211797 omymodels-0.9.0/omymodels/dataclass/templates.py
+-rw-r--r--   0        0        0      685 2021-08-14 22:10:55.403085 omymodels-0.9.0/omymodels/dataclass/types.py
+-rw-r--r--   0        0        0      277 2021-08-14 17:45:50.917537 omymodels-0.9.0/omymodels/errors.py
+-rw-r--r--   0        0        0     4765 2021-08-14 21:35:57.027134 omymodels-0.9.0/omymodels/gino/core.py
+-rw-r--r--   0        0        0       48 2021-07-18 08:31:56.216318 omymodels-0.9.0/omymodels/gino/gino.jinja2
+-rw-r--r--   0        0        0     1386 2021-07-18 08:31:56.218021 omymodels-0.9.0/omymodels/gino/templates.py
+-rw-r--r--   0        0        0      744 2021-08-14 22:10:55.412863 omymodels-0.9.0/omymodels/gino/types.py
+-rw-r--r--   0        0        0     3362 2021-07-24 22:12:18.556579 omymodels-0.9.0/omymodels/logic.py
+-rw-r--r--   0        0        0     1192 2021-08-14 18:27:40.371945 omymodels-0.9.0/omymodels/meta_model.py
+-rw-r--r--   0        0        0     5430 2021-08-14 21:36:14.054548 omymodels-0.9.0/omymodels/pydantic/core.py
+-rw-r--r--   0        0        0       26 2021-07-18 08:31:56.223033 omymodels-0.9.0/omymodels/pydantic/pydantic.jinja2
+-rw-r--r--   0        0        0      601 2021-07-18 08:31:56.224568 omymodels-0.9.0/omymodels/pydantic/templates.py
+-rw-r--r--   0        0        0      706 2021-08-14 22:20:26.246100 omymodels-0.9.0/omymodels/pydantic/types.py
+-rw-r--r--   0        0        0     4524 2021-08-14 21:35:24.815202 omymodels-0.9.0/omymodels/sqlalchemy/core.py
+-rw-r--r--   0        0        0      133 2021-07-18 08:31:56.229571 omymodels-0.9.0/omymodels/sqlalchemy/sqlalchemy.jinja2
+-rw-r--r--   0        0        0     1490 2021-07-18 14:02:10.488891 omymodels-0.9.0/omymodels/sqlalchemy/templates.py
+-rw-r--r--   0        0        0      799 2021-08-14 22:18:03.570853 omymodels-0.9.0/omymodels/sqlalchemy/types.py
+-rw-r--r--   0        0        0    10372 2021-08-14 22:10:55.871304 omymodels-0.9.0/omymodels/sqlalchemy_core/core.py
+-rw-r--r--   0        0        0      121 2021-07-18 08:31:56.235750 omymodels-0.9.0/omymodels/sqlalchemy_core/sqlalchemy_core.jinja2
+-rw-r--r--   0        0        0     1234 2021-07-18 08:31:56.237422 omymodels-0.9.0/omymodels/sqlalchemy_core/templates.py
+-rw-r--r--   0        0        0      420 2021-08-14 17:45:03.855545 omymodels-0.9.0/omymodels/test.py
+-rw-r--r--   0        0        0     4321 2021-08-14 22:26:13.696401 omymodels-0.9.0/omymodels/types.py
+-rw-r--r--   0        0        0     1731 2021-08-14 18:31:26.014908 omymodels-0.9.0/omymodels/utils.py
+-rw-r--r--   0        0        0     1176 2021-08-14 22:24:52.848354 omymodels-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    13483 2021-08-14 22:26:51.023150 omymodels-0.9.0/setup.py
+-rw-r--r--   0        0        0    13146 2021-08-14 22:26:51.024453 omymodels-0.9.0/PKG-INFO
```

### Comparing `omymodels-0.8.4/LICENSE` & `omymodels-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omymodels-0.8.4/docs/README.rst` & `omymodels-0.9.0/docs/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -289,14 +289,61 @@
 Please describe issue that you want to solve and open the PR, I will review it as soon as possible.
 
 Any questions? Ping me in Telegram: https://t.me/xnuinside
 
 Changelog
 ---------
 
+**v0.9.0**
+Features:
+
+
+#. Added beta models converter from one type of models to another.
+   To use models convertor:
+
+.. code-block:: python
+
+   from omymodels import convert_models
+
+
+   models_from = """
+
+   class MaterialType(str, Enum):
+
+       article = "article"
+       video = "video"
+
+
+   @dataclass
+   class Material:
+
+       id: int
+       title: str
+       description: str
+       link: str
+       type: MaterialType
+       additional_properties: Union[dict, list]
+       created_at: datetime.datetime
+       updated_at: datetime.datetime
+
+   """
+
+   result = convert_models(models_from, models_type="gino")
+   print(result)
+
+where ``models_type`` - type of models that you want to get as a result
+
+
+#. Now if O!MyModels does not know how to convert type - he just leave it as is.
+
+Fixes:
+
+
+#. In Dataclass & Pydantic generators now Decimals & Floats converted to float (previously was int).
+
 **v0.8.4**
 
 
 #. Now if tables was not found in input DDL - models generator raise NoTable error. if you want to have still silent exit if no tables, please use flag: exit_silent
 
 **v0.8.3**
```

### Comparing `omymodels-0.8.4/omymodels/cli.py` & `omymodels-0.9.0/omymodels/cli.py`

 * *Files identical despite different names*

### Comparing `omymodels-0.8.4/omymodels/common.py` & `omymodels-0.9.0/omymodels/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,37 +80,42 @@
     folder = os.path.dirname(dump_path)
     if folder:
         os.makedirs(folder, exist_ok=True)
     with open(dump_path, "w+") as f:
         f.write(models)
 
 
-def generate_models_file(
-    data: Dict[str, List],
-    singular: bool = False,
-    exceptions: Optional[List] = None,
-    models_type: str = "gino",
-    schema_global: bool = True,
-    defaults_off: Optional[bool] = False,
-) -> str:
-    """ method to prepare full file with all Models &  """
-    models_str = ""
+def get_generator_by_type(models_type: str):
     models = {
         "gino": g,
         "pydantic": p,
         "dataclass": d,
         "sqlalchemy": s,
         "sqlalchemy_core": sc,
     }
     model = models.get(models_type)
     if not model:
         raise ValueError(
             f"Unsupported models type {models_type}. Possible variants: {models.keys()}"
         )
-    model_generator = getattr(model, "ModelGenerator")()
+    return getattr(model, "ModelGenerator")()
+
+
+def generate_models_file(
+    data: Dict[str, List],
+    singular: bool = False,
+    exceptions: Optional[List] = None,
+    models_type: str = "gino",
+    schema_global: bool = True,
+    defaults_off: Optional[bool] = False,
+) -> str:
+    """ method to prepare full file with all Models &  """
+    models_str = ""
+    model_generator = get_generator_by_type(models_type)
+
     for _type in data["types"]:
         models_str += model_generator.generate_type(_type, singular, exceptions)
     for table in data["tables"]:
         models_str += model_generator.generate_model(
             table,
             singular,
             exceptions,
```

### Comparing `omymodels-0.8.4/omymodels/dataclass/core.py` & `omymodels-0.9.0/omymodels/dataclass/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, List, Dict
 from omymodels.dataclass import templates as dt
 from omymodels.utils import create_class_name, enum_number_name_list
-from omymodels.dataclass.types import types_mapping, datetime_types
+from omymodels.dataclass.types import types_mapping
+from omymodels.types import datetime_types
 
 
 class ModelGenerator:
     def __init__(self):
 
         self.types_for_import = ["Union"]
         self.datetime_import = False
```

### Comparing `omymodels-0.8.4/omymodels/dataclass/templates.py` & `omymodels-0.9.0/omymodels/dataclass/templates.py`

 * *Files identical despite different names*

### Comparing `omymodels-0.8.4/omymodels/gino/core.py` & `omymodels-0.9.0/omymodels/gino/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional, List, Dict
 import omymodels.gino.templates as gt
-from omymodels.gino.types import types_mapping, datetime_types
+from omymodels.gino.types import types_mapping
+from omymodels.types import datetime_types
 from omymodels.utils import create_class_name, enum_number_name_list
 from omymodels import logic
 
 
 class ModelGenerator:
     def __init__(self):
         self.state = set()
```

### Comparing `omymodels-0.8.4/omymodels/gino/templates.py` & `omymodels-0.9.0/omymodels/gino/templates.py`

 * *Files identical despite different names*

### Comparing `omymodels-0.8.4/omymodels/logic.py` & `omymodels-0.9.0/omymodels/logic.py`

 * *Files identical despite different names*

### Comparing `omymodels-0.8.4/omymodels/meta_model.py` & `omymodels-0.9.0/omymodels/meta_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 class TableMeta(BaseModel):
     name: str = Field(alias="table_name")
     table_schema: Optional[str] = Field(alias="schema")
     columns: List[Column]
     indexes: Optional[List[dict]] = Field(alias="index")
-    alter: Optional[dict]
+    alter: Optional[dict] = {}
     checks: Optional[List[dict]]
     properties: Optional[TableProperties]
     primary_key: List
 
     class Config:
         """ pydantic class config """
```

### Comparing `omymodels-0.8.4/omymodels/pydantic/core.py` & `omymodels-0.9.0/omymodels/pydantic/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, List, Dict
 from omymodels.pydantic import templates as pt
 from omymodels.utils import create_class_name, enum_number_name_list
-from omymodels.pydantic.types import types_mapping, datetime_types
+from omymodels.pydantic.types import types_mapping
+from omymodels.types import datetime_types
 
 
 class ModelGenerator:
     def __init__(self):
 
         self.imports = set([pt.base_model])
         self.types_for_import = ["Json"]
```

### Comparing `omymodels-0.8.4/omymodels/pydantic/templates.py` & `omymodels-0.9.0/omymodels/pydantic/templates.py`

 * *Files identical despite different names*

### Comparing `omymodels-0.8.4/omymodels/sqlalchemy/core.py` & `omymodels-0.9.0/omymodels/sqlalchemy/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional, List, Dict
 import omymodels.sqlalchemy.templates as st
-from omymodels.sqlalchemy.types import types_mapping, datetime_types
+from omymodels.sqlalchemy.types import types_mapping
+from omymodels.types import datetime_types
 from omymodels.utils import create_class_name, enum_number_name_list
 from omymodels import logic
 
 
 class ModelGenerator:
     def __init__(self):
         self.state = set()
```

### Comparing `omymodels-0.8.4/omymodels/sqlalchemy/templates.py` & `omymodels-0.9.0/omymodels/sqlalchemy/templates.py`

 * *Files identical despite different names*

### Comparing `omymodels-0.8.4/omymodels/sqlalchemy_core/core.py` & `omymodels-0.9.0/omymodels/sqlalchemy_core/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from typing import Optional, List, Dict
 import omymodels.sqlalchemy_core.templates as st
-from omymodels.sqlalchemy_core.types import (
-    types_mapping,
-    postgresql_dialect,
-    datetime_types,
-)
-from omymodels.utils import create_class_name, type_not_found, enum_number_name_list
+from omymodels.sqlalchemy.types import types_mapping, postgresql_dialect
+from omymodels.types import datetime_types
+
+from omymodels.utils import create_class_name, enum_number_name_list
 from omymodels.meta_model import Column
 
 
 class ModelGenerator:
     def __init__(self):
         self.state = set()
         self.postgresql_dialect_cols = set()
@@ -19,30 +17,30 @@
         self.custom_types = {}
 
     def add_custom_type(self, column_data_type: str, column_type: str) -> str:
         column_type = self.custom_types.get(column_data_type, column_type)
         if isinstance(column_type, tuple):
             column_data_type = column_type[1]
             column_type = column_type[0]
-        if column_type != type_not_found:
+        if column_type is not None:
             column_type = f"{column_type}({column_data_type})"
             self.no_need_par = True
         return column_type
 
     def prepare_column_type(self, column_data: Dict) -> str:
         """ extract and map column type """
         self.no_need_par = False
-        column_type = type_not_found
+        column_type = None
         if "." in column_data.type:
             column_data_type = column_data.type.split(".")[1]
         else:
             column_data_type = column_data.type.lower().split("[")[0]
         if self.custom_types:
             column_type = self.add_custom_type(column_data_type, column_type)
-        if column_type == type_not_found:
+        if column_type is None:
             column_type = types_mapping.get(column_data_type, column_type)
         if column_type in postgresql_dialect:
             self.postgresql_dialect_cols.add(column_type)
         if column_type == "UUID":
             self.no_need_par = True
         if column_data.size:
             column_type = self.add_size_to_column_type(column_data.size)
```

### Comparing `omymodels-0.8.4/omymodels/sqlalchemy_core/templates.py` & `omymodels-0.9.0/omymodels/sqlalchemy_core/templates.py`

 * *Files identical despite different names*

### Comparing `omymodels-0.8.4/omymodels/utils.py` & `omymodels-0.9.0/omymodels/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from typing import Optional, List, Text
 
-type_not_found = "OMM_UNMAPPED_TYPE"
-
 
 def get_singular_name(table_name: Text, exceptions: Optional[List] = None) -> Text:
     endings = {"ies": lambda x: x[:-3] + "y", "es": lambda x: x[:-1]}
     if not exceptions:
         exceptions = []
     exception_endings = [x for x in exceptions if table_name.endswith(x)]
     model_name = None
```

### Comparing `omymodels-0.8.4/pyproject.toml` & `omymodels-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "omymodels"
-version = "0.8.4"
-description = "O! My Models (omymodels) is a library to generate Python Models for SQLAlchemy (ORM & Core), GinoORM, Pydantic, Pydal tables & Python Dataclasses from SQL DDL. "
+version = "0.9.0"
+description = "O! My Models (omymodels) is a library to generate Python Models for SQLAlchemy (ORM & Core), GinoORM, Pydantic, Pydal tables & Python Dataclasses from SQL DDL. And convert one models to another."
 authors = ["Iuliia Volkova <xnuinside@gmail.com>"]
 license = "MIT"
 readme = "docs/README.rst"
 homepage = "https://github.com/xnuinside/omymodels"
 repository = "https://github.com/xnuinside/omymodels"
 classifiers = [
     "Programming Language :: PL/SQL",
```

### Comparing `omymodels-0.8.4/setup.py` & `omymodels-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,17 +19,17 @@
  'simple-ddl-parser==0.16.0']
 
 entry_points = \
 {'console_scripts': ['omm = omymodels.cli:main']}
 
 setup_kwargs = {
     'name': 'omymodels',
-    'version': '0.8.4',
-    'description': 'O! My Models (omymodels) is a library to generate Python Models for SQLAlchemy (ORM & Core), GinoORM, Pydantic, Pydal tables & Python Dataclasses from SQL DDL. ',
-    'long_description': '\nO! My Models\n------------\n\n\n.. image:: https://img.shields.io/pypi/v/omymodels\n   :target: https://img.shields.io/pypi/v/omymodels\n   :alt: badge1\n \n.. image:: https://img.shields.io/pypi/l/omymodels\n   :target: https://img.shields.io/pypi/l/omymodels\n   :alt: badge2\n \n.. image:: https://img.shields.io/pypi/pyversions/omymodels\n   :target: https://img.shields.io/pypi/pyversions/omymodels\n   :alt: badge3\n\n.. image:: https://github.com/xnuinside/omymodels/actions/workflows/main.yml/badge.svg\n   :target: https://github.com/xnuinside/omymodels/actions/workflows/main.yml/badge.svg\n   :alt: workflow\n\n\nBig example you can find in example/ folder on the github: https://github.com/xnuinside/omymodels/tree/main/example\n\nO! My Models (omymodels) is a library to generate from SQL DDL Python Models for SQLAlchemy (models), SQLAlchemy Core (tables), GinoORM (I hope to add several more ORMs in future), Pydantic classes and Python Dataclasses (dataclasses module).\n\nBy default method **create_models** generate GinoORM models, to get Pydantic models output use the argument ``models_type=\'pydantic\'`` (\'sqlalchemy\' for SQLAlchemy models; \'dataclass\' for Dataclasses; \'sqlalchemy_core\' for Sqlalchemy Core Tables).\n\nA lot of examples in tests/ - https://github.com/xnuinside/omymodels/tree/main/tests.\n\nFor example,\n\n.. code-block:: python\n\n   from omymodels import create_models\n\n\n   ddl = """\n   CREATE table user_history (\n        runid                 decimal(21) null\n       ,job_id                decimal(21)  null\n       ,id                    varchar(100) not null\n       ,user              varchar(100) not null\n       ,status                varchar(10) not null\n       ,event_time            timestamp not null default now()\n       ,comment           varchar(1000) not null default \'none\'\n       ) ;\n\n\n   """\n   result = create_models(ddl, models_type=\'pydantic\')[\'code\']\n\n    # and output will be:    \n   import datetime\n   from typing import Optional\n   from pydantic import BaseModel\n\n\n   class UserHistory(BaseModel):\n\n       runid: Optional[int]\n       job_id: Optional[int]\n       id: str\n       user: str\n       status: str\n       event_time: datetime.datetime\n       comment: str\n\nTo generate Dataclasses from DDL use argument ``models_type=\'dataclass\'``\n\nfor example:\n\n.. code-block:: python\n\n       #  (same DDL as in Pydantic sample)\n       result = create_models(ddl, schema_global=False, models_type=\'dataclass\')[\'code\']\n\n       # and result will be: \n       import datetime\n       from dataclasses import dataclass\n\n\n       @dataclass\n       class UserHistory:\n\n           id: str\n           user: str\n           status: str\n           runid: int = None\n           job_id: int = None\n           event_time: datetime.datetime = datetime.datetime.now()\n           comment: str = \'none\'\n\nGinoORM example. If you provide an input like:\n\n.. code-block:: sql\n\n\n   CREATE TABLE "users" (\n     "id" SERIAL PRIMARY KEY,\n     "name" varchar,\n     "created_at" timestamp,\n     "updated_at" timestamp,\n     "country_code" int,\n     "default_language" int\n   );\n\n   CREATE TABLE "languages" (\n     "id" int PRIMARY KEY,\n     "code" varchar(2) NOT NULL,\n     "name" varchar NOT NULL\n   );\n\nand you will get output:\n\n.. code-block:: python\n\n\n       from gino import Gino\n\n\n       db = Gino()\n\n\n       class Users(db.Model):\n\n           __tablename__ = \'users\'\n\n           id = db.Column(db.Integer(), autoincrement=True, primary_key=True)\n           name = db.Column(db.String())\n           created_at = db.Column(db.TIMESTAMP())\n           updated_at = db.Column(db.TIMESTAMP())\n           country_code = db.Column(db.Integer())\n           default_language = db.Column(db.Integer())\n\n\n       class Languages(db.Model):\n\n           __tablename__ = \'languages\'\n\n           id = db.Column(db.Integer(), primary_key=True)\n           code = db.Column(db.String(2))\n           name = db.Column(db.String())\n\nHow to install\n^^^^^^^^^^^^^^\n\n.. code-block:: bash\n\n\n       pip install omymodels\n\nHow to use\n^^^^^^^^^^\n\nFrom cli\n~~~~~~~~\n\n.. code-block:: bash\n\n\n       omm path/to/your.ddl\n\n       # for example\n       omm tests/test_two_tables.sql\n\nYou can define target path where to save models with **-t**\\ , **--target** flag:\n\n.. code-block:: bash\n\n\n       # for example\n       omm tests/test_two_tables.sql -t test_path/test_models.py\n\nIf you want generate the Pydantic or Dataclasses models - just use flag **-m** or **--models_type=\'pydantic\'** / **--models_type=\'dataclass\'**\n\n.. code-block:: bash\n\n\n       omm /path/to/your.ddl -m dataclass\n\n       # or \n       omm /path/to/your.ddl --models_type pydantic\n\nSmall library is used for parse DDL- https://github.com/xnuinside/simple-ddl-parser.\n\nWhat to do if types not supported in O! My Models and you cannot wait until PR will be approved\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nFirst of all, to parse types correct from DDL to models - they must be in types mypping, for Gino it exitst in this file:\n\nomymodels/gino/types.py  **types_mapping**\n\nIf you need to use fast type that not exist in mapping - just do a path before call code with types_mapping.update()\n\nfor example:\n\n.. code-block:: python\n\n\n       from omymodels.gino import types\n       from omymodels import create_models\n\n       types.types_mapping.update({\'your_type_from_ddl\': \'db.TypeInGino\'})\n\n       ddl = "YOUR DDL with your custom your_type_from_ddl"\n\n       models = create_models(ddl)\n\n       #### And similar for Pydantic types\n\n       from omymodels.pydantic import types  types_mapping\n       from omymodels import create_models\n\n       types.types_mapping.update({\'your_type_from_ddl\': \'db.TypeInGino\'})\n\n       ddl = "YOUR DDL with your custom your_type_from_ddl"\n\n       models = create_models(ddl, models_type=\'pydantic\')\n\nSchema defenition\n^^^^^^^^^^^^^^^^^\n\nThere is 2 ways how to define schema in Models:\n\n1) Globally in Gino() class and it will be like this:\n\n.. code-block:: python\n\n\n       from gino import Gino\n       db = Gino(schema="schema_name")\n\nAnd this is a default way for put schema during generation - it takes first schema in tables and use it. \n\n2) But if you work with tables in different schemas, you need to define schema in each model in table_args. O!MyModels can do this also. Just use flag ``--no-global-schema`` if you use cli or put argument \'schema_global=False\' to create_models() function if you use library from code. Like this:\n\n.. code-block:: python\n\n\n       ddl = """\n       CREATE TABLE "prefix--schema-name"."table" (\n       _id uuid PRIMARY KEY,\n       one_more_id int\n       );\n           create unique index table_pk on "prefix--schema-name"."table" (one_more_id) ;\n           create index table_ix2 on "prefix--schema-name"."table" (_id) ;\n       """\n       result = create_models(ddl, schema_global=False)\n\nAnd result will be this:\n\n.. code-block:: python\n\n\n       from sqlalchemy.dialects.postgresql import UUID\n       from sqlalchemy.schema import UniqueConstraint\n       from sqlalchemy import Index\n       from gino import Gino\n\n       db = Gino()\n\n\n       class Table(db.Model):\n\n           __tablename__ = \'table\'\n\n           _id = db.Column(UUID, primary_key=True)\n           one_more_id = db.Column(db.Integer())\n\n           __table_args__ = (\n\n           UniqueConstraint(one_more_id, name=\'table_pk\'),\n           Index(\'table_ix2\', _id),\n           dict(schema="prefix--schema-name")\n                   )\n\nTODO in next releases\n---------------------\n\n\n#. Add Sequence generation in Models (Gino, SQLAlchemy)\n#. Generate Tortoise ORM models (https://tortoise-orm.readthedocs.io/en/latest/)\n#. Convert SQLAlchemy models to DjangoORM, Pydantic, SQLAlchemy Tables, Dataclasses (?)\n\nHow to contribute\n-----------------\n\nPlease describe issue that you want to solve and open the PR, I will review it as soon as possible.\n\nAny questions? Ping me in Telegram: https://t.me/xnuinside\n\nChangelog\n---------\n\n**v0.8.4**\n\n\n#. Now if tables was not found in input DDL - models generator raise NoTable error. if you want to have still silent exit if no tables, please use flag: exit_silent\n\n**v0.8.3**\n\n\n#. Added fundamental concept of TableMetaModel - class that unifies metadata parsed from different classes/ORM models types/DDLs to one standard to allow easy way convert one models to another\n   in next releases it will be used for converter from one type of models to another.\n#. Fixed issue: https://github.com/xnuinside/omymodels/issues/18 "NOW() not recognized as now()"\n#. Fixed issue: https://github.com/xnuinside/omymodels/issues/19 "Default value of now() always returns same time, use field for dataclass"\n\n**v0.8.1**\n\n\n#. Parser version is updated (fixed several issues with generation)\n#. Fixed issue with Unique Constraint after schema in SQLAlchemy Core\n\n**v0.8.0**\n\n\n#. Fix --defaults-off flag in cli\n#. Added support for SQLAlchemy Core Tables generating\n#. Added examples folder in github ``omymodels/example``\n#. Fix issue with ForeignKey in SQLAlchemy\n\n**v0.7.0**\n\n\n#. Added generation for SQLAlchemy models (defaults from DDLs are setting up as \'server_default\')\n#. Added defaults for Pydantic models\n#. Added flag to generate Pydantic & Dataclass models WITHOUT defaults ``defaults_off=True`` (by default it is False). And cli flag --defaults-off\n#. Fixed issue with Enum types with lower case names in DDLs\n#. Fixed several issues with Dataclass generation (default with datetime & Enums)\n#. \'"\' do not remove from defaults now\n\n**v0.6.0**\n\n\n#. O!MyModels now also can generate python Dataclass from DDL. Use argument models_type=\'dataclass\' or if you use the cli flag --models_type dataclass or -m dataclass\n#. Added ForeignKey generation to GinoORM Models, added support for ondelete and onupdate\n\n**v0.5.0**\n\n\n#. Added Enums/IntEnums types for Gino & Pydantic\n#. Added UUID type\n#. Added key ``schema_global`` in create_models method (by default schema_global = True). \n   If you set schema_global=False schema if it exists in ddl will be defined for each table (model) in table args.\n   This way you can have differen schemas per model (table). By default schema_global=True - this mean for all \n   table only one schema and it is defined in ``db = Gino(schema="prefix--schema-name")``.\n#. If column is a primary key (primary_key=True) nullable argument not showed, because primary keys always are not null.\n#. To cli was added flag \'--no-global-schema\' to set schema in table_args.\n\n**v0.4.1**\n\n\n#. Added correct work with table names contains multiple \'-\'\n\n**v0.4.0**\n\n\n#. Added generation for Pydantic models from ddl\n#. Main method create_gino_models renamed to create_models\n\n**v0.3.0**\n\n\n#. Generated Index for \'index\' statement in **table_args** (not unique constrait as previously)\n#. Fix issue with column size as tuple (4,2)\n\n**v0.2.0**\n\n\n#. Valid generating columns in models: autoincrement, default, type, arrays, unique, primary key and etc.\n#. Added creating **table_args** for indexes\n',
+    'version': '0.9.0',
+    'description': 'O! My Models (omymodels) is a library to generate Python Models for SQLAlchemy (ORM & Core), GinoORM, Pydantic, Pydal tables & Python Dataclasses from SQL DDL. And convert one models to another.',
+    'long_description': '\nO! My Models\n------------\n\n\n.. image:: https://img.shields.io/pypi/v/omymodels\n   :target: https://img.shields.io/pypi/v/omymodels\n   :alt: badge1\n \n.. image:: https://img.shields.io/pypi/l/omymodels\n   :target: https://img.shields.io/pypi/l/omymodels\n   :alt: badge2\n \n.. image:: https://img.shields.io/pypi/pyversions/omymodels\n   :target: https://img.shields.io/pypi/pyversions/omymodels\n   :alt: badge3\n\n.. image:: https://github.com/xnuinside/omymodels/actions/workflows/main.yml/badge.svg\n   :target: https://github.com/xnuinside/omymodels/actions/workflows/main.yml/badge.svg\n   :alt: workflow\n\n\nBig example you can find in example/ folder on the github: https://github.com/xnuinside/omymodels/tree/main/example\n\nO! My Models (omymodels) is a library to generate from SQL DDL Python Models for SQLAlchemy (models), SQLAlchemy Core (tables), GinoORM (I hope to add several more ORMs in future), Pydantic classes and Python Dataclasses (dataclasses module).\n\nBy default method **create_models** generate GinoORM models, to get Pydantic models output use the argument ``models_type=\'pydantic\'`` (\'sqlalchemy\' for SQLAlchemy models; \'dataclass\' for Dataclasses; \'sqlalchemy_core\' for Sqlalchemy Core Tables).\n\nA lot of examples in tests/ - https://github.com/xnuinside/omymodels/tree/main/tests.\n\nFor example,\n\n.. code-block:: python\n\n   from omymodels import create_models\n\n\n   ddl = """\n   CREATE table user_history (\n        runid                 decimal(21) null\n       ,job_id                decimal(21)  null\n       ,id                    varchar(100) not null\n       ,user              varchar(100) not null\n       ,status                varchar(10) not null\n       ,event_time            timestamp not null default now()\n       ,comment           varchar(1000) not null default \'none\'\n       ) ;\n\n\n   """\n   result = create_models(ddl, models_type=\'pydantic\')[\'code\']\n\n    # and output will be:    \n   import datetime\n   from typing import Optional\n   from pydantic import BaseModel\n\n\n   class UserHistory(BaseModel):\n\n       runid: Optional[int]\n       job_id: Optional[int]\n       id: str\n       user: str\n       status: str\n       event_time: datetime.datetime\n       comment: str\n\nTo generate Dataclasses from DDL use argument ``models_type=\'dataclass\'``\n\nfor example:\n\n.. code-block:: python\n\n       #  (same DDL as in Pydantic sample)\n       result = create_models(ddl, schema_global=False, models_type=\'dataclass\')[\'code\']\n\n       # and result will be: \n       import datetime\n       from dataclasses import dataclass\n\n\n       @dataclass\n       class UserHistory:\n\n           id: str\n           user: str\n           status: str\n           runid: int = None\n           job_id: int = None\n           event_time: datetime.datetime = datetime.datetime.now()\n           comment: str = \'none\'\n\nGinoORM example. If you provide an input like:\n\n.. code-block:: sql\n\n\n   CREATE TABLE "users" (\n     "id" SERIAL PRIMARY KEY,\n     "name" varchar,\n     "created_at" timestamp,\n     "updated_at" timestamp,\n     "country_code" int,\n     "default_language" int\n   );\n\n   CREATE TABLE "languages" (\n     "id" int PRIMARY KEY,\n     "code" varchar(2) NOT NULL,\n     "name" varchar NOT NULL\n   );\n\nand you will get output:\n\n.. code-block:: python\n\n\n       from gino import Gino\n\n\n       db = Gino()\n\n\n       class Users(db.Model):\n\n           __tablename__ = \'users\'\n\n           id = db.Column(db.Integer(), autoincrement=True, primary_key=True)\n           name = db.Column(db.String())\n           created_at = db.Column(db.TIMESTAMP())\n           updated_at = db.Column(db.TIMESTAMP())\n           country_code = db.Column(db.Integer())\n           default_language = db.Column(db.Integer())\n\n\n       class Languages(db.Model):\n\n           __tablename__ = \'languages\'\n\n           id = db.Column(db.Integer(), primary_key=True)\n           code = db.Column(db.String(2))\n           name = db.Column(db.String())\n\nHow to install\n^^^^^^^^^^^^^^\n\n.. code-block:: bash\n\n\n       pip install omymodels\n\nHow to use\n^^^^^^^^^^\n\nFrom cli\n~~~~~~~~\n\n.. code-block:: bash\n\n\n       omm path/to/your.ddl\n\n       # for example\n       omm tests/test_two_tables.sql\n\nYou can define target path where to save models with **-t**\\ , **--target** flag:\n\n.. code-block:: bash\n\n\n       # for example\n       omm tests/test_two_tables.sql -t test_path/test_models.py\n\nIf you want generate the Pydantic or Dataclasses models - just use flag **-m** or **--models_type=\'pydantic\'** / **--models_type=\'dataclass\'**\n\n.. code-block:: bash\n\n\n       omm /path/to/your.ddl -m dataclass\n\n       # or \n       omm /path/to/your.ddl --models_type pydantic\n\nSmall library is used for parse DDL- https://github.com/xnuinside/simple-ddl-parser.\n\nWhat to do if types not supported in O! My Models and you cannot wait until PR will be approved\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nFirst of all, to parse types correct from DDL to models - they must be in types mypping, for Gino it exitst in this file:\n\nomymodels/gino/types.py  **types_mapping**\n\nIf you need to use fast type that not exist in mapping - just do a path before call code with types_mapping.update()\n\nfor example:\n\n.. code-block:: python\n\n\n       from omymodels.gino import types\n       from omymodels import create_models\n\n       types.types_mapping.update({\'your_type_from_ddl\': \'db.TypeInGino\'})\n\n       ddl = "YOUR DDL with your custom your_type_from_ddl"\n\n       models = create_models(ddl)\n\n       #### And similar for Pydantic types\n\n       from omymodels.pydantic import types  types_mapping\n       from omymodels import create_models\n\n       types.types_mapping.update({\'your_type_from_ddl\': \'db.TypeInGino\'})\n\n       ddl = "YOUR DDL with your custom your_type_from_ddl"\n\n       models = create_models(ddl, models_type=\'pydantic\')\n\nSchema defenition\n^^^^^^^^^^^^^^^^^\n\nThere is 2 ways how to define schema in Models:\n\n1) Globally in Gino() class and it will be like this:\n\n.. code-block:: python\n\n\n       from gino import Gino\n       db = Gino(schema="schema_name")\n\nAnd this is a default way for put schema during generation - it takes first schema in tables and use it. \n\n2) But if you work with tables in different schemas, you need to define schema in each model in table_args. O!MyModels can do this also. Just use flag ``--no-global-schema`` if you use cli or put argument \'schema_global=False\' to create_models() function if you use library from code. Like this:\n\n.. code-block:: python\n\n\n       ddl = """\n       CREATE TABLE "prefix--schema-name"."table" (\n       _id uuid PRIMARY KEY,\n       one_more_id int\n       );\n           create unique index table_pk on "prefix--schema-name"."table" (one_more_id) ;\n           create index table_ix2 on "prefix--schema-name"."table" (_id) ;\n       """\n       result = create_models(ddl, schema_global=False)\n\nAnd result will be this:\n\n.. code-block:: python\n\n\n       from sqlalchemy.dialects.postgresql import UUID\n       from sqlalchemy.schema import UniqueConstraint\n       from sqlalchemy import Index\n       from gino import Gino\n\n       db = Gino()\n\n\n       class Table(db.Model):\n\n           __tablename__ = \'table\'\n\n           _id = db.Column(UUID, primary_key=True)\n           one_more_id = db.Column(db.Integer())\n\n           __table_args__ = (\n\n           UniqueConstraint(one_more_id, name=\'table_pk\'),\n           Index(\'table_ix2\', _id),\n           dict(schema="prefix--schema-name")\n                   )\n\nTODO in next releases\n---------------------\n\n\n#. Add Sequence generation in Models (Gino, SQLAlchemy)\n#. Generate Tortoise ORM models (https://tortoise-orm.readthedocs.io/en/latest/)\n#. Convert SQLAlchemy models to DjangoORM, Pydantic, SQLAlchemy Tables, Dataclasses (?)\n\nHow to contribute\n-----------------\n\nPlease describe issue that you want to solve and open the PR, I will review it as soon as possible.\n\nAny questions? Ping me in Telegram: https://t.me/xnuinside\n\nChangelog\n---------\n\n**v0.9.0**\nFeatures:\n\n\n#. Added beta models converter from one type of models to another.\n   To use models convertor:\n\n.. code-block:: python\n\n   from omymodels import convert_models\n\n\n   models_from = """\n\n   class MaterialType(str, Enum):\n\n       article = "article"\n       video = "video"\n\n\n   @dataclass\n   class Material:\n\n       id: int\n       title: str\n       description: str\n       link: str\n       type: MaterialType\n       additional_properties: Union[dict, list]\n       created_at: datetime.datetime\n       updated_at: datetime.datetime\n\n   """\n\n   result = convert_models(models_from, models_type="gino")\n   print(result)\n\nwhere ``models_type`` - type of models that you want to get as a result\n\n\n#. Now if O!MyModels does not know how to convert type - he just leave it as is.\n\nFixes:\n\n\n#. In Dataclass & Pydantic generators now Decimals & Floats converted to float (previously was int).\n\n**v0.8.4**\n\n\n#. Now if tables was not found in input DDL - models generator raise NoTable error. if you want to have still silent exit if no tables, please use flag: exit_silent\n\n**v0.8.3**\n\n\n#. Added fundamental concept of TableMetaModel - class that unifies metadata parsed from different classes/ORM models types/DDLs to one standard to allow easy way convert one models to another\n   in next releases it will be used for converter from one type of models to another.\n#. Fixed issue: https://github.com/xnuinside/omymodels/issues/18 "NOW() not recognized as now()"\n#. Fixed issue: https://github.com/xnuinside/omymodels/issues/19 "Default value of now() always returns same time, use field for dataclass"\n\n**v0.8.1**\n\n\n#. Parser version is updated (fixed several issues with generation)\n#. Fixed issue with Unique Constraint after schema in SQLAlchemy Core\n\n**v0.8.0**\n\n\n#. Fix --defaults-off flag in cli\n#. Added support for SQLAlchemy Core Tables generating\n#. Added examples folder in github ``omymodels/example``\n#. Fix issue with ForeignKey in SQLAlchemy\n\n**v0.7.0**\n\n\n#. Added generation for SQLAlchemy models (defaults from DDLs are setting up as \'server_default\')\n#. Added defaults for Pydantic models\n#. Added flag to generate Pydantic & Dataclass models WITHOUT defaults ``defaults_off=True`` (by default it is False). And cli flag --defaults-off\n#. Fixed issue with Enum types with lower case names in DDLs\n#. Fixed several issues with Dataclass generation (default with datetime & Enums)\n#. \'"\' do not remove from defaults now\n\n**v0.6.0**\n\n\n#. O!MyModels now also can generate python Dataclass from DDL. Use argument models_type=\'dataclass\' or if you use the cli flag --models_type dataclass or -m dataclass\n#. Added ForeignKey generation to GinoORM Models, added support for ondelete and onupdate\n\n**v0.5.0**\n\n\n#. Added Enums/IntEnums types for Gino & Pydantic\n#. Added UUID type\n#. Added key ``schema_global`` in create_models method (by default schema_global = True). \n   If you set schema_global=False schema if it exists in ddl will be defined for each table (model) in table args.\n   This way you can have differen schemas per model (table). By default schema_global=True - this mean for all \n   table only one schema and it is defined in ``db = Gino(schema="prefix--schema-name")``.\n#. If column is a primary key (primary_key=True) nullable argument not showed, because primary keys always are not null.\n#. To cli was added flag \'--no-global-schema\' to set schema in table_args.\n\n**v0.4.1**\n\n\n#. Added correct work with table names contains multiple \'-\'\n\n**v0.4.0**\n\n\n#. Added generation for Pydantic models from ddl\n#. Main method create_gino_models renamed to create_models\n\n**v0.3.0**\n\n\n#. Generated Index for \'index\' statement in **table_args** (not unique constrait as previously)\n#. Fix issue with column size as tuple (4,2)\n\n**v0.2.0**\n\n\n#. Valid generating columns in models: autoincrement, default, type, arrays, unique, primary key and etc.\n#. Added creating **table_args** for indexes\n',
     'author': 'Iuliia Volkova',
     'author_email': 'xnuinside@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/xnuinside/omymodels',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `omymodels-0.8.4/PKG-INFO` & `omymodels-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: omymodels
-Version: 0.8.4
-Summary: O! My Models (omymodels) is a library to generate Python Models for SQLAlchemy (ORM & Core), GinoORM, Pydantic, Pydal tables & Python Dataclasses from SQL DDL. 
+Version: 0.9.0
+Summary: O! My Models (omymodels) is a library to generate Python Models for SQLAlchemy (ORM & Core), GinoORM, Pydantic, Pydal tables & Python Dataclasses from SQL DDL. And convert one models to another.
 Home-page: https://github.com/xnuinside/omymodels
 License: MIT
 Author: Iuliia Volkova
 Author-email: xnuinside@gmail.com
 Requires-Python: >=3.6.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: PL/SQL
@@ -317,14 +317,61 @@
 Please describe issue that you want to solve and open the PR, I will review it as soon as possible.
 
 Any questions? Ping me in Telegram: https://t.me/xnuinside
 
 Changelog
 ---------
 
+**v0.9.0**
+Features:
+
+
+#. Added beta models converter from one type of models to another.
+   To use models convertor:
+
+.. code-block:: python
+
+   from omymodels import convert_models
+
+
+   models_from = """
+
+   class MaterialType(str, Enum):
+
+       article = "article"
+       video = "video"
+
+
+   @dataclass
+   class Material:
+
+       id: int
+       title: str
+       description: str
+       link: str
+       type: MaterialType
+       additional_properties: Union[dict, list]
+       created_at: datetime.datetime
+       updated_at: datetime.datetime
+
+   """
+
+   result = convert_models(models_from, models_type="gino")
+   print(result)
+
+where ``models_type`` - type of models that you want to get as a result
+
+
+#. Now if O!MyModels does not know how to convert type - he just leave it as is.
+
+Fixes:
+
+
+#. In Dataclass & Pydantic generators now Decimals & Floats converted to float (previously was int).
+
 **v0.8.4**
 
 
 #. Now if tables was not found in input DDL - models generator raise NoTable error. if you want to have still silent exit if no tables, please use flag: exit_silent
 
 **v0.8.3**
```

