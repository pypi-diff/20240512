# Comparing `tmp/llm_bench-0.4.4.tar.gz` & `tmp/llm_bench-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bench-0.4.4.tar", max compression
+gzip compressed data, was "llm_bench-0.4.5.tar", max compression
```

## Comparing `llm_bench-0.4.4.tar` & `llm_bench-0.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1104 2024-05-11 10:29:11.472246 llm_bench-0.4.4/LICENSE
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.522998 llm_bench-0.4.4/llm_bench/__init__.py
--rw-r--r--   0        0        0     1780 2024-05-12 09:23:29.963261 llm_bench-0.4.4/llm_bench/check_models.py
--rw-r--r--   0        0        0      693 2024-05-11 10:29:11.523998 llm_bench-0.4.4/llm_bench/check_ollama.py
--rw-r--r--   0        0        0     1329 2024-05-12 09:24:23.489265 llm_bench-0.4.4/llm_bench/data/benchmark_instructions.yml
--rw-r--r--   0        0        0       63 2024-05-11 13:43:33.813866 llm_bench-0.4.4/llm_bench/data/large_models.yml
--rw-r--r--   0        0        0      100 2024-05-11 13:41:58.654626 llm_bench-0.4.4/llm_bench/data/medium_models.yml
--rw-r--r--   0        0        0      100 2024-05-12 09:04:42.355530 llm_bench-0.4.4/llm_bench/data/small_models.yml
--rw-r--r--   0        0        0     3168 2024-05-12 09:26:55.218440 llm_bench-0.4.4/llm_bench/main.py
--rw-r--r--   0        0        0     1623 2024-05-11 10:29:11.541528 llm_bench-0.4.4/llm_bench/query_llm.py
--rw-r--r--   0        0        0     4967 2024-05-12 09:20:14.504351 llm_bench-0.4.4/llm_bench/run_benchmark.py
--rw-r--r--   0        0        0     2338 2024-05-11 10:29:11.541528 llm_bench-0.4.4/llm_bench/run_benchmark_one.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.541528 llm_bench-0.4.4/llm_bench/security_connection/__init__.py
--rw-r--r--   0        0        0      752 2024-05-11 10:29:11.543151 llm_bench-0.4.4/llm_bench/security_connection/connection.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.4/llm_bench/security_connection/security.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.4/llm_bench/systeminfo/__init__.py
--rw-r--r--   0        0        0     8957 2024-05-11 10:29:11.544069 llm_bench-0.4.4/llm_bench/systeminfo/sysmain.py
--rw-r--r--   0        0        0      815 2024-05-12 09:25:46.497246 llm_bench-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2195 2024-05-11 16:50:03.191116 llm_bench-0.4.4/README.md
--rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 llm_bench-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-05-11 10:29:11.472246 llm_bench-0.4.5/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.522998 llm_bench-0.4.5/llm_bench/__init__.py
+-rw-r--r--   0        0        0     1780 2024-05-12 09:23:29.963261 llm_bench-0.4.5/llm_bench/check_models.py
+-rw-r--r--   0        0        0      693 2024-05-11 10:29:11.523998 llm_bench-0.4.5/llm_bench/check_ollama.py
+-rw-r--r--   0        0        0     1329 2024-05-12 09:24:23.489265 llm_bench-0.4.5/llm_bench/data/benchmark_instructions.yml
+-rw-r--r--   0        0        0       63 2024-05-11 13:43:33.813866 llm_bench-0.4.5/llm_bench/data/large_models.yml
+-rw-r--r--   0        0        0      100 2024-05-11 13:41:58.654626 llm_bench-0.4.5/llm_bench/data/medium_models.yml
+-rw-r--r--   0        0        0      100 2024-05-12 09:04:42.355530 llm_bench-0.4.5/llm_bench/data/small_models.yml
+-rw-r--r--   0        0        0     3168 2024-05-12 09:26:55.218440 llm_bench-0.4.5/llm_bench/main.py
+-rw-r--r--   0        0        0     1623 2024-05-11 10:29:11.541528 llm_bench-0.4.5/llm_bench/query_llm.py
+-rw-r--r--   0        0        0     5313 2024-05-12 14:13:46.435749 llm_bench-0.4.5/llm_bench/run_benchmark.py
+-rw-r--r--   0        0        0     2338 2024-05-11 10:29:11.541528 llm_bench-0.4.5/llm_bench/run_benchmark_one.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.541528 llm_bench-0.4.5/llm_bench/security_connection/__init__.py
+-rw-r--r--   0        0        0      752 2024-05-11 10:29:11.543151 llm_bench-0.4.5/llm_bench/security_connection/connection.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.5/llm_bench/security_connection/security.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.5/llm_bench/systeminfo/__init__.py
+-rw-r--r--   0        0        0     8957 2024-05-11 10:29:11.544069 llm_bench-0.4.5/llm_bench/systeminfo/sysmain.py
+-rw-r--r--   0        0        0      815 2024-05-12 14:17:54.326500 llm_bench-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2195 2024-05-11 16:50:03.191116 llm_bench-0.4.5/README.md
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 llm_bench-0.4.5/PKG-INFO
```

### Comparing `llm_bench-0.4.4/LICENSE` & `llm_bench-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.4/llm_bench/check_models.py` & `llm_bench-0.4.5/llm_bench/check_models.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.4/llm_bench/check_ollama.py` & `llm_bench-0.4.5/llm_bench/check_ollama.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.4/llm_bench/data/benchmark_instructions.yml` & `llm_bench-0.4.5/llm_bench/data/benchmark_instructions.yml`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.4/llm_bench/main.py` & `llm_bench-0.4.5/llm_bench/main.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.4/llm_bench/query_llm.py` & `llm_bench-0.4.5/llm_bench/query_llm.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.4/llm_bench/run_benchmark.py` & `llm_bench-0.4.5/llm_bench/run_benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,28 +30,34 @@
         try:
             data = yaml.safe_load(stream)
         except yaml.YAMLError as e:
             print(e)
     return data
 
 def parse_duration(duration_str):
-    """ Parse duration from strings in various formats (s, ms, m+s) to seconds as a float. """
+    """ Parse duration from strings in various formats (s, ms, µs, m+s) to seconds as a float. """
     if 'ms' in duration_str:
         return float(duration_str.replace('ms', '')) / 1000.0
+    elif 'µs' in duration_str:
+        return float(duration_str.replace('µs', '')) / 1000000.0
     elif 's' in duration_str:
         match = re.match(r'(?:(\d+)m)?(\d*\.?\d*)s', duration_str)
         if match:
             minutes = int(match.group(1)) if match.group(1) else 0
             seconds = float(match.group(2)) if match.group(2) else 0
             return 60 * minutes + seconds
         else:
             raise ValueError(f"Unsupported duration format: {duration_str}")
     else:
         raise ValueError("Unsupported duration format")
 
+def remove_ansi_escape_sequences(text):
+    ansi_escape_pattern = re.compile(r'\x1B[@-_][0-?]*[ -/]*[@-~]')
+    return ansi_escape_pattern.sub('', text)
+
 def run_benchmark(models_file_path, benchmark_file_path, ollamabin):
     models_dict = parse_yaml(models_file_path)
     benchmark_dict = parse_yaml(benchmark_file_path)
     allowed_models = {e['model'] for e in models_dict['models']}
     ans = {}
 
     for model in models_dict['models']:
@@ -72,15 +78,16 @@
                         [ollamabin, 'run', model_name, prompt_text, '--verbose'],
                         capture_output=True,
                         text=True,
                         check=True,
                         encoding='utf-8'
                     )
                     std_err = result.stderr or ''
-                    print("STDERR:", std_err)
+                    cleaned_stderr = remove_ansi_escape_sequences(std_err)
+                    print("STDERR:", cleaned_stderr)
                     
                     for line in std_err.split('\n'):
                         if line.lstrip().startswith("prompt"):
                             continue
                         if 'eval rate:' in line:
                             number = float(line.split()[-2])
                             stored_nums.append(number)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llm_bench-0.4.4/llm_bench/run_benchmark_one.py` & `llm_bench-0.4.5/llm_bench/run_benchmark_one.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.4/llm_bench/security_connection/connection.py` & `llm_bench-0.4.5/llm_bench/security_connection/connection.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.4/llm_bench/systeminfo/sysmain.py` & `llm_bench-0.4.5/llm_bench/systeminfo/sysmain.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.4/pyproject.toml` & `llm_bench-0.4.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm_bench"
-version = "0.4.4"
+version = "0.4.5"
 description = "Forked off of LLM Benchmark for Throughputs via Ollama"
 authors = ["Snaas"]
 license = "MIT"
 homepage = "https://github.com/b-Snaas/ollama-benchmark.git"
 readme = "README.md"
 keywords = [
     "benchmark",
```

### Comparing `llm_bench-0.4.4/README.md` & `llm_bench-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.4/PKG-INFO` & `llm_bench-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_bench
-Version: 0.4.4
+Version: 0.4.5
 Summary: Forked off of LLM Benchmark for Throughputs via Ollama
 Home-page: https://github.com/b-Snaas/ollama-benchmark.git
 License: MIT
 Keywords: benchmark,llama,ollama,llms,local
 Author: Snaas
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

