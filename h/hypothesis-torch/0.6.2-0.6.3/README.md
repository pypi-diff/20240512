# Comparing `tmp/hypothesis_torch-0.6.2.tar.gz` & `tmp/hypothesis_torch-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypothesis_torch-0.6.2.tar", last modified: Fri May 10 14:47:10 2024, max compression
+gzip compressed data, was "hypothesis_torch-0.6.3.tar", last modified: Sun May 12 02:19:21 2024, max compression
```

## Comparing `hypothesis_torch-0.6.2.tar` & `hypothesis_torch-0.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 14:47:10.177393 hypothesis_torch-0.6.2/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8491 2024-05-10 14:47:10.177393 hypothesis_torch-0.6.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5282 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 14:47:10.177393 hypothesis_torch-0.6.2/hypothesis_torch/
--rw-r--r--   0 root         (0) root         (0)     2168 2024-05-10 14:47:06.000000 hypothesis_torch-0.6.2/hypothesis_torch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1408 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/device.py
--rw-r--r--   0 root         (0) root         (0)     2757 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/dtype.py
--rw-r--r--   0 root         (0) root         (0)    11506 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/huggingface.py
--rw-r--r--   0 root         (0) root         (0)     2841 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/inspection_util.py
--rw-r--r--   0 root         (0) root         (0)      735 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/layout.py
--rw-r--r--   0 root         (0) root         (0)      846 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/memory_format.py
--rw-r--r--   0 root         (0) root         (0)    11178 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/module.py
--rw-r--r--   0 root         (0) root         (0)     4586 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/optim.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/py.typed
--rw-r--r--   0 root         (0) root         (0)      866 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/register_random_torch_state.py
--rw-r--r--   0 root         (0) root         (0)     9464 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/tensor.py
--rw-r--r--   0 root         (0) root         (0)     1442 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/hypothesis_torch/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 14:47:10.177393 hypothesis_torch-0.6.2/hypothesis_torch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8491 2024-05-10 14:47:10.000000 hypothesis_torch-0.6.2/hypothesis_torch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      665 2024-05-10 14:47:10.000000 hypothesis_torch-0.6.2/hypothesis_torch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 14:47:10.000000 hypothesis_torch-0.6.2/hypothesis_torch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2024-05-10 14:47:10.000000 hypothesis_torch-0.6.2/hypothesis_torch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-10 14:47:10.000000 hypothesis_torch-0.6.2/hypothesis_torch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-05-10 14:47:10.000000 hypothesis_torch-0.6.2/hypothesis_torch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2690 2024-05-10 14:46:12.000000 hypothesis_torch-0.6.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 14:47:10.181393 hypothesis_torch-0.6.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:19:21.289204 hypothesis_torch-0.6.3/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9045 2024-05-12 02:19:21.289204 hypothesis_torch-0.6.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5465 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:19:21.285204 hypothesis_torch-0.6.3/hypothesis_torch/
+-rw-r--r--   0 root         (0) root         (0)     2168 2024-05-12 02:19:17.000000 hypothesis_torch-0.6.3/hypothesis_torch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/device.py
+-rw-r--r--   0 root         (0) root         (0)     2757 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/dtype.py
+-rw-r--r--   0 root         (0) root         (0)    11506 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/huggingface.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/inspection_util.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/layout.py
+-rw-r--r--   0 root         (0) root         (0)      846 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/memory_format.py
+-rw-r--r--   0 root         (0) root         (0)    11178 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/module.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/optim.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/py.typed
+-rw-r--r--   0 root         (0) root         (0)      866 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/register_random_torch_state.py
+-rw-r--r--   0 root         (0) root         (0)     9464 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     1442 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/hypothesis_torch/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 02:19:21.285204 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9045 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      665 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-12 02:19:21.000000 hypothesis_torch-0.6.3/hypothesis_torch.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-05-12 02:18:47.000000 hypothesis_torch-0.6.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-12 02:19:21.289204 hypothesis_torch-0.6.3/setup.cfg
```

### Comparing `hypothesis_torch-0.6.2/LICENSE` & `hypothesis_torch-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/PKG-INFO` & `hypothesis_torch-0.6.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.6.2
+Version: 0.6.3
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,30 +22,35 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/qthequartermasterman/hypothesis-torch
-Project-URL: Documentation, https://hypothesis-torch.readthedocs.io/en/latest/
+Project-URL: Documentation, https://hypothesis-torch.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/qthequartermasterman/hypothesis-torch.git
 Project-URL: Issues, https://github.com/qthequartermasterman/hypothesis-torch/issues
