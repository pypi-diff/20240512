# Comparing `tmp/llm_bench-0.4.8.tar.gz` & `tmp/llm_bench-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bench-0.4.8.tar", max compression
+gzip compressed data, was "llm_bench-0.4.9.tar", max compression
```

## Comparing `llm_bench-0.4.8.tar` & `llm_bench-0.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1104 2024-05-11 10:29:11.472246 llm_bench-0.4.8/LICENSE
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.522998 llm_bench-0.4.8/llm_bench/__init__.py
--rw-r--r--   0        0        0     1780 2024-05-12 09:23:29.963261 llm_bench-0.4.8/llm_bench/check_models.py
--rw-r--r--   0        0        0      693 2024-05-11 10:29:11.523998 llm_bench-0.4.8/llm_bench/check_ollama.py
--rw-r--r--   0        0        0     1329 2024-05-12 14:30:23.580222 llm_bench-0.4.8/llm_bench/data/benchmark_instructions.yml
--rw-r--r--   0        0        0       63 2024-05-11 13:43:33.813866 llm_bench-0.4.8/llm_bench/data/large_models.yml
--rw-r--r--   0        0        0      100 2024-05-11 13:41:58.654626 llm_bench-0.4.8/llm_bench/data/medium_models.yml
--rw-r--r--   0        0        0      100 2024-05-12 09:04:42.355530 llm_bench-0.4.8/llm_bench/data/small_models.yml
--rw-r--r--   0        0        0      342 2024-05-12 14:30:52.587779 llm_bench-0.4.8/llm_bench/data/test_benchmark.yml
--rw-r--r--   0        0        0       44 2024-05-12 14:46:39.321470 llm_bench-0.4.8/llm_bench/data/test_model.yml
--rw-r--r--   0        0        0     3425 2024-05-12 14:48:49.687604 llm_bench-0.4.8/llm_bench/main.py
--rw-r--r--   0        0        0     1623 2024-05-11 10:29:11.541528 llm_bench-0.4.8/llm_bench/query_llm.py
--rw-r--r--   0        0        0     5792 2024-05-12 14:52:08.927981 llm_bench-0.4.8/llm_bench/run_benchmark.py
--rw-r--r--   0        0        0     2338 2024-05-11 10:29:11.541528 llm_bench-0.4.8/llm_bench/run_benchmark_one.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.541528 llm_bench-0.4.8/llm_bench/security_connection/__init__.py
--rw-r--r--   0        0        0      752 2024-05-11 10:29:11.543151 llm_bench-0.4.8/llm_bench/security_connection/connection.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.8/llm_bench/security_connection/security.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.8/llm_bench/systeminfo/__init__.py
--rw-r--r--   0        0        0     8957 2024-05-11 10:29:11.544069 llm_bench-0.4.8/llm_bench/systeminfo/sysmain.py
--rw-r--r--   0        0        0      815 2024-05-12 14:52:28.935766 llm_bench-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     2195 2024-05-11 16:50:03.191116 llm_bench-0.4.8/README.md
--rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 llm_bench-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-05-11 10:29:11.472246 llm_bench-0.4.9/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.522998 llm_bench-0.4.9/llm_bench/__init__.py
+-rw-r--r--   0        0        0     1780 2024-05-12 09:23:29.963261 llm_bench-0.4.9/llm_bench/check_models.py
+-rw-r--r--   0        0        0      693 2024-05-11 10:29:11.523998 llm_bench-0.4.9/llm_bench/check_ollama.py
+-rw-r--r--   0        0        0     1329 2024-05-12 14:30:23.580222 llm_bench-0.4.9/llm_bench/data/benchmark_instructions.yml
+-rw-r--r--   0        0        0       63 2024-05-11 13:43:33.813866 llm_bench-0.4.9/llm_bench/data/large_models.yml
+-rw-r--r--   0        0        0      100 2024-05-11 13:41:58.654626 llm_bench-0.4.9/llm_bench/data/medium_models.yml
+-rw-r--r--   0        0        0      100 2024-05-12 09:04:42.355530 llm_bench-0.4.9/llm_bench/data/small_models.yml
+-rw-r--r--   0        0        0      342 2024-05-12 14:30:52.587779 llm_bench-0.4.9/llm_bench/data/test_benchmark.yml
+-rw-r--r--   0        0        0       44 2024-05-12 14:46:39.321470 llm_bench-0.4.9/llm_bench/data/test_model.yml
+-rw-r--r--   0        0        0     3435 2024-05-12 14:56:11.520087 llm_bench-0.4.9/llm_bench/main.py
+-rw-r--r--   0        0        0     1623 2024-05-11 10:29:11.541528 llm_bench-0.4.9/llm_bench/query_llm.py
+-rw-r--r--   0        0        0     5792 2024-05-12 14:52:08.927981 llm_bench-0.4.9/llm_bench/run_benchmark.py
+-rw-r--r--   0        0        0     2338 2024-05-11 10:29:11.541528 llm_bench-0.4.9/llm_bench/run_benchmark_one.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.541528 llm_bench-0.4.9/llm_bench/security_connection/__init__.py
+-rw-r--r--   0        0        0      752 2024-05-11 10:29:11.543151 llm_bench-0.4.9/llm_bench/security_connection/connection.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.9/llm_bench/security_connection/security.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.9/llm_bench/systeminfo/__init__.py
+-rw-r--r--   0        0        0     8957 2024-05-11 10:29:11.544069 llm_bench-0.4.9/llm_bench/systeminfo/sysmain.py
+-rw-r--r--   0        0        0      815 2024-05-12 14:56:39.996192 llm_bench-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     2195 2024-05-11 16:50:03.191116 llm_bench-0.4.9/README.md
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 llm_bench-0.4.9/PKG-INFO
```

### Comparing `llm_bench-0.4.8/LICENSE` & `llm_bench-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.8/llm_bench/check_models.py` & `llm_bench-0.4.9/llm_bench/check_models.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.8/llm_bench/check_ollama.py` & `llm_bench-0.4.9/llm_bench/check_ollama.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.8/llm_bench/data/benchmark_instructions.yml` & `llm_bench-0.4.9/llm_bench/data/benchmark_instructions.yml`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.8/llm_bench/main.py` & `llm_bench-0.4.9/llm_bench/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         case_sensitive=False, show_choices=True
     ),
     test: bool = typer.Option(
         False, '--test', help="Flag to toggle between default and alternative benchmark tests."
     )
 ):
     if test:
-        benchmark_file = pkg_resources.resource_filename('llm_bench', 'data/test.yml')
+        benchmark_file = pkg_resources.resource_filename('llm_bench', 'data/test_benchmark.yml')
         models_file = pkg_resources.resource_filename('llm_bench', 'data/test_model.yml')
     else:
         benchmark_file = pkg_resources.resource_filename('llm_bench', 'data/benchmark_instructions.yml')
         models_file = get_model_path(models)
 
     sys_info = sysmain.get_extra()
     print(f"Total memory size : {sys_info['memory']:.2f} GB")
```

