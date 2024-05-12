# Comparing `tmp/csa_ai_foundation_model_api_clients-0.0.9.tar.gz` & `tmp/csa_ai_foundation_model_api_clients-0.1.0.tar.gz`

## Comparing `csa_ai_foundation_model_api_clients-0.0.9.tar` & `csa_ai_foundation_model_api_clients-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rwxr-xr-x   0        0        0      333 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/manual-package-update.md
--rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/setup-venv.sh
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/.github/workflows/release.yml
--rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/src/csa_ai_foundation_model_api_clients/__init__.py
--rwxr-xr-x   0        0        0     4082 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
--rwxr-xr-x   0        0        0     3023 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
--rwxr-xr-x   0        0        0     2515 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
--rwxr-xr-x   0        0        0     1688 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
--rwxr-xr-x   0        0        0      578 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/tests/ask-chatgpt-the-capital-of-france.py
--rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/tests/ask-claude-the-capital-of-france.py
--rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/tests/ask-gemini-the-capital-of-france.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/LICENSE
--rwxr-xr-x   0        0        0     1418 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/README.md
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.0.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/TODO.md
+-rwxr-xr-x   0        0        0      358 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/manual-package-update.md
+-rwxr-xr-x   0        0        0     1188 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/output-example.json
+-rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/setup-venv.sh
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/__init__.py
+-rwxr-xr-x   0        0        0     6559 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
+-rwxr-xr-x   0        0        0     3412 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
+-rwxr-xr-x   0        0        0     2900 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
+-rwxr-xr-x   0        0        0     2353 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
+-rwxr-xr-x   0        0        0      717 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/tests/dev/ask-chatgpt-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      715 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/tests/dev/ask-claude-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      715 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/tests/dev/ask-gemini-the-capital-of-france.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/.gitignore
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/LICENSE
+-rwxr-xr-x   0        0        0     2139 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/README.md
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.0/PKG-INFO
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.9/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py` & `csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,16 +56,18 @@
             "completion_tokens": tokens_output,
             "total_tokens": total_tokens
         }
     }
     
     try:
         response_message = completion.choices[0].message.content
+        status = "success"
     except AttributeError:
         response_message = None
+        status = "error"
 
     ai_output = {
         "$id": "csa-ai-toolkit-openai-chatgpt4-JSON-v1_00",
         "metadata": {
             "system": system_prompt,
             "user-prompt": user_prompt,
             "user-data": kwargs.get('user_data'),
@@ -80,10 +82,22 @@
             "time_complete": TIME_FINISHED,
             "time_to_run": TIME_TO_RUN
         },
         "extracted_data": response_message,
         "completion": serialized_completion
     }
 
-    ai_output = {key: value for key, value in ai_output.items() if value is not None}
+    api_response = {
+        "status": "success",
+        "ai_query_time": TIME_START,
+        "ai_response_time": TIME_FINISHED,
+        "ai_runtime": TIME_TO_RUN,
+        "tokens_input": tokens_input,
+        "tokens_output": tokens_output,
+        "tokens_total": total_tokens,
+        "ai_response_http_status_code": None,
+        "ai_response_stop_reason": None,
+        "ai_response_data": response_message
+    }
+
 
-    return ai_output
+    return api_response
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.9/src/csa_ai_foundation_model_api_clients/ai_client/claude.py` & `csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/claude.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,16 +45,18 @@
             "completion_tokens": tokens_output,
             "total_tokens": total_tokens
         }
     }
 
     try:
         response_message = completion.content[0].text
+        status = "success"
     except AttributeError:
         response_message = None
+        status = "error"
 
     ai_output = {
         "$id": "csa-ai-toolkit-anthropic-claude3-JSON-v1_00",
         "metadata": {
             "system": system_prompt,
             "user-prompt": user_prompt,
             "user-data": kwargs.get('user_data'),
@@ -69,10 +71,21 @@
             "time_complete": TIME_FINISHED,
             "time_to_run": TIME_TO_RUN
         },
         "extracted_data": response_message,
         "completion": serialized_completion
     }
 
-    ai_output = {key: value for key, value in ai_output.items() if value is not None}
+    api_response = {
+        "status": status,
+        "ai_query_time": TIME_START,
+        "ai_response_time": TIME_FINISHED,
+        "ai_runtime": TIME_TO_RUN,
+        "tokens_input": tokens_input,
+        "tokens_output": tokens_output,
+        "tokens_total": total_tokens,
+        "ai_response_http_status_code": None,
+        "ai_response_stop_reason": None,
+        "ai_response_data": response_message
+    }
 
-    return ai_output
+    return api_response
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.9/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py` & `csa_ai_foundation_model_api_clients-0.1.0/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,14 +29,25 @@
 
     time_start = datetime.datetime.fromisoformat(TIME_START)
     time_complete = datetime.datetime.fromisoformat(TIME_FINISHED)
 
     duration = time_complete - time_start
     TIME_TO_RUN = duration.total_seconds()
 
+    try:
+        response_message = response.text
+        status = "success"
+    except AttributeError:
+        response_message = None
+        status = "error"
+
+    # https://cloud.google.com/vertex-ai/generative-ai/docs/multimodal/get-token-count
+    # response = model.count_tokens(prompt)
+    # print(f"Prompt Token Count: {response.total_tokens}")
+
     ai_output = {
         "$id": "csa-ai-toolkit-google-gemini1.5-JSON-v1_00",
         "metadata": {
             "system": system_prompt,
             "user-prompt": user_prompt,
             "user-data": kwargs.get('user_data'),
             "output": kwargs.get('output_file'),
@@ -46,10 +57,21 @@
             "time_start": TIME_START,
             "time_complete": TIME_FINISHED,
             "time_to_run": TIME_TO_RUN
         },
         "extracted_data": response.text
     }
 
