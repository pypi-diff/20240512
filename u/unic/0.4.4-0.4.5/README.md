# Comparing `tmp/unic-0.4.4.tar.gz` & `tmp/unic-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unic-0.4.4.tar", max compression
+gzip compressed data, was "unic-0.4.5.tar", max compression
```

## Comparing `unic-0.4.4.tar` & `unic-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.4.4/LICENSE
--rw-r--r--   0        0        0      888 2024-05-03 14:58:45.336312 unic-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2398 2024-05-03 12:41:18.395441 unic-0.4.4/README.md
--rw-r--r--   0        0        0      897 2023-12-11 12:31:51.919297 unic-0.4.4/unic/__init__.py
--rw-r--r--   0        0        0      912 2023-12-11 13:01:08.512829 unic-0.4.4/unic/configs/metirc_system/settings.toml
--rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.4.4/unic/configs/timeunit/settings.toml
--rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.4.4/unic/configs/timezone/settings.toml
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.4/unic/length_unit/metric_system/__init__.py
--rw-r--r--   0        0        0     1128 2024-01-23 12:43:39.352115 unic-0.4.4/unic/length_unit/metric_system/metric_system_model.py
--rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-0.4.4/unic/time_unit/datetime/__init__.py
--rw-r--r--   0        0        0     1914 2024-05-02 14:04:45.039895 unic-0.4.4/unic/time_unit/datetime/datetime_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.4/unic/time_unit/time/__init__.py
--rw-r--r--   0        0        0     1107 2024-01-29 12:03:05.141190 unic-0.4.4/unic/time_unit/time/time_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.4.4/unic/time_unit/unixtime/__init__.py
--rw-r--r--   0        0        0     1310 2024-02-09 13:22:45.717612 unic-0.4.4/unic/time_unit/unixtime/unixtime_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.4/unic/utils/__init__.py
--rw-r--r--   0        0        0      391 2023-10-29 05:14:04.780174 unic-0.4.4/unic/utils/config_parser.py
--rw-r--r--   0        0        0     3040 2024-02-23 14:53:18.111216 unic-0.4.4/unic/utils/validators.py
--rw-r--r--   0        0        0     3097 1970-01-01 00:00:00.000000 unic-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.4.5/LICENSE
+-rw-r--r--   0        0        0      888 2024-05-12 14:10:18.293002 unic-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2398 2024-05-03 12:41:18.395441 unic-0.4.5/README.md
+-rw-r--r--   0        0        0      897 2023-12-11 12:31:51.919297 unic-0.4.5/unic/__init__.py
+-rw-r--r--   0        0        0      912 2023-12-11 13:01:08.512829 unic-0.4.5/unic/configs/metirc_system/settings.toml
+-rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.4.5/unic/configs/timeunit/settings.toml
+-rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.4.5/unic/configs/timezone/settings.toml
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.5/unic/length_unit/metric_system/__init__.py
+-rw-r--r--   0        0        0      683 2024-05-10 14:37:46.429999 unic-0.4.5/unic/length_unit/metric_system/metric_system_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.5/unic/length_unit/validators/__init__.py
+-rw-r--r--   0        0        0     1279 2024-05-10 14:36:03.640060 unic-0.4.5/unic/length_unit/validators/validators.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-0.4.5/unic/time_unit/datetime/__init__.py
+-rw-r--r--   0        0        0     1301 2024-05-10 14:38:56.907969 unic-0.4.5/unic/time_unit/datetime/datetime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.5/unic/time_unit/time/__init__.py
+-rw-r--r--   0        0        0      660 2024-05-10 14:34:06.458160 unic-0.4.5/unic/time_unit/time/time_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.4.5/unic/time_unit/unixtime/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-10 14:34:11.031532 unic-0.4.5/unic/time_unit/unixtime/unixtime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.5/unic/time_unit/validators/__init__.py
+-rw-r--r--   0        0        0     2557 2024-05-10 14:33:34.102958 unic-0.4.5/unic/time_unit/validators/validators.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.5/unic/utils/__init__.py
+-rw-r--r--   0        0        0      391 2023-10-29 05:14:04.780174 unic-0.4.5/unic/utils/config_parser.py
+-rw-r--r--   0        0        0     3097 1970-01-01 00:00:00.000000 unic-0.4.5/PKG-INFO
```

### Comparing `unic-0.4.4/LICENSE` & `unic-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unic-0.4.4/pyproject.toml` & `unic-0.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unic"
-version = "0.4.4"
+version = "0.4.5"
 description = "Python package for converting various units."
 authors = ["Subretu"]
 maintainers = ["Subretu"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/subretu/unic'
 keywords = ['unit', 'convert', 'time', 'timestamp', 'length']
```

### Comparing `unic-0.4.4/README.md` & `unic-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `unic-0.4.4/unic/__init__.py` & `unic-0.4.5/unic/__init__.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.4/unic/configs/metirc_system/settings.toml` & `unic-0.4.5/unic/configs/metirc_system/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.4.4/unic/configs/timezone/settings.toml` & `unic-0.4.5/unic/configs/timezone/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.4.4/unic/time_unit/datetime/datetime_model.py` & `unic-0.4.5/unic/time_unit/datetime/datetime_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,41 @@
 from pydantic import ValidationError
 from datetime import date, datetime, timezone, timedelta
-from unic.utils import config_parser, validators
+from unic.utils import config_parser
+from unic.time_unit.validators import validators
 from typing import Union
+import math
 
 
 class DatetimeModel:
-    def convert(self, data: int, **kwargs: any) -> Union[date, datetime]:
+    def convert(self, data: int, format: str, tz: str = None) -> Union[date, datetime]:
         try:
-            self.check_parameter_name(kwargs)
-
-            tz = kwargs.get("tz", None)
-
-            target_format = kwargs["format"]
-
             input_data = validators.DatetimeModelValidator(
-                data=data, format=target_format, tz=tz
+                data=data, format=format, tz=tz
             )
         except ValidationError as e:
             raise ValueError(e.errors()[0]["msg"])
 
         timezone_hour = 0
-
         if tz:
             parameter = config_parser.parse_toml("timezone")
             timezone_hour = parameter[tz]["value"]
 
         converted_data = self.convert_timestamp_by_digits(
-            input_data.data, timezone_hour, target_format
+            input_data.data, timezone_hour, format
         )
 
         return converted_data
 
     def convert_timestamp_by_digits(
         self, data: int, timezone_hour: int, target_format: str
     ) -> Union[date, datetime]:
-        digits = len(str(abs(data)))
-
-        processed_data = data if digits == 10 else data / 1000
-
         timestamp_data = datetime.fromtimestamp(
-            processed_data,
+            data,
             timezone(timedelta(hours=timezone_hour)),
         )
 
         result = (
             timestamp_data if target_format == "datetime" else timestamp_data.date()
         )
 
         return result
-
-    def check_parameter_name(self, parameter_name: dict) -> None:
-        if (len(parameter_name) == 1) and ("format" in parameter_name):
-            pass
-        elif (
-            (len(parameter_name) == 2)
-            and ("format" in parameter_name)
-            and ("tz" in parameter_name)
-        ):
-            pass
-        else:
-            raise ValueError("Invalid parameter name.")
```

### Comparing `unic-0.4.4/unic/utils/validators.py` & `unic-0.4.5/unic/time_unit/validators/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pydantic import BaseModel, StrictFloat, field_validator, StrictInt, StrictStr
 from typing import Union
 from datetime import datetime
 from unic.utils import config_parser
+import math
 
 
 class ValidatorMixin:
     @classmethod
     def validate_units(cls, v, valid_units, parameter):
         if v not in valid_units:
             raise ValueError(
@@ -38,17 +39,19 @@
 class DatetimeModelValidator(BaseModel, ValidatorMixin):
     data: StrictInt
     format: StrictStr
     tz: Union[StrictStr, None]
 
     @field_validator("data")
     def data_check(cls, v):
-        digits = len(str(abs(v)))
-        if digits == 10 or digits == 13:
+        digits = math.floor(math.log10(abs(v))) + 1
+        if digits == 10:
             return v
+        if digits == 13:
+            return v / 1000
         else:
             raise ValueError("Unixtime digits is 10 or 13.")
 
     @field_validator("format")
     def format_check(cls, v):
         return cls.validate_units(v, ["datetime", "date"], "format")
 
@@ -73,25 +76,7 @@
         raise ValueError(
             f"'{v}' is invalid date format. Allowed formats are {date_formats}."
         )
 
     @field_validator("tz")
     def timezone_check(cls, v):
         return cls.validate_timezone(v)
-
-
-class MetricSystemModelValidator(BaseModel, ValidatorMixin):
-    data: Union[StrictInt, StrictFloat]
-    from_unit: StrictStr
-    to_unit: StrictStr
-
-    @field_validator("from_unit")
-    def from_unit_check(cls, v):
-        return cls.validate_units(
-            v, ["nm", "um", "mm", "cm", "m", "km", "Mm", "Gm", "Tm"], "from_unit"
-        )
-
-    @field_validator("to_unit")
-    def to_unit_check(cls, v):
-        return cls.validate_units(
-            v, ["nm", "um", "mm", "cm", "m", "km", "Mm", "Gm", "Tm"], "to_unit"
-        )
```

### Comparing `unic-0.4.4/PKG-INFO` & `unic-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unic
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python package for converting various units.
 Home-page: https://github.com/subretu/unic
 License: MIT
 Keywords: unit,convert,time,timestamp,length
 Author: Subretu
 Maintainer: Subretu
 Requires-Python: >=3.8,<4.0
```