### Comparing `llm_bench-0.4.8/llm_bench/query_llm.py` & `llm_bench-0.4.9/llm_bench/query_llm.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.8/llm_bench/run_benchmark.py` & `llm_bench-0.4.9/llm_bench/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.8/llm_bench/run_benchmark_one.py` & `llm_bench-0.4.9/llm_bench/run_benchmark_one.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.8/llm_bench/security_connection/connection.py` & `llm_bench-0.4.9/llm_bench/security_connection/connection.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.8/llm_bench/systeminfo/sysmain.py` & `llm_bench-0.4.9/llm_bench/systeminfo/sysmain.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.8/pyproject.toml` & `llm_bench-0.4.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm_bench"
-version = "0.4.8"
+version = "0.4.9"
 description = "Forked off of LLM Benchmark for Throughputs via Ollama"
 authors = ["Snaas"]
 license = "MIT"
 homepage = "https://github.com/b-Snaas/ollama-benchmark.git"
 readme = "README.md"
 keywords = [
     "benchmark",
```

### Comparing `llm_bench-0.4.8/README.md` & `llm_bench-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.8/PKG-INFO` & `llm_bench-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_bench
-Version: 0.4.8
+Version: 0.4.9
 Summary: Forked off of LLM Benchmark for Throughputs via Ollama
 Home-page: https://github.com/b-Snaas/ollama-benchmark.git
 License: MIT
 Keywords: benchmark,llama,ollama,llms,local
 Author: Snaas
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

