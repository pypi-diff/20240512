# Comparing `tmp/xorius-0.0.3.tar.gz` & `tmp/xorius-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xorius-0.0.3.tar", last modified: Fri Mar 22 09:25:00 2024, max compression
+gzip compressed data, was "xorius-0.0.4.tar", last modified: Sun May 12 04:46:21 2024, max compression
```

## Comparing `xorius-0.0.3.tar` & `xorius-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:25:00.345519 xorius-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-22 09:25:00.341519 xorius-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-22 09:24:55.000000 xorius-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-22 09:24:55.000000 xorius-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 09:25:00.345519 xorius-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:25:00.341519 xorius-0.0.3/xorius/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 09:24:55.000000 xorius-0.0.3/xorius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-03-22 09:24:55.000000 xorius-0.0.3/xorius/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:25:00.341519 xorius-0.0.3/xorius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-22 09:25:00.000000 xorius-0.0.3/xorius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-22 09:25:00.000000 xorius-0.0.3/xorius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 09:25:00.000000 xorius-0.0.3/xorius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-22 09:25:00.000000 xorius-0.0.3/xorius.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-22 09:25:00.000000 xorius-0.0.3/xorius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-22 09:25:00.000000 xorius-0.0.3/xorius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 04:46:21.149530 xorius-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-12 04:46:21.149530 xorius-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-12 04:46:16.000000 xorius-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-12 04:46:16.000000 xorius-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 04:46:21.149530 xorius-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 04:46:21.149530 xorius-0.0.4/xorius/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 04:46:16.000000 xorius-0.0.4/xorius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-12 04:46:16.000000 xorius-0.0.4/xorius/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 04:46:21.149530 xorius-0.0.4/xorius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-12 04:46:21.000000 xorius-0.0.4/xorius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-12 04:46:21.000000 xorius-0.0.4/xorius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 04:46:21.000000 xorius-0.0.4/xorius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 04:46:21.000000 xorius-0.0.4/xorius.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-12 04:46:21.000000 xorius-0.0.4/xorius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-12 04:46:21.000000 xorius-0.0.4/xorius.egg-info/top_level.txt
```

### Comparing `xorius-0.0.3/pyproject.toml` & `xorius-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 [project]
 name = "xorius"
-version = "0.0.3"
+version = "0.0.4"
 description = "A LLM-based agent."
 authors = [
     {name = "Linusp", email = "linusp1024@gmail.com"},
 ]
 dependencies = [
-    "openai>=1.0.0",
-    "langchain>=0.1.12",
-    "anthropic>=0.21.1",
-    "google-generativeai>=0.4.0",
-    "groq>=0.4.0",
     "pydantic",
     "click",
     "rich",
     "tiktoken",
+    "ullm>=0.1.3",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -81,8 +77,9 @@
     "venv",
 ]
 line-length = 100
 indent-width = 4
 
 [tool.ruff.lint]
 select = ["E", "F"]
+extend-select = ["I"]
 ignore = ["E201", "E202"]
```

### Comparing `xorius-0.0.3/xorius/cli.py` & `xorius-0.0.4/xorius/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,96 @@
+import json
+
 import click
-import openai
 import tiktoken
-from langchain.chat_models import ChatOpenAI
-from langchain.memory import ChatMessageHistory
-from langchain.schema import AIMessage, HumanMessage, SystemMessage
 from rich.console import Console
+from ullm import LanguageModel
 
 
-def num_tokens_from_messages(messages, model="gpt-3.5-turbo-0301"):
+def num_tokens_from_messages(messages):
     """Returns the number of tokens used by a list of messages."""
-    try:
-        encoding = tiktoken.encoding_for_model(model)
-    except KeyError:
-        encoding = tiktoken.get_encoding("cl100k_base")
-
-    if model == "gpt-3.5-turbo-0301":  # note: future models may deviate from this
-        num_tokens = 0
-        for message in messages:
-            num_tokens += 4  # every message follows <im_start>{role/name}\n{content}<im_end>\n
-            for key, value in message.items():
-                num_tokens += len(encoding.encode(value))
-                if key == "name":  # if there's a name, the role is omitted
-                    num_tokens += -1  # role is always required and always 1 token
-
-        return num_tokens
-    else:
-        raise NotImplementedError(
-            f"num_tokens_from_messages() is not presently implemented for model {model}.\n"
-            "See https://github.com/openai/openai-python/blob/main/chatml.md "
-            "for information on how messages are converted to tokens."
-        )
+    encoding = tiktoken.get_encoding("cl100k_base")
+    num_tokens = 0
+    for message in messages:
+        num_tokens += 4  # every message follows <im_start>{role/name}\n{content}<im_end>\n
+        for key, value in message.items():
+            num_tokens += len(encoding.encode(value))
+            if key == "name":  # if there's a name, the role is omitted
+                num_tokens += -1  # role is always required and always 1 token
+
+    return num_tokens
 
 
 def select_messages(messages, max_total_tokens=4096, max_output_tokens=1024):
     tokens_num = 0
     selected = []
     for message in messages[::-1]:
