# Comparing `tmp/pytest_ranking-0.2.9.tar.gz` & `tmp/pytest_ranking-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_ranking-0.2.9.tar", last modified: Fri May 10 20:49:27 2024, max compression
+gzip compressed data, was "pytest_ranking-0.3.0.tar", last modified: Sun May 12 12:30:03 2024, max compression
```

## Comparing `pytest_ranking-0.2.9.tar` & `pytest_ranking-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-10 20:49:27.363125 pytest_ranking-0.2.9/
--rw-r--r--   0 samcheng   (501) staff       (20)     1091 2023-12-04 16:30:45.000000 pytest_ranking-0.2.9/LICENSE
--rw-r--r--   0 samcheng   (501) staff       (20)       96 2024-02-17 03:47:33.000000 pytest_ranking-0.2.9/MANIFEST.in
--rw-r--r--   0 samcheng   (501) staff       (20)     6257 2024-05-10 20:49:27.362877 pytest_ranking-0.2.9/PKG-INFO
--rw-r--r--   0 samcheng   (501) staff       (20)     4776 2024-05-07 18:44:25.000000 pytest_ranking-0.2.9/README.md
--rw-r--r--   0 samcheng   (501) staff       (20)       38 2024-05-10 20:49:27.363172 pytest_ranking-0.2.9/setup.cfg
--rw-r--r--   0 samcheng   (501) staff       (20)     2211 2024-05-10 20:43:30.000000 pytest_ranking-0.2.9/setup.py
-drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-10 20:49:27.360260 pytest_ranking-0.2.9/src/
-drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-10 20:49:27.361436 pytest_ranking-0.2.9/src/pytest_ranking/
--rw-r--r--   0 samcheng   (501) staff       (20)       22 2024-02-17 03:49:46.000000 pytest_ranking-0.2.9/src/pytest_ranking/__init__.py
--rw-r--r--   0 samcheng   (501) staff       (20)     2747 2024-05-10 20:39:33.000000 pytest_ranking-0.2.9/src/pytest_ranking/change_tracker.py
--rw-r--r--   0 samcheng   (501) staff       (20)    10555 2024-05-08 19:54:23.000000 pytest_ranking-0.2.9/src/pytest_ranking/plugin.py
--rw-r--r--   0 samcheng   (501) staff       (20)      191 2024-05-08 19:54:27.000000 pytest_ranking-0.2.9/src/pytest_ranking/plugin_utils.py
-drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-10 20:49:27.362575 pytest_ranking-0.2.9/src/pytest_ranking.egg-info/
--rw-r--r--   0 samcheng   (501) staff       (20)     6257 2024-05-10 20:49:27.000000 pytest_ranking-0.2.9/src/pytest_ranking.egg-info/PKG-INFO
--rw-r--r--   0 samcheng   (501) staff       (20)      453 2024-05-10 20:49:27.000000 pytest_ranking-0.2.9/src/pytest_ranking.egg-info/SOURCES.txt
--rw-r--r--   0 samcheng   (501) staff       (20)        1 2024-05-10 20:49:27.000000 pytest_ranking-0.2.9/src/pytest_ranking.egg-info/dependency_links.txt
--rw-r--r--   0 samcheng   (501) staff       (20)       50 2024-05-10 20:49:27.000000 pytest_ranking-0.2.9/src/pytest_ranking.egg-info/entry_points.txt
--rw-r--r--   0 samcheng   (501) staff       (20)       20 2024-05-10 20:49:27.000000 pytest_ranking-0.2.9/src/pytest_ranking.egg-info/requires.txt
--rw-r--r--   0 samcheng   (501) staff       (20)       15 2024-05-10 20:49:27.000000 pytest_ranking-0.2.9/src/pytest_ranking.egg-info/top_level.txt
-drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-10 20:49:27.362365 pytest_ranking-0.2.9/tests/
--rw-r--r--   0 samcheng   (501) staff       (20)    14016 2024-05-07 21:07:06.000000 pytest_ranking-0.2.9/tests/test_pytest_ranking.py
+drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-12 12:30:03.725811 pytest_ranking-0.3.0/
+-rw-r--r--   0 samcheng   (501) staff       (20)     1091 2023-12-04 16:30:45.000000 pytest_ranking-0.3.0/LICENSE
+-rw-r--r--   0 samcheng   (501) staff       (20)       96 2024-02-17 03:47:33.000000 pytest_ranking-0.3.0/MANIFEST.in
+-rw-r--r--   0 samcheng   (501) staff       (20)     6257 2024-05-12 12:30:03.725529 pytest_ranking-0.3.0/PKG-INFO
+-rw-r--r--   0 samcheng   (501) staff       (20)     4776 2024-05-07 18:44:25.000000 pytest_ranking-0.3.0/README.md
+-rw-r--r--   0 samcheng   (501) staff       (20)       38 2024-05-12 12:30:03.725862 pytest_ranking-0.3.0/setup.cfg
+-rw-r--r--   0 samcheng   (501) staff       (20)     2211 2024-05-12 12:23:47.000000 pytest_ranking-0.3.0/setup.py
+drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-12 12:30:03.722549 pytest_ranking-0.3.0/src/
+drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-12 12:30:03.723828 pytest_ranking-0.3.0/src/pytest_ranking/
+-rw-r--r--   0 samcheng   (501) staff       (20)       22 2024-02-17 03:49:46.000000 pytest_ranking-0.3.0/src/pytest_ranking/__init__.py
+-rw-r--r--   0 samcheng   (501) staff       (20)     2721 2024-05-12 12:23:47.000000 pytest_ranking-0.3.0/src/pytest_ranking/change_tracker.py
+-rw-r--r--   0 samcheng   (501) staff       (20)    10555 2024-05-08 19:54:23.000000 pytest_ranking-0.3.0/src/pytest_ranking/plugin.py
+-rw-r--r--   0 samcheng   (501) staff       (20)      191 2024-05-08 19:54:27.000000 pytest_ranking-0.3.0/src/pytest_ranking/plugin_utils.py
+drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-12 12:30:03.725063 pytest_ranking-0.3.0/src/pytest_ranking.egg-info/
+-rw-r--r--   0 samcheng   (501) staff       (20)     6257 2024-05-12 12:30:03.000000 pytest_ranking-0.3.0/src/pytest_ranking.egg-info/PKG-INFO
+-rw-r--r--   0 samcheng   (501) staff       (20)      453 2024-05-12 12:30:03.000000 pytest_ranking-0.3.0/src/pytest_ranking.egg-info/SOURCES.txt
+-rw-r--r--   0 samcheng   (501) staff       (20)        1 2024-05-12 12:30:03.000000 pytest_ranking-0.3.0/src/pytest_ranking.egg-info/dependency_links.txt
+-rw-r--r--   0 samcheng   (501) staff       (20)       50 2024-05-12 12:30:03.000000 pytest_ranking-0.3.0/src/pytest_ranking.egg-info/entry_points.txt
+-rw-r--r--   0 samcheng   (501) staff       (20)       20 2024-05-12 12:30:03.000000 pytest_ranking-0.3.0/src/pytest_ranking.egg-info/requires.txt
+-rw-r--r--   0 samcheng   (501) staff       (20)       15 2024-05-12 12:30:03.000000 pytest_ranking-0.3.0/src/pytest_ranking.egg-info/top_level.txt
+drwxr-xr-x   0 samcheng   (501) staff       (20)        0 2024-05-12 12:30:03.724825 pytest_ranking-0.3.0/tests/
+-rw-r--r--   0 samcheng   (501) staff       (20)    14016 2024-05-07 21:07:06.000000 pytest_ranking-0.3.0/tests/test_pytest_ranking.py
```

### Comparing `pytest_ranking-0.2.9/LICENSE` & `pytest_ranking-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_ranking-0.2.9/PKG-INFO` & `pytest_ranking-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ranking
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Pytest plugin for automatically prioritizing/ranking tests to speed up failure detection
 Home-page: https://github.com/softwareTestingResearch/pytest-ranking
 Author: softwareTestingResearch
 Author-email: testingresearch4all@gmail.com
 Maintainer: softwareTestingResearch
 Maintainer-email: testingresearch4all@gmail.com
 License: MIT
