# Comparing `tmp/falcon_challenge-0.3.4.tar.gz` & `tmp/falcon_challenge-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon_challenge-0.3.4.tar", last modified: Tue May  7 02:38:06 2024, max compression
+gzip compressed data, was "falcon_challenge-0.3.5.tar", last modified: Sun May 12 15:59:09 2024, max compression
```

## Comparing `falcon_challenge-0.3.4.tar` & `falcon_challenge-0.3.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:06.886031 falcon_challenge-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-07 02:38:06.886031 falcon_challenge-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:06.882031 falcon_challenge-0.3.4/decoder_demos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/decoding_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/ndt2_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/random_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/rnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13694 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/sklearn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/decoder_demos/sklearn_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:06.886031 falcon_challenge-0.3.4/falcon_challenge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/challenge_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    26588 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/falcon_challenge/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:06.886031 falcon_challenge-0.3.4/falcon_challenge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-07 02:38:06.000000 falcon_challenge-0.3.4/falcon_challenge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-07 02:38:06.000000 falcon_challenge-0.3.4/falcon_challenge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:38:06.000000 falcon_challenge-0.3.4/falcon_challenge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-07 02:38:06.000000 falcon_challenge-0.3.4/falcon_challenge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 02:38:06.000000 falcon_challenge-0.3.4/falcon_challenge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:06.886031 falcon_challenge-0.3.4/preproc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/assemble_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/h2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/m1_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/m1_reachgrasp_preprocv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/m2_fewshot_trial_counts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/m2_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/merge_answers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/nwb_create_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/wrapper_convert_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/preproc/zip_data.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:38:06.890031 falcon_challenge-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 02:38:02.000000 falcon_challenge-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:09.299744 falcon_challenge-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-12 15:59:09.299744 falcon_challenge-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:09.295744 falcon_challenge-0.3.5/decoder_demos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/decoding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/ndt2_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/random_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/rnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13812 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/sklearn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/decoder_demos/sklearn_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:09.295744 falcon_challenge-0.3.5/falcon_challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/challenge_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28393 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/falcon_challenge/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:09.299744 falcon_challenge-0.3.5/falcon_challenge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-12 15:59:09.000000 falcon_challenge-0.3.5/falcon_challenge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-12 15:59:09.000000 falcon_challenge-0.3.5/falcon_challenge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:59:09.000000 falcon_challenge-0.3.5/falcon_challenge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-12 15:59:09.000000 falcon_challenge-0.3.5/falcon_challenge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-12 15:59:09.000000 falcon_challenge-0.3.5/falcon_challenge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:09.299744 falcon_challenge-0.3.5/preproc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/assemble_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/h2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/m1_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24166 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/m1_reachgrasp_preprocv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/m2_fewshot_trial_counts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16660 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/m2_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/merge_answers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/nwb_create_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/wrapper_convert_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/preproc/zip_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:59:09.299744 falcon_challenge-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-12 15:59:05.000000 falcon_challenge-0.3.5/setup.py
```

### Comparing `falcon_challenge-0.3.4/LICENSE` & `falcon_challenge-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/PKG-INFO` & `falcon_challenge-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.4
+Version: 0.3.5
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.4/README.md` & `falcon_challenge-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/decoder_demos/decoding_utils.py` & `falcon_challenge-0.3.5/decoder_demos/decoding_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/decoder_demos/filtering.py` & `falcon_challenge-0.3.5/decoder_demos/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/decoder_demos/ndt2_sample.py` & `falcon_challenge-0.3.5/decoder_demos/ndt2_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/decoder_demos/random_decoder.py` & `falcon_challenge-0.3.5/decoder_demos/random_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/decoder_demos/rnn_decoder.py` & `falcon_challenge-0.3.5/decoder_demos/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/decoder_demos/sklearn_decoder.py` & `falcon_challenge-0.3.5/decoder_demos/sklearn_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,18 @@
                     raise ValueError(f"Dataset tag {dataset_tag} not found decoder set {self.clf.keys()}")
             self.local_clf = [self.clf[dataset_tag] for dataset_tag in dataset_tags]
         else:
             self.local_clf = self.clf
         self.raw_history_buffer = np.zeros_like(self.raw_history_buffer)
         self.observation_buffer = np.zeros_like(self.observation_buffer)
 