-    ai_output = {key: value for key, value in ai_output.items() if value is not None}
+    api_response = {
+        "status": "success",
+        "ai_query_time": TIME_START,
+        "ai_response_time": TIME_FINISHED,
+        "ai_runtime": TIME_TO_RUN,
+        "tokens_input": None,
+        "tokens_output": None,
+        "tokens_total": None,
+        "ai_response_http_status_code": None,
+        "ai_response_stop_reason": None,
+        "ai_response_data": response_message
+    }
 
-    return ai_output
+    return api_response
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.9/.gitignore` & `csa_ai_foundation_model_api_clients-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.9/LICENSE` & `csa_ai_foundation_model_api_clients-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.0.9/README.md` & `csa_ai_foundation_model_api_clients-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -23,30 +23,38 @@
 * top_p
 * top_k
 * model specific paramaters
 
 Please note this code does not have tests, or good error handling, but it works. Also with respect to handling rate
 limiting that is on the todo, but currently if you use this tool put a sleep statement to slow it down.
 
+The code will be looking for the API key as an env variable:
+
+* ANTHROPIC_CLAUDE_API_KEY
+* GOOGLE_GEMINI_API_KEY
+* OPENAI_CHATGPT_API_KEY
+
 ## Examples:
 
+Using this as a library:
+
 ```
 #!/usr/bin/env python3
 
 import os
 
-from foundation_model_api_clients import FoundationModelAPIClient
+from csa_ai_foundation_model_api_clients import FoundationModelAPIClient
 
 def main():
-    model_name = 'claude'
-    api_key = os.getenv('ANTHROPIC_CLAUDE_API_KEY')
+    model_name = 'claude' # or "claude-haiku" or "chatgpt" or "gemini"
+    api_key = "SECRET_API_KEY_VALUE" # You can remove api_key here if the env variable is set 
 
-    client = FoundationModelAPIClient(model_name, api_key)
+    client = FoundationModelAPIClient(model_name, api_key) # You can remove api_key here if the env variable is set 
 
-    system_prompt = "You are a helpful assistant."
+    system_prompt = "You are a helpful assistant who speaks in rhymes."
     user_prompt = "What is the capital of France?"
     user_data = None
     output_file = 'response.json'
 
     response = client.generate_response(
         system_prompt,
         user_prompt,
@@ -56,8 +64,20 @@
         output_file=output_file
     )
 
 if __name__ == '__main__':
     main()
 ```
 
+Using this as a command line tool (you must be in the directory where foundation_model_api_clients.py is because of a relative import path):
+
+```
+./foundation_model_api_clients.py \
+    --model chatgpt \
+    --system system-prompt.txt \
+    --user-prompt user-prompt.txt \
+    --user-data user-data.txt \
+    --output output.json \
+    --temperature 0.9 \
+    --max_tokens 2000
+```
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.9/pyproject.toml` & `csa_ai_foundation_model_api_clients-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "csa_ai_foundation_model_api_clients"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Kurt Seifried", email="kseifried@cloudsecurityalliance.org" },
 ]
 description = "Cloud Security Alliance AI Foundation Model API Clients"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `csa_ai_foundation_model_api_clients-0.0.9/PKG-INFO` & `csa_ai_foundation_model_api_clients-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: csa_ai_foundation_model_api_clients
-Version: 0.0.9
+Version: 0.1.0
 Summary: Cloud Security Alliance AI Foundation Model API Clients
 Project-URL: Homepage, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients
 Project-URL: Issues, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients/issues
 Author-email: Kurt Seifried <kseifried@cloudsecurityalliance.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -40,30 +40,38 @@
 * top_p
 * top_k
 * model specific paramaters
 
 Please note this code does not have tests, or good error handling, but it works. Also with respect to handling rate
 limiting that is on the todo, but currently if you use this tool put a sleep statement to slow it down.
 
+The code will be looking for the API key as an env variable:
+
+* ANTHROPIC_CLAUDE_API_KEY
+* GOOGLE_GEMINI_API_KEY
+* OPENAI_CHATGPT_API_KEY
+
 ## Examples:
 
+Using this as a library:
+
 ```
 #!/usr/bin/env python3
 
 import os
 
-from foundation_model_api_clients import FoundationModelAPIClient
+from csa_ai_foundation_model_api_clients import FoundationModelAPIClient
 
 def main():
-    model_name = 'claude'
-    api_key = os.getenv('ANTHROPIC_CLAUDE_API_KEY')
+    model_name = 'claude' # or "claude-haiku" or "chatgpt" or "gemini"
+    api_key = "SECRET_API_KEY_VALUE" # You can remove api_key here if the env variable is set 
 
-    client = FoundationModelAPIClient(model_name, api_key)
+    client = FoundationModelAPIClient(model_name, api_key) # You can remove api_key here if the env variable is set 
 
-    system_prompt = "You are a helpful assistant."
+    system_prompt = "You are a helpful assistant who speaks in rhymes."
     user_prompt = "What is the capital of France?"
     user_data = None
     output_file = 'response.json'
 
     response = client.generate_response(
         system_prompt,
         user_prompt,
@@ -73,8 +81,20 @@
         output_file=output_file
     )
 
 if __name__ == '__main__':
     main()
 ```
 
+Using this as a command line tool (you must be in the directory where foundation_model_api_clients.py is because of a relative import path):
+
+```
+./foundation_model_api_clients.py \
+    --model chatgpt \
+    --system system-prompt.txt \
+    --user-prompt user-prompt.txt \
+    --user-data user-data.txt \
+    --output output.json \
+    --temperature 0.9 \
+    --max_tokens 2000
+```
```

