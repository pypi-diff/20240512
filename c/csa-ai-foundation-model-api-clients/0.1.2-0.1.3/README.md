# Comparing `tmp/csa_ai_foundation_model_api_clients-0.1.2.tar.gz` & `tmp/csa_ai_foundation_model_api_clients-0.1.3.tar.gz`

## Comparing `csa_ai_foundation_model_api_clients-0.1.2.tar` & `csa_ai_foundation_model_api_clients-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/TODO.md
--rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/manual-package-update.md
--rwxr-xr-x   0        0        0     1188 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/output-example.json
--rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/setup-venv.sh
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/.github/workflows/release.yml
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/src/csa_ai_foundation_model_api_clients/__init__.py
--rwxr-xr-x   0        0        0     6559 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py
--rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
--rwxr-xr-x   0        0        0     3412 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
--rwxr-xr-x   0        0        0     2900 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
--rwxr-xr-x   0        0        0     2353 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
--rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/tests/dev/ask-chatgpt-the-capital-of-france.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/tests/dev/ask-claude-the-capital-of-france.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/tests/dev/ask-gemini-the-capital-of-france.py
--rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/.gitignore
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/LICENSE
--rwxr-xr-x   0        0        0     2153 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/README.md
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/TODO.md
+-rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/manual-package-update.md
+-rwxr-xr-x   0        0        0     1188 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/output-example.json
+-rwxr-xr-x   0        0        0      486 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/setup-venv.sh
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/src/csa_ai_foundation_model_api_clients/__init__.py
+-rwxr-xr-x   0        0        0     6594 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/src/csa_ai_foundation_model_api_clients/ai_client/__init__.py
+-rwxr-xr-x   0        0        0     3412 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py
+-rwxr-xr-x   0        0        0     2900 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/src/csa_ai_foundation_model_api_clients/ai_client/claude.py
+-rwxr-xr-x   0        0        0     2353 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py
+-rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/tests/dev/ask-chatgpt-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/tests/dev/ask-claude-the-capital-of-france.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/tests/dev/ask-gemini-the-capital-of-france.py
+-rwxr-xr-x   0        0        0     3078 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/.gitignore
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/LICENSE
+-rwxr-xr-x   0        0        0     2153 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/README.md
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 csa_ai_foundation_model_api_clients-0.1.3/PKG-INFO
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/TODO.md` & `csa_ai_foundation_model_api_clients-0.1.3/TODO.md`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/output-example.json` & `csa_ai_foundation_model_api_clients-0.1.3/output-example.json`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py` & `csa_ai_foundation_model_api_clients-0.1.3/src/csa_ai_foundation_model_api_clients/csa_ai_foundation_model_api_clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 
 import os
 import argparse
 import json
-from .ai_client import claude, chatgpt, gemini
+from csa_ai_foundation_model_api_clients.ai_client import claude, chatgpt, gemini
 
 class FoundationModelAPIClient:
     def __init__(self, *, model, api_key=None, system_prompt, system_prompt_type, user_prompt, user_prompt_type, user_data=None, user_data_type, output_file=None, temperature=None, max_tokens=None):
         #
         # Increment this when updating the model
         #
-        self.csa_ai_foundation_model_api_clients_version = "0.1.2"
+        self.csa_ai_foundation_model_api_clients_version = "0.1.3"
         self.model = model
         self.api_key = api_key or self.get_model_api_key()
         self.model_name = self.get_model_mapping()
         self.system_prompt = system_prompt
         self.system_prompt_type = system_prompt_type
         self.user_prompt = user_prompt
         self.user_prompt_type = user_prompt_type
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py` & `csa_ai_foundation_model_api_clients-0.1.3/src/csa_ai_foundation_model_api_clients/ai_client/chatgpt.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/src/csa_ai_foundation_model_api_clients/ai_client/claude.py` & `csa_ai_foundation_model_api_clients-0.1.3/src/csa_ai_foundation_model_api_clients/ai_client/claude.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py` & `csa_ai_foundation_model_api_clients-0.1.3/src/csa_ai_foundation_model_api_clients/ai_client/gemini.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/tests/dev/ask-chatgpt-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.3/tests/dev/ask-chatgpt-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/tests/dev/ask-claude-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.3/tests/dev/ask-claude-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/tests/dev/ask-gemini-the-capital-of-france.py` & `csa_ai_foundation_model_api_clients-0.1.3/tests/dev/ask-gemini-the-capital-of-france.py`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/.gitignore` & `csa_ai_foundation_model_api_clients-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/LICENSE` & `csa_ai_foundation_model_api_clients-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/README.md` & `csa_ai_foundation_model_api_clients-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/pyproject.toml` & `csa_ai_foundation_model_api_clients-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "csa_ai_foundation_model_api_clients"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Kurt Seifried", email="kseifried@cloudsecurityalliance.org" },
 ]
 description = "Cloud Security Alliance AI Foundation Model API Clients"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `csa_ai_foundation_model_api_clients-0.1.2/PKG-INFO` & `csa_ai_foundation_model_api_clients-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: csa_ai_foundation_model_api_clients
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cloud Security Alliance AI Foundation Model API Clients
 Project-URL: Homepage, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients
 Project-URL: Issues, https://github.com/CloudSecurityAlliance/csa-ai-foundation-model-api-clients/issues
 Author-email: Kurt Seifried <kseifried@cloudsecurityalliance.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

