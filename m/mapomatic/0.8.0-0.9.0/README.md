# Comparing `tmp/mapomatic-0.8.0.tar.gz` & `tmp/mapomatic-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapomatic-0.8.0.tar", last modified: Wed Mar  1 14:25:21 2023, max compression
+gzip compressed data, was "mapomatic-0.9.0.tar", last modified: Tue Aug 29 18:19:43 2023, max compression
```

## Comparing `mapomatic-0.8.0.tar` & `mapomatic-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-03-01 14:25:21.119159 mapomatic-0.8.0/
--rw-r--r--   0 paul       (501) staff       (20)    11357 2023-01-06 18:17:08.000000 mapomatic-0.8.0/LICENSE
--rw-r--r--   0 paul       (501) staff       (20)       45 2023-01-06 18:17:08.000000 mapomatic-0.8.0/MANIFEST.in
--rw-r--r--   0 paul       (501) staff       (20)      837 2023-03-01 14:25:21.119028 mapomatic-0.8.0/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)    13249 2023-03-01 14:07:40.000000 mapomatic-0.8.0/README.md
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-03-01 14:25:21.116499 mapomatic-0.8.0/mapomatic/
--rw-r--r--   0 paul       (501) staff       (20)      991 2023-01-06 18:17:08.000000 mapomatic-0.8.0/mapomatic/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     4135 2023-03-01 14:07:37.000000 mapomatic-0.8.0/mapomatic/circuits.py
--rw-r--r--   0 paul       (501) staff       (20)     8699 2023-03-01 14:24:53.000000 mapomatic-0.8.0/mapomatic/layouts.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-03-01 14:25:21.118810 mapomatic-0.8.0/mapomatic/tests/
--rw-r--r--   0 paul       (501) staff       (20)      480 2023-01-06 18:17:08.000000 mapomatic-0.8.0/mapomatic/tests/__init__.py
--rw-r--r--   0 paul       (501) staff       (20)     2773 2023-03-01 14:07:37.000000 mapomatic-0.8.0/mapomatic/tests/test_best_layout.py
--rw-r--r--   0 paul       (501) staff       (20)     4013 2023-01-06 18:17:08.000000 mapomatic-0.8.0/mapomatic/tests/test_best_layout_custom.py
--rw-r--r--   0 paul       (501) staff       (20)     2067 2023-01-06 18:17:08.000000 mapomatic-0.8.0/mapomatic/tests/test_deflate_barriers.py
--rw-r--r--   0 paul       (501) staff       (20)     2029 2023-03-01 14:07:37.000000 mapomatic-0.8.0/mapomatic/tests/test_inflate.py
--rw-r--r--   0 paul       (501) staff       (20)     1424 2023-01-06 18:17:08.000000 mapomatic-0.8.0/mapomatic/tests/test_matching_layout.py
--rw-r--r--   0 paul       (501) staff       (20)     1371 2023-01-06 18:17:08.000000 mapomatic-0.8.0/mapomatic/tests/test_subgraphs.py
--rw-r--r--   0 paul       (501) staff       (20)     1225 2023-01-06 18:17:08.000000 mapomatic-0.8.0/mapomatic/tests/test_transpiler_layout.py
--rw-r--r--   0 paul       (501) staff       (20)      177 2023-03-01 14:25:20.000000 mapomatic-0.8.0/mapomatic/version.py
-drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-03-01 14:25:21.117279 mapomatic-0.8.0/mapomatic.egg-info/
--rw-r--r--   0 paul       (501) staff       (20)      837 2023-03-01 14:25:21.000000 mapomatic-0.8.0/mapomatic.egg-info/PKG-INFO
--rw-r--r--   0 paul       (501) staff       (20)      633 2023-03-01 14:25:21.000000 mapomatic-0.8.0/mapomatic.egg-info/SOURCES.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-03-01 14:25:21.000000 mapomatic-0.8.0/mapomatic.egg-info/dependency_links.txt
--rw-r--r--   0 paul       (501) staff       (20)        1 2023-03-01 14:25:21.000000 mapomatic-0.8.0/mapomatic.egg-info/not-zip-safe
--rw-r--r--   0 paul       (501) staff       (20)       37 2023-03-01 14:25:21.000000 mapomatic-0.8.0/mapomatic.egg-info/requires.txt
--rw-r--r--   0 paul       (501) staff       (20)       10 2023-03-01 14:25:21.000000 mapomatic-0.8.0/mapomatic.egg-info/top_level.txt
--rw-r--r--   0 paul       (501) staff       (20)       37 2023-03-01 14:07:37.000000 mapomatic-0.8.0/requirements.txt
--rw-r--r--   0 paul       (501) staff       (20)       38 2023-03-01 14:25:21.119196 mapomatic-0.8.0/setup.cfg
--rw-r--r--   0 paul       (501) staff       (20)     4945 2023-03-01 14:07:37.000000 mapomatic-0.8.0/setup.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-29 18:19:43.357688 mapomatic-0.9.0/
+-rw-r--r--   0 paul       (501) staff       (20)    11357 2023-08-29 17:58:15.000000 mapomatic-0.9.0/LICENSE
+-rw-r--r--   0 paul       (501) staff       (20)       45 2023-08-29 17:58:15.000000 mapomatic-0.9.0/MANIFEST.in
+-rw-r--r--   0 paul       (501) staff       (20)      837 2023-08-29 18:19:43.357544 mapomatic-0.9.0/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)    14096 2023-08-29 18:18:32.000000 mapomatic-0.9.0/README.md
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-29 18:19:43.354563 mapomatic-0.9.0/mapomatic/
+-rw-r--r--   0 paul       (501) staff       (20)      991 2023-08-29 17:58:15.000000 mapomatic-0.9.0/mapomatic/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     4135 2023-08-29 17:58:15.000000 mapomatic-0.9.0/mapomatic/circuits.py
+-rw-r--r--   0 paul       (501) staff       (20)     8704 2023-08-29 18:18:32.000000 mapomatic-0.9.0/mapomatic/layouts.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-29 18:19:43.357316 mapomatic-0.9.0/mapomatic/tests/
+-rw-r--r--   0 paul       (501) staff       (20)      480 2023-08-29 17:58:15.000000 mapomatic-0.9.0/mapomatic/tests/__init__.py
+-rw-r--r--   0 paul       (501) staff       (20)     2773 2023-08-29 18:18:32.000000 mapomatic-0.9.0/mapomatic/tests/test_best_layout.py
+-rw-r--r--   0 paul       (501) staff       (20)     4013 2023-08-29 17:58:15.000000 mapomatic-0.9.0/mapomatic/tests/test_best_layout_custom.py
+-rw-r--r--   0 paul       (501) staff       (20)     2067 2023-08-29 17:58:15.000000 mapomatic-0.9.0/mapomatic/tests/test_deflate_barriers.py
+-rw-r--r--   0 paul       (501) staff       (20)     2029 2023-08-29 17:58:15.000000 mapomatic-0.9.0/mapomatic/tests/test_inflate.py
+-rw-r--r--   0 paul       (501) staff       (20)     1424 2023-08-29 17:58:15.000000 mapomatic-0.9.0/mapomatic/tests/test_matching_layout.py
+-rw-r--r--   0 paul       (501) staff       (20)     1371 2023-08-29 17:58:15.000000 mapomatic-0.9.0/mapomatic/tests/test_subgraphs.py
+-rw-r--r--   0 paul       (501) staff       (20)     1225 2023-08-29 17:58:15.000000 mapomatic-0.9.0/mapomatic/tests/test_transpiler_layout.py
+-rw-r--r--   0 paul       (501) staff       (20)      163 2023-08-29 18:19:43.000000 mapomatic-0.9.0/mapomatic/version.py
+drwxr-xr-x   0 paul       (501) staff       (20)        0 2023-08-29 18:19:43.355954 mapomatic-0.9.0/mapomatic.egg-info/
+-rw-r--r--   0 paul       (501) staff       (20)      837 2023-08-29 18:19:43.000000 mapomatic-0.9.0/mapomatic.egg-info/PKG-INFO
+-rw-r--r--   0 paul       (501) staff       (20)      633 2023-08-29 18:19:43.000000 mapomatic-0.9.0/mapomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-08-29 18:19:43.000000 mapomatic-0.9.0/mapomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 paul       (501) staff       (20)        1 2023-08-29 18:19:43.000000 mapomatic-0.9.0/mapomatic.egg-info/not-zip-safe
+-rw-r--r--   0 paul       (501) staff       (20)       37 2023-08-29 18:19:43.000000 mapomatic-0.9.0/mapomatic.egg-info/requires.txt
+-rw-r--r--   0 paul       (501) staff       (20)       10 2023-08-29 18:19:43.000000 mapomatic-0.9.0/mapomatic.egg-info/top_level.txt
+-rw-r--r--   0 paul       (501) staff       (20)       37 2023-08-29 17:58:15.000000 mapomatic-0.9.0/requirements.txt
+-rw-r--r--   0 paul       (501) staff       (20)       38 2023-08-29 18:19:43.357735 mapomatic-0.9.0/setup.cfg
+-rw-r--r--   0 paul       (501) staff       (20)     4944 2023-08-29 18:18:32.000000 mapomatic-0.9.0/setup.py
```

### Comparing `mapomatic-0.8.0/LICENSE` & `mapomatic-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapomatic-0.8.0/PKG-INFO` & `mapomatic-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapomatic
-Version: 0.8.0
+Version: 0.9.0
 Summary: Mapomatic
 Home-page: 
 Author: Paul Nation
 Author-email: paul.nation@ibm.com
 License: Apache 2.0
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mapomatic-0.8.0/README.md` & `mapomatic-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,28 @@
 
 ## Overview
 
 One of the main painpoints in executing circuits on IBM Quantum hardware is finding the best qubit mapping.  For a given circuit, one typically tries to pick the best `initial_layout` for a given target system, and then SWAP maps using that set of qubits as the starting point.  However there are a couple of issues with that execution model.  First, an `initial_layout` selected, for example with respect to the noise characteristics of the system, need not be optimal for the SWAP mapping.  In practice this leads to either low-noise layouts with extra SWAP gates inserted in the circuit, or optimally SWAP mapped circuits on (possibly) lousy qubits.  Second, there is no way to know if the system you targeted in the compilation is actually the best one to execute the compiled circuit on.  With 20+ quantum systems, it is hard to determine which device is actually ideal for a given problem.
 
 `mapomatic` tries to tackle these issues in a different way. `mapomatic` is a post-compilation routine that finds the best low noise sub-graph on which to run a circuit given one or more quantum systems as target devices.  Once compiled, a circuit has been rewritten so that its two-qubit gate structure matches that of a given sub-graph on the target system.  `mapomatic` then searches for matching sub-graphs using the VF2 mapper in [Qiskit](https://github.com/Qiskit/qiskit-terra) ([retworkx](https://github.com/Qiskit/retworkx) actually), and uses a heuristic to rank them based on error rates determined by the current calibration data. That is to say that given a single target system, `mapomatic` will return the best set of qubits on which to execute the compiled circuit.  Or, given a list of systems, it will find the best system and set of qubits on which to run your circuit.  Given the current size of quantum hardware, and the excellent performance of the VF2 mapper, this whole process is actually very fast.
 
+### Qiskit Transpiler
+
+The same algorithm used in mapomatic is integrated into the Qiskit transpiler
+by default as the `VF2PostLayout` pass (https://qiskit.org/documentation/stubs/qiskit.transpiler.passes.VF2PostLayout.html)
+which gets run by default in optimization levels 1, 2, and 3. Using mapomatic
+as a standalone tool has two primary advantages, the first is to enable
+running over multiple backends, and the second is to experiment with alternative
+heuristic scoring (`VF2PostLayout` supports custom heuristic scoring, but it
+is more difficult to integrate that into `transpile()`).
+
+## Installation
+`mapomatic` can be installed via `pip`: `pip install mapomatic` or installed from source.
+
+
 ## Usage
 
 To begin we first import what we need and load our IBM Quantum account.
 
 ```python
 import numpy as np
 from qiskit import *
@@ -324,7 +338,11 @@
  ([4, 0, 1, 2, 3], 'ibm_auckland', 0.2448657847182769),
  ([4, 0, 1, 2, 3], 'ibmq_guadalupe', 0.3104200973685135),
  ([0, 2, 1, 3, 4], 'ibmq_lima', 0.31936325970774426),
  ([5, 15, 4, 3, 2], 'ibm_washington', 0.35009793314185045),
  ([4, 0, 1, 2, 3], 'ibmq_toronto', 0.39020468922200047),
  ([4, 0, 1, 2, 3], 'ibm_cairo', 0.4133587550267118)]
  ```
+
+# Citing
+
+If you use mapomatic in your research, we would be delighted if you cite it in your work using the included [BibTeX file](CITATION.bib).
```

### Comparing `mapomatic-0.8.0/mapomatic/__init__.py` & `mapomatic-0.9.0/mapomatic/__init__.py`

 * *Files identical despite different names*

### Comparing `mapomatic-0.8.0/mapomatic/circuits.py` & `mapomatic-0.9.0/mapomatic/circuits.py`

 * *Files identical despite different names*

### Comparing `mapomatic-0.8.0/mapomatic/layouts.py` & `mapomatic-0.9.0/mapomatic/layouts.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,15 @@
                 layouts[key] = matching_layouts(circ, config.coupling_map,
                                                 call_limit=call_limit)
             layout_and_error = evaluate_layouts(circ, layouts[key], backend,
                                                 cost_function=cost_function)
             if any(layout_and_error):
                 layout = layout_and_error[0][0]
                 error = layout_and_error[0][1]
-                best_out.append((layout, backend.name(), error))
+                best_out.append((layout, config.backend_name, error))
     best_out.sort(key=lambda x: x[2])
     if successors:
         return best_out
     return best_out[0]
 
 
 def default_cost(circ, layouts, backend):
```

### Comparing `mapomatic-0.8.0/mapomatic/tests/test_best_layout.py` & `mapomatic-0.9.0/mapomatic/tests/test_best_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,14 +53,14 @@
     qc.cx(qr_a[0], qr_b[1])
     qc.measure(qr_a, cr_b)
     qc.measure(qr_b, cr_a)
     trans_qc = transpile(qc, FakeLima(), seed_transpiler=102442)
     small_circ = mm.deflate_circuit(trans_qc)
     backends = [FakeBelem(), FakeQuito(), FakeLima()]
     res = mm.best_overall_layout(small_circ, backends, successors=True)
-    expected_res = [([0, 1, 2, 3], 'fake_lima', 0.13133288833556145),
-                    ([2, 1, 3, 0], 'fake_belem', 0.16103780370236487),
-                    ([3, 1, 0, 2], 'fake_quito', 0.29391929118639826)]
+    expected_res = [([0, 1, 3, 2], 'fake_lima', 0.13133288833556145),
+                    ([2, 1, 0, 3], 'fake_belem', 0.16103780370236487),
+                    ([3, 1, 2, 0], 'fake_quito', 0.29391929118639826)]
     for index, expected in enumerate(expected_res):
         assert res[index][0] == expected[0]
         assert res[index][1] == expected[1]
         assert np.allclose(res[index][2], expected[2])
```

### Comparing `mapomatic-0.8.0/mapomatic/tests/test_best_layout_custom.py` & `mapomatic-0.9.0/mapomatic/tests/test_best_layout_custom.py`

 * *Files identical despite different names*

### Comparing `mapomatic-0.8.0/mapomatic/tests/test_deflate_barriers.py` & `mapomatic-0.9.0/mapomatic/tests/test_deflate_barriers.py`

 * *Files identical despite different names*

### Comparing `mapomatic-0.8.0/mapomatic/tests/test_inflate.py` & `mapomatic-0.9.0/mapomatic/tests/test_inflate.py`

 * *Files identical despite different names*

### Comparing `mapomatic-0.8.0/mapomatic/tests/test_matching_layout.py` & `mapomatic-0.9.0/mapomatic/tests/test_matching_layout.py`

 * *Files identical despite different names*

### Comparing `mapomatic-0.8.0/mapomatic/tests/test_subgraphs.py` & `mapomatic-0.9.0/mapomatic/tests/test_subgraphs.py`

 * *Files identical despite different names*

### Comparing `mapomatic-0.8.0/mapomatic/tests/test_transpiler_layout.py` & `mapomatic-0.9.0/mapomatic/tests/test_transpiler_layout.py`

 * *Files identical despite different names*

### Comparing `mapomatic-0.8.0/mapomatic.egg-info/PKG-INFO` & `mapomatic-0.9.0/mapomatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapomatic
-Version: 0.8.0
+Version: 0.9.0
 Summary: Mapomatic
 Home-page: 
 Author: Paul Nation
 Author-email: paul.nation@ibm.com
 License: Apache 2.0
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `mapomatic-0.8.0/mapomatic.egg-info/SOURCES.txt` & `mapomatic-0.9.0/mapomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapomatic-0.8.0/setup.py` & `mapomatic-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import os
 import sys
 import subprocess
 import setuptools
 
 
 MAJOR = 0
-MINOR = 8
+MINOR = 9
 MICRO = 0
 
-ISRELEASED = False
+ISRELEASED = True
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 REQUIREMENTS = []
 with open("requirements.txt") as f:
     for line in f:
         req = line.split('#')[0]
         if req:
```

