# Comparing `tmp/gptfunction-0.1.3-py3-none-any.whl.zip` & `tmp/gptfunction-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6301 bytes, number of entries: 7
--rw-r--r--  2.0 unx     7120 b- defN 23-Dec-13 13:50 gptfunction/GPTFunction.py
--rw-r--r--  2.0 unx       49 b- defN 23-Dec-13 13:50 gptfunction/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Dec-13 13:50 gptfunction-0.1.3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     4331 b- defN 23-Dec-13 13:50 gptfunction-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-13 13:50 gptfunction-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Dec-13 13:50 gptfunction-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      570 b- defN 23-Dec-13 13:50 gptfunction-0.1.3.dist-info/RECORD
-7 files, 13240 bytes uncompressed, 5285 bytes compressed:  60.1%
+Zip file size: 6479 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     7708 b- defN 24-May-12 16:50 gptfunction/GPTFunction.py
+-rw-r--r--  2.0 unx       49 b- defN 24-May-12 16:50 gptfunction/__init__.py
+-rw-r--r--  2.0 unx     1066 b- defN 24-May-12 16:50 gptfunction-0.2.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     4450 b- defN 24-May-12 16:50 gptfunction-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-12 16:50 gptfunction-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-May-12 16:50 gptfunction-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      570 b- defN 24-May-12 16:50 gptfunction-0.2.0.dist-info/RECORD
+7 files, 13947 bytes uncompressed, 5463 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: gptfunction/GPTFunction.py
 Comment: 
 
 Filename: gptfunction/__init__.py
 Comment: 
 
-Filename: gptfunction-0.1.3.dist-info/LICENSE.md
+Filename: gptfunction-0.2.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: gptfunction-0.1.3.dist-info/METADATA
+Filename: gptfunction-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: gptfunction-0.1.3.dist-info/WHEEL
+Filename: gptfunction-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: gptfunction-0.1.3.dist-info/top_level.txt
+Filename: gptfunction-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gptfunction-0.1.3.dist-info/RECORD
+Filename: gptfunction-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gptfunction/GPTFunction.py

```diff
@@ -44,14 +44,15 @@
     """
 
     @dataclass
     class _FunctionParam:
         name: str
         typing: type
         description: str
+        required: bool
 
     def __init__(self, func: Callable[..., Any]) -> None:
         self.func = func
 
     @no_type_check
     def __call__(self, *args, **kwargs) -> Optional[str]:
         result = self.func(*args, **kwargs)
@@ -61,28 +62,29 @@
             return result
 
         if getattr(result, "__str__"):
             return str(result)
 
         return ""
 
-    def schema(self) -> object:
+    def schema(self, use_required: bool = True) -> object:
         """
         Generates the schema required for passing a function to GPT.
         """
         docstring = docstring_parser.parse(self.func.__doc__)
         return {
             "type": "function",
             "function": {
                 "name": self.func.__name__,
                 "description": docstring.short_description,
                 "parameters": GPTFunction._parse_params(
                     GPTFunction._create_function_params(
                         self.func.__annotations__, docstring.params
                     ),
+                    use_required=use_required,
                 ),
             },
         }
 
     def name(self) -> str:
         """
         Get the name of this function.
@@ -140,42 +142,57 @@
             del annotations["return"]
 
         keyed_docstring_params = {p.arg_name: p for p in docstring_params}
 
         function_params = []
         for key in annotations:
             desc = ""
+            required = False
             if key in keyed_docstring_params:
                 desc = keyed_docstring_params[key].description
+                required = not keyed_docstring_params[key].is_optional
             else:
                 logging.warning(
                     f"Function param {key} has no docstring description. Add a docstring description for more accurate use by GPT."
                 )
 
             function_params.append(
-                GPTFunction._FunctionParam(key, annotations[key], desc)
+                GPTFunction._FunctionParam(
+                    name=key,
+                    typing=annotations[key],
+                    description=desc,
+                    required=required,
+                )
             )
 
         return function_params
 
     @staticmethod
-    def _parse_params(params: List[_FunctionParam]) -> Dict[str, Any]:
+    def _parse_params(
+        params: List[_FunctionParam], use_required: bool
+    ) -> Dict[str, Any]:
         """
         Converts a function's params into a 'parameters' object used by the function calling schema.
         :param params: The function parameters to parse into the schema.
         :return: The parameters part of the function calling schema.
         """
         schema_params: Dict[str, Any] = {}
+        required_params: list[str] = []
         for param in params:
             schema_params |= {
                 param.name: GPTFunction._parse_param_type(param.typing)
                 | {"description": param.description}
             }
+            if param.required:
+                required_params.append(param.name)
 
-        return {"type": "object", "properties": schema_params}
+        return {
+            "type": "object",
+            "properties": schema_params,
+        } | ({"required": required_params} if use_required else {})
 
     @staticmethod
     def _parse_param_type(
         param_type: Union[type, object],
     ) -> Dict[str, Union[str, List[str]]]:
         """
         Converts a `typing` hint into a param object used by the function calling schema.
```

## Comparing `gptfunction-0.1.3.dist-info/LICENSE.md` & `gptfunction-0.2.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `gptfunction-0.1.3.dist-info/METADATA` & `gptfunction-0.2.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptfunction
-Version: 0.1.3
+Version: 0.2.0
 Summary: A decorator for wrapping Python functions to generate an OpenAI GPT function calling schema.
 Author: PandasAreBears
 License: Copyright (c) 2023 PandasAreBears
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -92,15 +92,16 @@
 
 ### Decorator
 
 - `@gptfunction`: This decorator should be used above the function definition. It processes the function and creates a GPT function schema.
 
 ### Methods
 
-- `schema()`: Returns the JSON schema of the wrapped function.
+- `schema(use_required: bool)`: Returns the JSON schema of the wrapped function.
+    - use_required: Indicates whether the schema should specify required parameters (default: True).
 - `description()`: Retrieves the function's description from its docstring.
 - `name()`: Returns the name of the function.
 
 ## Contributing
 
 Contributions to improve `GPTFunction` are welcome. Please follow the standard procedures for submitting issues and pull requests on the project's GitHub repository.
```