+    def on_done(self, dones: np.ndarray):
+        # unnecessary for this decoder
+        pass
+    
     def predict(self, neural_observations: np.ndarray):
         r"""
             neural_observations: array of shape (batch, n_channels), binned spike counts
             
             return: array of shape (batch, n_features), predicted kinematics
         """
         self.observe(neural_observations)
@@ -259,15 +263,16 @@
     else:
         day_unique = set([f.stem.split('_')[1] for f in all_datafiles])
     all_decoders = {}
     x_means = {}
     x_stds = {}
     for day in sorted(day_unique): # separate decoder
         print(f"Training on day {day}")
-        fit_datafiles = [d for d in all_datafiles if day in task_config.hash_dataset(d)]
+        fit_datafiles = [d for d in all_datafiles if day == task_config.hash_dataset(d).split('_set_')[0]]
+
         (
             neural_data,
             covariates,
             trial_change,
             eval_mask
         ) = zip(*[load_nwb(fn, task_config.task) for fn in fit_datafiles])
         neural_data = np.concatenate(neural_data)
```

### Comparing `falcon_challenge-0.3.4/decoder_demos/sklearn_sample.py` & `falcon_challenge-0.3.5/decoder_demos/sklearn_sample.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/falcon_challenge/config.py` & `falcon_challenge-0.3.5/falcon_challenge/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,18 +113,18 @@
             # sub-MonkeyL-held-in-minival_ses-20120924_behavior+ecephys.nwb
             # or L_20120924_held_in_eval.nwb
             if 'behavior+ecephys' in handle:
                 return handle.split('_')[-2].split('-')[-1]
             return handle.split('_')[1]
         elif self.task == FalconTask.m2:
             if 'behavior+ecephys' in handle: # public sub-MonkeyN-held-in-calib_ses-2020-10-19-Run1_behavior+ecephys.nwb
-                return handle.split('_')[-2][4:] # -> 2020-10-19-Run1
+                run_str = handle.split('_')[1][-4:]
+                date_str = ''.join(handle.split('_')[1].split('-')[1:4])
             # sub-MonkeyNRun1_20201019_held_in_eval.nwb 
-            run_str = handle.split('_')[0][-4:]
-            date_str = handle.split('_')[1]
-            date = datetime.datetime.strptime(date_str, '%Y%m%d')
-            date_str_fmt = date.strftime('%Y-%m-%d')
-            return f'{date_str_fmt}-{run_str}'
+            else:
+                run_str = handle.split('_')[0][-4:]
+                date_str = handle.split('_')[1][:8]
+            return f'{run_str}_{date_str}'
             
 
 cs = ConfigStore.instance()
 cs.store(name="falcon_config", node=FalconConfig)
```

### Comparing `falcon_challenge-0.3.4/falcon_challenge/dataloaders.py` & `falcon_challenge-0.3.5/falcon_challenge/dataloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,20 @@
     if not dataset in [FalconTask.h1, FalconTask.h2, FalconTask.m1, FalconTask.m2]:
         raise ValueError(f"Unknown dataset {dataset}")
     with NWBHDF5IO(str(fn), 'r') as io:
         nwbfile = io.read()
         if dataset == FalconTask.h1:
             units = nwbfile.units.to_dataframe()
             kin = nwbfile.acquisition['OpenLoopKinematicsVelocity'].data[:]
