# Comparing `tmp/llama_cpp_agent-0.1.4.tar.gz` & `tmp/llama_cpp_agent-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_cpp_agent-0.1.4.tar", last modified: Tue May  7 18:10:28 2024, max compression
+gzip compressed data, was "llama_cpp_agent-0.2.0.tar", last modified: Sun May 12 16:24:11 2024, max compression
```

## Comparing `llama_cpp_agent-0.1.4.tar` & `llama_cpp_agent-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.579935 llama_cpp_agent-0.1.4/
--rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama_cpp_agent-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    10696 2024-05-07 18:10:28.578935 llama_cpp_agent-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     9639 2024-05-07 18:09:11.000000 llama_cpp_agent-0.1.4/ReadMe.md
--rw-rw-rw-   0        0        0      990 2024-05-07 18:09:11.000000 llama_cpp_agent-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-07 18:10:28.579935 llama_cpp_agent-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.543169 llama_cpp_agent-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.558793 llama_cpp_agent-0.1.4/src/llama_cpp_agent/
--rw-rw-rw-   0        0        0        0 2024-01-04 14:13:41.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.569317 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/
--rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/__init__.py
--rw-rw-rw-   0        0        0     3408 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/core_memory_manager.py
--rw-rw-rw-   0        0        0     1636 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/event_memory.py
--rw-rw-rw-   0        0        0     3876 2024-05-05 05:07:17.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/event_memory_manager.py
--rw-rw-rw-   0        0        0     9949 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/memory_tools.py
--rw-rw-rw-   0        0        0     5031 2024-04-18 21:27:19.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/retrieval_memory.py
--rw-rw-rw-   0        0        0     1640 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
--rw-rw-rw-   0        0        0    13499 2024-05-06 00:08:47.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/chain.py
--rw-rw-rw-   0        0        0    31285 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/function_calling.py
--rw-rw-rw-   0        0        0    19446 2024-05-05 20:26:45.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/function_calling_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.570316 llama_cpp_agent-0.1.4/src/llama_cpp_agent/gbnf_grammar_generator/
--rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
--rw-rw-rw-   0        0        0    71258 2024-05-05 20:17:35.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
--rw-rw-rw-   0        0        0    13437 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/hermes_2_pro_agent.py
--rw-rw-rw-   0        0        0    73714 2024-05-05 20:17:35.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/llm_agent.py
--rw-rw-rw-   0        0        0     7027 2024-03-29 17:24:31.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/llm_prompt_template.py
--rw-rw-rw-   0        0        0     6022 2024-05-01 05:39:37.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/llm_settings.py
--rw-rw-rw-   0        0        0     8664 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/messages.py
--rw-rw-rw-   0        0        0    22118 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/messages_formatter.py
--rw-rw-rw-   0        0        0     4313 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/mixtral_8x22b_agent.py
--rw-rw-rw-   0        0        0     3613 2024-04-18 21:27:19.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/output_parser.py
-drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.574440 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/
--rw-rw-rw-   0        0        0        0 2024-01-08 13:25:58.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/__init__.py
--rw-rw-rw-   0        0        0     7135 2024-05-05 05:07:17.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py
--rw-rw-rw-   0        0        0    14586 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py
--rw-rw-rw-   0        0        0     9740 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/openai_endpoint_provider.py
--rw-rw-rw-   0        0        0    10078 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/provider_base.py
-drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.577423 llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/
--rw-rw-rw-   0        0        0        0 2024-05-05 05:07:17.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/__init__.py
--rw-rw-rw-   0        0        0     2359 2024-05-05 05:07:17.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/rag_colbert_reranker.py
--rw-rw-rw-   0        0        0     3945 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/text_utils.py
--rw-rw-rw-   0        0        0    11126 2024-05-05 20:17:34.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent/structured_output_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-07 18:10:28.577930 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/
--rw-rw-rw-   0        0        0    10696 2024-05-07 18:10:28.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1645 2024-05-07 18:10:28.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 18:10:28.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2024-05-07 18:10:28.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-07 18:10:28.000000 llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.305178 llama_cpp_agent-0.2.0/
+-rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama_cpp_agent-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    10017 2024-05-12 16:24:11.304177 llama_cpp_agent-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8792 2024-05-12 16:23:39.000000 llama_cpp_agent-0.2.0/ReadMe.md
+-rw-rw-rw-   0        0        0     1054 2024-05-12 16:23:39.000000 llama_cpp_agent-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 16:24:11.305178 llama_cpp_agent-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.251598 llama_cpp_agent-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.271722 llama_cpp_agent-0.2.0/src/llama_cpp_agent/
+-rw-rw-rw-   0        0        0      342 2024-05-12 15:02:27.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.281765 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/
+-rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/__init__.py
+-rw-rw-rw-   0        0        0     3408 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/core_memory_manager.py
+-rw-rw-rw-   0        0        0     1654 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/event_memory.py
+-rw-rw-rw-   0        0        0     3882 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/event_memory_manager.py
+-rw-rw-rw-   0        0        0     9949 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/memory_tools.py
+-rw-rw-rw-   0        0        0     5031 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/retrieval_memory.py
+-rw-rw-rw-   0        0        0     1640 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+-rw-rw-rw-   0        0        0    12570 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chain.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.286499 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/
+-rw-rw-rw-   0        0        0      307 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/__init__.py
+-rw-rw-rw-   0        0        0     6999 2024-05-12 00:16:58.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/basic_chat_history.py
+-rw-rw-rw-   0        0        0     1834 2024-05-12 00:07:51.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/chat_history_base.py
+-rw-rw-rw-   0        0        0     3144 2024-05-12 11:29:01.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/messages.py
+-rw-rw-rw-   0        0        0    10771 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/function_calling.py
+-rw-rw-rw-   0        0        0    12448 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/function_calling_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.288169 llama_cpp_agent-0.2.0/src/llama_cpp_agent/gbnf_grammar_generator/
+-rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
+-rw-rw-rw-   0        0        0    52886 2024-05-11 21:21:16.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+-rw-rw-rw-   0        0        0    13675 2024-05-12 13:59:03.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/hermes_2_pro_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.290177 llama_cpp_agent-0.2.0/src/llama_cpp_agent/json_schema_generator/
+-rw-rw-rw-   0        0        0       53 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/json_schema_generator/__init__.py
+-rw-rw-rw-   0        0        0    11683 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/json_schema_generator/schema_generator.py
+-rw-rw-rw-   0        0        0    21379 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.292177 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_documentation/
+-rw-rw-rw-   0        0        0      116 2024-05-09 08:09:41.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_documentation/__init__.py
+-rw-rw-rw-   0        0        0    18850 2024-05-12 00:42:14.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_documentation/documentation_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.294177 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_output_settings/
+-rw-rw-rw-   0        0        0       76 2024-05-09 12:50:53.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_output_settings/__init__.py
+-rw-rw-rw-   0        0        0    32939 2024-05-12 05:26:57.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_output_settings/settings.py
+-rw-rw-rw-   0        0        0     7027 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_prompt_template.py
+-rw-rw-rw-   0        0        0    22304 2024-05-12 04:37:01.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/messages_formatter.py
+-rw-rw-rw-   0        0        0     3990 2024-05-12 13:53:06.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/mixtral_8x22b_agent.py
+-rw-rw-rw-   0        0        0     3613 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/output_parser.py
+-rw-rw-rw-   0        0        0     5296 2024-05-12 04:02:32.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/prompt_templates.py
+-rw-rw-rw-   0        0        0      816 2024-05-12 03:46:37.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/prompts.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.300177 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/
+-rw-rw-rw-   0        0        0      277 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/__init__.py
+-rw-rw-rw-   0        0        0     8076 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/llama_cpp_python.py
+-rw-rw-rw-   0        0        0    13772 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/llama_cpp_server.py
+-rw-rw-rw-   0        0        0     5392 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/provider_base.py
+-rw-rw-rw-   0        0        0     9067 2024-05-12 03:32:34.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/tgi_server.py
+-rw-rw-rw-   0        0        0     6607 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/vllm_server.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.302177 llama_cpp_agent-0.2.0/src/llama_cpp_agent/rag/
+-rw-rw-rw-   0        0        0        0 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/rag/__init__.py
+-rw-rw-rw-   0        0        0     2359 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/rag/rag_colbert_reranker.py
+-rw-rw-rw-   0        0        0     7073 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/structured_output_agent.py
+-rw-rw-rw-   0        0        0     3945 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/text_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.302177 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/
+-rw-rw-rw-   0        0        0    10017 2024-05-12 16:24:11.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2187 2024-05-12 16:24:11.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 16:24:11.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      206 2024-05-12 16:24:11.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-12 16:24:11.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/top_level.txt
```

### Comparing `llama_cpp_agent-0.1.4/LICENSE` & `llama_cpp_agent-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.4/PKG-INFO` & `llama_cpp_agent-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.1.4
+Version: 0.2.0
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,18 @@
 Provides-Extra: agent-memory
 Requires-Dist: chromadb; extra == "agent-memory"
 Requires-Dist: SQLAlchemy; extra == "agent-memory"
 Requires-Dist: numpy; extra == "agent-memory"
 Requires-Dist: scipy; extra == "agent-memory"
 Provides-Extra: rag
 Requires-Dist: ragatouille; extra == "rag"
