# Comparing `tmp/llm_bench-0.4.6.tar.gz` & `tmp/llm_bench-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bench-0.4.6.tar", max compression
+gzip compressed data, was "llm_bench-0.4.7.tar", max compression
```

## Comparing `llm_bench-0.4.6.tar` & `llm_bench-0.4.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1104 2024-05-11 10:29:11.472246 llm_bench-0.4.6/LICENSE
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.522998 llm_bench-0.4.6/llm_bench/__init__.py
--rw-r--r--   0        0        0     1780 2024-05-12 09:23:29.963261 llm_bench-0.4.6/llm_bench/check_models.py
--rw-r--r--   0        0        0      693 2024-05-11 10:29:11.523998 llm_bench-0.4.6/llm_bench/check_ollama.py
--rw-r--r--   0        0        0     1329 2024-05-12 14:30:23.580222 llm_bench-0.4.6/llm_bench/data/benchmark_instructions.yml
--rw-r--r--   0        0        0       63 2024-05-11 13:43:33.813866 llm_bench-0.4.6/llm_bench/data/large_models.yml
--rw-r--r--   0        0        0      100 2024-05-11 13:41:58.654626 llm_bench-0.4.6/llm_bench/data/medium_models.yml
--rw-r--r--   0        0        0      100 2024-05-12 09:04:42.355530 llm_bench-0.4.6/llm_bench/data/small_models.yml
--rw-r--r--   0        0        0      342 2024-05-12 14:30:52.587779 llm_bench-0.4.6/llm_bench/data/test.yml
--rw-r--r--   0        0        0     3328 2024-05-12 14:31:33.588240 llm_bench-0.4.6/llm_bench/main.py
--rw-r--r--   0        0        0     1623 2024-05-11 10:29:11.541528 llm_bench-0.4.6/llm_bench/query_llm.py
--rw-r--r--   0        0        0     5548 2024-05-12 14:24:08.384567 llm_bench-0.4.6/llm_bench/run_benchmark.py
--rw-r--r--   0        0        0     2338 2024-05-11 10:29:11.541528 llm_bench-0.4.6/llm_bench/run_benchmark_one.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.541528 llm_bench-0.4.6/llm_bench/security_connection/__init__.py
--rw-r--r--   0        0        0      752 2024-05-11 10:29:11.543151 llm_bench-0.4.6/llm_bench/security_connection/connection.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.6/llm_bench/security_connection/security.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.6/llm_bench/systeminfo/__init__.py
--rw-r--r--   0        0        0     8957 2024-05-11 10:29:11.544069 llm_bench-0.4.6/llm_bench/systeminfo/sysmain.py
--rw-r--r--   0        0        0      815 2024-05-12 14:34:05.647920 llm_bench-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     2195 2024-05-11 16:50:03.191116 llm_bench-0.4.6/README.md
--rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 llm_bench-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-05-11 10:29:11.472246 llm_bench-0.4.7/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.522998 llm_bench-0.4.7/llm_bench/__init__.py
+-rw-r--r--   0        0        0     1780 2024-05-12 09:23:29.963261 llm_bench-0.4.7/llm_bench/check_models.py
+-rw-r--r--   0        0        0      693 2024-05-11 10:29:11.523998 llm_bench-0.4.7/llm_bench/check_ollama.py
+-rw-r--r--   0        0        0     1329 2024-05-12 14:30:23.580222 llm_bench-0.4.7/llm_bench/data/benchmark_instructions.yml
+-rw-r--r--   0        0        0       63 2024-05-11 13:43:33.813866 llm_bench-0.4.7/llm_bench/data/large_models.yml
+-rw-r--r--   0        0        0      100 2024-05-11 13:41:58.654626 llm_bench-0.4.7/llm_bench/data/medium_models.yml
+-rw-r--r--   0        0        0      100 2024-05-12 09:04:42.355530 llm_bench-0.4.7/llm_bench/data/small_models.yml
+-rw-r--r--   0        0        0      342 2024-05-12 14:30:52.587779 llm_bench-0.4.7/llm_bench/data/test.yml
+-rw-r--r--   0        0        0     3330 2024-05-12 14:40:08.091836 llm_bench-0.4.7/llm_bench/main.py
+-rw-r--r--   0        0        0     1623 2024-05-11 10:29:11.541528 llm_bench-0.4.7/llm_bench/query_llm.py
+-rw-r--r--   0        0        0     5548 2024-05-12 14:24:08.384567 llm_bench-0.4.7/llm_bench/run_benchmark.py
+-rw-r--r--   0        0        0     2338 2024-05-11 10:29:11.541528 llm_bench-0.4.7/llm_bench/run_benchmark_one.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.541528 llm_bench-0.4.7/llm_bench/security_connection/__init__.py
+-rw-r--r--   0        0        0      752 2024-05-11 10:29:11.543151 llm_bench-0.4.7/llm_bench/security_connection/connection.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.7/llm_bench/security_connection/security.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.7/llm_bench/systeminfo/__init__.py
+-rw-r--r--   0        0        0     8957 2024-05-11 10:29:11.544069 llm_bench-0.4.7/llm_bench/systeminfo/sysmain.py
+-rw-r--r--   0        0        0      815 2024-05-12 14:40:17.764237 llm_bench-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     2195 2024-05-11 16:50:03.191116 llm_bench-0.4.7/README.md
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 llm_bench-0.4.7/PKG-INFO
```

### Comparing `llm_bench-0.4.6/LICENSE` & `llm_bench-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.6/llm_bench/check_models.py` & `llm_bench-0.4.7/llm_bench/check_models.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.6/llm_bench/check_ollama.py` & `llm_bench-0.4.7/llm_bench/check_ollama.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.6/llm_bench/data/benchmark_instructions.yml` & `llm_bench-0.4.7/llm_bench/data/benchmark_instructions.yml`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.6/llm_bench/main.py` & `llm_bench-0.4.7/llm_bench/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typer
 import pkg_resources
 import speedtest
 import time
-from systeminfo import sysmain
-from security_connection import connection 
+from .systeminfo import sysmain
+from .security_connection import connection 
 from llm_bench import check_models, check_ollama, run_benchmark
 
 app = typer.Typer()
 
 @app.command()
 def get_model_path(size: str) -> str:
     """ Helper function to return the correct file path based on the model size """
```

