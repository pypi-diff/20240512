# Comparing `tmp/kaizen_cloudcode-0.1.0.tar.gz` & `tmp/kaizen_cloudcode-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaizen_cloudcode-0.1.0.tar", max compression
+gzip compressed data, was "kaizen_cloudcode-0.1.1.tar", max compression
```

## Comparing `kaizen_cloudcode-0.1.0.tar` & `kaizen_cloudcode-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34523 2024-04-16 19:38:13.717245 kaizen_cloudcode-0.1.0/LICENSE
--rw-r--r--   0        0        0     4135 2024-04-19 02:02:48.353320 kaizen_cloudcode-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-17 18:08:20.272050 kaizen_cloudcode-0.1.0/kaizen/actors/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 18:08:20.272374 kaizen_cloudcode-0.1.0/kaizen/generator/__init__.py
--rw-r--r--   0        0        0     4311 2024-04-18 22:07:33.124525 kaizen_cloudcode-0.1.0/kaizen/generator/ui.py
--rw-r--r--   0        0        0        0 2024-04-17 18:08:20.272684 kaizen_cloudcode-0.1.0/kaizen/helpers/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 02:55:31.311764 kaizen_cloudcode-0.1.0/kaizen/helpers/chunker.py
--rw-r--r--   0        0        0     1670 2024-04-18 22:06:52.505224 kaizen_cloudcode-0.1.0/kaizen/helpers/general.py
--rw-r--r--   0        0        0     2637 2024-05-10 14:53:15.132138 kaizen_cloudcode-0.1.0/kaizen/helpers/output.py
--rw-r--r--   0        0        0     1038 2024-05-10 14:53:15.112097 kaizen_cloudcode-0.1.0/kaizen/helpers/parser.py
--rw-r--r--   0        0        0        0 2024-04-17 18:08:20.273920 kaizen_cloudcode-0.1.0/kaizen/integrations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 18:08:20.274038 kaizen_cloudcode-0.1.0/kaizen/llms/__init__.py
--rw-r--r--   0        0        0     7183 2024-05-10 15:29:40.545078 kaizen_cloudcode-0.1.0/kaizen/llms/prompts.py
--rw-r--r--   0        0        0     1900 2024-05-10 15:32:01.508108 kaizen_cloudcode-0.1.0/kaizen/llms/provider.py
--rw-r--r--   0        0        0        0 2024-04-17 18:08:20.276705 kaizen_cloudcode-0.1.0/kaizen/reviewer/__init__.py
--rw-r--r--   0        0        0     2969 2024-05-10 14:53:15.133807 kaizen_cloudcode-0.1.0/kaizen/reviewer/code_review.py
--rw-r--r--   0        0        0     1386 2024-05-10 15:32:09.312980 kaizen_cloudcode-0.1.0/kaizen/reviewer/work_summarizer.py
--rw-r--r--   0        0        0        0 2024-04-17 18:08:20.277013 kaizen_cloudcode-0.1.0/kaizen/utils/__init__.py
--rw-r--r--   0        0        0     1103 2024-04-17 18:08:20.277545 kaizen_cloudcode-0.1.0/kaizen/utils/config.py
--rw-r--r--   0        0        0      753 2024-05-11 23:19:36.838459 kaizen_cloudcode-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-11 23:53:49.165611 kaizen_cloudcode-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4135 2024-05-11 23:53:49.165611 kaizen_cloudcode-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/actors/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/generator/__init__.py
+-rw-r--r--   0        0        0     3075 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/generator/ui.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/helpers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/helpers/chunker.py
+-rw-r--r--   0        0        0     1467 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/helpers/general.py
+-rw-r--r--   0        0        0     3611 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/helpers/output.py
+-rw-r--r--   0        0        0     1038 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/helpers/parser.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/integrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/llms/__init__.py
+-rw-r--r--   0        0        0     7183 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/llms/prompts.py
+-rw-r--r--   0        0        0     1900 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/llms/provider.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/reviewer/__init__.py
+-rw-r--r--   0        0        0     2969 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/reviewer/code_review.py
+-rw-r--r--   0        0        0     1386 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/reviewer/work_summarizer.py
+-rw-r--r--   0        0        0        0 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/utils/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/kaizen/utils/config.py
+-rw-r--r--   0        0        0      753 2024-05-11 23:53:49.169611 kaizen_cloudcode-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 kaizen_cloudcode-0.1.1/PKG-INFO
```

### Comparing `kaizen_cloudcode-0.1.0/LICENSE` & `kaizen_cloudcode-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.0/README.md` & `kaizen_cloudcode-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.0/kaizen/helpers/general.py` & `kaizen_cloudcode-0.1.1/kaizen/helpers/general.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import subprocess
 import json
 import os
 import re
 
 
 def run_test(code):
