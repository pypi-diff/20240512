# Comparing `tmp/agent_dingo-0.1.0rc1.tar.gz` & `tmp/agent_dingo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_dingo-0.1.0rc1.tar", last modified: Sun Jun 25 10:26:02 2023, max compression
+gzip compressed data, was "agent_dingo-1.0.0.tar", last modified: Sun May 12 08:29:25 2024, max compression
```

## Comparing `agent_dingo-0.1.0rc1.tar` & `agent_dingo-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,55 @@
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 10:26:02.588700 agent_dingo-0.1.0rc1/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1071 2023-06-23 11:05:22.000000 agent_dingo-0.1.0rc1/LICENSE
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     9769 2023-06-25 10:26:02.588700 agent_dingo-0.1.0rc1/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     9310 2023-06-25 10:23:37.000000 agent_dingo-0.1.0rc1/README.md
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 10:26:02.584700 agent_dingo-0.1.0rc1/agent_dingo/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      118 2023-06-25 10:25:44.000000 agent_dingo-0.1.0rc1/agent_dingo/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     7528 2023-06-23 20:46:52.000000 agent_dingo-0.1.0rc1/agent_dingo/agent.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1069 2023-06-25 08:27:51.000000 agent_dingo-0.1.0rc1/agent_dingo/chat.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      113 2023-06-23 19:23:44.000000 agent_dingo-0.1.0rc1/agent_dingo/context.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2166 2023-06-23 19:49:50.000000 agent_dingo-0.1.0rc1/agent_dingo/docgen.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1472 2023-06-23 19:25:05.000000 agent_dingo-0.1.0rc1/agent_dingo/helpers.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1907 2023-06-23 19:25:34.000000 agent_dingo-0.1.0rc1/agent_dingo/parser.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 10:26:02.588700 agent_dingo-0.1.0rc1/agent_dingo.egg-info/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     9769 2023-06-25 10:26:02.000000 agent_dingo-0.1.0rc1/agent_dingo.egg-info/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      486 2023-06-25 10:26:02.000000 agent_dingo-0.1.0rc1/agent_dingo.egg-info/SOURCES.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-06-25 10:26:02.000000 agent_dingo-0.1.0rc1/agent_dingo.egg-info/dependency_links.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       56 2023-06-25 10:26:02.000000 agent_dingo-0.1.0rc1/agent_dingo.egg-info/requires.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       12 2023-06-25 10:26:02.000000 agent_dingo-0.1.0rc1/agent_dingo.egg-info/top_level.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      654 2023-06-25 10:25:54.000000 agent_dingo-0.1.0rc1/pyproject.toml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-06-25 10:26:02.588700 agent_dingo-0.1.0rc1/setup.cfg
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-06-25 10:26:02.588700 agent_dingo-0.1.0rc1/tests/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1516 2023-06-24 13:12:51.000000 agent_dingo-0.1.0rc1/tests/test_agent.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      692 2023-06-24 13:12:48.000000 agent_dingo-0.1.0rc1/tests/test_extract_substr.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1321 2023-06-24 13:12:52.000000 agent_dingo-0.1.0rc1/tests/test_get_required_args.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     4307 2023-06-24 13:12:53.000000 agent_dingo-0.1.0rc1/tests/test_parser.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1349 2023-06-24 13:12:01.000000 agent_dingo-0.1.0rc1/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.269979 agent_dingo-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-12 08:29:25.269979 agent_dingo-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.261979 agent_dingo-1.0.0/agent_dingo/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.265979 agent_dingo-1.0.0/agent_dingo/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/agent/chat_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/agent/docgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/agent/function_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/agent/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/agent/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/agent/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/agent/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.265979 agent_dingo-1.0.0/agent_dingo/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/core/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/core/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.265979 agent_dingo-1.0.0/agent_dingo/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/llm/gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/llm/litellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/llm/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/llm/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.265979 agent_dingo-1.0.0/agent_dingo/rag/
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.265979 agent_dingo-1.0.0/agent_dingo/rag/chunkers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/chunkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/chunkers/recursive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.265979 agent_dingo-1.0.0/agent_dingo/rag/embedders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/embedders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/embedders/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/embedders/sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/prompt_modifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.269979 agent_dingo-1.0.0/agent_dingo/rag/readers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/readers/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/readers/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/readers/word.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.269979 agent_dingo-1.0.0/agent_dingo/rag/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/vector_stores/chromadb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/rag/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/agent_dingo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 08:29:25.269979 agent_dingo-1.0.0/agent_dingo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-12 08:29:25.000000 agent_dingo-1.0.0/agent_dingo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-12 08:29:25.000000 agent_dingo-1.0.0/agent_dingo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 08:29:25.000000 agent_dingo-1.0.0/agent_dingo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-12 08:29:25.000000 agent_dingo-1.0.0/agent_dingo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 08:29:25.000000 agent_dingo-1.0.0/agent_dingo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-12 08:29:09.000000 agent_dingo-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 08:29:25.269979 agent_dingo-1.0.0/setup.cfg
```

### Comparing `agent_dingo-0.1.0rc1/LICENSE` & `agent_dingo-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agent_dingo-0.1.0rc1/agent_dingo/docgen.py` & `agent_dingo-1.0.0/agent_dingo/agent/docgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Callable
 import inspect
