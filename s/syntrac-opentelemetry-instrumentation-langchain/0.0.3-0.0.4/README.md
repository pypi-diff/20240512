# Comparing `tmp/syntrac_opentelemetry_instrumentation_langchain-0.0.3.tar.gz` & `tmp/syntrac_opentelemetry_instrumentation_langchain-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntrac_opentelemetry_instrumentation_langchain-0.0.3.tar", max compression
+gzip compressed data, was "syntrac_opentelemetry_instrumentation_langchain-0.0.4.tar", max compression
```

## Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.3.tar` & `syntrac_opentelemetry_instrumentation_langchain-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1164 2024-05-08 11:05:49.789487 syntrac_opentelemetry_instrumentation_langchain-0.0.3/README.md
--rw-r--r--   0        0        0     1183 2024-05-08 11:05:49.799750 syntrac_opentelemetry_instrumentation_langchain-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5978 2024-05-08 11:05:49.792343 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0       42 2024-05-08 11:05:49.794483 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/config.py
--rw-r--r--   0        0        0     3895 2024-05-08 11:05:49.794623 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/custom_chat_wrapper.py
--rw-r--r--   0        0        0     2165 2024-05-08 11:05:49.794860 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py
--rw-r--r--   0        0        0     2958 2024-05-08 11:05:49.794998 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/task_wrapper.py
--rw-r--r--   0        0        0     2627 2024-05-08 11:05:49.795137 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/utils.py
--rw-r--r--   0        0        0       22 2024-05-08 11:05:49.795287 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/version.py
--rw-r--r--   0        0        0     2318 2024-05-08 11:05:49.795420 syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_langchain-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1164 2024-05-12 08:50:06.500940 syntrac_opentelemetry_instrumentation_langchain-0.0.4/README.md
+-rw-r--r--   0        0        0     1183 2024-05-12 08:50:06.510609 syntrac_opentelemetry_instrumentation_langchain-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5978 2024-05-12 08:50:06.502436 syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0       42 2024-05-12 08:50:06.505019 syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/config.py
+-rw-r--r--   0        0        0     3905 2024-05-12 08:50:06.505351 syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/custom_chat_wrapper.py
+-rw-r--r--   0        0        0     2165 2024-05-12 08:50:06.505566 syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py
+-rw-r--r--   0        0        0     2672 2024-05-12 08:50:06.505785 syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/task_wrapper.py
+-rw-r--r--   0        0        0     2657 2024-05-12 08:50:06.506018 syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/utils.py
+-rw-r--r--   0        0        0       22 2024-05-12 08:50:06.506188 syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/version.py
+-rw-r--r--   0        0        0     2032 2024-05-12 08:50:06.506414 syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 syntrac_opentelemetry_instrumentation_langchain-0.0.4/PKG-INFO
```

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.3/README.md` & `syntrac_opentelemetry_instrumentation_langchain-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.3/pyproject.toml` & `syntrac_opentelemetry_instrumentation_langchain-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "syntrac-opentelemetry-instrumentation-langchain"
-version = "0.0.3"
+version = "0.0.4"
 description = "OpenTelemetry Langchain instrumentation"
 authors = [ "Vuong Ngo <vuongngo.pd@gmail.com>" ]
 repository = "https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-instrumentation-langchain"
 license = "Apache-2.0"
 readme = "README.md"
 
   [[tool.poetry.packages]]