-Keywords: hypothesis,torch,pytorch,testing,property-based testing
+Keywords: hypothesis,torch,pytorch,testing,property-based testing,deep learning,tensor,neural network,artificial intelligence,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Hypothesis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hypothesis<=6.98.8,>=6.0.0
 Requires-Dist: torch<=2.3.0,>=1.13.0
 Provides-Extra: huggingface
 Requires-Dist: transformers<=4.40.0,>=4.0.0; extra == "huggingface"
@@ -57,14 +62,16 @@
 Requires-Dist: mkdocs==1.6.0; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.25.1; extra == "docs"
 Requires-Dist: mkdocs-autolinks-plugin==0.7.1; extra == "docs"
 Requires-Dist: mkdocs-material==9.4.6; extra == "docs"
 Requires-Dist: mkdocs-snippets==1.3.0; extra == "docs"
 Requires-Dist: mkdocs-exclude==1.0.2; extra == "docs"
 
+[![PyPI version](https://img.shields.io/pypi/v/hypothesis-torch.svg)](https://pypi.org/project/hypothesis-torch) ![PyPI - Downloads](https://img.shields.io/pypi/dm/hypothesis-torch)
+
 # hypothesis-torch
 Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 
 ## Installation
```

### Comparing `hypothesis_torch-0.6.2/README.md` & `hypothesis_torch-0.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![PyPI version](https://img.shields.io/pypi/v/hypothesis-torch.svg)](https://pypi.org/project/hypothesis-torch) ![PyPI - Downloads](https://img.shields.io/pypi/dm/hypothesis-torch)
+
 # hypothesis-torch
 Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 
 ## Installation
```

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/__init__.py` & `hypothesis_torch-0.6.3/hypothesis_torch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 """
 
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 import importlib.util
 
 from hypothesis_torch.device import (
     device_strategy,
     AVAILABLE_CPU_DEVICES,
     AVAILABLE_CUDA_DEVICES,
     AVAILABLE_MPS_DEVICES,
```

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/device.py` & `hypothesis_torch-0.6.3/hypothesis_torch/device.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/dtype.py` & `hypothesis_torch-0.6.3/hypothesis_torch/dtype.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/huggingface.py` & `hypothesis_torch-0.6.3/hypothesis_torch/huggingface.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/inspection_util.py` & `hypothesis_torch-0.6.3/hypothesis_torch/inspection_util.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/layout.py` & `hypothesis_torch-0.6.3/hypothesis_torch/layout.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/memory_format.py` & `hypothesis_torch-0.6.3/hypothesis_torch/memory_format.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/module.py` & `hypothesis_torch-0.6.3/hypothesis_torch/module.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/optim.py` & `hypothesis_torch-0.6.3/hypothesis_torch/optim.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     "etas": st.tuples(
         st.floats(min_value=0.0, max_value=1.0, exclude_min=True, exclude_max=True),
         st.floats(min_value=1.0, max_value=2.0, exclude_min=True, exclude_max=True),
     ),
     "dampening": _ZERO_TO_ONE_FLOATS,
     "nesterov": st.booleans(),
     "initial_accumulator_value": _ZERO_TO_ONE_FLOATS,
+    "fused": st.booleans() if torch.cuda.is_available() else st.just(False),
 }
 
 
 def optimizer_type_strategy(
     allowed_optimizer_types: Sequence[type[torch.optim.Optimizer]] | None = None,
 ) -> st.SearchStrategy[type[torch.optim.Optimizer]]:
     """Strategy for generating torch optimizers.
@@ -108,14 +109,18 @@
         else:
             kwargs[param.name] = draw(st.from_type(param.annotation))
     if "nesterov" in kwargs and kwargs["nesterov"] and "momentum" in kwargs:
         kwargs["dampening"] = 0
     kwargs.pop("self", None)  # Remove self if a type was inferred
     kwargs.pop("params", None)  # Remove params if a type was inferred
 
+    # Adam cannot be both fused and differentiable simultaneously
+    if "differentiable" in kwargs and kwargs["differentiable"] and "fused" in kwargs and kwargs["fused"]:
+        kwargs.pop("differentiable")
+
     hypothesis.note(f"Chosen optimizer type: {optimizer_type}")
     hypothesis.note(f"Chosen optimizer hyperparameters: {kwargs}")
 
     def optimizer_factory(params: Sequence[torch.nn.Parameter]) -> torch.optim.Optimizer:
         return optimizer_type(params, **kwargs)
 
     return optimizer_factory
```

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/register_random_torch_state.py` & `hypothesis_torch-0.6.3/hypothesis_torch/register_random_torch_state.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/tensor.py` & `hypothesis_torch-0.6.3/hypothesis_torch/tensor.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch/utils.py` & `hypothesis_torch-0.6.3/hypothesis_torch/utils.py`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch.egg-info/PKG-INFO` & `hypothesis_torch-0.6.3/hypothesis_torch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypothesis-torch
-Version: 0.6.2
+Version: 0.6.3
 Summary: Hypothesis strategies for various Pytorch structures, including tensors and modules.
 Author-email: "Andrew P. Sansom" <andrew@euleriancircuit.com>
 License: MIT License
         
         Copyright (c) 2024 Andrew Sansom
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,30 +22,35 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/qthequartermasterman/hypothesis-torch
-Project-URL: Documentation, https://hypothesis-torch.readthedocs.io/en/latest/
+Project-URL: Documentation, https://hypothesis-torch.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/qthequartermasterman/hypothesis-torch.git
 Project-URL: Issues, https://github.com/qthequartermasterman/hypothesis-torch/issues
-Keywords: hypothesis,torch,pytorch,testing,property-based testing
+Keywords: hypothesis,torch,pytorch,testing,property-based testing,deep learning,tensor,neural network,artificial intelligence,machine learning
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Hypothesis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hypothesis<=6.98.8,>=6.0.0
 Requires-Dist: torch<=2.3.0,>=1.13.0
 Provides-Extra: huggingface
 Requires-Dist: transformers<=4.40.0,>=4.0.0; extra == "huggingface"
@@ -57,14 +62,16 @@
 Requires-Dist: mkdocs==1.6.0; extra == "docs"
 Requires-Dist: mkdocstrings[python]==0.25.1; extra == "docs"
 Requires-Dist: mkdocs-autolinks-plugin==0.7.1; extra == "docs"
 Requires-Dist: mkdocs-material==9.4.6; extra == "docs"
 Requires-Dist: mkdocs-snippets==1.3.0; extra == "docs"
 Requires-Dist: mkdocs-exclude==1.0.2; extra == "docs"
 
+[![PyPI version](https://img.shields.io/pypi/v/hypothesis-torch.svg)](https://pypi.org/project/hypothesis-torch) ![PyPI - Downloads](https://img.shields.io/pypi/dm/hypothesis-torch)
+
 # hypothesis-torch
 Hypothesis strategies for various Pytorch structures (including tensors and modules).
 
 [Hypothesis](https://hypothesis.readthedocs.io/en/latest/) is a powerful property-based testing library for Python. It
 lacks built-in support for Pytorch tensors and modules, so this library provides strategies for generating them.
 
 ## Installation
```

### Comparing `hypothesis_torch-0.6.2/hypothesis_torch.egg-info/SOURCES.txt` & `hypothesis_torch-0.6.3/hypothesis_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypothesis_torch-0.6.2/pyproject.toml` & `hypothesis_torch-0.6.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,34 +11,37 @@
     "hypothesis>=6.0.0,<=6.98.8",
     "torch>=1.13.0,<=2.3.0",
 ]
 requires-python = ">=3.9"
 authors=[{name="Andrew P. Sansom", email="andrew@euleriancircuit.com"}]
 readme="README.md"
 license={file="LICENSE"}
-keywords = ["hypothesis", "torch", "pytorch", "testing", "property-based testing"]
+keywords = ["hypothesis", "torch", "pytorch", "testing", "property-based testing", "deep learning", "tensor", "neural network", "artificial intelligence", "machine learning"]
 classifiers = [
-  "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 2 - Pre-Alpha",
 
-  # Indicate who your project is intended for
-  "Intended Audience :: Developers",
-  "Framework :: Hypothesis",
+    "Intended Audience :: Developers",
+    "Framework :: Hypothesis",
 
-  # Pick your license as you wish (see also "license" above)
-  "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: MIT License",
 
-  # Specify the Python versions you support here.
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+
     "Topic :: Software Development :: Testing",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Scientific/Engineering :: Mathematics",
+    "Topic :: Software Development",
+    "Topic :: Software Development :: Libraries",
+    "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 [project.entry-points."hypothesis"]
 _ = "hypothesis_torch.register_random_torch_state:_register_random_torch_state"
 
 [project.optional-dependencies]
 huggingface = [
   "transformers<=4.40.0,>=4.0.0",
@@ -55,15 +58,15 @@
   "mkdocs-material==9.4.6",
   "mkdocs-snippets==1.3.0",
   "mkdocs-exclude==1.0.2",
 ]
 
 [project.urls]
 Homepage = "https://github.com/qthequartermasterman/hypothesis-torch"
-Documentation = "https://hypothesis-torch.readthedocs.io/en/latest/"
+Documentation = "https://hypothesis-torch.readthedocs.io/en/stable/"
 Repository = "https://github.com/qthequartermasterman/hypothesis-torch.git"
 Issues = "https://github.com/qthequartermasterman/hypothesis-torch/issues"
 
 [tool.ruff]
 line-length = 120
 
 [tool.semantic_release]
```

