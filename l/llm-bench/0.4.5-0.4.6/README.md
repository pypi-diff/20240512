# Comparing `tmp/llm_bench-0.4.5.tar.gz` & `tmp/llm_bench-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bench-0.4.5.tar", max compression
+gzip compressed data, was "llm_bench-0.4.6.tar", max compression
```

## Comparing `llm_bench-0.4.5.tar` & `llm_bench-0.4.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1104 2024-05-11 10:29:11.472246 llm_bench-0.4.5/LICENSE
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.522998 llm_bench-0.4.5/llm_bench/__init__.py
--rw-r--r--   0        0        0     1780 2024-05-12 09:23:29.963261 llm_bench-0.4.5/llm_bench/check_models.py
--rw-r--r--   0        0        0      693 2024-05-11 10:29:11.523998 llm_bench-0.4.5/llm_bench/check_ollama.py
--rw-r--r--   0        0        0     1329 2024-05-12 09:24:23.489265 llm_bench-0.4.5/llm_bench/data/benchmark_instructions.yml
--rw-r--r--   0        0        0       63 2024-05-11 13:43:33.813866 llm_bench-0.4.5/llm_bench/data/large_models.yml
--rw-r--r--   0        0        0      100 2024-05-11 13:41:58.654626 llm_bench-0.4.5/llm_bench/data/medium_models.yml
--rw-r--r--   0        0        0      100 2024-05-12 09:04:42.355530 llm_bench-0.4.5/llm_bench/data/small_models.yml
--rw-r--r--   0        0        0     3168 2024-05-12 09:26:55.218440 llm_bench-0.4.5/llm_bench/main.py
--rw-r--r--   0        0        0     1623 2024-05-11 10:29:11.541528 llm_bench-0.4.5/llm_bench/query_llm.py
--rw-r--r--   0        0        0     5313 2024-05-12 14:13:46.435749 llm_bench-0.4.5/llm_bench/run_benchmark.py
--rw-r--r--   0        0        0     2338 2024-05-11 10:29:11.541528 llm_bench-0.4.5/llm_bench/run_benchmark_one.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.541528 llm_bench-0.4.5/llm_bench/security_connection/__init__.py
--rw-r--r--   0        0        0      752 2024-05-11 10:29:11.543151 llm_bench-0.4.5/llm_bench/security_connection/connection.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.5/llm_bench/security_connection/security.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.5/llm_bench/systeminfo/__init__.py
--rw-r--r--   0        0        0     8957 2024-05-11 10:29:11.544069 llm_bench-0.4.5/llm_bench/systeminfo/sysmain.py
--rw-r--r--   0        0        0      815 2024-05-12 14:17:54.326500 llm_bench-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2195 2024-05-11 16:50:03.191116 llm_bench-0.4.5/README.md
--rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 llm_bench-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-05-11 10:29:11.472246 llm_bench-0.4.6/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.522998 llm_bench-0.4.6/llm_bench/__init__.py
+-rw-r--r--   0        0        0     1780 2024-05-12 09:23:29.963261 llm_bench-0.4.6/llm_bench/check_models.py
+-rw-r--r--   0        0        0      693 2024-05-11 10:29:11.523998 llm_bench-0.4.6/llm_bench/check_ollama.py
+-rw-r--r--   0        0        0     1329 2024-05-12 14:30:23.580222 llm_bench-0.4.6/llm_bench/data/benchmark_instructions.yml
+-rw-r--r--   0        0        0       63 2024-05-11 13:43:33.813866 llm_bench-0.4.6/llm_bench/data/large_models.yml
+-rw-r--r--   0        0        0      100 2024-05-11 13:41:58.654626 llm_bench-0.4.6/llm_bench/data/medium_models.yml
+-rw-r--r--   0        0        0      100 2024-05-12 09:04:42.355530 llm_bench-0.4.6/llm_bench/data/small_models.yml
+-rw-r--r--   0        0        0      342 2024-05-12 14:30:52.587779 llm_bench-0.4.6/llm_bench/data/test.yml
+-rw-r--r--   0        0        0     3328 2024-05-12 14:31:33.588240 llm_bench-0.4.6/llm_bench/main.py
+-rw-r--r--   0        0        0     1623 2024-05-11 10:29:11.541528 llm_bench-0.4.6/llm_bench/query_llm.py
+-rw-r--r--   0        0        0     5548 2024-05-12 14:24:08.384567 llm_bench-0.4.6/llm_bench/run_benchmark.py
+-rw-r--r--   0        0        0     2338 2024-05-11 10:29:11.541528 llm_bench-0.4.6/llm_bench/run_benchmark_one.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.541528 llm_bench-0.4.6/llm_bench/security_connection/__init__.py
+-rw-r--r--   0        0        0      752 2024-05-11 10:29:11.543151 llm_bench-0.4.6/llm_bench/security_connection/connection.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.6/llm_bench/security_connection/security.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.6/llm_bench/systeminfo/__init__.py
+-rw-r--r--   0        0        0     8957 2024-05-11 10:29:11.544069 llm_bench-0.4.6/llm_bench/systeminfo/sysmain.py
+-rw-r--r--   0        0        0      815 2024-05-12 14:34:05.647920 llm_bench-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2195 2024-05-11 16:50:03.191116 llm_bench-0.4.6/README.md
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 llm_bench-0.4.6/PKG-INFO
```

### Comparing `llm_bench-0.4.5/LICENSE` & `llm_bench-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.5/llm_bench/check_models.py` & `llm_bench-0.4.6/llm_bench/check_models.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.5/llm_bench/check_ollama.py` & `llm_bench-0.4.6/llm_bench/check_ollama.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.5/llm_bench/data/benchmark_instructions.yml` & `llm_bench-0.4.6/llm_bench/data/benchmark_instructions.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 version: 1.0
 models:
