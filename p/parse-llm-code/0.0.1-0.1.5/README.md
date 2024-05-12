# Comparing `tmp/parse_llm_code-0.0.1.tar.gz` & `tmp/parse_llm_code-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parse_llm_code-0.0.1.tar", last modified: Sat May 11 18:46:49 2024, max compression
+gzip compressed data, was "parse_llm_code-0.1.5.tar", last modified: Sun May 12 12:03:20 2024, max compression
```

## Comparing `parse_llm_code-0.0.1.tar` & `parse_llm_code-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-11 18:46:49.580712 parse_llm_code-0.0.1/
--rw-r--r--   0 apple      (501) staff       (20)     1239 2024-05-11 18:46:49.580525 parse_llm_code-0.0.1/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      843 2024-05-11 18:45:33.000000 parse_llm_code-0.0.1/README.md
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-11 18:46:49.579488 parse_llm_code-0.0.1/parse_llm_code/
--rw-r--r--   0 apple      (501) staff       (20)       24 2024-05-11 17:50:26.000000 parse_llm_code-0.0.1/parse_llm_code/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1524 2024-05-11 18:44:00.000000 parse_llm_code-0.0.1/parse_llm_code/extract_code.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-11 18:46:49.580356 parse_llm_code-0.0.1/parse_llm_code.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     1239 2024-05-11 18:46:49.000000 parse_llm_code-0.0.1/parse_llm_code.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      273 2024-05-11 18:46:49.000000 parse_llm_code-0.0.1/parse_llm_code.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2024-05-11 18:46:49.000000 parse_llm_code-0.0.1/parse_llm_code.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       21 2024-05-11 18:46:49.000000 parse_llm_code-0.0.1/parse_llm_code.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)       38 2024-05-11 18:46:49.580752 parse_llm_code-0.0.1/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)      628 2024-05-11 18:04:35.000000 parse_llm_code-0.0.1/setup.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-11 18:46:49.580175 parse_llm_code-0.0.1/tests/
--rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-11 18:16:52.000000 parse_llm_code-0.0.1/tests/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1735 2024-05-11 18:43:27.000000 parse_llm_code-0.0.1/tests/test_extract_code.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-12 12:03:20.383337 parse_llm_code-0.1.5/
+-rw-r--r--   0 apple      (501) staff       (20)     2566 2024-05-12 12:03:20.383116 parse_llm_code-0.1.5/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     2170 2024-05-12 04:20:35.000000 parse_llm_code-0.1.5/README.md
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-12 12:03:20.381957 parse_llm_code-0.1.5/parse_llm_code/
+-rw-r--r--   0 apple      (501) staff       (20)      189 2024-05-12 03:59:03.000000 parse_llm_code-0.1.5/parse_llm_code/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1945 2024-05-12 03:34:57.000000 parse_llm_code-0.1.5/parse_llm_code/extract_code.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-12 12:03:20.382910 parse_llm_code-0.1.5/parse_llm_code.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     2566 2024-05-12 12:03:20.000000 parse_llm_code-0.1.5/parse_llm_code.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      307 2024-05-12 12:03:20.000000 parse_llm_code-0.1.5/parse_llm_code.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2024-05-12 12:03:20.000000 parse_llm_code-0.1.5/parse_llm_code.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)       21 2024-05-12 12:03:20.000000 parse_llm_code-0.1.5/parse_llm_code.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)       38 2024-05-12 12:03:20.383383 parse_llm_code-0.1.5/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)      628 2024-05-12 12:03:16.000000 parse_llm_code-0.1.5/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2024-05-12 12:03:20.382741 parse_llm_code-0.1.5/tests/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2024-05-11 18:16:52.000000 parse_llm_code-0.1.5/tests/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1719 2024-05-12 04:13:51.000000 parse_llm_code-0.1.5/tests/test_extract_codes.py
+-rw-r--r--   0 apple      (501) staff       (20)     1257 2024-05-12 04:11:36.000000 parse_llm_code-0.1.5/tests/test_extract_first_code.py
```

### Comparing `parse_llm_code-0.0.1/parse_llm_code/extract_code.py` & `parse_llm_code-0.1.5/parse_llm_code/extract_code.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         }
 
 
 class CodeBlocks:
     def __init__(self, code_list: List[CodeBlock]):
         self.length: int = len(code_list)
         self.code_list: List[CodeBlock] = code_list
+        self.first: CodeBlock = code_list[0] if len(code_list) > 0 else None
         self.code_dict_list: List = [
             {
                 "language": code.language,
                 "context": code.context,
                 "length": code.length,
                 "lines": code.lines,
                 "include_try": code.include_try,
@@ -45,7 +46,18 @@
     pattern = r"```(\w+)\n(.*?)\n```"
     matches = re.findall(pattern, md_string, re.DOTALL)
     for match in matches:
         language = match[0]
         context = match[1]
         code_blocks.append(CodeBlock(language, context))
     return CodeBlocks(code_blocks)
+
+
+def extract_first_code(md_string) -> CodeBlock:
+    code_blocks = []
+    pattern = r"```(\w+)\n(.*?)\n```"
+    matches = re.findall(pattern, md_string, re.DOTALL)
+    for match in matches:
+        language = match[0]
+        context = match[1]
+        code_blocks.append(CodeBlock(language, context))
+    return CodeBlocks(code_blocks).first
```

### Comparing `parse_llm_code-0.0.1/setup.py` & `parse_llm_code-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="parse_llm_code",
-    version="0.0.1",
+    version="0.1.5",
     author="aboutmydreams",
     author_email="aboutmydreams@163.com",
     description="a lib to parse llm answer to code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/parse_llm_code",
     packages=setuptools.find_packages(),
```

### Comparing `parse_llm_code-0.0.1/tests/test_extract_code.py` & `parse_llm_code-0.1.5/tests/test_extract_codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from parse_llm_code.extract_code import extract_code_blocks
+from parse_llm_code import extract_code_blocks
 
 import unittest
 
 test_string = """
 ```python
 print('first line')
 print('second line')
@@ -18,29 +18,28 @@
     def test_length(self):
         result = extract_code_blocks(test_string)
         self.assertEqual(result.length, 2, "length test failed: expected 2")
 
     def test_language(self):
         result = extract_code_blocks(test_string)
         self.assertEqual(
-            result.codes[0].language,
+            result.code_list[0].language,
             "python",
-            f"language test case failed: {result.codes[0].language} != 'python' ",
+            f"language test case failed: {result.code_list[0].language} != 'python' ",
         )
         self.assertEqual(
-            result.codes[1].language,
+            result.code_list[1].language,
             "typescript",
-            f"language test case failed: {result.codes[1].language} != 'typescript' ",
+            f"language test case failed: {result.code_list[1].language} != 'typescript' ",
         )
 
     def test_blocks_dic_list(self):
         result = extract_code_blocks(test_string)
-        print(result.dict)
         self.assertEqual(
-            result.length,
+            result.code_dict_list,
             [
                 {
                     "language": "python",
                     "context": "print('first line')\nprint('second line')",
                     "length": 40,
                     "lines": 2,
                     "include_try": False,
```

