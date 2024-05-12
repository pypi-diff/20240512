# Comparing `tmp/llm_bench-0.4.3.tar.gz` & `tmp/llm_bench-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_bench-0.4.3.tar", max compression
+gzip compressed data, was "llm_bench-0.4.4.tar", max compression
```

## Comparing `llm_bench-0.4.3.tar` & `llm_bench-0.4.4.tar`

### file list

```diff
@@ -1,25 +1,20 @@
--rw-r--r--   0        0        0     1104 2024-05-11 10:29:11.472246 llm_bench-0.4.3/LICENSE
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.522998 llm_bench-0.4.3/llm_bench/__init__.py
--rw-r--r--   0        0        0     1837 2024-05-11 10:29:11.523998 llm_bench-0.4.3/llm_bench/check_models.py
--rw-r--r--   0        0        0      693 2024-05-11 10:29:11.523998 llm_bench-0.4.3/llm_bench/check_ollama.py
--rw-r--r--   0        0        0      912 2024-05-11 13:40:43.867959 llm_bench-0.4.3/llm_bench/data/benchmark_instructions.yml
--rw-r--r--   0        0        0   596759 2024-05-11 10:29:11.529984 llm_bench-0.4.3/llm_bench/data/img/sample1.jpg
--rw-r--r--   0        0        0   243536 2024-05-11 10:29:11.530992 llm_bench-0.4.3/llm_bench/data/img/sample2.jpg
--rw-r--r--   0        0        0   518611 2024-05-11 10:29:11.534527 llm_bench-0.4.3/llm_bench/data/img/sample3.jpg
--rw-r--r--   0        0        0   236523 2024-05-11 10:29:11.536539 llm_bench-0.4.3/llm_bench/data/img/sample4.jpg
--rw-r--r--   0        0        0   534025 2024-05-11 10:29:11.540526 llm_bench-0.4.3/llm_bench/data/img/sample5.jpg
--rw-r--r--   0        0        0       63 2024-05-11 13:43:33.813866 llm_bench-0.4.3/llm_bench/data/large_models.yml
--rw-r--r--   0        0        0      100 2024-05-11 13:41:58.654626 llm_bench-0.4.3/llm_bench/data/medium_models.yml
--rw-r--r--   0        0        0      100 2024-05-11 13:42:04.646159 llm_bench-0.4.3/llm_bench/data/small_models.yml
--rw-r--r--   0        0        0     2832 2024-05-11 14:39:18.022274 llm_bench-0.4.3/llm_bench/main.py
--rw-r--r--   0        0        0     1623 2024-05-11 10:29:11.541528 llm_bench-0.4.3/llm_bench/query_llm.py
--rw-r--r--   0        0        0     3143 2024-05-11 13:20:54.821991 llm_bench-0.4.3/llm_bench/run_benchmark.py
--rw-r--r--   0        0        0     2338 2024-05-11 10:29:11.541528 llm_bench-0.4.3/llm_bench/run_benchmark_one.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.541528 llm_bench-0.4.3/llm_bench/security_connection/__init__.py
--rw-r--r--   0        0        0      752 2024-05-11 10:29:11.543151 llm_bench-0.4.3/llm_bench/security_connection/connection.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.3/llm_bench/security_connection/security.py
--rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.3/llm_bench/systeminfo/__init__.py
--rw-r--r--   0        0        0     8957 2024-05-11 10:29:11.544069 llm_bench-0.4.3/llm_bench/systeminfo/sysmain.py
--rw-r--r--   0        0        0      815 2024-05-11 14:41:51.395477 llm_bench-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2397 2024-05-11 10:29:11.472246 llm_bench-0.4.3/README.md
--rw-r--r--   0        0        0     3343 1970-01-01 00:00:00.000000 llm_bench-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-05-11 10:29:11.472246 llm_bench-0.4.4/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.522998 llm_bench-0.4.4/llm_bench/__init__.py
+-rw-r--r--   0        0        0     1780 2024-05-12 09:23:29.963261 llm_bench-0.4.4/llm_bench/check_models.py
+-rw-r--r--   0        0        0      693 2024-05-11 10:29:11.523998 llm_bench-0.4.4/llm_bench/check_ollama.py
+-rw-r--r--   0        0        0     1329 2024-05-12 09:24:23.489265 llm_bench-0.4.4/llm_bench/data/benchmark_instructions.yml
+-rw-r--r--   0        0        0       63 2024-05-11 13:43:33.813866 llm_bench-0.4.4/llm_bench/data/large_models.yml
+-rw-r--r--   0        0        0      100 2024-05-11 13:41:58.654626 llm_bench-0.4.4/llm_bench/data/medium_models.yml
+-rw-r--r--   0        0        0      100 2024-05-12 09:04:42.355530 llm_bench-0.4.4/llm_bench/data/small_models.yml
+-rw-r--r--   0        0        0     3168 2024-05-12 09:26:55.218440 llm_bench-0.4.4/llm_bench/main.py
+-rw-r--r--   0        0        0     1623 2024-05-11 10:29:11.541528 llm_bench-0.4.4/llm_bench/query_llm.py
+-rw-r--r--   0        0        0     4967 2024-05-12 09:20:14.504351 llm_bench-0.4.4/llm_bench/run_benchmark.py
+-rw-r--r--   0        0        0     2338 2024-05-11 10:29:11.541528 llm_bench-0.4.4/llm_bench/run_benchmark_one.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.541528 llm_bench-0.4.4/llm_bench/security_connection/__init__.py
+-rw-r--r--   0        0        0      752 2024-05-11 10:29:11.543151 llm_bench-0.4.4/llm_bench/security_connection/connection.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.4/llm_bench/security_connection/security.py
+-rw-r--r--   0        0        0        0 2024-05-11 10:29:11.543151 llm_bench-0.4.4/llm_bench/systeminfo/__init__.py
+-rw-r--r--   0        0        0     8957 2024-05-11 10:29:11.544069 llm_bench-0.4.4/llm_bench/systeminfo/sysmain.py
+-rw-r--r--   0        0        0      815 2024-05-12 09:25:46.497246 llm_bench-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2195 2024-05-11 16:50:03.191116 llm_bench-0.4.4/README.md
+-rw-r--r--   0        0        0     3147 1970-01-01 00:00:00.000000 llm_bench-0.4.4/PKG-INFO
```

### Comparing `llm_bench-0.4.3/LICENSE` & `llm_bench-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.3/llm_bench/check_models.py` & `llm_bench-0.4.4/llm_bench/check_models.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,14 @@
             data=yaml.safe_load(stream)
             #print(d)
         except yaml.YAMLError as e:
             print(e)
     return data
 
 def pull_models(models_file_path):