-from agent_dingo.chat import send_message
+from agent_dingo.core.blocks import BaseLLM
 import re
 
 _SYSTEM_MSG = "You are a code generation tool. Your responses are limited to providing the docstrings of functions."
 
 _PROMPT = """
 You will be provided with a Python function. Your task is to generate a docstring in a Google style for that python function and return only the docsting delimited by triple backticks. Do not return the function itself.
 
 Python function:
 ```{code}```
 
 Docstring:
 """
 
 
-def generate_docstring(func: Callable, model: str) -> str:
+def generate_docstring(func: Callable, model: BaseLLM) -> str:
     """Generates a docstring for a given function.
 
     Parameters
     ----------
     func : Callable
         The function to generate a docstring for.
     model : str
@@ -31,15 +31,15 @@
         The generated docstring.
     """
     code = inspect.getsource(func)
     messages = [
         {"role": "system", "content": _SYSTEM_MSG},
         {"role": "user", "content": _PROMPT.format(code=code)},
     ]
-    response = send_message(messages, model=model, temperature=0.0)
+    response = model.send_message(messages, temperature=0.0)
 
     response = (
         response["content"]
         .replace("```python\n", "")
         .replace("```", "")
         .replace('"""', "")
         .replace("'''", "")
```

### Comparing `agent_dingo-0.1.0rc1/agent_dingo/helpers.py` & `agent_dingo-1.0.0/agent_dingo/agent/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from agent_dingo.context import ChatContext
+from agent_dingo.core.state import Context
 from typing import Callable, List
 import inspect
+from agent_dingo.agent.chat_context import ChatContext
 
 
 def construct_json_repr(
     name: str, description: str, properties: dict, required: List[str]
 ) -> dict:
     """Constructs a JSON representation of a function.
```

### Comparing `agent_dingo-0.1.0rc1/agent_dingo/parser.py` & `agent_dingo-1.0.0/agent_dingo/agent/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from docstring_parser import parse as _parse
 import ast
 
+
 _types = {
     "str": "string",
     "int": "integer",
     "float": "number",
     "bool": "boolean",
     "list": "array",
-    "dict": "object"
+    "dict": "object",
 }
 
+
 def parse(docstring: str) -> dict:
     """Parses a docstring.
 
     Parameters
     ----------
     docstring : str
         The docstring to parse.
@@ -25,40 +27,40 @@
 
     Raises
     ------
     ValueError
         If the docstring has no description.
     """
     parsed = _parse(docstring)
-    description = ''
+    description = ""
     if parsed.short_description:
         description = parsed.short_description
     if parsed.long_description:
-        if description != '':
-            description += '\n' + parsed.long_description
+        if description != "":
+            description += "\n" + parsed.long_description
         else:
             description = parsed.long_description
-    if description == '':
-        raise ValueError('Docstring has no description')
+    if description == "":
+        raise ValueError("Docstring has no description")
     args = {}
     requires_context = False
     for arg in parsed.params:
-        if arg.arg_name == 'chat_context' and arg.type_name == 'ChatContext':
+        if arg.arg_name == "chat_context" and arg.type_name == "ChatContext":
             requires_context = True
             continue
         d = {}
         if "Enum:" in arg.description:
             arg_description = arg.description.split("Enum:")[0].strip()
             enum = arg.description.split("Enum:")[1].strip()
             try:
                 enum = ast.literal_eval(enum)
                 d = {"description": arg_description, "enum": enum}
             except Exception:
                 d = {"description": arg_description}
         else:
             d = {"description": arg.description}
         if arg.type_name in _types:
-            args[arg.arg_name] = {'type': _types[arg.type_name]}
+            args[arg.arg_name] = {"type": _types[arg.type_name]}
         else:
-             args[arg.arg_name] = {'type': "string"}
+            args[arg.arg_name] = {"type": "string"}
         args[arg.arg_name].update(d)
-    return {'description': description, 'properties': args}, requires_context
+    return {"description": description, "properties": args}, requires_context
```

