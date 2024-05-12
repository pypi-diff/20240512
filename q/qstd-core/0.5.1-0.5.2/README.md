# Comparing `tmp/qstd_core-0.5.1.tar.gz` & `tmp/qstd_core-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qstd_core-0.5.1.tar", last modified: Sun May  5 16:04:04 2024, max compression
+gzip compressed data, was "qstd_core-0.5.2.tar", last modified: Sun May 12 13:08:34 2024, max compression
```

## Comparing `qstd_core-0.5.1.tar` & `qstd_core-0.5.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.917523 qstd_core-0.5.1/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_core-0.5.1/LICENSE
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-05-05 16:04:04.917523 qstd_core-0.5.1/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       42 2024-04-16 16:54:41.000000 qstd_core-0.5.1/README.md
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.913524 qstd_core-0.5.1/qstd_core/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      150 2024-04-16 15:25:55.000000 qstd_core-0.5.1/qstd_core/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.913524 qstd_core-0.5.1/qstd_core/exceptions/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       48 2024-04-16 16:15:44.000000 qstd_core-0.5.1/qstd_core/exceptions/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      830 2024-04-16 16:17:31.000000 qstd_core-0.5.1/qstd_core/exceptions/base.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1385 2024-04-16 16:17:31.000000 qstd_core-0.5.1/qstd_core/exceptions/localization.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.917523 qstd_core-0.5.1/qstd_core/localization/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2176 2024-04-16 16:33:14.000000 qstd_core-0.5.1/qstd_core/localization/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.917523 qstd_core-0.5.1/qstd_core/logger/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       69 2024-04-21 19:21:33.000000 qstd_core-0.5.1/qstd_core/logger/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.917523 qstd_core-0.5.1/qstd_core/marshmallow/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      177 2024-05-01 11:16:49.000000 qstd_core-0.5.1/qstd_core/marshmallow/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     9670 2024-05-01 15:31:17.000000 qstd_core-0.5.1/qstd_core/marshmallow/fields.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1504 2024-05-01 15:34:26.000000 qstd_core-0.5.1/qstd_core/marshmallow/schema.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4358 2024-05-01 15:24:31.000000 qstd_core-0.5.1/qstd_core/marshmallow/validate.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.917523 qstd_core-0.5.1/qstd_core/openapi/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       81 2024-03-31 12:25:01.000000 qstd_core-0.5.1/qstd_core/openapi/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5915 2024-04-26 15:07:56.000000 qstd_core-0.5.1/qstd_core/openapi/decorators.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      244 2024-03-13 13:59:27.000000 qstd_core-0.5.1/qstd_core/openapi/enum.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      382 2024-03-31 12:25:14.000000 qstd_core-0.5.1/qstd_core/openapi/router.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     9221 2024-04-26 10:28:32.000000 qstd_core-0.5.1/qstd_core/openapi/spec.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     8906 2024-05-05 15:59:18.000000 qstd_core-0.5.1/qstd_core/openapi/utils.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.917523 qstd_core-0.5.1/qstd_core/sanic/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-04-06 09:59:29.000000 qstd_core-0.5.1/qstd_core/sanic/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.917523 qstd_core-0.5.1/qstd_core/sanic/request/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      852 2024-04-16 16:31:39.000000 qstd_core-0.5.1/qstd_core/sanic/request/__init__.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.917523 qstd_core-0.5.1/qstd_core/sanic/server/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       20 2024-04-16 15:25:27.000000 qstd_core-0.5.1/qstd_core/sanic/server/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      319 2024-04-21 19:19:40.000000 qstd_core-0.5.1/qstd_core/sanic/server/utils.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.917523 qstd_core-0.5.1/qstd_core/validator/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2008 2024-04-25 11:21:18.000000 qstd_core-0.5.1/qstd_core/validator/ValidatorABS.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2693 2024-05-05 16:02:29.000000 qstd_core-0.5.1/qstd_core/validator/ValidatorMarshmallow.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1191 2024-04-25 11:11:00.000000 qstd_core-0.5.1/qstd_core/validator/ValidatorPydantic.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1834 2024-04-23 09:26:58.000000 qstd_core-0.5.1/qstd_core/validator/__init__.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      134 2024-04-21 19:14:09.000000 qstd_core-0.5.1/qstd_core/validator/enums.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1428 2024-05-05 15:31:12.000000 qstd_core-0.5.1/qstd_core/validator/exceptions.py
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      139 2024-04-16 14:18:23.000000 qstd_core-0.5.1/qstd_core/validator/types.py
-drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-05 16:04:04.913524 qstd_core-0.5.1/qstd_core.egg-info/
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-05-05 16:04:04.000000 qstd_core-0.5.1/qstd_core.egg-info/PKG-INFO
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1062 2024-05-05 16:04:04.000000 qstd_core-0.5.1/qstd_core.egg-info/SOURCES.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-05-05 16:04:04.000000 qstd_core-0.5.1/qstd_core.egg-info/dependency_links.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       65 2024-05-05 16:04:04.000000 qstd_core-0.5.1/qstd_core.egg-info/requires.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       10 2024-05-05 16:04:04.000000 qstd_core-0.5.1/qstd_core.egg-info/top_level.txt
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-05-05 16:04:04.917523 qstd_core-0.5.1/setup.cfg
--rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      706 2024-05-05 16:02:49.000000 qstd_core-0.5.1/setup.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1054 2024-03-24 20:15:12.000000 qstd_core-0.5.2/LICENSE
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-05-12 13:08:34.173718 qstd_core-0.5.2/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       42 2024-04-16 16:54:41.000000 qstd_core-0.5.2/README.md
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      150 2024-04-16 15:25:55.000000 qstd_core-0.5.2/qstd_core/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core/exceptions/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       48 2024-04-16 16:15:44.000000 qstd_core-0.5.2/qstd_core/exceptions/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      830 2024-04-16 16:17:31.000000 qstd_core-0.5.2/qstd_core/exceptions/base.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1385 2024-04-16 16:17:31.000000 qstd_core-0.5.2/qstd_core/exceptions/localization.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core/localization/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2176 2024-04-16 16:33:14.000000 qstd_core-0.5.2/qstd_core/localization/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core/logger/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       69 2024-04-21 19:21:33.000000 qstd_core-0.5.2/qstd_core/logger/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core/marshmallow/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      177 2024-05-01 11:16:49.000000 qstd_core-0.5.2/qstd_core/marshmallow/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     9670 2024-05-01 15:31:17.000000 qstd_core-0.5.2/qstd_core/marshmallow/fields.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1664 2024-05-12 13:07:29.000000 qstd_core-0.5.2/qstd_core/marshmallow/schema.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     4358 2024-05-01 15:24:31.000000 qstd_core-0.5.2/qstd_core/marshmallow/validate.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/qstd_core/openapi/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       81 2024-03-31 12:25:01.000000 qstd_core-0.5.2/qstd_core/openapi/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     5915 2024-04-26 15:07:56.000000 qstd_core-0.5.2/qstd_core/openapi/decorators.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      244 2024-03-13 13:59:27.000000 qstd_core-0.5.2/qstd_core/openapi/enum.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      382 2024-03-31 12:25:14.000000 qstd_core-0.5.2/qstd_core/openapi/router.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     9221 2024-04-26 10:28:32.000000 qstd_core-0.5.2/qstd_core/openapi/spec.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     8906 2024-05-05 15:59:18.000000 qstd_core-0.5.2/qstd_core/openapi/utils.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/qstd_core/sanic/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       22 2024-04-06 09:59:29.000000 qstd_core-0.5.2/qstd_core/sanic/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/qstd_core/sanic/request/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      852 2024-04-16 16:31:39.000000 qstd_core-0.5.2/qstd_core/sanic/request/__init__.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/qstd_core/sanic/server/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       20 2024-04-16 15:25:27.000000 qstd_core-0.5.2/qstd_core/sanic/server/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      319 2024-04-21 19:19:40.000000 qstd_core-0.5.2/qstd_core/sanic/server/utils.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.173718 qstd_core-0.5.2/qstd_core/validator/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2008 2024-04-25 11:21:18.000000 qstd_core-0.5.2/qstd_core/validator/ValidatorABS.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     2693 2024-05-05 16:02:29.000000 qstd_core-0.5.2/qstd_core/validator/ValidatorMarshmallow.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1191 2024-04-25 11:11:00.000000 qstd_core-0.5.2/qstd_core/validator/ValidatorPydantic.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1834 2024-04-23 09:26:58.000000 qstd_core-0.5.2/qstd_core/validator/__init__.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      134 2024-04-21 19:14:09.000000 qstd_core-0.5.2/qstd_core/validator/enums.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1428 2024-05-05 15:31:12.000000 qstd_core-0.5.2/qstd_core/validator/exceptions.py
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      139 2024-04-16 14:18:23.000000 qstd_core-0.5.2/qstd_core/validator/types.py
+drwxrwxr-x   0 quisegosum  (1000) quisegosum  (1000)        0 2024-05-12 13:08:34.169718 qstd_core-0.5.2/qstd_core.egg-info/
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      362 2024-05-12 13:08:34.000000 qstd_core-0.5.2/qstd_core.egg-info/PKG-INFO
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)     1062 2024-05-12 13:08:34.000000 qstd_core-0.5.2/qstd_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)        1 2024-05-12 13:08:34.000000 qstd_core-0.5.2/qstd_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       65 2024-05-12 13:08:34.000000 qstd_core-0.5.2/qstd_core.egg-info/requires.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       10 2024-05-12 13:08:34.000000 qstd_core-0.5.2/qstd_core.egg-info/top_level.txt
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)       38 2024-05-12 13:08:34.173718 qstd_core-0.5.2/setup.cfg
+-rw-rw-r--   0 quisegosum  (1000) quisegosum  (1000)      706 2024-05-12 13:08:06.000000 qstd_core-0.5.2/setup.py
```

### Comparing `qstd_core-0.5.1/LICENSE` & `qstd_core-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/exceptions/base.py` & `qstd_core-0.5.2/qstd_core/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/exceptions/localization.py` & `qstd_core-0.5.2/qstd_core/exceptions/localization.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/localization/__init__.py` & `qstd_core-0.5.2/qstd_core/localization/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/marshmallow/fields.py` & `qstd_core-0.5.2/qstd_core/marshmallow/fields.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/marshmallow/schema.py` & `qstd_core-0.5.2/qstd_core/marshmallow/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from marshmallow import Schema as DefaultSchema
 
 from .validate import Range
 from .fields import Integer, List, Nested, Field
 
 
 class Schema(DefaultSchema):