-    print(f"LLM models file path：{models_file_path}")
     print(f"Checking and pulling the following LLM models")
     models_dict = parse_yaml(models_file_path)
     for x in models_dict['models']:
         model_name = x['model']
         print(model_name)
         ollama.pull(model_name)
```

### Comparing `llm_bench-0.4.3/llm_bench/check_ollama.py` & `llm_bench-0.4.4/llm_bench/check_ollama.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.3/llm_bench/main.py` & `llm_bench-0.4.4/llm_bench/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import typer
 import pkg_resources
 import speedtest
+import time
 from .systeminfo import sysmain
 from .security_connection import connection 
 from llm_bench import check_models, check_ollama, run_benchmark
 
 app = typer.Typer()
 
 @app.command()
@@ -31,20 +32,23 @@
         x = connection.send_sysinfo(sys_info)
         print(x)
     else:
         print(f"No print!")
 
 @app.command()
 def check_internet_speed():
+    start_time = time.time()
     st = speedtest.Speedtest()
     st.get_best_server()
     download_speed = st.download() / 1_000_000
     upload_speed = st.upload() / 1_000_000
+    elapsed_time = time.time() - start_time
     print(f"Download Speed: {download_speed:.2f} Mbps")
     print(f"Upload Speed: {upload_speed:.2f} Mbps")
