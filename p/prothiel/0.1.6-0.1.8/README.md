# Comparing `tmp/prothiel-0.1.6.tar.gz` & `tmp/prothiel-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prothiel-0.1.6.tar", last modified: Fri May 10 13:45:59 2024, max compression
+gzip compressed data, was "prothiel-0.1.8.tar", last modified: Fri May 10 13:59:10 2024, max compression
```

## Comparing `prothiel-0.1.6.tar` & `prothiel-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:45:59.166335 prothiel-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 13:45:53.000000 prothiel-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-10 13:45:59.166335 prothiel-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-10 13:45:53.000000 prothiel-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:45:59.166335 prothiel-0.1.6/prothiel/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 13:45:53.000000 prothiel-0.1.6/prothiel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-10 13:45:53.000000 prothiel-0.1.6/prothiel/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 13:45:53.000000 prothiel-0.1.6/prothiel/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-10 13:45:53.000000 prothiel-0.1.6/prothiel/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-10 13:45:53.000000 prothiel-0.1.6/prothiel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:45:59.166335 prothiel-0.1.6/prothiel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 13:45:59.000000 prothiel-0.1.6/prothiel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-10 13:45:53.000000 prothiel-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:45:59.166335 prothiel-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-10 13:45:53.000000 prothiel-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:45:59.166335 prothiel-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-10 13:45:53.000000 prothiel-0.1.6/tests/test_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:10.756093 prothiel-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-10 13:59:05.000000 prothiel-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-10 13:59:10.756093 prothiel-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-10 13:59:05.000000 prothiel-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:10.756093 prothiel-0.1.8/prothiel/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 13:59:05.000000 prothiel-0.1.8/prothiel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-10 13:59:05.000000 prothiel-0.1.8/prothiel/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-10 13:59:05.000000 prothiel-0.1.8/prothiel/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-10 13:59:05.000000 prothiel-0.1.8/prothiel/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-10 13:59:05.000000 prothiel-0.1.8/prothiel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:10.756093 prothiel-0.1.8/prothiel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-05-10 13:59:10.000000 prothiel-0.1.8/prothiel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-10 13:59:10.000000 prothiel-0.1.8/prothiel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:59:10.000000 prothiel-0.1.8/prothiel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-10 13:59:10.000000 prothiel-0.1.8/prothiel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-10 13:59:10.000000 prothiel-0.1.8/prothiel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 13:59:10.000000 prothiel-0.1.8/prothiel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-10 13:59:05.000000 prothiel-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:59:10.756093 prothiel-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-10 13:59:05.000000 prothiel-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:59:10.756093 prothiel-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-10 13:59:05.000000 prothiel-0.1.8/tests/test_extract.py
```

### Comparing `prothiel-0.1.6/LICENSE` & `prothiel-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `prothiel-0.1.6/PKG-INFO` & `prothiel-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prothiel
-Version: 0.1.6
+Version: 0.1.8
 Home-page: https://github.com/Sunwood-ai-labs/Prothiel
 Author: Maki
 Author-email: sunwood.ai.labs@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `prothiel-0.1.6/README.md` & `prothiel-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `prothiel-0.1.6/prothiel/cli.py` & `prothiel-0.1.8/prothiel/cli.py`

 * *Files identical despite different names*

### Comparing `prothiel-0.1.6/prothiel/extract.py` & `prothiel-0.1.8/prothiel/extract.py`

 * *Files identical despite different names*

### Comparing `prothiel-0.1.6/prothiel/run_tests.py` & `prothiel-0.1.8/prothiel/run_tests.py`

 * *Files identical despite different names*

### Comparing `prothiel-0.1.6/prothiel.egg-info/PKG-INFO` & `prothiel-0.1.8/prothiel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prothiel
-Version: 0.1.6
+Version: 0.1.8
 Home-page: https://github.com/Sunwood-ai-labs/Prothiel
 Author: Maki
 Author-email: sunwood.ai.labs@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
```

### Comparing `prothiel-0.1.6/setup.py` & `prothiel-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # READMEファイルの内容を読み込む
 with open("README.md", "r", encoding="utf-8") as fh:
    long_description = fh.read()
 
 setup(
     name='prothiel',
-    version="0.1.6",
+    version="0.1.8",
     # PyPIに表示される長い説明文
     long_description=long_description,
     # 長い説明文のフォーマット
     long_description_content_type="text/markdown",
     # プロジェクトのURL
     url="https://github.com/Sunwood-ai-labs/Prothiel",
     author='Maki',
```

### Comparing `prothiel-0.1.6/tests/test_extract.py` & `prothiel-0.1.8/tests/test_extract.py`

 * *Files identical despite different names*

