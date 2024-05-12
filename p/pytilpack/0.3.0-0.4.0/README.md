# Comparing `tmp/pytilpack-0.3.0.tar.gz` & `tmp/pytilpack-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytilpack-0.3.0.tar", max compression
+gzip compressed data, was "pytilpack-0.4.0.tar", max compression
```

## Comparing `pytilpack-0.3.0.tar` & `pytilpack-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1061 2024-05-05 13:35:01.448651 pytilpack-0.3.0/LICENSE
--rw-r--r--   0        0        0      503 2024-05-05 13:35:01.448651 pytilpack-0.3.0/README.md
--rw-r--r--   0        0        0     2409 2024-05-05 13:35:15.004858 pytilpack-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/__init__.py
--rw-r--r--   0        0        0      942 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/csv_.py
--rw-r--r--   0        0        0     1920 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/flask_.py
--rw-r--r--   0        0        0     4556 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/openai_.py
--rw-r--r--   0        0        0      566 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/pathlib_.py
--rw-r--r--   0        0        0      690 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/python_.py
--rw-r--r--   0        0        0     2392 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/sqlalchemy_.py
--rw-r--r--   0        0        0     8055 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/tiktoken_.py
--rw-r--r--   0        0        0      523 2024-05-05 13:35:01.448651 pytilpack-0.3.0/pytilpack/tqdm_.py
--rw-r--r--   0        0        0     1864 1970-01-01 00:00:00.000000 pytilpack-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-12 14:03:16.438969 pytilpack-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1114 2024-05-12 14:03:16.438969 pytilpack-0.4.0/README.md
+-rw-r--r--   0        0        0     2493 2024-05-12 14:03:28.735081 pytilpack-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-12 14:03:16.438969 pytilpack-0.4.0/pytilpack/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-12 14:03:16.438969 pytilpack-0.4.0/pytilpack/csv_.py
+-rw-r--r--   0        0        0     5390 2024-05-12 14:03:16.438969 pytilpack-0.4.0/pytilpack/flask_.py
+-rw-r--r--   0        0        0     4820 2024-05-12 14:03:16.438969 pytilpack-0.4.0/pytilpack/openai_.py
+-rw-r--r--   0        0        0      566 2024-05-12 14:03:16.438969 pytilpack-0.4.0/pytilpack/pathlib_.py
+-rw-r--r--   0        0        0      690 2024-05-12 14:03:16.438969 pytilpack-0.4.0/pytilpack/python_.py
+-rw-r--r--   0        0        0     2392 2024-05-12 14:03:16.438969 pytilpack-0.4.0/pytilpack/sqlalchemy_.py
+-rw-r--r--   0        0        0     8055 2024-05-12 14:03:16.438969 pytilpack-0.4.0/pytilpack/tiktoken_.py
+-rw-r--r--   0        0        0      523 2024-05-12 14:03:16.438969 pytilpack-0.4.0/pytilpack/tqdm_.py
+-rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 pytilpack-0.4.0/PKG-INFO
```

### Comparing `pytilpack-0.3.0/LICENSE` & `pytilpack-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytilpack-0.3.0/pyproject.toml` & `pytilpack-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytilpack"
-version = "0.3.0"  # using poetry-dynamic-versioning
+version = "0.4.0"  # using poetry-dynamic-versioning
 description = "Python Utility Pack"
 license = "MIT"
 authors = ["aki. <mark@aur.ll.to>"]
 readme = "README.md"
 homepage = "https://github.com/ak110/pytilpack"
 classifiers = [
     "Environment :: Console",
@@ -15,36 +15,39 @@
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "pep440"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
+html5lib = {version = "*", optional = true}
 flask = {version = ">=2.2", optional = true}
 httpx = {version = "*", optional = true}
 openai = {version = ">=1.25", optional = true}
 pillow = {version = "*", optional = true}
 sqlalchemy = {version = ">=2.0", optional = true}
 tiktoken = {version = ">=0.6", optional = true}
 tqdm = {version = ">=4.66", optional = true}
 typing-extensions = ">=4.0"
 
 [tool.poetry.group.dev.dependencies]
 pyfltr = "*"
 
 [tool.poetry.extras]
 all = [
+    "html5lib",
     "flask",
     "httpx",
     "openai",
     "pillow",
     "sqlalchemy",
     "tiktoken",
     "tqdm",
 ]
+html5lib = ["html5lib"]
 flask = ["flask"]
 openai = ["openai"]
 sqlalchemy = ["sqlalchemy"]
 tiktoken = ["tiktoken", "openai", "httpx", "pillow"]
 tqdm = ["tqdm"]
 
 [build-system]
```

### Comparing `pytilpack-0.3.0/pytilpack/csv_.py` & `pytilpack-0.4.0/pytilpack/csv_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.3.0/pytilpack/openai_.py` & `pytilpack-0.4.0/pytilpack/openai_.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,96 @@
 """OpenAI Python Library用のユーティリティ集。"""
 
 import logging
+import typing
 
 import openai
 import openai.types.chat
 
 import pytilpack.python_
 
 logger = logging.getLogger(__name__)
 
 
 def gather_chunks(
-    chunks: list[openai.types.chat.ChatCompletionChunk],
+    chunks: typing.Iterable[openai.types.chat.ChatCompletionChunk],
 ) -> openai.types.chat.ChatCompletion:
     """ストリーミングのチャンクを結合する。"""
+    chunks = list(chunks)
+    if len(chunks) == 0:
+        return openai.types.chat.ChatCompletion(
+            id="", choices=[], created=0, model="", object="chat.completion"
+        )
     max_choices = max(len(chunk.choices) for chunk in chunks)
     choices = [_make_choice(chunks, i) for i in range(max_choices)]
-    return openai.types.chat.ChatCompletion(
+    response = openai.types.chat.ChatCompletion(
         id=chunks[0].id,
         choices=choices,
         created=chunks[0].created,
         model=chunks[0].model,
         object="chat.completion",
-        system_fingerprint=pytilpack.python_.coalesce(
-            c.system_fingerprint for c in chunks
-        ),
     )
+    if (
+        system_fingerprint := pytilpack.python_.coalesce(
+            c.system_fingerprint for c in chunks
+        )
+    ) is not None:
+        response.system_fingerprint = system_fingerprint
+    return response
 
 
 def _make_choice(
     chunks: list[openai.types.chat.ChatCompletionChunk], i: int
 ) -> openai.types.chat.chat_completion.Choice:
     """ストリーミングのチャンクからChoiceを作成する。"""
-    logprobs = pytilpack.python_.coalesce(
-        c.choices[i].logprobs for c in chunks if len(c.choices) >= i
-    )
-    return openai.types.chat.chat_completion.Choice(
+    message = openai.types.chat.ChatCompletionMessage(role="assistant")
+    if (
+        len(
+            content := pytilpack.python_.remove_none(
+                c.choices[i].delta.content for c in chunks if len(c.choices) >= i
+            )
+        )
+        > 0
+    ):
+        message.content = "".join(content)
+    if (
+        len(
+            function_calls := pytilpack.python_.remove_none(
+                c.choices[i].delta.function_call for c in chunks if len(c.choices) >= i
+            )
+        )
+        > 0
+    ):
+        message.function_call = _make_function_call(function_calls)
+    if (
+        len(
+            tool_calls_list := pytilpack.python_.remove_none(
+                c.choices[i].delta.tool_calls for c in chunks if len(c.choices) >= i
+            )
+        )
+        > 0
+    ):
+        message.tool_calls = _make_tool_calls(tool_calls_list)
+
+    choice = openai.types.chat.chat_completion.Choice(
         finish_reason=pytilpack.python_.coalesce(
             (c.choices[i].finish_reason for c in chunks if len(c.choices) >= i), "stop"
         ),
         index=i,
-        logprobs=(
-            None
-            if logprobs is None
-            else openai.types.chat.chat_completion.ChoiceLogprobs(
-                content=logprobs.content
-            )
-        ),
-        message=openai.types.chat.ChatCompletionMessage(
-            content="".join(
-                pytilpack.python_.remove_none(
-                    c.choices[i].delta.content for c in chunks if len(c.choices) >= i
-                )
-            ),
-            # role=pytilpack.python_.coalesce(
-            #     (c.choices[i].delta.role for c in chunks if len(c.choices) >= i),
-            #     "assistant",
-            # ),
-            role="assistant",
-            function_call=_make_function_call(
-                pytilpack.python_.remove_none(
-                    c.choices[i].delta.function_call
-                    for c in chunks
-                    if len(c.choices) >= i
-                )
-            ),
-            tool_calls=_make_tool_calls(
-                pytilpack.python_.remove_none(
-                    c.choices[i].delta.tool_calls for c in chunks if len(c.choices) >= i
-                )
-            ),
-        ),
+        message=message,
     )
+    if (
+        logprobs := pytilpack.python_.coalesce(
+            c.choices[i].logprobs for c in chunks if len(c.choices) >= i
+        )
+    ) is not None:
+        choice.logprobs = openai.types.chat.chat_completion.ChoiceLogprobs(
+            content=logprobs.content
+        )
+    return choice
 
 
 def _make_function_call(
     deltas: list[openai.types.chat.chat_completion_chunk.ChoiceDeltaFunctionCall],
 ) -> openai.types.chat.chat_completion_message.FunctionCall | None:
     """ChoiceDeltaFunctionCallを作成する。"""
     if len(deltas) == 0:
```

### Comparing `pytilpack-0.3.0/pytilpack/pathlib_.py` & `pytilpack-0.4.0/pytilpack/pathlib_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.3.0/pytilpack/python_.py` & `pytilpack-0.4.0/pytilpack/python_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.3.0/pytilpack/sqlalchemy_.py` & `pytilpack-0.4.0/pytilpack/sqlalchemy_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.3.0/pytilpack/tiktoken_.py` & `pytilpack-0.4.0/pytilpack/tiktoken_.py`

 * *Files identical despite different names*

### Comparing `pytilpack-0.3.0/pytilpack/tqdm_.py` & `pytilpack-0.4.0/pytilpack/tqdm_.py`

 * *Files identical despite different names*

