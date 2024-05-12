# Comparing `tmp/zarth_utils-1.0.tar.gz` & `tmp/zarth_utils-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarth_utils-1.0.tar", last modified: Sun Mar 17 18:37:54 2024, max compression
+gzip compressed data, was "zarth_utils-1.1.tar", last modified: Sun May 12 15:18:13 2024, max compression
```

## Comparing `zarth_utils-1.0.tar` & `zarth_utils-1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-03-17 18:37:54.117778 zarth_utils-1.0/
--rw-r--r--   0 ghzhang    (501) staff       (20)      973 2024-03-17 18:37:54.117579 zarth_utils-1.0/PKG-INFO
--rw-r--r--   0 ghzhang    (501) staff       (20)       57 2023-11-29 00:34:14.000000 zarth_utils-1.0/README.md
--rw-r--r--   0 ghzhang    (501) staff       (20)      614 2023-11-29 00:36:15.000000 zarth_utils-1.0/pyproject.toml
--rw-r--r--   0 ghzhang    (501) staff       (20)       90 2023-11-29 00:34:14.000000 zarth_utils-1.0/requirements.txt
--rw-r--r--   0 ghzhang    (501) staff       (20)       38 2024-03-17 18:37:54.117850 zarth_utils-1.0/setup.cfg
-drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-03-17 18:37:54.113714 zarth_utils-1.0/tests/
--rw-r--r--   0 ghzhang    (501) staff       (20)     1227 2023-11-29 00:35:23.000000 zarth_utils-1.0/tests/test_config.py
-drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-03-17 18:37:54.116062 zarth_utils-1.0/zarth_utils/
--rw-r--r--   0 ghzhang    (501) staff       (20)       78 2023-11-29 00:34:14.000000 zarth_utils-1.0/zarth_utils/__init__.py
--rw-r--r--   0 ghzhang    (501) staff       (20)     9978 2023-11-29 00:35:23.000000 zarth_utils-1.0/zarth_utils/config.py
--rw-r--r--   0 ghzhang    (501) staff       (20)     7215 2023-11-29 00:34:14.000000 zarth_utils-1.0/zarth_utils/drawer.py
--rw-r--r--   0 ghzhang    (501) staff       (20)      517 2023-11-29 00:34:14.000000 zarth_utils-1.0/zarth_utils/general_utils.py
--rw-r--r--   0 ghzhang    (501) staff       (20)      276 2023-11-29 00:34:14.000000 zarth_utils-1.0/zarth_utils/jupyter_utils.py
--rw-r--r--   0 ghzhang    (501) staff       (20)     1547 2023-11-29 00:34:14.000000 zarth_utils-1.0/zarth_utils/logger.py
--rw-r--r--   0 ghzhang    (501) staff       (20)    10011 2023-11-29 00:35:23.000000 zarth_utils-1.0/zarth_utils/nn_utils.py
--rw-r--r--   0 ghzhang    (501) staff       (20)    13043 2023-11-29 00:34:14.000000 zarth_utils-1.0/zarth_utils/result_recorder.py
--rw-r--r--   0 ghzhang    (501) staff       (20)     2255 2023-11-29 00:34:14.000000 zarth_utils-1.0/zarth_utils/text_processing.py
--rw-r--r--   0 ghzhang    (501) staff       (20)     2583 2023-11-29 00:34:14.000000 zarth_utils-1.0/zarth_utils/timer.py
-drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-03-17 18:37:54.116817 zarth_utils-1.0/zarth_utils.egg-info/
--rw-r--r--   0 ghzhang    (501) staff       (20)      973 2024-03-17 18:37:54.000000 zarth_utils-1.0/zarth_utils.egg-info/PKG-INFO
--rw-r--r--   0 ghzhang    (501) staff       (20)      491 2024-03-17 18:37:54.000000 zarth_utils-1.0/zarth_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ghzhang    (501) staff       (20)        1 2024-03-17 18:37:54.000000 zarth_utils-1.0/zarth_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ghzhang    (501) staff       (20)      211 2024-03-17 18:37:54.000000 zarth_utils-1.0/zarth_utils.egg-info/requires.txt
--rw-r--r--   0 ghzhang    (501) staff       (20)       12 2024-03-17 18:37:54.000000 zarth_utils-1.0/zarth_utils.egg-info/top_level.txt
+drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-12 15:18:13.871268 zarth_utils-1.1/
+-rw-r--r--   0 ghzhang    (501) staff       (20)      973 2024-05-12 15:18:13.871041 zarth_utils-1.1/PKG-INFO
+-rw-r--r--   0 ghzhang    (501) staff       (20)       57 2023-11-29 00:34:14.000000 zarth_utils-1.1/README.md
+-rw-r--r--   0 ghzhang    (501) staff       (20)      614 2024-05-12 15:12:05.000000 zarth_utils-1.1/pyproject.toml
+-rw-r--r--   0 ghzhang    (501) staff       (20)       90 2023-11-29 00:34:14.000000 zarth_utils-1.1/requirements.txt
+-rw-r--r--   0 ghzhang    (501) staff       (20)       38 2024-05-12 15:18:13.871322 zarth_utils-1.1/setup.cfg
+drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-12 15:18:13.866597 zarth_utils-1.1/tests/
+-rw-r--r--   0 ghzhang    (501) staff       (20)     1227 2023-11-29 00:35:23.000000 zarth_utils-1.1/tests/test_config.py
+drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-12 15:18:13.869183 zarth_utils-1.1/zarth_utils/
+-rw-r--r--   0 ghzhang    (501) staff       (20)       78 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/__init__.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)     9939 2024-05-12 15:11:46.000000 zarth_utils-1.1/zarth_utils/config.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)     7215 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/drawer.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)      517 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/general_utils.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)      276 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/jupyter_utils.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)     1547 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/logger.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)    10011 2023-11-29 00:35:23.000000 zarth_utils-1.1/zarth_utils/nn_utils.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)    13043 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/result_recorder.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)     2255 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/text_processing.py
+-rw-r--r--   0 ghzhang    (501) staff       (20)     2583 2023-11-29 00:34:14.000000 zarth_utils-1.1/zarth_utils/timer.py
+drwxr-xr-x   0 ghzhang    (501) staff       (20)        0 2024-05-12 15:18:13.870072 zarth_utils-1.1/zarth_utils.egg-info/
+-rw-r--r--   0 ghzhang    (501) staff       (20)      973 2024-05-12 15:18:13.000000 zarth_utils-1.1/zarth_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ghzhang    (501) staff       (20)      491 2024-05-12 15:18:13.000000 zarth_utils-1.1/zarth_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ghzhang    (501) staff       (20)        1 2024-05-12 15:18:13.000000 zarth_utils-1.1/zarth_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ghzhang    (501) staff       (20)      211 2024-05-12 15:18:13.000000 zarth_utils-1.1/zarth_utils.egg-info/requires.txt
+-rw-r--r--   0 ghzhang    (501) staff       (20)       12 2024-05-12 15:18:13.000000 zarth_utils-1.1/zarth_utils.egg-info/top_level.txt
```

### Comparing `zarth_utils-1.0/PKG-INFO` & `zarth_utils-1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zarth_utils
-Version: 1.0
+Version: 1.1
 Summary: Package used for my personal development on ML projects.
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Requires-Dist: pandas
 Requires-Dist: numpy