-            timestamps = nwbfile.acquisition['OpenLoopKinematics'].offset + np.arange(kin.shape[0]) * nwbfile.acquisition['OpenLoopKinematics'].rate
-            eval_mask = nwbfile.acquisition['eval_mask'].data[:].astype(bool)
+            try:
+                eval_mask = nwbfile.acquisition['eval_mask'].data[:].astype(bool)
+                timestamps = nwbfile.acquisition['OpenLoopKinematics'].offset + np.arange(kin.shape[0]) * nwbfile.acquisition['OpenLoopKinematics'].rate
+            except: #for older format oracle data
+                eval_mask = ~nwbfile.acquisition['Blacklist'].data[:].astype(bool)
+                timestamps = nwbfile.acquisition['OpenLoopKinematics'].offset + np.arange(kin.shape[0]) * .02
             binned_units = bin_units(units, bin_size_s=0.02, bin_timestamps=timestamps)
             return binned_units, kin, np.zeros(kin.shape[0]), eval_mask
         elif dataset == FalconTask.h2: 
             binned_spikes = nwbfile.acquisition['binned_spikes'].data[()]
             time = nwbfile.acquisition['binned_spikes'].timestamps[()]
             eval_mask = nwbfile.acquisition['eval_mask'].data[()].astype(bool)
             trial_info = (
```

### Comparing `falcon_challenge-0.3.4/falcon_challenge/evaluator.py` & `falcon_challenge-0.3.5/falcon_challenge/evaluator.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 from pathlib import Path
 from tqdm import tqdm
 from sklearn.metrics import r2_score
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import Dataset, DataLoader
 from edit_distance import SequenceMatcher
+from time import time, sleep
 
 from falcon_challenge.config import FalconTask, FalconConfig
 from falcon_challenge.interface import BCIDecoder
 from falcon_challenge.dataloaders import load_nwb
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
@@ -89,20 +90,28 @@
             '2023.05.31', 
             '2023.06.28', 
             '2023.08.16', 
             '2023.10.09'
         ]
     },
     'm2': {
-        'held_in': ['2020-10-19-Run1', '2020-10-19-Run2', '2020-10-20-Run1', '2020-10-20-Run2', '2020-10-27-Run1', '2020-10-27-Run2', '2020-10-28-Run1'],
-        'held_out': ['2020-10-30-Run1', '2020-10-30-Run2', '2020-11-18-Run1', '2020-11-19-Run1', '2020-11-24-Run1', '2020-11-24-Run2'],
+        'held_in': ['Run1_20201019', 'Run2_20201019', 'Run1_20201020', 'Run2_20201020', 'Run1_20201027', 'Run2_20201027', 'Run1_20201028'],
+        'held_out': ['Run1_20201030', 'Run2_20201030', 'Run1_20201118', 'Run1_20201119', 'Run1_20201124', 'Run2_20201124'],
     },
 }
 
 # Used to label test server data file names to look for
+# These act as a _reduction_ set of the full list of datafiles considered, to specific sessions. Relevant for H1/M2.
+def reduce_key(key):
+    if key.startswith('Run'):
+        return key.split('_')[1]
+    if key.startswith('L_'):
+        return key
+    return key
+
 HELD_IN_KEYS = {
     FalconTask.h1: ['S0_', 'S1_', 'S2_', 'S3_', 'S4_', 'S5_'],
     FalconTask.m1: ['L_20120924', 'L_20120926', 'L_20120927', 'L_20120928'],
     FalconTask.m2: ['20201019', '20201020', '20201027', '20201028'],
     FalconTask.h2: DATASET_HELDINOUT_MAP['h2']['held_in'],
 }
 
@@ -121,14 +130,16 @@
 }
 
 # Development time flag. False allows direct evaluation without payload writing, only usable for local minival.
 # Should be set to true for remote evaluation.
 # USE_PKLS = False
 USE_PKLS = True
 