```

### Comparing `pytest_ranking-0.2.9/README.md` & `pytest_ranking-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_ranking-0.2.9/setup.py` & `pytest_ranking-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-ranking',
-    version='0.2.9',
+    version='0.3.0',
     author='softwareTestingResearch',
     author_email='testingresearch4all@gmail.com',
     maintainer='softwareTestingResearch',
     maintainer_email='testingresearch4all@gmail.com',
     license='MIT',
     url='https://github.com/softwareTestingResearch/pytest-ranking',
     description='A Pytest plugin for automatically'
```

### Comparing `pytest_ranking-0.2.9/src/pytest_ranking/change_tracker.py` & `pytest_ranking-0.3.0/src/pytest_ranking/change_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 def tokenize(string: str) -> list[str]:
     return re.findall(r'[a-zA-Z0-9]+', string.lower())
 
 
 class changeTracker:
     def __init__(self, pytest_config: Config) -> None:
         self.pytest_config = pytest_config
-        # record overhead
-        self.overhead = 0
         self.delta = set()
+        self.num_delta_files = 0
+        self.overhead = 0
         # get data of the set of changed files
         self.get_delta()
 
     def get_all_file_paths(self):
         """Get all file paths in the codebase"""
         pattern = os.path.join(self.pytest_config.rootpath, "**/*.py")
         file_paths = glob.glob(pattern, recursive=True)
@@ -56,15 +56,14 @@
 
         # if hashes are computed for the first time
         if old_hashes == {}:
             self.overhead += time.time() - start_time
             return len(file_paths)
 
         # get files with a different/new hash since last run
-        self.num_delta_files = 0
         for path, hash in hashes.items():
             if path not in old_hashes or old_hashes[path] != hash:
                 self.delta = self.delta.union(tokenize(path))
                 self.num_delta_files += 1
         self.overhead += time.time() - start_time
 
     def compute_test_suite_relatedness(self, items: list[Item]) -> None:
```

### Comparing `pytest_ranking-0.2.9/src/pytest_ranking/plugin.py` & `pytest_ranking-0.3.0/src/pytest_ranking/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_ranking-0.2.9/src/pytest_ranking.egg-info/PKG-INFO` & `pytest_ranking-0.3.0/src/pytest_ranking.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ranking
-Version: 0.2.9
+Version: 0.3.0
 Summary: A Pytest plugin for automatically prioritizing/ranking tests to speed up failure detection
 Home-page: https://github.com/softwareTestingResearch/pytest-ranking
 Author: softwareTestingResearch
 Author-email: testingresearch4all@gmail.com
 Maintainer: softwareTestingResearch
 Maintainer-email: testingresearch4all@gmail.com
 License: MIT
```

### Comparing `pytest_ranking-0.2.9/tests/test_pytest_ranking.py` & `pytest_ranking-0.3.0/tests/test_pytest_ranking.py`

 * *Files identical despite different names*