### Comparing `llm_bench-0.4.6/llm_bench/query_llm.py` & `llm_bench-0.4.7/llm_bench/query_llm.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.6/llm_bench/run_benchmark.py` & `llm_bench-0.4.7/llm_bench/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.6/llm_bench/run_benchmark_one.py` & `llm_bench-0.4.7/llm_bench/run_benchmark_one.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.6/llm_bench/security_connection/connection.py` & `llm_bench-0.4.7/llm_bench/security_connection/connection.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.6/llm_bench/systeminfo/sysmain.py` & `llm_bench-0.4.7/llm_bench/systeminfo/sysmain.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.6/pyproject.toml` & `llm_bench-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm_bench"
-version = "0.4.6"
+version = "0.4.7"
 description = "Forked off of LLM Benchmark for Throughputs via Ollama"
 authors = ["Snaas"]
 license = "MIT"
 homepage = "https://github.com/b-Snaas/ollama-benchmark.git"
 readme = "README.md"
 keywords = [
     "benchmark",
```

### Comparing `llm_bench-0.4.6/README.md` & `llm_bench-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.6/PKG-INFO` & `llm_bench-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_bench
-Version: 0.4.6
+Version: 0.4.7
 Summary: Forked off of LLM Benchmark for Throughputs via Ollama
 Home-page: https://github.com/b-Snaas/ollama-benchmark.git
 License: MIT
 Keywords: benchmark,llama,ollama,llms,local
 Author: Snaas
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

