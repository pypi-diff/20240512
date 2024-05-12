# Comparing `tmp/pklue-0.3.2.tar.gz` & `tmp/pklue-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pklue-0.3.2.tar", last modified: Sun Mar 31 11:37:24 2024, max compression
+gzip compressed data, was "pklue-1.0.0.tar", last modified: Sun May 12 07:22:30 2024, max compression
```

## Comparing `pklue-0.3.2.tar` & `pklue-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 11:37:24.260154 pklue-0.3.2/
--rw-rw-rw-   0        0        0      162 2024-03-31 11:37:24.259161 pklue-0.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-31 11:37:24.234215 pklue-0.3.2/pklue/
--rw-rw-rw-   0        0        0       54 2024-03-31 11:36:16.000000 pklue-0.3.2/pklue/__init__.py
--rw-rw-rw-   0        0        0     2128 2024-03-02 15:31:04.000000 pklue-0.3.2/pklue/korean_utils.py
--rw-rw-rw-   0        0        0     2110 2024-03-26 10:57:04.000000 pklue-0.3.2/pklue/pklue.py
--rw-rw-rw-   0        0        0     9140 2024-03-28 11:48:52.000000 pklue-0.3.2/pklue/processors.py
--rw-rw-rw-   0        0        0    29151 2024-03-02 15:31:04.000000 pklue-0.3.2/pklue/templates.py
--rw-rw-rw-   0        0        0     1666 2024-03-02 15:31:04.000000 pklue-0.3.2/pklue/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-31 11:37:24.255628 pklue-0.3.2/pklue.egg-info/
--rw-rw-rw-   0        0        0      162 2024-03-31 11:37:23.000000 pklue-0.3.2/pklue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-03-31 11:37:24.000000 pklue-0.3.2/pklue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 11:37:23.000000 pklue-0.3.2/pklue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-31 11:37:23.000000 pklue-0.3.2/pklue.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-31 11:37:23.000000 pklue-0.3.2/pklue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 11:37:24.260154 pklue-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      301 2024-03-31 11:36:20.000000 pklue-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:22:30.860888 pklue-1.0.0/
+-rw-rw-rw-   0        0        0      162 2024-05-12 07:22:30.859914 pklue-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-12 07:22:30.833030 pklue-1.0.0/pklue/
+-rw-rw-rw-   0        0        0       54 2024-05-12 07:20:07.000000 pklue-1.0.0/pklue/__init__.py
+-rw-rw-rw-   0        0        0     2128 2024-03-02 15:31:04.000000 pklue-1.0.0/pklue/korean_utils.py
+-rw-rw-rw-   0        0        0     1899 2024-05-12 07:00:10.000000 pklue-1.0.0/pklue/pklue.py
+-rw-rw-rw-   0        0        0     2399 2024-05-12 07:00:10.000000 pklue-1.0.0/pklue/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 07:22:30.858918 pklue-1.0.0/pklue.egg-info/
+-rw-rw-rw-   0        0        0      162 2024-05-12 07:22:30.000000 pklue-1.0.0/pklue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-05-12 07:22:30.000000 pklue-1.0.0/pklue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 07:22:30.000000 pklue-1.0.0/pklue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 07:22:30.000000 pklue-1.0.0/pklue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-12 07:22:30.000000 pklue-1.0.0/pklue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 07:22:30.861880 pklue-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      301 2024-05-12 07:20:07.000000 pklue-1.0.0/setup.py
```

### Comparing `pklue-0.3.2/pklue/korean_utils.py` & `pklue-1.0.0/pklue/korean_utils.py`

 * *Files identical despite different names*

### Comparing `pklue-0.3.2/pklue/pklue.py` & `pklue-1.0.0/pklue/pklue.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,45 +9,43 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import List
+from pathlib import Path
+import importlib
 
 import datasets
 from datasets import concatenate_datasets
 
-from . import processors
-
-AVAILABLE_DATASETS = ['kullm_v2', 'kobest', 'klue', 'ko_arc', 'ko_commongenv2', 'ko_mmlu', 'ko_truthfulqa', 'korquad_v1',
-                      'kullm3_alpaca_gpt4', 'kullm3_xp3x_filtered_gpt4', 'kullm3_dolly_gpt4', 'kullm3_aya',
-                      'kullm3_personal_info', 'kullm3_square_gpt4_sampled',
-                      'koalpaca_v1_1', 'alpaca_gpt4']
-
 
 def get_mixture(
         dataset_names: List[str],
         max_examples: int = None,
         split: str = 'train',
-        verbose: bool = False) -> datasets.Dataset:
+) -> datasets.Dataset:
     """Make mixed huggingface dataset with selected datasets.
 
     Args:
         dataset_names: list of dataset names. names are case-insensitive.
         max_examples: the number of maximum length of examples when do truncation.
         split: 'train' or 'test'
-        verbose: if set True, it prints debugging message.
     Returns:
         Huggingface dataset which contains mixture of 'dataset_names'.
-        Returned dataset's columns are like {"instruction", "input", "output"}
+        Returned dataset's columns are like
+        {"chat": [['user', '...'], ['assistant', '...'], ...]}
     """
-    assert all(n.lower() in AVAILABLE_DATASETS for n in dataset_names), "Invalid dataset name"
+    available_dataset = [e.name for e in (Path(__file__).parent / "available_dataset/").glob("*/")]
+    assert all(n in available_dataset for n in dataset_names), f"Invalid dataset name. available: {available_dataset}"
 
-    processed_datasets = [getattr(processors, f"_{d}_processor")(max_examples, split) for d in dataset_names]
+    processed_datasets = []
+    for dataset_name in dataset_names:
+        module = importlib.import_module(f".available_dataset.{dataset_name}.processor", package='pklue')
+        processed_datasets.append(module.process(max_examples, split))
 
-    # return concatenate_datasets(processed_datasets).shuffle()
     return concatenate_datasets(processed_datasets)
 
 
 if __name__ == '__main__':
     raise NotImplementedError
```