+    print(f"Internet speed test duration: {elapsed_time:.2f} seconds")
 
 @app.command()
 def run(
     ollamabin: str = typer.Option('ollama', help="Path to the Ollama binary."),
     sendinfo: bool = typer.Option(True, help="Flag to send system info."),
     models: str = typer.Option(
         "small", help="Select model size: small, medium, or large.",
@@ -59,22 +63,26 @@
     sys_info = sysmain.get_extra()
     print(f"Total memory size : {sys_info['memory']:.2f} GB") 
     print(f"cpu_info: {sys_info['cpu']}")
     print(f"gpu_info: {sys_info['gpu']}")
     print(f"os_version: {sys_info['os_version']}")
 
     ollama_version = check_ollama.check_ollama_version(ollamabin)
-    print(f"ollama_version: {ollama_version}")
+    print(f"ollama_version: {ollama_version} \n")
+
+    print("Internet speed test: ")
+    check_internet_speed()
     print('-' * 10)
 
+    start_time = time.time()
     check_models.pull_models(models_file)
+    elapsed_time = time.time() - start_time
+    print(f"Model pulling time: {elapsed_time:.2f} seconds")
     print('-' * 10)
 
-    check_internet_speed()
-
     bench_results_info = {}
     result = run_benchmark.run_benchmark(models_file, benchmark_file, ollamabin)
     bench_results_info.update(result)
 
     print(bench_results_info)
 
 if __name__ == "__main__":
```

### Comparing `llm_bench-0.4.3/llm_bench/query_llm.py` & `llm_bench-0.4.4/llm_bench/query_llm.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.3/llm_bench/run_benchmark.py` & `llm_bench-0.4.4/llm_bench/run_benchmark_one.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,59 @@
 import argparse
 import yaml
 import subprocess
 import datetime
-import pkg_resources
 
 parser = argparse.ArgumentParser(
     prog="python3 check_models.py",
     description="Before running check_models.py, please make sure you installed ollama successfully \
-        on macOS, Linux, or WSL2 on Windows. You can check the website: https://ollama.com",
+        on macOS, Linux, or WSL2 on Windows. You can check the website: https://ollama.ai",
     epilog="Author: Jason Chuang")
 
 parser.add_argument("-v",
                     "--verbose",
                     action="store_true",
                     help="this program helps you check whether you have ollama benchmark models installed")
 
 parser.add_argument("-m",
                     "--models",
                     type=str,
                     help="provide benchmark models YAML file path. ex. ../data/benchmark_models.yml")
 
-parser.add_argument("-b",
-                    "--benchmark",
-                    type=str,
-                    help="provide benchmark YAML file path. ex. ../data/benchmark1.yml")
-
-
 def parse_yaml(yaml_file_path):
     with open(yaml_file_path, 'r') as stream:
         try:
             data=yaml.safe_load(stream)
             #print(d)
         except yaml.YAMLError as e:
             print(e)
     return data
 
-def run_benchmark(models_file_path, benchmark_file_path, ollamabin):
-    models_dict = parse_yaml(models_file_path)
-    benchmark_dict = parse_yaml(benchmark_file_path)
-    allowed_models = {e['model'] for e in models_dict['models']}
-    ans = {}
-
-    for model in models_dict['models']:
-        model_name = model['model']
-        if model_name in allowed_models:
-            loc_dt = datetime.datetime.today()
-            file_path = f'log_{loc_dt.strftime("%Y-%m-%d-%H%M%S")}.log'
-            with open(file_path, "w", encoding='utf-8') as file:
-                stored_nums = []
-                for prompt in benchmark_dict['prompts']:
-                    prompt_text = prompt['prompt']
-                    print(f"prompt = {prompt_text}")
-                    result = subprocess.run([ollamabin, 'run', model_name, prompt_text, '--verbose'], capture_output=True, text=True, check=True, encoding='utf-8')
-                    std_err = result.stderr
-                    file.write(std_err)
-                    
-                    for line in std_err.split('\n'):
-                        if 'eval rate' in line and 'prompt' not in line:
-                            print(line)
-                            number = float(line[-20:-8])
-                            stored_nums.append(number)
-
-                print("-"*20) 
-                if stored_nums:
-                    average = sum(stored_nums) / len(stored_nums)
-                    print("Average of eval rate: ", round(average,3), " tokens/s")
-                    ans[model_name] = f"{round(average,3):.2f}"
-                print("-"*40)
-                file.write("\n"+"-"*40)
-
-    return ans
-
 if __name__ == "__main__": 
     args = parser.parse_args()
-    if (args.models is not None) and (args.benchmark is not None):
-        run_benchmark(args.models, args.benchmark)
-        print('-'*40)
+    #print(f"args.verbose value：{args.verbose}")
+    if (args.models is not None):
+        #print(f"args.models file path：{args.models}")
+        models_dict = parse_yaml(args.models)
         
-        
+        loc_dt = datetime.datetime.today()
+        # Writing to file
+        with open(f'log_{loc_dt.strftime("%Y-%m-%d-%H%M%S")}.log', "w") as file1:
+            for onemodel in models_dict['models']:
+                model_name = onemodel['model']
+                print(f'model_name =    {model_name}')
+                file1.write(f'\nmodel_name =    {model_name}\n')
+                
+                result = subprocess.run(['ollama', 'run', model_name,f'"Why is the sky blue?"','--verbose'], capture_output=True, text=True, check=True)
+                std_err = result.stderr
+                #print(result.stderr)
+                file1.write(std_err)
+                
+                for line in std_err.split('\n'):
+                    if ('eval rate' in line) and ('prompt' not in line):
+                        print(line)
+                        number = float(line[-20:-8])
+                        print(number)
+                        
+                
+                print("-"*40)
+                file1.write("\n"+"-"*40)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llm_bench-0.4.3/llm_bench/security_connection/connection.py` & `llm_bench-0.4.4/llm_bench/security_connection/connection.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.3/llm_bench/systeminfo/sysmain.py` & `llm_bench-0.4.4/llm_bench/systeminfo/sysmain.py`

 * *Files identical despite different names*

### Comparing `llm_bench-0.4.3/pyproject.toml` & `llm_bench-0.4.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm_bench"
-version = "0.4.3"
+version = "0.4.4"
 description = "Forked off of LLM Benchmark for Throughputs via Ollama"
 authors = ["Snaas"]
 license = "MIT"
 homepage = "https://github.com/b-Snaas/ollama-benchmark.git"
 readme = "README.md"
 keywords = [
     "benchmark",
```

### Comparing `llm_bench-0.4.3/README.md` & `llm_bench-0.4.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # llm-benchmark (ollama-benchmark)
 
 LLM Benchmark for Throughput via Ollama (Local LLMs)
 
 ## Installation Steps
 
 ```bash
-pip install llm-benchmark
+pip install llm-bench
 ```
 
 ## Usage for general users directly
 
 ```bash
-llm_benchmark run
+llm_bench run
 ```
 
-## Installation and Usage in Video format
-
-![llm-benchmark](https://github.com/aidatatools/ollama-benchmark/blob/main/llm-benchmark.gif)
-
-It's tested on Python 3.9 and above.
-
 ## ollama installation with the following models installed
 
 7B model can be run on machines with 8GB of RAM
 
 13B model can be run on machines with 16GB of RAM
 
 ## Usage explaination
@@ -78,25 +72,25 @@
 poetry install
 llm_benchmark hello jason
 ```
 
 ### Example #1 send systeminfo and benchmark results to a remote server
 
 ```bash
-llm_benchmark run
+llm_bench run
 ```
 
 ### Example #2 Do not send systeminfo and benchmark results to a remote server
 
 ```bash
-llm_benchmark run --no-sendinfo
+llm_bench run --no-sendinfo
 ```
 
 ### Example #3 Benchmark run on explicitly given the path to the ollama executable (When you built your own developer version of ollama)
 
 ```bash
-llm_benchmark run --ollamabin=~/code/ollama/ollama
+llm_bench run --ollamabin=~/code/ollama/ollama
 ```
 
 ## Reference
 
 [Ollama](https://ollama.com)
```

### Comparing `llm_bench-0.4.3/PKG-INFO` & `llm_bench-0.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_bench
-Version: 0.4.3
+Version: 0.4.4
 Summary: Forked off of LLM Benchmark for Throughputs via Ollama
 Home-page: https://github.com/b-Snaas/ollama-benchmark.git
 License: MIT
 Keywords: benchmark,llama,ollama,llms,local
 Author: Snaas
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -28,29 +28,23 @@
 # llm-benchmark (ollama-benchmark)
 
 LLM Benchmark for Throughput via Ollama (Local LLMs)
 
 ## Installation Steps
 
 ```bash
-pip install llm-benchmark
+pip install llm-bench
 ```
 
 ## Usage for general users directly
 
 ```bash
-llm_benchmark run
+llm_bench run
 ```
 
-## Installation and Usage in Video format
-
-![llm-benchmark](https://github.com/aidatatools/ollama-benchmark/blob/main/llm-benchmark.gif)
-
-It's tested on Python 3.9 and above.
-
 ## ollama installation with the following models installed
 
 7B model can be run on machines with 8GB of RAM
 
 13B model can be run on machines with 16GB of RAM
 
 ## Usage explaination
@@ -105,26 +99,26 @@
 poetry install
 llm_benchmark hello jason
 ```
 
 ### Example #1 send systeminfo and benchmark results to a remote server
 
 ```bash
-llm_benchmark run
+llm_bench run
 ```
 
 ### Example #2 Do not send systeminfo and benchmark results to a remote server
 
 ```bash
-llm_benchmark run --no-sendinfo
+llm_bench run --no-sendinfo
 ```
 
 ### Example #3 Benchmark run on explicitly given the path to the ollama executable (When you built your own developer version of ollama)
 
 ```bash
-llm_benchmark run --ollamabin=~/code/ollama/ollama
+llm_bench run --ollamabin=~/code/ollama/ollama
 ```
 
 ## Reference
 
 [Ollama](https://ollama.com)
```