-        role = "system"
-        if isinstance(message, AIMessage):
-            role = "assistant"
-        elif isinstance(message, HumanMessage):
-            role = "user"
-
-        cur_token_num = num_tokens_from_messages([{"role": role, "content": message.content}])
+        role = message["role"]
+        content = (
+            message["content"]
+            if isinstance(message["content"], str)
+            else message["content"][0]["text"]
+        )
+        cur_token_num = num_tokens_from_messages([{"role": role, "content": content}])
         if tokens_num + cur_token_num + 2 + max_output_tokens > max_total_tokens:
             break
 
         selected.append(message)
         tokens_num += cur_token_num
 
     selected = selected[::-1]
-    if isinstance(selected[0], AIMessage):  # 确保第一条是用户消息
+    if selected[0]["role"] != "user":  # 确保第一条是用户消息
         selected = selected[1:]
 
     if not selected:  # 假设 messages 里最后一条是当前用户输入
-        selected = message[-1]
+        selected = [messages[-1]]
 
     return selected
 
 
 @click.command()
-@click.option("--api-key", required=True)
+@click.option("--model-config-file", required=True)
 @click.option("--temperature", type=float, default=0.7, show_default=True)
-@click.option("--max-tokens", type=int, default=512, show_default=True)
-@click.option("--proxy")
-def main(api_key, temperature, max_tokens, proxy):
+@click.option("--max-tokens", type=int, default=4096, show_default=True)
+@click.option("--max-output-tokens", type=int, default=512, show_default=True)
+def main(model_config_file, temperature, max_tokens, max_output_tokens):
     console = Console(width=100)
     console.print("[bold green]Xorius[/]: 你好，我是 [bold green]Xorius[/]，你的 AI 助手！\n")
 
-    system_message = SystemMessage(
-        content=(
-            "You are an AI assistant. Your name is xorius. "
-            "You can discuss any ideas and topics with your users, "
-            "and you will help your users solve their problems as much as you can."
-        ),
-    )
-    if proxy:
-        openai.proxy = proxy
+    model_config = json.load(open(model_config_file))
+    llm = LanguageModel.from_config(model_config)
 
-    max_total_tokens = 4096 - num_tokens_from_messages(
-        [{"role": "system", "content": system_message.content}]
+    system_message = (
+        "You are an AI assistant. Your name is xorius. "
+        "You can discuss any ideas and topics with your users, "
+        "and you will help your users solve their problems as much as you can."
     )
-    llm = ChatOpenAI(temperature=temperature, openai_api_key=api_key, max_tokens=max_tokens)
-    memory = ChatMessageHistory()
+    max_total_tokens = max_tokens - num_tokens_from_messages(
+        [{"role": "system", "content": system_message}]
+    )
+    memory = []
     while True:
         user_input = console.input("[bold red]You[/]: ").strip()
         if not user_input:
             continue
 
-        memory.add_user_message(user_input)
+        memory.append({"role": "user", "content": user_input})
 
         console.print()
         with console.status("[bold green]Thinking..."):
             messages = select_messages(
-                memory.messages, max_total_tokens=max_total_tokens, max_output_tokens=max_tokens
+                memory, max_total_tokens=max_total_tokens, max_output_tokens=max_output_tokens
             )
+            for m in messages:
+                print(m)
 
-            answer = llm([system_message] + messages).content.strip()
-            console.print(f"[bold green]Xorius[/]: {answer}\n")
-            memory.add_ai_message(answer)
+            answer = llm.chat(
+                messages,
+                system=system_message,
+                config={"temperature": temperature, "max_output_tokens": max_output_tokens},
+            )
+            console.print(f"[bold green]Xorius[/]: {answer.content}\n")
+            memory.append(answer.to_message().model_dump(exclude_none=True))
 
 
 if __name__ == "__main__":
     main()
```