-    temp_file_path = "cloudcode/playwright/tests/temp.spec.js"
-    create_test_spec(code, temp_file_path)
-    result_json = run_test_script()
-    logs, test_result = extract_result(result_json)
-    delete_test_spec(temp_file_path)
 
-    return logs, test_result
+    # TODO: Update logic for pytest runner
+    
+    pass
 
 
 def clean_python_code(code):
     match = re.search(r"```(?:python)?\n(.*)\n```", code, re.DOTALL)
     if match:
         return match.group(1)
     return None
```

### Comparing `kaizen_cloudcode-0.1.0/kaizen/helpers/output.py` & `kaizen_cloudcode-0.1.1/kaizen/helpers/output.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 from playwright.async_api import async_playwright
 from bs4 import BeautifulSoup, Comment
 import asyncio
 import nest_asyncio
 import subprocess
 import os
+import json
+import general
 
 logger = logging.getLogger(__name__)
 
 
 PR_COLLAPSIBLE_TEMPLATE = """
 <details>
 <summary>{comment}</summary>
@@ -100,7 +102,32 @@
 
 def create_folder(folder_path):
     if not os.path.exists(folder_path):
         os.makedirs(folder_path)
         logger.debug(f"Folder '{folder_path}' created successfully.")
     else:
         logger.debug(f"Folder '{folder_path}' already exists.")
+
+
+def create_test_files(json_tests, folder_path):
+    with open(f"{folder_path}/tests.json", "w") as f:
+        f.write(json.dumps(json_tests))
+
+    for module in json_tests:
+        temp_folder_path = os.path.join(folder_path, module["folder_name"])
+        create_folder(temp_folder_path)
+
+        for test in module["tests"]:
+            file_path = os.path.join(
+                temp_folder_path,
+                "test_" + "_".join(test["test_name"].lower().split(" ")) + ".py",
+            )
+            with open(file_path, "w") as f:
+                cleaned_code = general.clean_python_code(test["code"])
+                if not cleaned_code:
+                    logger.info(f"Failed to clean code")
+                else:
+                    cleaned_code = (
+                        f"''' Module Name: {module['module_title']}\n '''\n\n"
+                        + cleaned_code
+                    )
+                    f.write(cleaned_code)
```

### Comparing `kaizen_cloudcode-0.1.0/kaizen/helpers/parser.py` & `kaizen_cloudcode-0.1.1/kaizen/helpers/parser.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.0/kaizen/llms/prompts.py` & `kaizen_cloudcode-0.1.1/kaizen/llms/prompts.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.0/kaizen/llms/provider.py` & `kaizen_cloudcode-0.1.1/kaizen/llms/provider.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.0/kaizen/reviewer/code_review.py` & `kaizen_cloudcode-0.1.1/kaizen/reviewer/code_review.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.0/kaizen/reviewer/work_summarizer.py` & `kaizen_cloudcode-0.1.1/kaizen/reviewer/work_summarizer.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.0/kaizen/utils/config.py` & `kaizen_cloudcode-0.1.1/kaizen/utils/config.py`

 * *Files identical despite different names*

### Comparing `kaizen_cloudcode-0.1.0/pyproject.toml` & `kaizen_cloudcode-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaizen-cloudcode"
-version = "0.1.0"
+version = "0.1.1"
 description = "An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly."
 authors = ["Saurav Panda <saurav.panda@cloudcode.ai>"]
 license = "Apache2.0"
 readme = "README.md"
 packages = [
     { include = "kaizen" }
 ]
```

### Comparing `kaizen_cloudcode-0.1.0/PKG-INFO` & `kaizen_cloudcode-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaizen-cloudcode
-Version: 0.1.0
+Version: 0.1.1
 Summary: An intelligent coding companion that accelerates your development workflow by providing efficient assistance, enabling you to craft high-quality code more rapidly.
 License: Apache2.0
 Author: Saurav Panda
 Author-email: saurav.panda@cloudcode.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.0 Summary: An
+Metadata-Version: 2.1 Name: kaizen-cloudcode Version: 0.1.1 Summary: An
 intelligent coding companion that accelerates your development workflow by
 providing efficient assistance, enabling you to craft high-quality code more
 rapidly. License: Apache2.0 Author: Saurav Panda Author-email:
 saurav.panda@cloudcode.ai Requires-Python: >=3.8.1,<4.0.0 Classifier: License
 :: Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

