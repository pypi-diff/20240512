# Comparing `tmp/csa_ai_foundation_model_api_clients-0.1.0.tar.gz` & `tmp/csa_ai_foundation_model_api_clients-0.1.1.tar.gz`

## Comparing `csa_ai_foundation_model_api_clients-0.1.0.tar` & `csa_ai_foundation_model_api_clients-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/TODO.md
--rwxr-xr-x   0        0        0      358 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/manual-package-update.md
--rwxr-xr-x   0        0        0     1188 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/output-example.json
--rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/setup-venv.sh
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/.github/workflows/release.yml
--rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/__init__.py
--rwxr-xr-x   0        0        0     6559 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
--rwxr-xr-x   0        0        0     3412 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
--rwxr-xr-x   0        0        0     2900 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
--rwxr-xr-x   0        0        0     2353 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
--rwxr-xr-x   0        0        0      717 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/tests/dev/ask-chatgpt-the-capital-of-france.py
--rwxr-xr-x   0        0        0      715 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/tests/dev/ask-claude-the-capital-of-france.py
--rwxr-xr-x   0        0        0      715 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/tests/dev/ask-gemini-the-capital-of-france.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     2139 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/README.md
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/TODO.md
+-rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/manual-package-update.md
+-rwxr-xr-x   0        0        0     1188 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/output-example.json
+-rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/setup-venv.sh
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/__init__.py
+-rwxr-xr-x   0        0        0     6559 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0     6594 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
+-rwxr-xr-x   0        0        0     3412 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
+-rwxr-xr-x   0        0        0     2900 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
+-rwxr-xr-x   0        0        0     2353 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
+-rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/tests/dev/ask-chatgpt-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/tests/dev/ask-claude-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/tests/dev/ask-gemini-the-capital-of-france.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/.gitignore
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     2153 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/README.md
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.1/PKG-INFO
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/TODO.md` & `csa_ai_foundation_model_api_clients-0.1.1/TODO.md`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/output-example.json` & `csa_ai_foundation_model_api_clients-0.1.1/output-example.json`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py` & `csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py` & `csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/claude.py` & `csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/ai_client/claude.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py` & `csa_ai_foundation_model_api_clients-0.1.1/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/tests/dev/ask-chatgpt-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.1/tests/dev/ask-chatgpt-the-capital-of-france.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 # This is a local test for dev
 
-from foundation_model_api_clients import FoundationModelAPIClient
+from csa_ai_foundation_model_api_clients import FoundationModelAPIClient
 
 def main():
     model = 'chatgpt'
     system_prompt = "You are a helpful assistant who answers in rhyme."
     user_prompt = "What is the capital of "
     user_data = "France?"
     output_file = 'chatgpt-response.json'
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/tests/dev/ask-claude-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.1/tests/dev/ask-claude-the-capital-of-france.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 # This is a local test for dev
 
-from foundation_model_api_clients import FoundationModelAPIClient
+from csa_ai_foundation_model_api_clients import FoundationModelAPIClient
 
 def main():
     model = 'claude'
     system_prompt = "You are a helpful assistant who answers in rhyme."
     user_prompt = "What is the capital of "
     user_data = "France?"
     output_file = 'claude-response.json'
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/tests/dev/ask-gemini-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.1/tests/dev/ask-gemini-the-capital-of-france.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 # This is a local test for dev
 
-from foundation_model_api_clients import FoundationModelAPIClient
+from csa_ai_foundation_model_api_clients import FoundationModelAPIClient
 
 def main():
     model = 'gemini'
     system_prompt = "You are a helpful assistant who answers in rhyme."
     user_prompt = "What is the capital of "
     user_data = "France?"
     output_file = 'gemini-response.json'
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/.gitignore` & `csa_ai_foundation_model_api_clients-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/LICENSE` & `csa_ai_foundation_model_api_clients-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/README.md` & `csa_ai_foundation_model_api_clients-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -64,18 +64,18 @@
         output_file=output_file
     )
 
 if __name__ == '__main__':
     main()
 ```
 
-Using this as a command line tool (you must be in the directory where foundation_model_api_clients.py is because of a relative import path):
+Using this as a command line tool (you must be in the directory where csa_ai_foundation_model_api_clients.py is because of a relative import path):
 
 ```
-./foundation_model_api_clients.py \
+./csa_ai_foundation_model_api_clients.py \
     --model chatgpt \
     --system system-prompt.txt \
     --user-prompt user-prompt.txt \
     --user-data user-data.txt \
     --output output.json \
     --temperature 0.9 \
     --max_tokens 2000
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/pyproject.toml` & `csa_ai_foundation_model_api_clients-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "csa_ai_foundation_model_api_clients"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Kurt Seifried", email="kseifried@cloudsecurityalliance.org" },
 ]
 description = "Cloud Security Alliance AI Foundation Model API Clients"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.0/PKG-INFO` & `csa_ai_foundation_model_api_clients-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: csa_ai_foundation_model_api_clients
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cloud Security Alliance AI Foundation Model API Clients
 Project-URL: Homepage, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients
 Project-URL: Issues, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients/issues
 Author-email: Kurt Seifried <kseifried@cloudsecurityalliance.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -81,18 +81,18 @@
         output_file=output_file
     )
 
 if __name__ == '__main__':
     main()
 ```
 
-Using this as a command line tool (you must be in the directory where foundation_model_api_clients.py is because of a relative import path):
+Using this as a command line tool (you must be in the directory where csa_ai_foundation_model_api_clients.py is because of a relative import path):
 
 ```
-./foundation_model_api_clients.py \
+./csa_ai_foundation_model_api_clients.py \
     --model chatgpt \
     --system system-prompt.txt \
     --user-prompt user-prompt.txt \
     --user-data user-data.txt \
     --output output.json \
     --temperature 0.9 \
     --max_tokens 2000
```