+BIN_SIZE = 0.02
+
 HELDIN_OR_OUT_MAP = {
     'held_in': "Held In",
     'held_out': "Held Out",
 }
 
 def evaluate(
     test_annotation_file: str, # The annotation file for the phase
@@ -181,41 +192,49 @@
         split_annotations = test_annotations[datasplit]
         split_result = {}
         split_result["Normalized Latency"] = user_submission[datasplit]["normalized_latency"]
         del user_submission[datasplit]["normalized_latency"]
         pred_dict = defaultdict(list)
         tgt_dict = defaultdict(list)
         mask_dict = defaultdict(list)
+        if 'h2' not in datasplit:
+            dset_len_dict = defaultdict(lambda: defaultdict(list))
         for dataset in user_submission[datasplit]:
             dataset_pred = user_submission[datasplit][dataset]
             dataset_tgt = split_annotations[dataset]['data']
             dataset_mask = split_annotations[dataset]['mask']
             dataset_pred = dataset_pred[:dataset_mask.shape[0]] # In case excess timesteps are predicted due to batching, reduce
             if dataset in DATASET_HELDINOUT_MAP[datasplit]['held_in']:
+                if 'h2' not in datasplit:
+                    session_id = reduce_key(dataset)
+                    dset_len_dict['held_in'][session_id].append(dataset_mask.shape[0])
                 pred_dict['held_in'].append(dataset_pred)
                 tgt_dict['held_in'].append(dataset_tgt)
                 mask_dict['held_in'].append(dataset_mask)
             elif dataset in DATASET_HELDINOUT_MAP[datasplit]['held_out']:
+                if not 'h2' in datasplit:
+                    session_id = reduce_key(dataset)
+                    dset_len_dict['held_out'][session_id].append(dataset_mask.shape[0])
                 pred_dict['held_out'].append(dataset_pred)
                 tgt_dict['held_out'].append(dataset_tgt)
                 mask_dict['held_out'].append(dataset_mask)
             else:
                 raise ValueError(f"Dataset {dataset} submitted but not found in held-in or held-out list of split {datasplit}.")
         for in_or_out in pred_dict:
             if len(pred_dict[in_or_out]) < len(DATASET_HELDINOUT_MAP[datasplit][in_or_out]):
                 raise ValueError(f"Missing predictions for {datasplit} {in_or_out}. User submitted: {user_submission[datasplit].keys()}. Expecting more like: {HELDIN_OR_OUT_MAP[datasplit][in_or_out]}.")
             pred = np.concatenate(pred_dict[in_or_out])
             if 'h2' in datasplit:
                 tgt = [y for x in tgt_dict[in_or_out] for y in x]
             else:
                 tgt = np.concatenate(tgt_dict[in_or_out])
+                dset_lens = dset_len_dict[in_or_out]
             mask = np.concatenate(mask_dict[in_or_out])
-            eval_fn = FalconEvaluator.compute_metrics_edit_distance if 'h2' in datasplit else FalconEvaluator.compute_metrics_regression
             try:
-                metrics = eval_fn(pred, tgt, mask)
+                metrics = FalconEvaluator.compute_metrics_edit_distance(pred, tgt, mask) if 'h2' in datasplit else FalconEvaluator.compute_metrics_regression(pred, tgt, mask, dset_lens)
             except Exception as e:
                 raise ValueError(f"Failed to compute metrics for {datasplit} {in_or_out}: {e}. Lengths submitted: {[len(piece) for piece in pred_dict[in_or_out]]}")
             for k in metrics:
                 split_result[f'{HELDIN_OR_OUT_MAP[in_or_out]} {k}'] = metrics[k]
         result.append({f'{phase_codename}_split_{datasplit}': split_result})
 
     print(f"Returning result from phase: {phase_codename}: {result}")
@@ -310,42 +329,45 @@
         handles = self.get_eval_handles(self.eval_remote, self.dataset, phase=phase)
         logger.info(f"Found {len(handles)} files.")
         if len(handles) == 0:
             raise FileNotFoundError(f"No files found in {self.dataset.name} for phase {phase}. Note test phase data is only available on EvalAI remote.")
         return handles
     
     def predict_files(self, decoder: BCIDecoder, eval_files: List):
-        # returns triple dict, keyed by datafile hash and contains preds, targets, and eval_mask respective
+        # returns triple dict, keyed by datafile hash and contains preds, targets, and eval_mask respective. also returns lists compute_time and neural_time
         # TODO this does not return uniquely identifiable data if eval_files is partial, e.g. if we only has set 2 of a day with 2 sets, we'll happily just provide partial predictions.
         # Pre-loop before starting batch loads
         file_neural_data = []
         file_trial_change = []
         file_targets = []
         file_eval_mask = []
+        all_neural_times = []
         datafiles = list(sorted(eval_files))
         for datafile in datafiles:
             if not datafile.exists():
                 raise FileNotFoundError(f"File {datafile} not found.")
             neural_data, decoding_targets, trial_change, eval_mask = load_nwb(datafile, dataset=self.dataset)
             file_neural_data.append(neural_data)
             file_trial_change.append(trial_change)
             file_targets.append(decoding_targets)
             file_eval_mask.append(eval_mask)
+            all_neural_times.append(neural_data.shape[0] * BIN_SIZE)
     
         dataset = EvalDataset(
             data=file_neural_data,
             trial_change=file_trial_change,
             targets=file_targets,
             eval_mask=file_eval_mask,
             datafiles=datafiles,
         )
         
         all_preds = defaultdict(list)
         all_targets = defaultdict(list)
         all_eval_mask = defaultdict(list)
+        all_compute_times = []
         
         num_workers = 8
         simple_collater_partial = partial(simple_collater, task=self.dataset)
         dataloader = DataLoader(
             dataset, shuffle=False,
             batch_size=decoder.batch_size,
             num_workers=num_workers,
@@ -367,21 +389,27 @@
             for neural_observations, trial_delta_obs, step_mask in zip(neural_data, trial_change, eval_mask):
                 neural_observations: np.ndarray
                 trial_delta_obs: np.ndarray
                 step_mask: np.ndarray
                 if self.dataset == FalconTask.h2:
                     assert neural_data.shape[1] == 1, "H2 expects batch size 1."
                     if step_mask[0]:
+                        start_time = time()
                         decoder.predict(neural_observations)
+                        end_time = time()
+                        all_compute_times.append(end_time - start_time)
                     if trial_delta_obs[0]:
                         trial_preds.append(decoder.on_done(trial_delta_obs))
                 else:
                     if not self.continual:
                         decoder.on_done(trial_delta_obs)
+                    start_time = time()
                     step_prediction = decoder.predict(neural_observations)
+                    end_time = time()
+                    all_compute_times.append(end_time - start_time)
                     assert step_prediction.shape[1] == self.cfg.out_dim, f"Prediction shape mismatch: {step_prediction.shape[1]} vs {self.cfg.out_dim}."
                     trial_preds.append(step_prediction)
                     
                     # if step_mask.any():
                     #     trial_preds.append(decoder.predict(neural_observations))
                     # else:
                     #     decoder.observe(neural_observations)
@@ -406,15 +434,15 @@
             if self.dataset == FalconTask.h2:
                 all_preds[k] = [x for y in all_preds[k] for x in y]
                 all_targets[k] = [x for y in all_targets[k] for x in y]
             else:
                 all_preds[k] = np.concatenate(all_preds[k])
                 all_targets[k] = np.concatenate(all_targets[k])
             all_eval_mask[k] = np.concatenate(all_eval_mask[k])
-        return all_preds, all_targets, all_eval_mask
+        return all_preds, all_targets, all_eval_mask, all_compute_times, all_neural_times
 
     def evaluate_files(self, decoder: BCIDecoder, eval_files: List):
         all_preds, all_targets, all_eval_mask = self.predict_files(decoder, eval_files)
         metrics = self.compute_metrics(all_preds, all_targets, all_eval_mask)
         return metrics
 
     def evaluate(
@@ -457,71 +485,75 @@
             eval_files_held_out = [f for f in eval_files if any(k in f.name for k in HELD_OUT_KEYS[self.dataset])]
             assert len(eval_files) == len(eval_files_held_in) + len(eval_files_held_out), f"Mismatch in extracted eval #: Eval file state is not consistent with benchmark creation settings. Found {len(eval_files)} files, {len(eval_files_held_in)} held in, {len(eval_files_held_out)} held out."
 
             if specific_keys:
                 raise NotImplementedError("not sure what metrics to compute for specific keys yet.")
             elif held_out_only:
                 eval_files_held_in = []
-            all_preds, all_targets, all_eval_mask = self.predict_files(decoder, eval_files_held_out)
+            all_preds, all_targets, all_eval_mask, all_compute_times, all_neural_times = self.predict_files(decoder, eval_files_held_out)
             if eval_files_held_in:
-                all_preds_held_in, all_targets_held_in, all_eval_mask_held_in = self.predict_files(decoder, eval_files_held_in)
+                all_preds_held_in, all_targets_held_in, all_eval_mask_held_in, _, _ = self.predict_files(decoder, eval_files_held_in)
                 all_preds.update(all_preds_held_in)
                 all_targets.update(all_targets_held_in)
                 all_eval_mask.update(all_eval_mask_held_in)
 
         else:
-            all_preds, all_targets, all_eval_mask = self.predict_files(decoder, eval_files)
+            all_preds, all_targets, all_eval_mask, all_compute_times, all_neural_times = self.predict_files(decoder, eval_files)
         # Indirect remote setup to satisfy EvalAI interface. Save metrics / comparison to file.
         if USE_PKLS:
             inner_pred = {**all_preds}
             inner_tgt_spoof = { # spoof for local mirror of eval ai path, in reality targets are already compiled on eval ai side.
                 k: {
                     'data': all_targets[k][all_eval_mask[k]] if self.dataset != FalconTask.h2 else all_targets[k],
                     'mask': all_eval_mask[k],
                 } for k in all_targets
             }
-            inner_pred['normalized_latency'] = 1 # TODO - CW insert timing code
+            inner_pred['normalized_latency'] = np.sum(all_compute_times) / np.sum(all_neural_times)
             pred_payload = {self.dataset.name: inner_pred}
             truth_payload = {self.dataset.name: inner_tgt_spoof}
         else:
             pass
             
         if USE_PKLS:
             Path(prediction_path).parent.mkdir(parents=True, exist_ok=True)
             with open(prediction_path, 'wb') as f:
                 pickle.dump(pred_payload, f)
             Path(gt_path).parent.mkdir(parents=True, exist_ok=True)
             with open(gt_path, 'wb') as f:
                 pickle.dump(truth_payload, f)
-            import time
 
             if self.eval_remote:
                 print("Sleeping before exiting for remote eval - feel free to interrupt for local eval.", flush=True)
                 # Gunjan, EvalAI contact says that current static code eval has an issue where the submission dump is only polled by the EvalAI worker comparison script every 5 minutes
                 # Sleep so it's definitely available
-                time.sleep(300) 
+                sleep(300) 
             else:
                 return evaluate(
                     test_annotation_file=gt_path,
                     user_submission_file=prediction_path,
                     phase_codename=phase
                 )
         else:
             for k, v in metrics.items():
                 logger.info("{}: {}".format(k, v))
         
     @staticmethod
-    def compute_metrics_regression(preds, targets, eval_mask):
+    def compute_metrics_regression(preds, targets, eval_mask, dset_lens):
+        dset_lens = np.cumsum([sum(dset_lens[key]) for key in sorted(dset_lens.keys())])
+        masked_points = np.cumsum(~eval_mask)
+        dset_lens = [0] + [dset_len - masked_points[dset_len - 1] for dset_len in dset_lens]
         # assumes targets are already masked
         preds = preds[eval_mask]
         if not targets.shape[0] == preds.shape[0]:
             raise ValueError(f"Targets and predictions have different lengths: {targets.shape[0]} vs {preds.shape[0]}.")
+        r2_scores = [r2_score(targets[dset_lens[i]:dset_lens[i+1]], preds[dset_lens[i]:dset_lens[i+1]], 
+                              multioutput='variance_weighted') for i in range(len(dset_lens) - 1)]
         return {
-            "R2": r2_score(targets, preds, multioutput='variance_weighted'),
-            "R2 Std.": 0, # TODO Clay
+            "R2 Mean": np.mean(r2_scores),
+            "R2 Std.": np.std(r2_scores)
         }
 
     @staticmethod
     def compute_metrics_edit_distance(preds, targets, eval_mask):
         if len(preds) != len(targets):
             raise ValueError(f"Targets and predictions have different lengths: {len(targets)} vs {len(preds)}.")
```

### Comparing `falcon_challenge-0.3.4/falcon_challenge/interface.py` & `falcon_challenge-0.3.5/falcon_challenge/interface.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/falcon_challenge.egg-info/PKG-INFO` & `falcon_challenge-0.3.5/falcon_challenge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falcon_challenge
-Version: 0.3.4
+Version: 0.3.5
 Home-page: https://github.com/snel-repo/stability-benchmark
 Author: Joel Ye
 Author-email: joelye9@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: hydra-core
```

### Comparing `falcon_challenge-0.3.4/falcon_challenge.egg-info/SOURCES.txt` & `falcon_challenge-0.3.5/falcon_challenge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/preproc/assemble_data.py` & `falcon_challenge-0.3.5/preproc/assemble_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/preproc/filtering.py` & `falcon_challenge-0.3.5/preproc/filtering.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/preproc/h2_preproc.py` & `falcon_challenge-0.3.5/preproc/h2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/preproc/m1_fewshot_trial_counts.py` & `falcon_challenge-0.3.5/preproc/m1_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/preproc/m1_reachgrasp_preprocv2.py` & `falcon_challenge-0.3.5/preproc/m1_reachgrasp_preprocv2.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/preproc/m2_fewshot_trial_counts.py` & `falcon_challenge-0.3.5/preproc/m2_fewshot_trial_counts.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/preproc/m2_preproc.py` & `falcon_challenge-0.3.5/preproc/m2_preproc.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/preproc/nwb_create_utils.py` & `falcon_challenge-0.3.5/preproc/nwb_create_utils.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/preproc/wrapper_convert_batch.py` & `falcon_challenge-0.3.5/preproc/wrapper_convert_batch.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/preproc/zip_data.py` & `falcon_challenge-0.3.5/preproc/zip_data.py`

 * *Files identical despite different names*

### Comparing `falcon_challenge-0.3.4/setup.py` & `falcon_challenge-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='falcon_challenge',
-    version='0.3.4',
+    version='0.3.5',
 
     url='https://github.com/snel-repo/stability-benchmark',
     author='Joel Ye',
     author_email='joelye9@gmail.com',
 
     packages=find_packages(exclude=['data_demos', 'data']),
     install_requires=[
```

