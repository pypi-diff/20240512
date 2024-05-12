# Comparing `tmp/malet-0.1.8.tar.gz` & `tmp/malet-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malet-0.1.8.tar", last modified: Tue Apr  2 13:52:29 2024, max compression
+gzip compressed data, was "malet-0.1.9.tar", last modified: Wed Apr 17 13:56:28 2024, max compression
```

## Comparing `malet-0.1.8.tar` & `malet-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:29.183107 malet-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-02 13:52:21.000000 malet-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-04-02 13:52:29.183107 malet-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22931 2024-04-02 13:52:21.000000 malet-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-02 13:52:21.000000 malet-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:52:29.183107 malet-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:29.179108 malet-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:29.179108 malet-0.1.8/src/malet/
--rw-r--r--   0 runner    (1001) docker     (127)    24765 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/get_slurm_run_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:29.183107 malet-0.1.8/src/malet/plot_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/plot_utils/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/plot_utils/plot_drawer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/plot_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-02 13:52:21.000000 malet-0.1.8/src/malet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:29.183107 malet-0.1.8/src/malet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 13:52:29.000000 malet-0.1.8/src/malet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:56:28.057901 malet-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-17 13:56:19.000000 malet-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    25213 2024-04-17 13:56:28.053901 malet-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23034 2024-04-17 13:56:19.000000 malet-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-17 13:56:19.000000 malet-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 13:56:28.057901 malet-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:56:28.049901 malet-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:56:28.053901 malet-0.1.9/src/malet/
+-rw-r--r--   0 runner    (1001) docker     (127)    25649 2024-04-17 13:56:19.000000 malet-0.1.9/src/malet/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-17 13:56:19.000000 malet-0.1.9/src/malet/get_slurm_run_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-17 13:56:19.000000 malet-0.1.9/src/malet/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:56:28.053901 malet-0.1.9/src/malet/plot_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-17 13:56:19.000000 malet-0.1.9/src/malet/plot_utils/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11417 2024-04-17 13:56:19.000000 malet-0.1.9/src/malet/plot_utils/plot_drawer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-17 13:56:19.000000 malet-0.1.9/src/malet/plot_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-17 13:56:19.000000 malet-0.1.9/src/malet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 13:56:28.053901 malet-0.1.9/src/malet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25213 2024-04-17 13:56:28.000000 malet-0.1.9/src/malet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-17 13:56:28.000000 malet-0.1.9/src/malet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 13:56:28.000000 malet-0.1.9/src/malet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-17 13:56:28.000000 malet-0.1.9/src/malet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-17 13:56:28.000000 malet-0.1.9/src/malet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 13:56:28.000000 malet-0.1.9/src/malet.egg-info/top_level.txt
```

### Comparing `malet-0.1.8/LICENSE` & `malet-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `malet-0.1.8/PKG-INFO` & `malet-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malet
-Version: 0.1.8
+Version: 0.1.9
 Summary: Malet: a tool for machine learning experiment
 Author-email: Dongyeop Lee <dylee23@postech.ac.kr>
 License: Copyright (c) 2023 Dongyeop Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -31,20 +31,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: absl-py==1.0.0
-Requires-Dist: numpy==1.22.0
+Requires-Dist: gitpython==3.1.40
 Requires-Dist: pandas==2.0.3
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: ml-collections==0.1.0
-Requires-Dist: seaborn==0.11.2
+Requires-Dist: numpy==1.22.0
 Requires-Dist: rich==13.6.0
+Requires-Dist: seaborn==0.11.2
 
 # Malet: a tool for machine learning experiment
 
 🔨 **Malet** (**Ma**chine **L**earning **E**xperiment **T**ool) is a tool for efficient machine learning experiment execution, logging, analysis, and plot making.
 
 The following features are provided:
 
@@ -66,18 +67,20 @@
 ```bash
 pip install git+https://github.com/edong6768/Malet.git
 ```
 
 ## Dependencies
 
 - absl-py 1.0.0
-- numpy 1.22.0
-- pandas 2.0.3
+- gitpython 3.1.40
 - matplotlib 3.7.0
 - ml-collections 0.1.0
+- numpy 1.22.0
+- pandas 2.0.3
+- rich 13.6.0
 - seaborn 0.11.2
 
 ## Documentation **(🚨 Will be migrated to Sphinx-based Read-the-docs in near future)**
 
 ### Contents
 
 **[Quick start](#quick-start)**
@@ -681,14 +684,17 @@
     ...
     return ckpt_dir
 
 def get_ckpt(ckpt_dir):
     ...
     return ckpt
 
+def save_ckpt(new_ckpt, ckpt_dir):
+    ...
+
 def train(config, experiment, ...):
 
     ... # set up
     
     # retrieve model/trainstate checkpoint if there exists
     # these are just placeholders for the logic
     ckpt_epoch = 0
@@ -701,30 +707,31 @@
     metric_dict = {
         'train_accuracies': [],
         'val_accuracies': [],
         'train_losses': [],
         'val_losses': [],
     }
     if config in experiment.log:
-      metric_dict = experiment.get_log_checkpoint(config, metric_dict)
+      metric_dict = experiment.get_log_checkpoint(config)[0]
     ###################################################################
     ...
     # training happens here
     for epoch in range(config.ckpt_epoch, config.epochs):
       
       ... # train
       
       ... # update metric_dict
 
-      if not epoch % config.ckpt_every:
+      if not (epoch+1) % config.ckpt_every:
 
         ... # train state, model checkpoint
 
         ####################### checkpoint log #######################
-        experiment.update_log(metric_dict, configs=config) 
+        save_ckpt(new_ckpt, ckpt_dir)
+        experiment.update_log(config, **metric_dict) 
         ##############################################################
     ...
 
     return metric_dict
 ```
 
 The `ExperimentLog.get_log_checkpoint` method retrieves the `metric_dict` based on the `status` field in the dataframe.