-  - model: gemma:2b
+  - model: gemma:7b
   - model: phi3
   - model: mistral
   - model: llama3
 prompts:
   - prompt: What are your thoughts on the latest scientific discovery regarding black holes?
   - prompt: In a world where time travel is possible, a scientist invents a device that allows people to visit any historical event. One day, a young woman decides to travel back in time to...
   - prompt: Write a step-by-step guide on how to bake a chocolate cake from scratch.
```

### Comparing `llm_bench-0.4.5/llm_bench/main.py` & `llm_bench-0.4.6/llm_bench/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typer
 import pkg_resources
 import speedtest
 import time
-from .systeminfo import sysmain
-from .security_connection import connection 
+from systeminfo import sysmain
+from security_connection import connection 
 from llm_bench import check_models, check_ollama, run_benchmark
 
 app = typer.Typer()
 
 @app.command()
 def get_model_path(size: str) -> str:
     """ Helper function to return the correct file path based on the model size """
@@ -50,19 +50,23 @@
 def run(
     ollamabin: str = typer.Option('ollama', help="Path to the Ollama binary."),
     sendinfo: bool = typer.Option(True, help="Flag to send system info."),
     models: str = typer.Option(
         "small", help="Select model size: small, medium, or large.",
         case_sensitive=False, show_choices=True
     ),
-    benchmark_file: str = typer.Option(
-        pkg_resources.resource_filename('llm_bench', 'data/benchmark_instructions.yml'),
-        help="Path to the benchmark instructions file."
+    test: bool = typer.Option(
+        False, '--test', help="Flag to toggle between default and alternative benchmark tests."
     )
 ):
+    if test:
+        benchmark_file = pkg_resources.resource_filename('llm_bench', 'data/test.yml')
+    else:
+        benchmark_file = pkg_resources.resource_filename('llm_bench', 'data/benchmark_instructions.yml')
+
     models_file = get_model_path(models)
     sys_info = sysmain.get_extra()
     print(f"Total memory size : {sys_info['memory']:.2f} GB") 
     print(f"cpu_info: {sys_info['cpu']}")
     print(f"gpu_info: {sys_info['gpu']}")
     print(f"os_version: {sys_info['os_version']}")
```

### Comparing `llm_bench-0.4.5/llm_bench/query_llm.py` & `llm_bench-0.4.6/llm_bench/query_llm.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.5/llm_bench/run_benchmark.py` & `llm_bench-0.4.6/llm_bench/run_benchmark.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,17 +46,24 @@
             seconds = float(match.group(2)) if match.group(2) else 0
             return 60 * minutes + seconds
         else:
             raise ValueError(f"Unsupported duration format: {duration_str}")
     else:
         raise ValueError("Unsupported duration format")
 
-def remove_ansi_escape_sequences(text):
-    ansi_escape_pattern = re.compile(r'\x1B[@-_][0-?]*[ -/]*[@-~]')
-    return ansi_escape_pattern.sub('', text)
+def clean_output(text):
+    # Regex to remove ANSI escape codes
+    ansi_escape = re.compile(r'\x1B[@-_][0-?]*[ -/]*[@-~]')
+    # Clean ANSI escape sequences
+    text = ansi_escape.sub('', text)
+    # Regex to remove common spinner characters
+    spinner_chars = re.compile(r'[⠙⠹⠸⠼⠴⠦⠧⠇⠏⠋]')
+    # Clean spinner characters
+    text = spinner_chars.sub('', text)
+    return text
 
 def run_benchmark(models_file_path, benchmark_file_path, ollamabin):
     models_dict = parse_yaml(models_file_path)
     benchmark_dict = parse_yaml(benchmark_file_path)
     allowed_models = {e['model'] for e in models_dict['models']}
     ans = {}
 
@@ -78,15 +85,15 @@
                         [ollamabin, 'run', model_name, prompt_text, '--verbose'],
                         capture_output=True,
                         text=True,
                         check=True,
                         encoding='utf-8'
                     )
                     std_err = result.stderr or ''
-                    cleaned_stderr = remove_ansi_escape_sequences(std_err)
+                    cleaned_stderr = clean_output(std_err)
                     print("STDERR:", cleaned_stderr)
                     
                     for line in std_err.split('\n'):
                         if line.lstrip().startswith("prompt"):
                             continue
                         if 'eval rate:' in line:
                             number = float(line.split()[-2])
```

### Comparing `llm_bench-0.4.5/llm_bench/run_benchmark_one.py` & `llm_bench-0.4.6/llm_bench/run_benchmark_one.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.5/llm_bench/security_connection/connection.py` & `llm_bench-0.4.6/llm_bench/security_connection/connection.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.5/llm_bench/systeminfo/sysmain.py` & `llm_bench-0.4.6/llm_bench/systeminfo/sysmain.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.5/pyproject.toml` & `llm_bench-0.4.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm_bench"
-version = "0.4.5"
+version = "0.4.6"
 description = "Forked off of LLM Benchmark for Throughputs via Ollama"
 authors = ["Snaas"]
 license = "MIT"
 homepage = "https://github.com/b-Snaas/ollama-benchmark.git"
 readme = "README.md"
 keywords = [
     "benchmark",
```

### Comparing `llm_bench-0.4.5/README.md` & `llm_bench-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.5/PKG-INFO` & `llm_bench-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_bench
-Version: 0.4.5
+Version: 0.4.6
 Summary: Forked off of LLM Benchmark for Throughputs via Ollama
 Home-page: https://github.com/b-Snaas/ollama-benchmark.git
 License: MIT
 Keywords: benchmark,llama,ollama,llms,local
 Author: Snaas
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