```

### Comparing `zarth_utils-1.0/pyproject.toml` & `zarth_utils-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zarth_utils"
 description = "Package used for my personal development on ML projects."
-version = "1.0"
+version = "1.1"
 dynamic = ["readme", "dependencies"]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
 all = ["nltk", "torch", "tensorflow", "jupyterlab"]
 hf = ["transformers", "accelerate", "trl", "datasets", "diffusers", "tokenizers", "huggingface_hub"]
```

### Comparing `zarth_utils-1.0/tests/test_config.py` & `zarth_utils-1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.0/zarth_utils/config.py` & `zarth_utils-1.1/zarth_utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,37 +99,37 @@
             return self[item]
         return default_value
 
     def show(self):
         """
         Show all the configs in logging. If get_logger is used before, then the outputs will also be in the log file.
         """
-        logging_info("\n%s" % json.dumps(self._nested_dict, sort_keys=True, indent=4, separators=(',', ': ')))
+        logging_info("\n%s" % json.dumps(self, sort_keys=True, indent=4, separators=(',', ': ')))
 
     def to_dict(self):
         """
         Return the config as a dict
         :return: config dict
         :rtype: dict
         """
-        return self._nested_dict
+        return self
 
     def dump(self, path_dump=None):
         """
         Dump the config in the path_dump.
         :param path_dump: the path to dump the config
         :type path_dump: str
         """
         if path_dump is None:
             makedir_if_not_exist(dir_configs)
             path_dump = os.path.join(dir_configs, "%s.json" % get_random_time_stamp())
         path_dump = "%s.json" % path_dump if not path_dump.endswith(".json") else path_dump
         assert not os.path.exists(path_dump)
         with open(path_dump, "w", encoding="utf-8") as fout:
-            json.dump(self._nested_dict, fout)
+            json.dump(self, fout)
 
 
 class Config(NestedDict):
     def __init__(self, default_config_file=None, default_config_dict=None, use_argparse=True, use_wandb=False):
         """
         Initialize the config. Note that either default_config_dict or default_config_file in json format must be
         provided! The keys will be transferred to argument names, and the type will be automatically detected. The
```

### Comparing `zarth_utils-1.0/zarth_utils/drawer.py` & `zarth_utils-1.1/zarth_utils/drawer.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.0/zarth_utils/general_utils.py` & `zarth_utils-1.1/zarth_utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.0/zarth_utils/logger.py` & `zarth_utils-1.1/zarth_utils/logger.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.0/zarth_utils/nn_utils.py` & `zarth_utils-1.1/zarth_utils/nn_utils.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.0/zarth_utils/result_recorder.py` & `zarth_utils-1.1/zarth_utils/result_recorder.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.0/zarth_utils/text_processing.py` & `zarth_utils-1.1/zarth_utils/text_processing.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.0/zarth_utils/timer.py` & `zarth_utils-1.1/zarth_utils/timer.py`

 * *Files identical despite different names*

### Comparing `zarth_utils-1.0/zarth_utils.egg-info/PKG-INFO` & `zarth_utils-1.1/zarth_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zarth_utils
-Version: 1.0
+Version: 1.1
 Summary: Package used for my personal development on ML projects.
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: matplotlib
 Requires-Dist: tqdm
 Requires-Dist: pandas
 Requires-Dist: numpy
```