```

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/__init__.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/custom_chat_wrapper.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/custom_chat_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                 generation[0].text,
             )
             try:
                 token_usage = generation[0].message.response_metadata['token_usage']
                 completion_tokens += token_usage.completion_tokens
                 prompt_tokens += token_usage.prompt_tokens
                 total_tokens += (token_usage.completion_tokens + token_usage.prompt_tokens)
-            except:
+            except Exception:
                 prompt_tokens = 0
 
         span.set_attribute(
             f"{SpanAttributes.LLM_USAGE_TOTAL_TOKENS}",
             total_tokens,
         )
         span.set_attribute(
```

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/custom_llm_wrapper.py`

 * *Files identical despite different names*

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/utils.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 import logging
 import os
 from opentelemetry import context as context_api
 from syntrac_opentelemetry.instrumentation.langchain.config import Config
 from syntrac_opentelemetry.semconv.ai import SpanAttributes
 
+
 def _with_tracer_wrapper(func):
     """Helper for providing tracer for wrapper functions."""
 
     def _with_tracer(tracer, to_wrap):
         def wrapper(wrapped, instance, args, kwargs):
             return func(tracer, to_wrap, wrapped, instance, args, kwargs)
 
@@ -52,15 +53,15 @@
             to_serialize.update(arg)
 
         if "callbacks" in to_serialize:
             to_serialize.pop("callbacks")
 
         span.set_attribute(
             SpanAttributes.SYNTRAC_ENTITY_INPUT,
-            json.dumps(
+            serialise_to_json(
                 {
                     "args": [],
                     "kwargs": to_serialize,
                 }
             ),
         )
 
@@ -84,14 +85,18 @@
         if isinstance(value, str):
             return value
 
         return json.dumps(value)
     except TypeError:
         return str(value)
 
+
+def non_serialize(value):
+    return f"<<non-serializable: {type(value).__qualname__}>>"
+
+
 def serialise_to_json(value):
     try:
-        default = lambda o: f"<<non-serializable: {type(o).__qualname__}>>"
-        return json.dumps(value, default=default)
+        return json.dumps(value, default=non_serialize)
     except Exception as e:
         print(e)
         return value
```

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.3/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py` & `syntrac_opentelemetry_instrumentation_langchain-0.0.4/syntrac_opentelemetry/instrumentation/langchain/workflow_wrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 
 from opentelemetry.instrumentation.utils import (
     _SUPPRESS_INSTRUMENTATION_KEY,
 )
 
 from syntrac_opentelemetry.semconv.ai import SpanAttributes, SyntracSpanKindValues
 
-from syntrac_opentelemetry.instrumentation.langchain.utils import _with_tracer_wrapper, serialise_to_json
+from syntrac_opentelemetry.instrumentation.langchain.utils import (
+  _with_tracer_wrapper,
+  process_request,
+  process_response,
+)
 
 
 @_with_tracer_wrapper
 def workflow_wrapper(tracer, to_wrap, wrapped, instance, args, kwargs):
     """Instruments and calls every function defined in TO_WRAP."""
     if context_api.get_value(_SUPPRESS_INSTRUMENTATION_KEY):
         return wrapped(*args, **kwargs)
@@ -23,22 +27,18 @@
 
     with tracer.start_as_current_span(name) as span:
         span.set_attribute(
             SpanAttributes.SYNTRAC_SPAN_KIND,
             kind,
         )
         span.set_attribute(SpanAttributes.SYNTRAC_ENTITY_NAME, name)
-        span.set_attribute(SpanAttributes.SYNTRAC_ENTITY_INPUT, serialise_to_json({
-          "args": args,
-          "kwargs": kwargs
-        }))
 
+        process_request(span, args, kwargs)
         return_value = wrapped(*args, **kwargs)
-
-        span.set_attribute(SpanAttributes.SYNTRAC_ENTITY_OUTPUT, serialise_to_json(return_value))
+        process_response(span, return_value)
 
     return return_value
 
 
 @_with_tracer_wrapper
 async def aworkflow_wrapper(tracer, to_wrap, wrapped, instance, args, kwargs):
     """Instruments and calls every function defined in TO_WRAP."""
@@ -52,16 +52,13 @@
 
     with tracer.start_as_current_span(name) as span:
         span.set_attribute(
             SpanAttributes.SYNTRAC_SPAN_KIND,
             kind,
         )
         span.set_attribute(SpanAttributes.SYNTRAC_ENTITY_NAME, name)
-        span.set_attribute(SpanAttributes.SYNTRAC_ENTITY_INPUT, serialise_to_json({
-          "args": args,
-          "kwargs": kwargs
-        }))
 
+        process_request(span, args, kwargs)
         return_value = await wrapped(*args, **kwargs)
-        span.set_attribute(SpanAttributes.SYNTRAC_ENTITY_OUTPUT, serialise_to_json(return_value))
+        process_response(span, return_value)
 
     return return_value
```

### Comparing `syntrac_opentelemetry_instrumentation_langchain-0.0.3/PKG-INFO` & `syntrac_opentelemetry_instrumentation_langchain-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syntrac-opentelemetry-instrumentation-langchain
-Version: 0.0.3
+Version: 0.0.4
 Summary: OpenTelemetry Langchain instrumentation
 Home-page: https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-instrumentation-langchain
 License: Apache-2.0
 Author: Vuong Ngo
 Author-email: vuongngo.pd@gmail.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: syntrac-opentelemetry-instrumentation-langchain
-Version: 0.0.3 Summary: OpenTelemetry Langchain instrumentation Home-page:
+Version: 0.0.4 Summary: OpenTelemetry Langchain instrumentation Home-page:
 https://github.com/syntracAI/syntrac/tree/main/packages/python/opentelemetry-
 instrumentation-langchain License: Apache-2.0 Author: Vuong Ngo Author-email:
 vuongngo.pd@gmail.com Requires-Python: >=3.9,<4 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
```