-    schema_title: str
-    schema_description: str
+    schema_title: typing.Optional[typing.Union[str, Field]]
+    schema_description: typing.Optional[typing.Union[str, Field]]
 
     fields: typing.Dict[str, Field]
 
     @classmethod
     def pagination(cls):
         class PaginationResponse(Schema):
             total = Integer(required=True, validate=Range(min=0))
@@ -20,20 +20,20 @@
 
     def openapi_schema(self):
         schema = dict(
             type='object',
             properties=dict(),
             required=list()
         )
-        if hasattr(self, 'title'):
-            schema['title'] = self.title
+        if hasattr(self, 'schema_title') and isinstance(self.schema_title, str):
+            schema['title'] = self.schema_title
         else:
             schema['title'] = self.__class__.__name__
-        if hasattr(self, 'schema_description'):
-            schema['properties']['description'] = self.schema_description
+        if hasattr(self, 'schema_description') and isinstance(self.schema_description, str):
+            schema['description'] = self.schema_description
         for field_name in self.fields:
             if self.only and field_name not in self.only:
                 continue
             field = self.fields[field_name]
             property_name = field.data_key or field_name
             schema['properties'][property_name] = field.openapi_schema()
             if field.required is True:
```

### Comparing `qstd_core-0.5.1/qstd_core/marshmallow/validate.py` & `qstd_core-0.5.2/qstd_core/marshmallow/validate.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/openapi/decorators.py` & `qstd_core-0.5.2/qstd_core/openapi/decorators.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/openapi/spec.py` & `qstd_core-0.5.2/qstd_core/openapi/spec.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/openapi/utils.py` & `qstd_core-0.5.2/qstd_core/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/sanic/request/__init__.py` & `qstd_core-0.5.2/qstd_core/sanic/request/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/validator/ValidatorABS.py` & `qstd_core-0.5.2/qstd_core/validator/ValidatorABS.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/validator/ValidatorMarshmallow.py` & `qstd_core-0.5.2/qstd_core/validator/ValidatorMarshmallow.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/validator/ValidatorPydantic.py` & `qstd_core-0.5.2/qstd_core/validator/ValidatorPydantic.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/validator/__init__.py` & `qstd_core-0.5.2/qstd_core/validator/__init__.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core/validator/exceptions.py` & `qstd_core-0.5.2/qstd_core/validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/qstd_core.egg-info/SOURCES.txt` & `qstd_core-0.5.2/qstd_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qstd_core-0.5.1/setup.py` & `qstd_core-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='qstd_core',
-    version='0.5.1',
+    version='0.5.2',
     author='QuisEgoSum',
     author_email='subbotin.evdokim@gmail.com',
     description='Application core based on sanic',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/QuisEgoSum/qstd-core',
     packages=find_packages(exclude=['tmp', 'example']),
```

