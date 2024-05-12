# Comparing `tmp/lfg_llama-1.3.2.tar.gz` & `tmp/lfg_llama-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.3.2.tar", last modified: Thu May  9 07:31:38 2024, max compression
+gzip compressed data, was "lfg_llama-1.3.3.tar", last modified: Sun May 12 07:32:58 2024, max compression
```

## Comparing `lfg_llama-1.3.2.tar` & `lfg_llama-1.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-09 07:31:38.732197 lfg_llama-1.3.2/
--rw-r--r--   0 ob907      (502) staff       (20)     1908 2024-05-09 07:31:38.732002 lfg_llama-1.3.2/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     1671 2024-05-09 07:31:10.000000 lfg_llama-1.3.2/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-09 07:31:38.730719 lfg_llama-1.3.2/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.3.2/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     3470 2024-05-09 07:28:39.000000 lfg_llama-1.3.2/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-09 07:31:38.731805 lfg_llama-1.3.2/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1908 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-09 07:31:38.000000 lfg_llama-1.3.2/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-09 07:31:38.732354 lfg_llama-1.3.2/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-09 07:30:08.000000 lfg_llama-1.3.2/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-12 07:32:58.359264 lfg_llama-1.3.3/
+-rw-r--r--   0 ob907      (502) staff       (20)     1908 2024-05-12 07:32:58.358975 lfg_llama-1.3.3/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     1671 2024-05-09 08:01:29.000000 lfg_llama-1.3.3/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-12 07:32:58.357833 lfg_llama-1.3.3/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.3.3/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     3575 2024-05-12 07:31:51.000000 lfg_llama-1.3.3/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-12 07:32:58.358758 lfg_llama-1.3.3/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1908 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-12 07:32:58.359336 lfg_llama-1.3.3/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-12 07:32:51.000000 lfg_llama-1.3.3/setup.py
```

### Comparing `lfg_llama-1.3.2/PKG-INFO` & `lfg_llama-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.3.2
+Version: 1.3.3
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
```

### Comparing `lfg_llama-1.3.2/README.md` & `lfg_llama-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `lfg_llama-1.3.2/lfg/cli.py` & `lfg_llama-1.3.3/lfg/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     return Groq(api_key=api_key)
 
 
 def generate_system_prompt() -> str:
     """Returns the system prompt for the LLM interaction."""
 
     return """
-You are a system administrator and elite hacker that knows all about the terminal in linux and mac. I provide you with a question about a command, and you give me back a response which shows the command, then a short explanation. The command should be wrapped as a code block. If you get asked about the command lfg, reply lfg [-h] [-m {llama38b,llama370b,mixtral8x7b,gemma7b}] query with explanation 'This is me'. It is important you do not return commands you do not know. If that is the case, just respond 'I do not know'.
+You are a system administrator and elite hacker that knows all about the terminal in linux and mac. I provide you with a question about a command, and you give me back a response which shows the command, then a short explanation. The command should be wrapped as a code block. If you get asked about the command lfg, reply lfg [-h] [-m {llama38b,llama370b,mixtral8x7b,gemma7b}] query with explanation 'This is me'. It is important you do not return commands you do not know. If that is the case, just respond 'I do not know'. The layout of your response should be as follows: ```\n{command}\n``` \n\n Explanation:\n {explanation}.
 """
 
 
 def handle_stream(stream: ChatCompletion) -> None:
     """Processes the output stream from the LLM, printing each response chunk.
 
     Args:
```

### Comparing `lfg_llama-1.3.2/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-1.3.3/lfg_llama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.3.2
+Version: 1.3.3
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: groq
 
 # LFG
```