+Provides-Extra: vllm-provider
+Requires-Dist: openai; extra == "vllm-provider"
+Provides-Extra: mixtral-agent
+Requires-Dist: mistral-common; extra == "mixtral-agent"
 
 # llama-cpp-agent
 
 <img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
 
 ## Table of Contents
 - [Introduction](#introduction)
@@ -48,62 +52,41 @@
     - [Predefined Messages Formatter](#predefined-messages-formatter)
     - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
 - [Contributing](#contributing)
 - [License](#license)
 - [FAQ](#faq)
 
 ## Introduction
-The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. The framework integrates seamlessly with the llama.cpp server, llama-cpp-python and OpenAI endpoints that support grammar, offering flexibility and extensibility.
+The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
+
+The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
+
+The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
 
 ## Key Features
 - **Simple Chat Interface**: Engage in seamless conversations with LLMs.
 - **Structured Output**: Generate structured output (objects) from LLMs.
 - **Single and Parallel Function Calling**: Execute functions using LLMs.
 - **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
 - **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
-- **Compatibility**: Works with llama-index tools and OpenAI tool schemas.
+- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
+- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
+- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
 - **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
 
 ## Installation
 Install the llama-cpp-agent framework using pip:
 ```shell
 pip install llama-cpp-agent
 ```
 ## Documentation
 You can find the latest documentation [here!](https://llama-cpp-agent.readthedocs.io/en/latest/)
 
 ## Getting Started
-1. Ensure you have the required dependencies installed, including pydantic and llama-cpp-python.
-2. Import the necessary classes and functions from the llama-cpp-agent framework.
-3. Set up your LLM provider (e.g., llama-cpp-python Llama class, OpenAI endpoint with grammar support like llama-cpp-python server, or llama.cpp server).
-4. Create an instance of the desired agent class (e.g., LlamaCppAgent, FunctionCallingAgent, StructuredOutputAgent).
-5. Interact with the agent using the provided methods and examples.
-
-Here's a basic example of using the LlamaCppAgent for a simple chat:
-
-```python
-from llama_cpp_agent.llm_agent import LlamaCppAgent
-from llama_cpp_agent.messages_formatter import MessagesFormatterType
-from llama_cpp_agent.providers.llama_cpp_endpoint_provider import LlamaCppEndpointSettings
-
-main_model = LlamaCppEndpointSettings(
-    completions_endpoint_url="http://127.0.0.1:8080/completion"
-)
-
-llama_cpp_agent = LlamaCppAgent(main_model, debug_output=False,
-                                system_prompt="You are Dolphin, an uncensored and unbiased AI assistant.",
-                                predefined_messages_formatter_type=MessagesFormatterType.CHATML)
-
-while True:
-    user_input = input("User: ")
-    if user_input == "exit":
-        break
-    user_input = llama_cpp_agent.get_chat_response(user_input, temperature=0.7)
-    print("AI: " + user_input)
-```
+You can find the get started guide [here!](https://llama-cpp-agent.readthedocs.io/en/latest/get-started/)
 
 ## Discord Community
 Join the Discord Community [here](https://discord.gg/6tGznupZGX)
 
 ## Usage Examples
 The llama-cpp-agent framework provides a wide range of examples demonstrating its capabilities. Here are some key examples:
```

### Comparing `llama_cpp_agent-0.1.4/ReadMe.md` & `llama_cpp_agent-0.2.0/ReadMe.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,62 +22,41 @@
     - [Predefined Messages Formatter](#predefined-messages-formatter)
     - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
 - [Contributing](#contributing)
 - [License](#license)
 - [FAQ](#faq)
 
 ## Introduction
-The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. The framework integrates seamlessly with the llama.cpp server, llama-cpp-python and OpenAI endpoints that support grammar, offering flexibility and extensibility.
+The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
+
+The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
+
+The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
 
 ## Key Features
 - **Simple Chat Interface**: Engage in seamless conversations with LLMs.
 - **Structured Output**: Generate structured output (objects) from LLMs.
 - **Single and Parallel Function Calling**: Execute functions using LLMs.
 - **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
 - **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
-- **Compatibility**: Works with llama-index tools and OpenAI tool schemas.
+- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
+- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
+- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
 - **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
 
 ## Installation
 Install the llama-cpp-agent framework using pip:
 ```shell
 pip install llama-cpp-agent
 ```
 ## Documentation
 You can find the latest documentation [here!](https://llama-cpp-agent.readthedocs.io/en/latest/)
 
 ## Getting Started
-1. Ensure you have the required dependencies installed, including pydantic and llama-cpp-python.
-2. Import the necessary classes and functions from the llama-cpp-agent framework.
-3. Set up your LLM provider (e.g., llama-cpp-python Llama class, OpenAI endpoint with grammar support like llama-cpp-python server, or llama.cpp server).
-4. Create an instance of the desired agent class (e.g., LlamaCppAgent, FunctionCallingAgent, StructuredOutputAgent).
-5. Interact with the agent using the provided methods and examples.
-
-Here's a basic example of using the LlamaCppAgent for a simple chat:
-
-```python
-from llama_cpp_agent.llm_agent import LlamaCppAgent
-from llama_cpp_agent.messages_formatter import MessagesFormatterType
-from llama_cpp_agent.providers.llama_cpp_endpoint_provider import LlamaCppEndpointSettings
-
-main_model = LlamaCppEndpointSettings(
-    completions_endpoint_url="http://127.0.0.1:8080/completion"
-)
-
-llama_cpp_agent = LlamaCppAgent(main_model, debug_output=False,
-                                system_prompt="You are Dolphin, an uncensored and unbiased AI assistant.",
-                                predefined_messages_formatter_type=MessagesFormatterType.CHATML)
-
-while True:
-    user_input = input("User: ")
-    if user_input == "exit":
-        break
-    user_input = llama_cpp_agent.get_chat_response(user_input, temperature=0.7)
-    print("AI: " + user_input)
-```
+You can find the get started guide [here!](https://llama-cpp-agent.readthedocs.io/en/latest/get-started/)
 
 ## Discord Community
 Join the Discord Community [here](https://discord.gg/6tGznupZGX)
 
 ## Usage Examples
 The llama-cpp-agent framework provides a wide range of examples demonstrating its capabilities. Here are some key examples:
```

### Comparing `llama_cpp_agent-0.1.4/pyproject.toml` & `llama_cpp_agent-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [  "setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llama-cpp-agent"
-version = "0.1.4"
+version = "0.2.0"
 description = "A framework for building LLM based AI agents with llama.cpp."
 
 readme = "ReadMe.md"
 dependencies = [
     "llama-cpp-python>=0.2.60",
     "pydantic>=2.5.3",
     "requests>=2.31.0",
@@ -22,14 +22,16 @@
 name = "Maximilian Winter"
 email = "maximilian.winter.91@gmail.com"
 
 
 [project.optional-dependencies]
 agent_memory = ["chromadb", "SQLAlchemy", "numpy", "scipy"]
 rag = ["ragatouille"]
+vllm_provider = ["openai"]
+mixtral_agent = ["mistral-common"]
 
 [project.urls]
 Homepage = "https://github.com/Maximilian-Winter/llama-cpp-agent"
 "Bug Tracker" = "https://github.com/Maximilian-Winter/llama-cpp-agent/issues"
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/core_memory_manager.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/core_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/event_memory.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/event_memory.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,18 +41,18 @@
         self.event_keywords = json.dumps(keywords)
 
     def to_dict(self):
         return {
             "event_type": self.event_type.value,
             "timestamp": self.timestamp.isoformat(),
             "content": self.content,
-            "metadata": self.metadata,
+            "event_keywords": self.event_keywords,
         }
 
     @staticmethod
     def from_dict(data):
         return Event(
             event_type=data["event_type"],
             timestamp=datetime.datetime.fromisoformat(data["timestamp"]),
             content=data["content"],
-            metadata=data["metadata"],
+            event_keywords=data["metadata"],
         )
```

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/event_memory_manager.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/event_memory_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         return messages
 
     def add_event_to_queue(self, event_type, content, metadata):
         new_event = Event(
             event_type=event_type,
             timestamp=datetime.datetime.now(),
             content=content,
-            metadata=json.dumps(metadata),
+            event_keywords=json.dumps(metadata),
         )
         self.event_queue.append(new_event)
 
         if len(self.event_queue) > self.event_queue_limit:
             self.commit_oldest_event()
 
     def commit_oldest_event(self):
```

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/memory_tools.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/memory_tools.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/retrieval_memory.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/retrieval_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/chain.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,94 +1,86 @@
 from typing import List, Callable
 
 from llama_cpp_agent.function_calling import LlamaCppFunctionTool
 from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.llm_output_settings import LlmStructuredOutputSettings
 from llama_cpp_agent.llm_prompt_template import PromptTemplate
+from llama_cpp_agent.providers.provider_base import LlmSamplingSettings
 
 
 class AgentChainElement:
     """
     Represents a single element in the chain of an agent-based framework. This element holds all necessary data to
     manage the prompt, process the input/output, and adjust the processing behavior based on given parameters.
 
     Attributes:
         output_identifier (str): Unique identifier for the output of this chain element.
         system_prompt (str): Template string for the system prompt.
         prompt (str): Template string for the main prompt to the language model.
-        grammar (str, optional): GBNF-Grammar to constrain the language model's output.
+
         preprocessor (Callable[[str, str, dict], tuple[str, str, dict]], optional): Function to preprocess the input
                 before sending it to the language model. Takes the system prompt with template fields replaced, the prompt
                 with template fields replaced, and the additional information dictionary as arguments and returns the
                 modified tuple of it.
         postprocessor (Callable[[str, str, dict, str], str], optional): Function to postprocess the output from
                 the language model. Takes the system prompt, the prompt, the additional information dictionary and the
                 result as arguments and returns the modified result.
         function_tool_registry (LlamaCppFunctionToolRegistry): Registry for LlamaCppFunctionTool and enables function calling.
         add_prompt_to_chat_history (bool): Flag to determine if the prompt should be added to the chat history.
         add_response_to_chat_history (bool): Flag to determine if the response should be added to the chat history.
-        temperature (float): Controls randomness in the generation process. Lower values make responses more deterministic.
-        top_p (float): Controls diversity via nucleus sampling: smaller values make responses more focused.
-        top_k (int): Controls diversity via top-k sampling: the number of highest probability vocabulary tokens considered.
+
     Methods:
         __init__: Constructs an instance of the AgentChain class.
     """
 
     def __init__(
         self,
         output_identifier: str,
         system_prompt: str,
         prompt: str,
         tools: List[LlamaCppFunctionTool] = None,
-        grammar: str = None,
+        structured_output_settings: LlmStructuredOutputSettings = None,
         preprocessor: Callable[[str, str, dict], tuple[str, str, dict]] = None,
         postprocessor: Callable[[str, str, dict, str], str] = None,
         add_prompt_to_chat_history: bool = False,
         add_response_to_chat_history: bool = False,
-        temperature: float = 0.35,
-        top_p: float = 1.0,
-        top_k: int = 0,
+        llm_sampling_settings: LlmSamplingSettings = None,
     ):
         """
         Constructs an instance of the AgentChainElement class.
 
         Args:
             output_identifier (str): Unique identifier for the output of this chain element.
             system_prompt (str): Template string for the system prompt.
             prompt (str): Template string for the main prompt to the language model.
             tools (List[LlamaCppFunctionTool], optional): List of function tools available for use in this chain element.
-            grammar (str, optional): GBNF-Grammar to constrain the language model's output.
             preprocessor (Callable[[str, str, dict], tuple[str, str, dict]], optional): Function to preprocess the input
                 before sending it to the language model. Takes the system prompt with template fields replaced, the prompt
                 with template fields replaced, and the additional information dictionary as arguments and returns the
                 modified tuple of it.
             postprocessor (Callable[[str, str, dict, str], str], optional): Function to postprocess the output from
                 the language model. Takes the system prompt, the prompt, the additional information dictionary and the
                 result as arguments and returns the modified result.
             add_prompt_to_chat_history (bool): Flag to determine if the prompt should be added to the chat history.
             add_response_to_chat_history (bool): Flag to determine if the response should be added to the chat history.
-            temperature (float): Controls randomness in the generation process. Lower values make responses more deterministic.
-            top_p (float): Controls diversity via nucleus sampling: smaller values make responses more focused.
-            top_k (int): Controls diversity via top-k sampling: the number of highest probability vocabulary tokens considered.
         """
         self.output_identifier = output_identifier
         self.system_prompt = system_prompt
         self.prompt = prompt
         self.add_prompt_to_chat_history = add_prompt_to_chat_history
         self.add_response_to_chat_history = add_response_to_chat_history
-        self.grammar = grammar
+        self.structured_output_settings = structured_output_settings
         self.preprocessor = preprocessor
         self.postprocessor = postprocessor
         self.function_tool_registry = None
         if tools is not None:
-            self.function_tool_registry = LlamaCppAgent.get_function_tool_registry(
-                tools
+            self.structured_output_settings = (
+                LlmStructuredOutputSettings.from_llama_cpp_function_tools(tools)
             )
-        self.temperature = temperature
-        self.top_p = top_p
-        self.top_k = top_k
+        self.llm_sampling_settings = llm_sampling_settings
 
 
 class AgentChain:
     """
     Represents a chain of AgentChainElements that are processed in a sequence to handle an interaction within an
     agent-based system.
 
@@ -141,31 +133,27 @@
                 sys_prompt, prompt, outputs = chain_element.preprocessor(
                     sys_prompt, prompt, outputs
                 )
 
             outputs[chain_element.output_identifier] = self.agent.get_chat_response(
                 user_message if user_message is not None else prompt,
                 system_prompt=sys_prompt,
-                penalize_nl=False,
-                temperature=chain_element.temperature,
-                top_p=chain_element.top_p,
-                top_k=chain_element.top_k,
-                function_tool_registry=chain_element.function_tool_registry,
-                grammar=chain_element.grammar,
+                structured_output_settings=chain_element.structured_output_settings,
                 add_response_to_chat_history=chain_element.add_response_to_chat_history,
                 add_message_to_chat_history=chain_element.add_prompt_to_chat_history,
+                llm_sampling_settings=chain_element.llm_sampling_settings,
             )
             if chain_element.function_tool_registry is not None:
                 outputs[chain_element.output_identifier] = outputs[
                     chain_element.output_identifier
                 ][0]["return_value"]
             if chain_element.postprocessor is not None:
-                outputs[chain_element.output_identifier] = (
-                    chain_element.postprocessor
-                ) = chain_element.postprocessor(
+                outputs[
+                    chain_element.output_identifier
+                ] = chain_element.postprocessor = chain_element.postprocessor(
                     sys_prompt,
                     prompt,
                     outputs,
                     outputs[chain_element.output_identifier],
                 )
         output = "\n".join(
             [val if isinstance(val, str) else str(val) for val in outputs.values()]
@@ -230,24 +218,22 @@
             user_message (str, optional): Initial user message to be included in the processing.
             additional_fields (dict, optional): Additional data to be used throughout the map and combine chains.
 
         Returns:
             tuple: A tuple containing the final output string from the combine chain and the outputs dictionary.
         """
         outputs = {}
-        if user_message is not None:
-            outputs["user_message"] = user_message
 
         if additional_fields is not None:
             for field, value in additional_fields.items():
                 outputs[field] = value
         else:
             additional_fields = {}
         results = []
         for item in items_to_map:
             additional_fields[self.item_identifier] = item
             result, result_dic = self.map_chain.run_chain(
-                additional_fields=additional_fields
+                user_message=user_message, additional_fields=additional_fields
             )
             results.append(result_dic[self.map_chain.chain[-1].output_identifier])
         additional_fields[self.map_output_identifier] = "\n\n".join(results)
         return self.combine_chain.run_chain(additional_fields=additional_fields)
```

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/hermes_2_pro_agent.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/hermes_2_pro_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,36 +6,24 @@
 from enum import Enum
 from typing import List, Dict, Literal, Tuple
 
 from llama_cpp import Llama
 from pydantic import ValidationError
 from transformers import AutoTokenizer
 
+from llama_cpp_agent.chat_history import ChatMessage, SystemMessage, UserMessage
+from llama_cpp_agent.chat_history.messages import convert_messages_to_list_of_dictionaries, ToolCall, FunctionCall, \
+    ToolMessage, AssistantMessage
 from llama_cpp_agent.function_calling import LlamaCppFunctionTool
 from llama_cpp_agent.llm_agent import LlamaCppAgent
+from llama_cpp_agent.llm_output_settings import LlmStructuredOutputSettings
 from llama_cpp_agent.llm_prompt_template import PromptTemplate
-from llama_cpp_agent.llm_settings import LlamaLLMSettings
-from llama_cpp_agent.messages import (
-    ToolCall,
-    FunctionCall,
-    ToolMessage,
-    AssistantMessage,
-    UserMessage,
-    ChatMessage,
-    convert_messages_to_list_of_dictionaries,
-    SystemMessage,
-)
-from llama_cpp_agent.messages_formatter import (
-    MessagesFormatterType,
-    get_predefined_messages_formatter,
-)
-from llama_cpp_agent.providers.llama_cpp_endpoint_provider import (
-    LlamaCppEndpointSettings,
-)
-from llama_cpp_agent.providers.openai_endpoint_provider import OpenAIEndpointSettings
+from llama_cpp_agent.messages_formatter import MessagesFormatter
+
+from llama_cpp_agent.providers.provider_base import LlmProvider
 
 
 def generate_id(length=8):
     # Characters to use in the ID
     characters = string.ascii_letters + string.digits
     # Random choice of characters
     return "".join(random.choice(characters) for _ in range(length))
@@ -59,23 +47,28 @@
             json_dicts.append(json_dict)
         except json.JSONDecodeError as e:
             print(f"Error decoding JSON: {e}")
 
     return json_dicts
 
 
-class Hermes2ProMessageFormatter:
+class Hermes2ProMessageFormatter(MessagesFormatter):
     """
     Class representing a messages formatter for LLMs.
     """
 
-    def __init__(self):
+    def __init__(self, PRE_PROMPT: str = "", SYS_PROMPT_START: str = "", SYS_PROMPT_END: str = "", USER_PROMPT_START: str = "",
+                 USER_PROMPT_END: str = "", ASSISTANT_PROMPT_START: str = "", ASSISTANT_PROMPT_END: str = "",
+                 INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE: bool = False, DEFAULT_STOP_SEQUENCES: List[str] = None):
         """
         Initializes a new MessagesFormatter object.
         """
+        super().__init__(PRE_PROMPT, SYS_PROMPT_START, SYS_PROMPT_END, USER_PROMPT_START, USER_PROMPT_END,
+                         ASSISTANT_PROMPT_START, ASSISTANT_PROMPT_END, INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE,
+                         DEFAULT_STOP_SEQUENCES)
         SYS_PROMPT_START_MIXTRAL = """"""
         SYS_PROMPT_END_MIXTRAL = """\n\n"""
         USER_PROMPT_START_MIXTRAL = """[INST] """
         USER_PROMPT_END_MIXTRAL = """ """
         ASSISTANT_PROMPT_START_MIXTRAL = """[/INST] """
         ASSISTANT_PROMPT_END_MIXTRAL = """</s>"""
         FUNCTION_PROMPT_START_MIXTRAL = """"""
@@ -90,16 +83,15 @@
         self.ASSISTANT_PROMPT_END = "<|im_end|>\n"
         self.INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE = False
 
         self.DEFAULT_STOP_SEQUENCES = [
             "<|im_end|>",
             "<|im_start|>assistant",
             "<|im_start|>user",
-            "<|im_start|>system",
-            "<|im_start|>tool",
+            "<|im_start|>system"
         ]
         self.FUNCTION_PROMPT_START = "<|im_start|>tool\n"
         self.FUNCTION_PROMPT_END = "<|im_end|>\n"
         self.USE_USER_ROLE_FUNCTION_CALL_RESULT = False
         self.STRIP_PROMPT = True
 
     def format_messages(
@@ -217,71 +209,63 @@
             else:
                 return formatted_messages + self.USER_PROMPT_START, "user"
 
 
 class Hermes2ProAgent:
     def __init__(
         self,
-        model: (
-            Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings
-        ),
+        provider: LlmProvider,
         system_prompt: str = None,
         debug_output: bool = False,
     ):
         self.messages: list[ChatMessage] = []
-        self.agent = LlamaCppAgent(model, debug_output=debug_output)
+        self.messages_formatter = Hermes2ProMessageFormatter()
+        self.agent = LlamaCppAgent(provider, debug_output=debug_output, custom_messages_formatter=self.messages_formatter)
         self.debug_output = debug_output
         if system_prompt is not None:
             self.system_prompt = system_prompt
         else:
             self.system_prompt = "You are a function calling AI model. You are provided with function signatures within <tools></tools> XML tags. You may call one or more functions to assist with the user query. Don't make assumptions about what values to plug into functions.\nHere are the available tools:"
         self.messages.append(SystemMessage(content="system_prompt"))
-        self.messages_formatter = Hermes2ProMessageFormatter()
+
         self.sys_prompt_template = """{system_prompt} <tools> {tools} </tools>
 Use the following pydantic model json schema for each tool call you will make: {"properties": {"arguments": {"title": "Arguments", "type": "object"}, "name": {"title": "Name", "type": "string"}}, "required": ["arguments", "name"], "title": "FunctionCall", "type": "object"} 
 For each function call return a json object with function name and arguments within <tool_call></tool_call> XML tags as follows:
 <tool_call>
 {"arguments": <args-dict>, "name": <function-name>}
 </tool_call>
 """
         self.system_prompter = PromptTemplate.from_string(self.sys_prompt_template)
 
     def get_response(
         self,
         message=None,
-        tools: list[LlamaCppFunctionTool] = None,
-        temperature=0.7,
-        top_p=1.0,
+        structured_output_settings: LlmStructuredOutputSettings = None,
     ):
-        if tools is None:
-            tools = []
         if message is not None:
             msg = UserMessage(content=message)
             self.messages.append(msg)
         openai_tools = []
         openai_tool_mapping = {}
-        for tool in tools:
+        for tool in structured_output_settings.function_tools:
             openai_tools.append(tool.to_openai_tool())
             openai_tool_mapping[tool.model.__name__] = tool
 
         self.messages[0].content = self.system_prompter.generate_prompt(
             {"tools": json.dumps(openai_tools), "system_prompt": self.system_prompt}
         )
         text, role = self.messages_formatter.format_messages(
             convert_messages_to_list_of_dictionaries(self.messages)
         )
 
         if self.debug_output:
             print(text)
         result = self.agent.get_text_response(
             text,
-            temperature=temperature,
-            top_p=top_p,
-            stop_sequences=self.messages_formatter.DEFAULT_STOP_SEQUENCES,
-            stream=self.debug_output,
+
             print_output=self.debug_output,
         )
 
         if "<tool_call>" in result:
             tool_calls = []
             if result.strip().endswith("</tool_call"):
                 result += ">"
@@ -313,11 +297,11 @@
                         AssistantMessage(content=result, tool_calls=tool_calls)
                     )
                     self.messages.extend(tool_messages)
             self.messages.append(
                 AssistantMessage(content=result, tool_calls=tool_calls)
             )
             self.messages.extend(tool_messages)
-            return self.get_response(tools=tools)
+            return self.get_response(structured_output_settings=structured_output_settings)
         else:
             self.messages.append(AssistantMessage(content=result.strip()))
             return result.strip()
```

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/llm_prompt_template.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_prompt_template.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/messages_formatter.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/messages_formatter.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from enum import Enum
 from typing import List, Dict, Tuple, Literal
 
 SYS_PROMPT_START_MIXTRAL = """"""
 SYS_PROMPT_END_MIXTRAL = """\n\n"""
 USER_PROMPT_START_MIXTRAL = """[INST] """
 USER_PROMPT_END_MIXTRAL = """ """
-ASSISTANT_PROMPT_START_MIXTRAL = """[/INST] """
+ASSISTANT_PROMPT_START_MIXTRAL = """[/INST]"""
 ASSISTANT_PROMPT_END_MIXTRAL = """</s>"""
 FUNCTION_PROMPT_START_MIXTRAL = """"""
 FUNCTION_PROMPT_END_MIXTRAL = """"""
 DEFAULT_MIXTRAL_STOP_SEQUENCES = ["</s>"]
 
 MIXTRAL_8x22_TOOL_JINJA_TEMPLATE = "{{bos_token}}{% set user_messages = messages | selectattr('role', 'equalto', 'user') | list %}{% for message in messages %}{% if message['role'] == 'user' %}{% if message == user_messages[-1] %}{{ '[AVAILABLE_TOOLS]'}}{% for tool in tools %}{{ tool }}{% endfor %}{{ '[/AVAILABLE_TOOLS]'}}{{ '[INST]' + message['content'] + '[/INST]' }}{% else %}{{ '[INST]' + message['content'] + '[/INST]' }}{% endif %}{% elif message['role'] == 'assistant' %}{{ ' ' + message['content'] + ' ' + eos_token}}{% elif message['role'] == 'tool_results' %}{{'[TOOL_RESULTS]' + message['content']|string + '[/TOOL_RESULTS]'}}{% elif message['role'] == 'tool_calls' %}{{'[TOOL_CALLS]' + message['content']|string + eos_token}}{% endif %}{% endfor %}"
 MIXTRAL_8x22_DEFAULT_JINJA_TEMPLATE = "{{bos_token}}{% for message in messages %}{% if (message['role'] == 'user') != (loop.index0 % 2 == 0) %}{{ raise_exception('Conversation roles must alternate user/assistant/user/assistant/...') }}{% endif %}{% if message['role'] == 'user' %}{{ ' [INST] ' + message['content'] + ' [/INST]' }}{% elif message['role'] == 'assistant' %}{{ ' ' + message['content'] + ' ' + eos_token}}{% else %}{{ raise_exception('Only user and assistant roles are supported!') }}{% endif %}{% endfor %}"
@@ -174,14 +174,16 @@
         ASSISTANT_PROMPT_END: str,
         INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE: bool,
         DEFAULT_STOP_SEQUENCES: List[str],
         USE_USER_ROLE_FUNCTION_CALL_RESULT: bool = True,
         FUNCTION_PROMPT_START: str = "",
         FUNCTION_PROMPT_END: str = "",
         STRIP_PROMPT: bool = True,
+        BOS_TOKEN: str = "<s>",
+        EOS_TOKEN: str = "</s>"
     ):
         """
         Initializes a new MessagesFormatter object.
 
         Args:
             PRE_PROMPT (str): The pre-prompt content.
             SYS_PROMPT_START (str): The system prompt start.
@@ -208,14 +210,18 @@
             INCLUDE_SYS_PROMPT_IN_FIRST_USER_MESSAGE
         )
         self.DEFAULT_STOP_SEQUENCES = DEFAULT_STOP_SEQUENCES
         self.FUNCTION_PROMPT_START = FUNCTION_PROMPT_START
         self.FUNCTION_PROMPT_END = FUNCTION_PROMPT_END
         self.USE_USER_ROLE_FUNCTION_CALL_RESULT = USE_USER_ROLE_FUNCTION_CALL_RESULT
         self.STRIP_PROMPT = STRIP_PROMPT
+        self.BOS_TOKEN = BOS_TOKEN
+        self.EOS_TOKEN = EOS_TOKEN
+    def get_bos_token(self):
+        return self.BOS_TOKEN
 
     def format_messages(
         self,
         messages: List[Dict[str, str]],
         response_role: Literal["user", "assistant"] | None = None,
     ) -> Tuple[str, str]:
         """
@@ -256,15 +262,15 @@
                     message["content"] = message["content"].strip()
                 formatted_messages += (
                     self.ASSISTANT_PROMPT_START
                     + message["content"]
                     + self.ASSISTANT_PROMPT_END
                 )
                 last_role = "assistant"
-            elif message["role"] == "function":
+            elif message["role"] == "tool":
                 if isinstance(message["content"], list):
                     message["content"] = "\n".join(
                         [json.dumps(m, indent=2) for m in message["content"]]
                     )
                 if self.USE_USER_ROLE_FUNCTION_CALL_RESULT:
                     formatted_messages += (
                         self.USER_PROMPT_START
@@ -274,16 +280,16 @@
                     last_role = "user"
                 else:
                     formatted_messages += (
                         self.FUNCTION_PROMPT_START
                         + message["content"]
                         + self.FUNCTION_PROMPT_END
                     )
-                    last_role = "function"
-        if last_role == "system" or last_role == "user" or last_role == "function":
+                    last_role = "tool"
+        if last_role == "system" or last_role == "user" or last_role == "tool":
             if self.STRIP_PROMPT:
                 if response_role is not None:
                     if response_role == "assistant":
                         return (
                             formatted_messages + self.ASSISTANT_PROMPT_START.strip(),
                             "assistant",
                         )
```

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/mixtral_8x22b_agent.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/mixtral_8x22b_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,56 +10,49 @@
     SystemMessage,
     AssistantMessage,
     ToolMessage,
 )
 from mistral_common.protocol.instruct.request import ChatCompletionRequest
 from mistral_common.protocol.instruct.tool_calls import ToolCall, FunctionCall
 from mistral_common.tokens.tokenizers.mistral import MistralTokenizer
-from mistralai.client import MistralClient
+
 
 from llama_cpp_agent.function_calling import LlamaCppFunctionTool
 from llama_cpp_agent.llm_agent import LlamaCppAgent
-from llama_cpp_agent.llm_settings import LlamaLLMSettings
-from llama_cpp_agent.providers.llama_cpp_endpoint_provider import (
-    LlamaCppEndpointSettings,
-)
-from llama_cpp_agent.providers.openai_endpoint_provider import OpenAIEndpointSettings
+from llama_cpp_agent.providers.provider_base import LlmProvider, LlmSamplingSettings
 
 
 def generate_id(length=8):
     # Characters to use in the ID
     characters = string.ascii_letters + string.digits
     # Random choice of characters
     return "".join(random.choice(characters) for _ in range(length))
 
 
 class Mixtral8x22BAgent:
     def __init__(
         self,
-        model: (
-            Llama | LlamaLLMSettings | LlamaCppEndpointSettings | OpenAIEndpointSettings
-        ),
+        provider: LlmProvider,
         system_prompt: str = None,
         debug_output: bool = False,
     ):
         self.messages: list[
             SystemMessage | UserMessage | AssistantMessage | ToolMessage
         ] = []
-        self.agent = LlamaCppAgent(model, debug_output=debug_output)
+        self.agent = LlamaCppAgent(provider, debug_output=debug_output)
         self.debug_output = debug_output
         if system_prompt is not None:
             self.messages.append(SystemMessage(content=system_prompt))
         self.tokenizer_v3 = MistralTokenizer.v3()
 
     def get_response(
         self,
         message=None,
         tools: list[LlamaCppFunctionTool] = None,
-        temperature=0.7,
-        top_p=1.0,
+        llm_sampling_settings: LlmSamplingSettings = None,
     ):
         if tools is None:
             tools = []
         if message is not None:
             msg = UserMessage(content=message)
             self.messages.append(msg)
         mistral_tools = []
@@ -73,18 +66,16 @@
             model="open-mixtral-8x22b",
         )
         tokenized = self.tokenizer_v3.encode_chat_completion(request)
         tokens, text = tokenized.tokens, tokenized.text
         if self.debug_output:
             print(text)
         result = self.agent.get_text_response(
-            tokens,
-            temperature=temperature,
-            top_p=top_p,
-            stream=self.debug_output,
+            text,
+            llm_sampling_settings=llm_sampling_settings,
             print_output=self.debug_output,
         )
 
         if result.strip().startswith("[TOOL_CALLS]"):
             tool_calls = []
 
             result = result.replace("[TOOL_CALLS]", "")
```

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/output_parser.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/structured_output_agent.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,225 +1,153 @@
 import json
 from copy import copy
-from dataclasses import dataclass, field
-from typing import List, Optional, Union
+from typing import Type, Callable, Union
 
-import requests
+from llama_cpp import Llama
+from pydantic import BaseModel
 
+from .llm_agent import LlamaCppAgent, StreamingResponse
+from .llm_output_settings import LlmStructuredOutputSettings, LlmStructuredOutputType
+from .llm_prompt_template import PromptTemplate
+from .output_parser import extract_object_from_response
+from .messages_formatter import MessagesFormatterType, MessagesFormatter
 
-@dataclass
-class KoboldCppGenerationSettings:
-    max_context_length: int
-    max_length: int
-    prompt: str
-    rep_pen: float
-    rep_pen_range: int
-    sampler_order: List[int]
-    sampler_seed: int
-    stop_sequence: List[str]
-    temperature: float
-    tfs: float
-    top_a: float
-    top_k: int
-    top_p: float
-    min_p: float
-    typical: float
-    stream: bool = True
-    use_default_badwordsids: bool = False
-    dynatemp_range: float = 0
-    mirostat: Optional[int] = None
-    mirostat_tau: float = 0
-    mirostat_eta: float = 0
-    genkey: Optional[str] = None
-    grammar_retain_state: bool = False
-    memory: Optional[str] = None
-    trim_stop: bool = False
-    logit_bias: Optional[dict] = field(default_factory=dict)
 
-    def save(self, file_path: str):
-        """
-        Save the settings to a file.
-
-        Args:
-            file_path (str): The path to the file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(self.as_dict(), file, indent=4)
-
-    @staticmethod
-    def load_from_file(file_path: str) -> "KoboldCppGenerationSettings":
-        """
-        Load the settings from a file.
-
-        Args:
-            file_path (str): The path to the file.
-
-        Returns:
-            KoboldCppGenerationSettings: The loaded settings.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_settings = json.load(file)
-            return KoboldCppGenerationSettings(**loaded_settings)
-
-    @staticmethod
-    def load_from_dict(settings: dict) -> "KoboldCppGenerationSettings":
-        """
-        Load the settings from a dictionary.
-
-        Args:
-            settings (dict): The dictionary containing the settings.
-
-        Returns:
-            KoboldCppGenerationSettings: The loaded settings.
-        """
-        return KoboldCppGenerationSettings(**settings)
-
-    def as_dict(self) -> dict:
-        """
-        Convert the settings to a dictionary.
-
-        Returns:
-            dict: The dictionary representation of the settings.
-        """
-        return self.__dict__
+from .providers.provider_base import LlmProvider, LlmSamplingSettings
 
 
-@dataclass
-class KoboldCppEndpointSettings:
+class StructuredOutputAgent:
     """
-    Settings for interacting with the kobold.cpp server.
+    An agent that creates structured output based on pydantic models from unstructured text.
 
     Args:
-        completions_endpoint_url (str): The URL for the completions endpoint.
+        llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings]): An instance of Llama, LlamaLLMSettings, LlamaCppServerLLMSettings, OpenAIEndpointSettings as LLM.
+        llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppGenerationSettings, OpenAIGenerationSettings]): Generation settings for Llama or LlamaCppServer.
+        messages_formatter_type (MessagesFormatterType): Type of messages formatter.
+        custom_messages_formatter (MessagesFormatter): Custom messages formatter.
+        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+        debug_output (bool): Enable debug output.
 
     Attributes:
-        completions_endpoint_url (str): The URL for the completions endpoint.
+        llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppServerGenerationSettings]): Generation settings for Llama or LlamaCppServer.
+        grammar_cache (dict): Cache for generated grammars.
+        system_prompt_template (PromptTemplate): Template for the system prompt.
+        creation_prompt_template (PromptTemplate): Template for the creation prompt.
+        llama_cpp_agent (LlamaCppAgent): LlamaCppAgent instance for interaction.
+        streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
 
     Methods:
-        save(file_path: str): Save the settings to a file.
-        load_from_file(file_path: str) -> LlamaCppServerLLMSettings: Load the settings from a file.
-        load_from_dict(settings: dict) -> LlamaCppServerLLMSettings: Load the settings from a dictionary.
-        as_dict() -> dict: Convert the settings to a dictionary.
-        create_completion(prompt, grammar, generation_settings: LlamaCppServerGenerationSettings): Create a completion using the server.
+        save(file_path: str): Save the agent's state to a file.
+        load_from_file(file_path: str, llama_llm, streaming_callback) -> StructuredOutputAgent: Load the agent's state from a file.
+        load_from_dict(agent_dict: dict) -> StructuredOutputAgent: Load the agent's state from a dictionary.
+        as_dict() -> dict: Convert the agent's state to a dictionary.
+        create_object(model: Type[BaseModel], data: str = "") -> object: Create an object of the given model from the given data.
 
     """
 
-    completions_endpoint_url: str
-
-    def save(self, file_path: str):
-        """
-        Save the settings to a file.
-
-        Args:
-            file_path (str): The path to the file.
-        """
-        with open(file_path, "w", encoding="utf-8") as file:
-            json.dump(self.as_dict(), file, indent=4)
-
-    @staticmethod
-    def load_from_file(file_path: str) -> "KoboldCppEndpointSettings":
+    def __init__(
+        self,
+        llama_llm: LlmProvider,
+        messages_formatter_type: MessagesFormatterType = MessagesFormatterType.CHATML,
+        custom_messages_formatter: MessagesFormatter = None,
+        streaming_callback: Callable[[StreamingResponse], None] = None,
+        debug_output: bool = False,
+    ):
         """
-        Load the settings from a file.
+        Initialize the StructuredOutputAgent.
 
         Args:
-            file_path (str): The path to the file.
+            llama_llm (Union[Llama, LlamaLLMSettings, LlamaCppEndpointSettings, OpenAIEndpointSettings]): An instance of Llama, LlamaLLMSettings, or LlamaCppServerLLMSettings as LLM.
+            llama_generation_settings (Union[LlamaLLMGenerationSettings, LlamaCppGenerationSettings, OpenAIGenerationSettings]): Generation settings for Llama or LlamaCppServer or OpenAIEndpoint.
+            messages_formatter_type (MessagesFormatterType): Type of messages formatter.
+            custom_messages_formatter (MessagesFormatter): Custom messages formatter.
+            streaming_callback (Callable[[StreamingResponse], None]): Callback function for streaming responses.
+            debug_output (bool): Enable debug output.
+        """
+        self.grammar_cache = {}
+        self.system_prompt_template = PromptTemplate.from_string(
+            "You are an advanced AI agent. You are tasked to assist the user by creating structured output in JSON format.\n\n{documentation}"
+        )
+        self.creation_prompt_template = PromptTemplate.from_string(
+            "Create an JSON response based on the following input.\n\nInput:\n\n{user_input}"
+        )
 
-        Returns:
-            KoboldCppEndpointSettings: The loaded settings.
-        """
-        with open(file_path, "r", encoding="utf-8") as file:
-            loaded_settings = json.load(file)
-            return KoboldCppEndpointSettings(**loaded_settings)
+        self.llama_cpp_agent = LlamaCppAgent(
+            llama_llm,
+            debug_output=debug_output,
+            system_prompt="",
+            predefined_messages_formatter_type=messages_formatter_type,
+            custom_messages_formatter=custom_messages_formatter,
+        )
+        self.streaming_callback = streaming_callback
 
-    @staticmethod
-    def load_from_dict(settings: dict) -> "KoboldCppEndpointSettings":
+    def save(self, file_path: str):
         """
-        Load the settings from a dictionary.
+        Save the agent's state to a file.
 
         Args:
-            settings (dict): The dictionary containing the settings.
-
-        Returns:
-            KoboldCppEndpointSettings: The loaded settings.
+            file_path (str): The path to the file.
         """
-        return KoboldCppEndpointSettings(**settings)
+        with open(file_path, "w", encoding="utf-8") as file:
+            dic = copy(self.as_dict())
+            del dic["llama_cpp_agent"]
+            del dic["grammar_cache"]
+            del dic["system_prompt_template"]
+            del dic["creation_prompt_template"]
+            del dic["streaming_callback"]
+            dic["debug_output"] = self.llama_cpp_agent.debug_output
+            dic["llama_generation_settings"] = self.llama_generation_settings.as_dict()
+            dic[
+                "custom_messages_formatter"
+            ] = self.llama_cpp_agent.messages_formatter.as_dict()
+            json.dump(dic, file, indent=4)
 
     def as_dict(self) -> dict:
         """
-        Convert the settings to a dictionary.
+        Convert the agent's state to a dictionary.
 
         Returns:
-            dict: The dictionary representation of the settings.
+            dict: The dictionary representation of the agent's state.
         """
         return self.__dict__
 
-    def create_completion(
-        self, prompt, grammar, generation_settings: KoboldCppGenerationSettings
-    ):
+    def create_object(
+        self,
+        model: Type[BaseModel],
+        data: str = "",
+        llm_sampling_settings: LlmSamplingSettings = None,
+    ) -> object:
         """
-        Create a completion using the Llama.cpp server.
+        Creates an object of the given model from the given data.
 
         Args:
-            prompt: The input prompt.
-            grammar: The grammar for completion.
-            generation_settings (LlamaCppGenerationSettings): The generation settings.
+            model (Type[BaseModel]): The model to create the object from.
+            data (str): The data to create the object from.
 
         Returns:
-            dict or generator: The completion response.
+            object: The created object.
         """
-        if generation_settings.stream:
-            return self.get_response_stream(prompt, grammar, generation_settings)
-
-        headers = {"Content-Type": "application/json"}
-
-        data = generation_settings.as_dict()
-        data["prompt"] = prompt
-        data["grammar"] = grammar
-        data["mirostat"] = data["mirostat_mode"]
-        data["stop"] = data["stop_sequences"]
-        del data["mirostat_mode"]
-        del data["stop_sequences"]
-
-        response = requests.post(
-            self.completions_endpoint_url, headers=headers, json=data
-        )
-        data = response.json()
-
-        returned_data = {"choices": [{"text": data["content"]}]}
-        return returned_data
-
-    def get_response_stream(self, prompt, grammar, generation_settings):
-        headers = {"Content-Type": "application/json"}
-
-        data = copy(generation_settings.as_dict())
-        data["prompt"] = prompt
-        data["grammar"] = grammar
-        data["mirostat"] = data["mirostat_mode"]
-        data["stop_sequence"] = data["stop_sequences"]
-        del data["mirostat_mode"]
-        del data["stop_sequences"]
-        response = requests.post(
-            self.completions_endpoint_url,
-            headers=headers,
-            json=data,
-            stream=generation_settings.stream,
-        )
-
-        # Check if the request was successful
-        response.raise_for_status()
-
-        # Define a generator function to yield text chunks
-        def generate_text_chunks():
-            try:
-                decoded_chunk = ""
-                for chunk in response.iter_lines():
-                    if chunk:
-                        decoded_chunk += chunk.decode("utf-8")
-                        new_data = json.loads(decoded_chunk.replace("data: ", ""))
-                        returned_data = {"choices": [{"text": new_data["content"]}]}
-                        yield returned_data
-                        decoded_chunk = ""
-
-            except requests.exceptions.RequestException as e:
-                print(f"Request failed: {e}")
+        output_settings = LlmStructuredOutputSettings.from_pydantic_models(
+            [model], output_type=LlmStructuredOutputType.object_instance
+        )
 
-        return generate_text_chunks()
+        system_prompt = self.system_prompt_template.generate_prompt(
+            {
+                "documentation": output_settings.get_llm_documentation(
+                    self.llama_cpp_agent.provider
+                ).strip()
+            }
+        )
+        if data == "":
+            prompt = "Create a random JSON response based on the response model."
+        else:
+            prompt = self.creation_prompt_template.generate_prompt({"user_input": data})
+        response = self.llama_cpp_agent.get_chat_response(
+            prompt,
+            system_prompt=system_prompt,
+            add_response_to_chat_history=False,
+            add_message_to_chat_history=False,
+            streaming_callback=self.streaming_callback,
+            structured_output_settings=output_settings,
+            llm_sampling_settings=llm_sampling_settings,
+        )
+        return response
```

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/rag_colbert_reranker.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/rag/rag_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent/rag/text_utils.py` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent/text_utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import re
+
+
 class TextChunker:
     def __init__(self, text, chunk_size, overlap=0):
         """
         Initializes the TextChunker instance.
 
         Parameters:
             text (str): The text to be chunked.
@@ -32,17 +35,14 @@
             if self.chunk_size <= self.overlap:
                 raise ValueError(
                     "Overlap must be less than chunk size to prevent infinite loops."
                 )
         return chunks
 
 
-import re
-
-
 class RecursiveCharacterTextSplitter:
     def __init__(
         self,
         separators,
         chunk_size,
         chunk_overlap,
         length_function=len,
```

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/PKG-INFO` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.1.4
+Version: 0.2.0
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,14 +19,18 @@
 Provides-Extra: agent-memory
 Requires-Dist: chromadb; extra == "agent-memory"
 Requires-Dist: SQLAlchemy; extra == "agent-memory"
 Requires-Dist: numpy; extra == "agent-memory"
 Requires-Dist: scipy; extra == "agent-memory"
 Provides-Extra: rag
 Requires-Dist: ragatouille; extra == "rag"
+Provides-Extra: vllm-provider
+Requires-Dist: openai; extra == "vllm-provider"
+Provides-Extra: mixtral-agent
+Requires-Dist: mistral-common; extra == "mixtral-agent"
 
 # llama-cpp-agent
 
 <img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
 
 ## Table of Contents
 - [Introduction](#introduction)
@@ -48,62 +52,41 @@
     - [Predefined Messages Formatter](#predefined-messages-formatter)
     - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
 - [Contributing](#contributing)
 - [License](#license)
 - [FAQ](#faq)
 
 ## Introduction
-The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. The framework integrates seamlessly with the llama.cpp server, llama-cpp-python and OpenAI endpoints that support grammar, offering flexibility and extensibility.
+The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
+
+The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
+
+The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
 
 ## Key Features
 - **Simple Chat Interface**: Engage in seamless conversations with LLMs.
 - **Structured Output**: Generate structured output (objects) from LLMs.
 - **Single and Parallel Function Calling**: Execute functions using LLMs.
 - **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
 - **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
-- **Compatibility**: Works with llama-index tools and OpenAI tool schemas.
+- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
+- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
+- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
 - **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
 
 ## Installation
 Install the llama-cpp-agent framework using pip:
 ```shell
 pip install llama-cpp-agent
 ```
 ## Documentation
 You can find the latest documentation [here!](https://llama-cpp-agent.readthedocs.io/en/latest/)
 
 ## Getting Started
-1. Ensure you have the required dependencies installed, including pydantic and llama-cpp-python.
-2. Import the necessary classes and functions from the llama-cpp-agent framework.
-3. Set up your LLM provider (e.g., llama-cpp-python Llama class, OpenAI endpoint with grammar support like llama-cpp-python server, or llama.cpp server).
-4. Create an instance of the desired agent class (e.g., LlamaCppAgent, FunctionCallingAgent, StructuredOutputAgent).
-5. Interact with the agent using the provided methods and examples.
-
-Here's a basic example of using the LlamaCppAgent for a simple chat:
-
-```python
-from llama_cpp_agent.llm_agent import LlamaCppAgent
-from llama_cpp_agent.messages_formatter import MessagesFormatterType
-from llama_cpp_agent.providers.llama_cpp_endpoint_provider import LlamaCppEndpointSettings
-
-main_model = LlamaCppEndpointSettings(
-    completions_endpoint_url="http://127.0.0.1:8080/completion"
-)
-
-llama_cpp_agent = LlamaCppAgent(main_model, debug_output=False,
-                                system_prompt="You are Dolphin, an uncensored and unbiased AI assistant.",
-                                predefined_messages_formatter_type=MessagesFormatterType.CHATML)
-
-while True:
-    user_input = input("User: ")
-    if user_input == "exit":
-        break
-    user_input = llama_cpp_agent.get_chat_response(user_input, temperature=0.7)
-    print("AI: " + user_input)
-```
+You can find the get started guide [here!](https://llama-cpp-agent.readthedocs.io/en/latest/get-started/)
 
 ## Discord Community
 Join the Discord Community [here](https://discord.gg/6tGznupZGX)
 
 ## Usage Examples
 The llama-cpp-agent framework provides a wide range of examples demonstrating its capabilities. Here are some key examples:
```

### Comparing `llama_cpp_agent-0.1.4/src/llama_cpp_agent.egg-info/SOURCES.txt` & `llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,35 +4,46 @@
 src/llama_cpp_agent/__init__.py
 src/llama_cpp_agent/chain.py
 src/llama_cpp_agent/function_calling.py
 src/llama_cpp_agent/function_calling_agent.py
 src/llama_cpp_agent/hermes_2_pro_agent.py
 src/llama_cpp_agent/llm_agent.py
 src/llama_cpp_agent/llm_prompt_template.py
-src/llama_cpp_agent/llm_settings.py
-src/llama_cpp_agent/messages.py
 src/llama_cpp_agent/messages_formatter.py
 src/llama_cpp_agent/mixtral_8x22b_agent.py
 src/llama_cpp_agent/output_parser.py
+src/llama_cpp_agent/prompt_templates.py
+src/llama_cpp_agent/prompts.py
 src/llama_cpp_agent/structured_output_agent.py
+src/llama_cpp_agent/text_utils.py
 src/llama_cpp_agent.egg-info/PKG-INFO
 src/llama_cpp_agent.egg-info/SOURCES.txt
 src/llama_cpp_agent.egg-info/dependency_links.txt
 src/llama_cpp_agent.egg-info/requires.txt
 src/llama_cpp_agent.egg-info/top_level.txt
 src/llama_cpp_agent/agent_memory/__init__.py
 src/llama_cpp_agent/agent_memory/core_memory_manager.py
 src/llama_cpp_agent/agent_memory/event_memory.py
 src/llama_cpp_agent/agent_memory/event_memory_manager.py
 src/llama_cpp_agent/agent_memory/memory_tools.py
 src/llama_cpp_agent/agent_memory/retrieval_memory.py
 src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+src/llama_cpp_agent/chat_history/__init__.py
+src/llama_cpp_agent/chat_history/basic_chat_history.py
+src/llama_cpp_agent/chat_history/chat_history_base.py
+src/llama_cpp_agent/chat_history/messages.py
 src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
 src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+src/llama_cpp_agent/json_schema_generator/__init__.py
+src/llama_cpp_agent/json_schema_generator/schema_generator.py
+src/llama_cpp_agent/llm_documentation/__init__.py
+src/llama_cpp_agent/llm_documentation/documentation_generation.py
+src/llama_cpp_agent/llm_output_settings/__init__.py
+src/llama_cpp_agent/llm_output_settings/settings.py
 src/llama_cpp_agent/providers/__init__.py
-src/llama_cpp_agent/providers/kobold_cpp_endpoint_provider.py
-src/llama_cpp_agent/providers/llama_cpp_endpoint_provider.py
-src/llama_cpp_agent/providers/openai_endpoint_provider.py
+src/llama_cpp_agent/providers/llama_cpp_python.py
+src/llama_cpp_agent/providers/llama_cpp_server.py
 src/llama_cpp_agent/providers/provider_base.py
+src/llama_cpp_agent/providers/tgi_server.py
+src/llama_cpp_agent/providers/vllm_server.py
 src/llama_cpp_agent/rag/__init__.py
-src/llama_cpp_agent/rag/rag_colbert_reranker.py
-src/llama_cpp_agent/rag/text_utils.py
+src/llama_cpp_agent/rag/rag_colbert_reranker.py
```