```

### Comparing `malet-0.1.8/README.md` & `malet-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 ```bash
 pip install git+https://github.com/edong6768/Malet.git
 ```
 
 ## Dependencies
 
 - absl-py 1.0.0
-- numpy 1.22.0
-- pandas 2.0.3
+- gitpython 3.1.40
 - matplotlib 3.7.0
 - ml-collections 0.1.0
+- numpy 1.22.0
+- pandas 2.0.3
+- rich 13.6.0
 - seaborn 0.11.2
 
 ## Documentation **(🚨 Will be migrated to Sphinx-based Read-the-docs in near future)**
 
 ### Contents
 
 **[Quick start](#quick-start)**
@@ -637,14 +639,17 @@
     ...
     return ckpt_dir
 
 def get_ckpt(ckpt_dir):
     ...
     return ckpt
 
+def save_ckpt(new_ckpt, ckpt_dir):
+    ...
+
 def train(config, experiment, ...):
 
     ... # set up
     
     # retrieve model/trainstate checkpoint if there exists
     # these are just placeholders for the logic
     ckpt_epoch = 0
@@ -657,30 +662,31 @@
     metric_dict = {
         'train_accuracies': [],
         'val_accuracies': [],
         'train_losses': [],
         'val_losses': [],
     }
     if config in experiment.log:
-      metric_dict = experiment.get_log_checkpoint(config, metric_dict)
+      metric_dict = experiment.get_log_checkpoint(config)[0]
     ###################################################################
     ...
     # training happens here
     for epoch in range(config.ckpt_epoch, config.epochs):
       
       ... # train
       
       ... # update metric_dict
 
-      if not epoch % config.ckpt_every:
+      if not (epoch+1) % config.ckpt_every:
 
         ... # train state, model checkpoint
 
         ####################### checkpoint log #######################
-        experiment.update_log(metric_dict, configs=config) 
+        save_ckpt(new_ckpt, ckpt_dir)
+        experiment.update_log(config, **metric_dict) 
         ##############################################################
     ...
 
     return metric_dict
 ```
 
 The `ExperimentLog.get_log_checkpoint` method retrieves the `metric_dict` based on the `status` field in the dataframe.
```

### Comparing `malet-0.1.8/pyproject.toml` & `malet-0.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools]
 packages = ["malet", "malet.plot_utils"]
 package-dir = {""="src"}
 
 [project]
 name = "malet"
-version = "0.1.8"
+version = "0.1.9"
 description = "Malet: a tool for machine learning experiment"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["machine learning", "experiment", "plot"]
 authors = [
   {name = "Dongyeop Lee", email = "dylee23@postech.ac.kr"},
@@ -24,20 +24,21 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     'absl-py==1.0.0',
-    'numpy==1.22.0',
+    'gitpython==3.1.40',
     'pandas==2.0.3',
     'matplotlib==3.7.0',
     'ml-collections==0.1.0',
-    'seaborn==0.11.2',
+    'numpy==1.22.0',
     'rich==13.6.0',
+    'seaborn==0.11.2',
 ]
 
 [project.scripts]
 malet-plot = "malet.plot:main"
 
 [project.urls]
 Repository = "https://github.com/edong6768/Malet.git"
```

### Comparing `malet-0.1.8/src/malet/experiment.py` & `malet-0.1.9/src/malet/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import yaml
 import re
 from functools import reduce, partial
 from typing import Optional, ClassVar, Callable, Union, TypeVar
 from dataclasses import dataclass
 from itertools import product, chain
 from datetime import datetime
+from git import Repo
 
 import pandas as pd
 import numpy as np
 from rich.progress import track
 
 from absl import logging
 from ml_collections.config_dict import ConfigDict
@@ -498,14 +499,16 @@
     - (current run checking) Save configs of currently running experiments to tsv so other running code can know.
   - Saves experiment logs, automatically resumes experiment using saved log.
   '''
   __RUNNING: ClassVar[str] = 'R'
   __FAILED: ClassVar[str] = 'F'
   __COMPLETED: ClassVar[str] = 'C'
   
+  infos: ClassVar[list] = ['datetime', 'duration', 'commit_hash', 'status']
+  
   def __init__(self, 
                exp_folder_path: str,
                exp_function: ExpFunc,
                exp_metrics: Optional[list] = None,
                total_splits: Union[int, str] = 1, 
                curr_split: Union[int, str] = 0,
                auto_update_tsv: bool = False,
@@ -526,14 +529,15 @@
     cfg_file, tsv_file, _ = self.get_paths(exp_folder_path)
     self.configs = ConfigIter(cfg_file)
     self.__process_split()
 
     if isinstance(self.exp_bs, int) and self.exp_bs>1 or isinstance(self.exp_bs, str):
       tsv_file = os.path.join(exp_folder_path, 'log_splits', f'split_{self.exp_bi}.tsv') # for saving seperate log for each split in plan slitting mode.
     
+    exp_metrics = self.infos + exp_metrics
     self.log = self.__get_log(tsv_file, exp_metrics, auto_update_tsv)
     
     
   def __process_split(self):
     
     assert self.exp_bs.isdigit() or (self.exp_bs in self.configs.grid_fields), \
         f'Enter valid splits (int | Literal{self.configs.grid_fields}).'
@@ -570,68 +574,85 @@
   @staticmethod
   def get_paths(exp_folder):
     cfg_file = os.path.join(exp_folder, 'exp_config.yaml')
     tsv_file = os.path.join(exp_folder, 'log.tsv')
     fig_dir = os.path.join(exp_folder, 'figure')
     return cfg_file, tsv_file, fig_dir
   
-  def get_log_checkpoint(self, config, empty_metric):
+  def get_log_checkpoint(self, config):
     metric_dict = self.log.get_metric(config)
-    if metric_dict['status'] == self.__FAILED:
-      return metric_dict
-    return empty_metric
-    
-  def update_log(self, metric_dict, config):
-    self.log.add_result(metric_dict, configs=config, 
-                        datetime=str(datetime.now()), status=self.__RUNNING)
+    info_dict = {k:v for k in self.infos if (k in metric_dict and pd.notna(v:=metric_dict.pop(k)))}
+    metric_dict = {k:v for k, v in metric_dict.items() if pd.notna(v)}
+    return metric_dict, info_dict
+    
+  def update_log(self, config, **metric_dict):
+    self.log.add_result(config, **metric_dict, 
+                        datetime=str(datetime.now()), 
+                        status=self.__RUNNING)
     self.log.to_tsv()
     
   def run(self):
     
+    try:
+      commit_hash = Repo.init().head.commit.hexsha
+    except:
+      commit_hash = None
+      logging.info('No git exist in current directory.')
+    
     # current experiment count
     if isinstance(self.exp_bs, int):
       logging.info(f'Experiment : {self.configs.name} (split : {self.exp_bi+1}/{self.exp_bs})')
     elif isinstance(self.exp_bs, str):
       logging.info(f'Experiment : {self.configs.name} (split : {self.exp_bi}/{self.configs.grid_dict[self.exp_bs]})')
     
     # run experiment plans 
     for i, config in enumerate(self.configs):
 
       if config in self.log:
-        metric_dict = self.log.get_metric(config)
-        if metric_dict.get('status') != self.__FAILED:
+        metric_dict, info_dict = self.get_log_checkpoint(config)
+        if info_dict.get('status') != self.__FAILED:
           continue # skip already executed runs
       
       # if config not in self.log or status==self.__FAILED
       if self.configs_save:
-        self.log.add_result(config, status=self.__RUNNING)
+        if config not in self.log: metric_dict = {}
+        self.log.add_result(config, **metric_dict,
+                            status=self.__RUNNING)
         self.log.to_tsv()
 
       logging.info('###################################')
       logging.info(f'   Experiment count : {i+1}/{len(self.configs)}')
       logging.info('###################################') 
 
 
+      start_t = datetime.now()
       try:
         if self.checkpoint:
           metric_dict = self.exp_func(config, self)
         else:
           metric_dict = self.exp_func(config)
+        status = self.__COMPLETED
+        
       except:
-        self.log.add_result(config, status=self.__FAILED)
-        self.log.to_tsv()
+        metric_dict = self.get_log_checkpoint(config)[0] if config in self.log else {}
+        status = self.__FAILED
         raise
       
-      # Open log file and add result
-      self.log.add_result(config, **metric_dict,
-                          datetime=str(datetime.now()), 
-                          status=self.__COMPLETED)
-      self.log.to_tsv()
+      finally:
+        end_t = datetime.now()
+        prev_duration = datetime.timedelta(info_dict['duration'] if (config in self.log and 'duration' in info_dict) else 0)
+        self.log.add_result(config, **metric_dict,
+                            datetime=end_t, 
+                            duration=prev_duration+(end_t-start_t),
+                            commit_hash=commit_hash,
+                            status=status)
+        self.log.to_tsv()
+        
+        logging.info("Saved experiment data to log")
       
-      logging.info("Saved experiment data to log")
       
       
   @staticmethod
   def resplit_logs(exp_folder_path: str, target_split: int=1, save_backup: bool=True):
     """Resplit splitted logs into ``target_split`` number of splits."""
     assert target_split > 0, 'Target split should be larger than 0'
```

### Comparing `malet-0.1.8/src/malet/get_slurm_run_status.py` & `malet-0.1.9/src/malet/get_slurm_run_status.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.8/src/malet/plot.py` & `malet-0.1.9/src/malet/plot.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.8/src/malet/plot_utils/data_processor.py` & `malet-0.1.9/src/malet/plot_utils/data_processor.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.8/src/malet/plot_utils/plot_drawer.py` & `malet-0.1.9/src/malet/plot_utils/plot_drawer.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.8/src/malet/plot_utils/utils.py` & `malet-0.1.9/src/malet/plot_utils/utils.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.8/src/malet/utils.py` & `malet-0.1.9/src/malet/utils.py`

 * *Files identical despite different names*

### Comparing `malet-0.1.8/src/malet.egg-info/PKG-INFO` & `malet-0.1.9/src/malet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malet
-Version: 0.1.8
+Version: 0.1.9
 Summary: Malet: a tool for machine learning experiment
 Author-email: Dongyeop Lee <dylee23@postech.ac.kr>
 License: Copyright (c) 2023 Dongyeop Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -31,20 +31,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: absl-py==1.0.0
-Requires-Dist: numpy==1.22.0
+Requires-Dist: gitpython==3.1.40
 Requires-Dist: pandas==2.0.3
 Requires-Dist: matplotlib==3.7.0
 Requires-Dist: ml-collections==0.1.0
-Requires-Dist: seaborn==0.11.2
+Requires-Dist: numpy==1.22.0
 Requires-Dist: rich==13.6.0
+Requires-Dist: seaborn==0.11.2
 
 # Malet: a tool for machine learning experiment
 
 🔨 **Malet** (**Ma**chine **L**earning **E**xperiment **T**ool) is a tool for efficient machine learning experiment execution, logging, analysis, and plot making.
 
 The following features are provided:
 
@@ -66,18 +67,20 @@
 ```bash
 pip install git+https://github.com/edong6768/Malet.git
 ```
 
 ## Dependencies
 
 - absl-py 1.0.0
-- numpy 1.22.0
-- pandas 2.0.3
+- gitpython 3.1.40
 - matplotlib 3.7.0
 - ml-collections 0.1.0
+- numpy 1.22.0
+- pandas 2.0.3
+- rich 13.6.0
 - seaborn 0.11.2
 
 ## Documentation **(🚨 Will be migrated to Sphinx-based Read-the-docs in near future)**
 
 ### Contents
 
 **[Quick start](#quick-start)**
@@ -681,14 +684,17 @@
     ...
     return ckpt_dir
 
 def get_ckpt(ckpt_dir):
     ...
     return ckpt
 
+def save_ckpt(new_ckpt, ckpt_dir):
+    ...
+
 def train(config, experiment, ...):
 
     ... # set up
     
     # retrieve model/trainstate checkpoint if there exists
     # these are just placeholders for the logic
     ckpt_epoch = 0
@@ -701,30 +707,31 @@
     metric_dict = {
         'train_accuracies': [],
         'val_accuracies': [],
         'train_losses': [],
         'val_losses': [],
     }
     if config in experiment.log:
-      metric_dict = experiment.get_log_checkpoint(config, metric_dict)
+      metric_dict = experiment.get_log_checkpoint(config)[0]
     ###################################################################
     ...
     # training happens here
     for epoch in range(config.ckpt_epoch, config.epochs):
       
       ... # train
       
       ... # update metric_dict
 
-      if not epoch % config.ckpt_every:
+      if not (epoch+1) % config.ckpt_every:
 
         ... # train state, model checkpoint
 
         ####################### checkpoint log #######################
-        experiment.update_log(metric_dict, configs=config) 
+        save_ckpt(new_ckpt, ckpt_dir)
+        experiment.update_log(config, **metric_dict) 
         ##############################################################
     ...
 
     return metric_dict
 ```
 
 The `ExperimentLog.get_log_checkpoint` method retrieves the `metric_dict` based on the `status` field in the dataframe.
```

