# Comparing `tmp/PyAcoustiX-0.9.11.tar.gz` & `tmp/PyAcoustiX-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAcoustiX-0.9.11.tar", last modified: Sun May 12 14:31:14 2024, max compression
+gzip compressed data, was "PyAcoustiX-0.9.9.tar", last modified: Sun May 12 14:12:12 2024, max compression
```

## Comparing `PyAcoustiX-0.9.11.tar` & `PyAcoustiX-0.9.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:31:14.415159 PyAcoustiX-0.9.11/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1070 2024-05-05 18:15:22.000000 PyAcoustiX-0.9.11/LICENSE
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4674 2024-05-12 14:31:14.415159 PyAcoustiX-0.9.11/PKG-INFO
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:31:14.415159 PyAcoustiX-0.9.11/PyAcoustiX.egg-info/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4674 2024-05-12 14:31:14.000000 PyAcoustiX-0.9.11/PyAcoustiX.egg-info/PKG-INFO
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1126 2024-05-12 14:31:14.000000 PyAcoustiX-0.9.11/PyAcoustiX.egg-info/SOURCES.txt
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        1 2024-05-12 14:31:14.000000 PyAcoustiX-0.9.11/PyAcoustiX.egg-info/dependency_links.txt
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       48 2024-05-12 14:31:14.000000 PyAcoustiX-0.9.11/PyAcoustiX.egg-info/entry_points.txt
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       29 2024-05-12 14:31:14.000000 PyAcoustiX-0.9.11/PyAcoustiX.egg-info/requires.txt
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       18 2024-05-12 14:31:14.000000 PyAcoustiX-0.9.11/PyAcoustiX.egg-info/top_level.txt
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4033 2024-05-12 14:26:17.000000 PyAcoustiX-0.9.11/README.md
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:31:14.415159 PyAcoustiX-0.9.11/SAcouS/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)      256 2024-05-10 19:03:16.000000 PyAcoustiX-0.9.11/SAcouS/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2982 2024-05-12 13:38:16.000000 PyAcoustiX-0.9.11/SAcouS/__main__.py
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:31:14.415159 PyAcoustiX-0.9.11/SAcouS/acxfem/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3518 2024-05-11 14:03:42.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/BCs_impose.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        1 2024-05-05 19:02:57.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    16704 2024-05-11 14:04:49.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/assembly.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3944 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/basis.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    13450 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/dofhandler.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    10497 2024-05-11 15:07:27.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/materials.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4557 2024-05-11 19:19:16.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/mesh.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    10565 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/physic_assembler.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     7452 2023-12-23 11:17:09.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/polynomial.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4461 2024-05-11 20:07:37.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/postprocess.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2869 2024-05-11 20:22:08.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/precompute_matrices.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3464 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/precompute_matrices_lag.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    12018 2023-12-23 19:04:28.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/quadratures.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4544 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/solver.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1658 2023-09-11 19:45:03.000000 PyAcoustiX-0.9.11/SAcouS/acxfem/utilities.py
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:31:14.415159 PyAcoustiX-0.9.11/SAcouS/acxmor/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:03:30.000000 PyAcoustiX-0.9.11/SAcouS/acxmor/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2510 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.11/SAcouS/acxmor/modal_reduction.py
--rw-------   0 shaoqi    (1000) shaoqi    (1000)     2797 2023-12-02 20:22:21.000000 PyAcoustiX-0.9.11/SAcouS/acxmor/myEIM.py
--rw-------   0 shaoqi    (1000) shaoqi    (1000)     9494 2023-12-02 20:22:26.000000 PyAcoustiX-0.9.11/SAcouS/acxmor/myRBSolver.py
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:31:14.415159 PyAcoustiX-0.9.11/SAcouS/acxtmm/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1678 2023-08-25 21:15:58.000000 PyAcoustiX-0.9.11/SAcouS/acxtmm/BC_matrix.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:03:05.000000 PyAcoustiX-0.9.11/SAcouS/acxtmm/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1773 2024-05-11 14:04:55.000000 PyAcoustiX-0.9.11/SAcouS/acxtmm/adm_assembler.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    11062 2023-11-09 20:58:34.000000 PyAcoustiX-0.9.11/SAcouS/acxtmm/adm_basis.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     7867 2023-08-20 17:00:10.000000 PyAcoustiX-0.9.11/SAcouS/acxtmm/tmm.py
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:31:14.415159 PyAcoustiX-0.9.11/SAcouS/interface/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-10 19:03:05.000000 PyAcoustiX-0.9.11/SAcouS/interface/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     9860 2024-05-11 20:22:16.000000 PyAcoustiX-0.9.11/SAcouS/interface/parser.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4985 2024-05-12 13:11:48.000000 PyAcoustiX-0.9.11/SAcouS/interface/sol_setup.py
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:31:14.415159 PyAcoustiX-0.9.11/analytical/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     5547 2023-07-31 19:01:24.000000 PyAcoustiX-0.9.11/analytical/Biot_sol.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     6372 2024-05-05 19:00:03.000000 PyAcoustiX-0.9.11/analytical/Fluid_Biot_sol.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:07:10.000000 PyAcoustiX-0.9.11/analytical/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3896 2024-05-11 14:04:27.000000 PyAcoustiX-0.9.11/analytical/fluid_sol.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       38 2024-05-12 14:31:14.415159 PyAcoustiX-0.9.11/setup.cfg
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1175 2024-05-12 14:30:21.000000 PyAcoustiX-0.9.11/setup.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1070 2024-05-05 18:15:22.000000 PyAcoustiX-0.9.9/LICENSE
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4111 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/PKG-INFO
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4111 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/PKG-INFO
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1126 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/SOURCES.txt
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        1 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/dependency_links.txt
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       48 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/entry_points.txt
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       29 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/requires.txt
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       18 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/top_level.txt
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3486 2024-05-11 20:49:00.000000 PyAcoustiX-0.9.9/README.md
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/SAcouS/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)      256 2024-05-10 19:03:16.000000 PyAcoustiX-0.9.9/SAcouS/__init__.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2982 2024-05-12 13:38:16.000000 PyAcoustiX-0.9.9/SAcouS/__main__.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/SAcouS/acxfem/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3518 2024-05-11 14:03:42.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/BCs_impose.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        1 2024-05-05 19:02:57.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/__init__.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    16704 2024-05-11 14:04:49.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/assembly.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3944 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/basis.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    13450 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/dofhandler.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    10497 2024-05-11 15:07:27.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/materials.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4557 2024-05-11 19:19:16.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/mesh.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    10565 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/physic_assembler.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     7452 2023-12-23 11:17:09.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/polynomial.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4461 2024-05-11 20:07:37.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/postprocess.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2869 2024-05-11 20:22:08.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/precompute_matrices.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3464 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/precompute_matrices_lag.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    12018 2023-12-23 19:04:28.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/quadratures.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4544 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/solver.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1658 2023-09-11 19:45:03.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/utilities.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/SAcouS/acxmor/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:03:30.000000 PyAcoustiX-0.9.9/SAcouS/acxmor/__init__.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2510 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxmor/modal_reduction.py
+-rw-------   0 shaoqi    (1000) shaoqi    (1000)     2797 2023-12-02 20:22:21.000000 PyAcoustiX-0.9.9/SAcouS/acxmor/myEIM.py
+-rw-------   0 shaoqi    (1000) shaoqi    (1000)     9494 2023-12-02 20:22:26.000000 PyAcoustiX-0.9.9/SAcouS/acxmor/myRBSolver.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/SAcouS/acxtmm/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1678 2023-08-25 21:15:58.000000 PyAcoustiX-0.9.9/SAcouS/acxtmm/BC_matrix.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:03:05.000000 PyAcoustiX-0.9.9/SAcouS/acxtmm/__init__.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1773 2024-05-11 14:04:55.000000 PyAcoustiX-0.9.9/SAcouS/acxtmm/adm_assembler.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    11062 2023-11-09 20:58:34.000000 PyAcoustiX-0.9.9/SAcouS/acxtmm/adm_basis.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     7867 2023-08-20 17:00:10.000000 PyAcoustiX-0.9.9/SAcouS/acxtmm/tmm.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/SAcouS/interface/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-10 19:03:05.000000 PyAcoustiX-0.9.9/SAcouS/interface/__init__.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     9860 2024-05-11 20:22:16.000000 PyAcoustiX-0.9.9/SAcouS/interface/parser.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4985 2024-05-12 13:11:48.000000 PyAcoustiX-0.9.9/SAcouS/interface/sol_setup.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/analytical/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     5547 2023-07-31 19:01:24.000000 PyAcoustiX-0.9.9/analytical/Biot_sol.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     6372 2024-05-05 19:00:03.000000 PyAcoustiX-0.9.9/analytical/Fluid_Biot_sol.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:07:10.000000 PyAcoustiX-0.9.9/analytical/__init__.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3896 2024-05-11 14:04:27.000000 PyAcoustiX-0.9.9/analytical/fluid_sol.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       38 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/setup.cfg
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1159 2024-05-12 14:07:32.000000 PyAcoustiX-0.9.9/setup.py
```

### Comparing `PyAcoustiX-0.9.11/LICENSE` & `PyAcoustiX-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/PKG-INFO` & `PyAcoustiX-0.9.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: PyAcoustiX
-Version: 0.9.11
-Summary: A pure Python package/software for acoustic analysis
+Version: 0.9.9
+Summary: A Python package for acoustic analysis
 Home-page: https://github.com/Shaoqigit/PyXfem
 Author: Shaoqi WU
 Author-email: shaoqiwu@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **S**imple **A**coustic **S**imulator(SAcouS)
 [comment]: <> ( - AcoustiX based Sound simulation library)
 [comment]: <> ( - put following badges centre)
@@ -24,46 +24,32 @@
 [![PyPi Version](https://img.shields.io/pypi/v/pyacoustix.svg?style=flat-square)](https://pypi.org/project/PyAcoustiX/)
 
 </center>
 
                                  based on Finite Element Method
                                  contact: Shaoqiwu@outlook.com
 
-**SAcouS** is pure python software based on an Finite Element libraray 'PyacoustiX' (AcoustiX in cpp version found in my git repo https://github.com/Shaoqigit/AcoustiX), mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
+**SAcouS** is pure python software based on an Finite Element libraray 'PyacoustiX' (AcoustiX in cpp version found in my git repo), mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
 
 ## Installation and Usage
 ```bash
 pip install pyacoustix
 ```
-- You can use either as a standalone library or as a part of your project. The following is a simple example to use the library:
+You can use either as a standalone library or as a part of your project. The following is a simple example to use the library:
 ```python
 from SAcouS import *
 ```
-- either used with executable with standard pyacoustix input file format .axi. To do so, you need first install the package as
+either used with executable with standard pyacoustix input file format .axi. To do so, you need first install the package as
 ```bash
 pip install .
 ```
 Then you can run the following command to execute the simulation:
 ```bash
 sacous -i input_file.axi
 ```
-- This software is also a wrap of python interpreter, so you can use it interactively with the comsole by entering:
-```bash
-sacous
-```
-you get into PyacoustiX console, where you can use the library interactively. For example:
-```bash
-Welcome to PyAcoustiX console!
-PyAcoustiX 0.9.10
-base on python 3.10.13 (main, Sep 11 2023, 13:44:35) [GCC 11.2.0] on linux
-Type "help", "copyright" or "license" for more information.
-Author: Shaoqiwu@outlook.com
-(PyAcoustiXInteractiveConsole)
->>> import numpy as np
-```
 
 ## Main special features/architecture of the library compared to other existing lib:
 > * Apart from classical Linear/Quadratic Larange polynomial, **High order (lobatto)** shape functions are supported.
 > * The element type (interpolation order of shape functions) can be **varied** on each element (mesh).
 > * **Extended elements** and double node techinique are used to deal with discontitnuity.
 > * Various common Acoustic materials are supported, including porous rigid, Limp and **Biot-up** models.
 > * FEM-**TMM** coupling is supported to model multi-layered configuration in general geometry problems.
```

### Comparing `PyAcoustiX-0.9.11/PyAcoustiX.egg-info/PKG-INFO` & `PyAcoustiX-0.9.9/PyAcoustiX.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: PyAcoustiX
-Version: 0.9.11
-Summary: A pure Python package/software for acoustic analysis
+Version: 0.9.9
+Summary: A Python package for acoustic analysis
 Home-page: https://github.com/Shaoqigit/PyXfem
 Author: Shaoqi WU
 Author-email: shaoqiwu@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **S**imple **A**coustic **S**imulator(SAcouS)
 [comment]: <> ( - AcoustiX based Sound simulation library)
 [comment]: <> ( - put following badges centre)
@@ -24,46 +24,32 @@
 [![PyPi Version](https://img.shields.io/pypi/v/pyacoustix.svg?style=flat-square)](https://pypi.org/project/PyAcoustiX/)
 
 </center>
 
                                  based on Finite Element Method
                                  contact: Shaoqiwu@outlook.com
 
-**SAcouS** is pure python software based on an Finite Element libraray 'PyacoustiX' (AcoustiX in cpp version found in my git repo https://github.com/Shaoqigit/AcoustiX), mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
+**SAcouS** is pure python software based on an Finite Element libraray 'PyacoustiX' (AcoustiX in cpp version found in my git repo), mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
 
 ## Installation and Usage
 ```bash
 pip install pyacoustix
 ```
-- You can use either as a standalone library or as a part of your project. The following is a simple example to use the library:
+You can use either as a standalone library or as a part of your project. The following is a simple example to use the library:
 ```python
 from SAcouS import *
 ```
-- either used with executable with standard pyacoustix input file format .axi. To do so, you need first install the package as
+either used with executable with standard pyacoustix input file format .axi. To do so, you need first install the package as
 ```bash
 pip install .
 ```
 Then you can run the following command to execute the simulation:
 ```bash
 sacous -i input_file.axi
 ```
-- This software is also a wrap of python interpreter, so you can use it interactively with the comsole by entering:
-```bash
-sacous
-```
-you get into PyacoustiX console, where you can use the library interactively. For example:
-```bash
-Welcome to PyAcoustiX console!
-PyAcoustiX 0.9.10
-base on python 3.10.13 (main, Sep 11 2023, 13:44:35) [GCC 11.2.0] on linux
-Type "help", "copyright" or "license" for more information.
-Author: Shaoqiwu@outlook.com
-(PyAcoustiXInteractiveConsole)
->>> import numpy as np
-```
 
 ## Main special features/architecture of the library compared to other existing lib:
 > * Apart from classical Linear/Quadratic Larange polynomial, **High order (lobatto)** shape functions are supported.
 > * The element type (interpolation order of shape functions) can be **varied** on each element (mesh).
 > * **Extended elements** and double node techinique are used to deal with discontitnuity.
 > * Various common Acoustic materials are supported, including porous rigid, Limp and **Biot-up** models.
 > * FEM-**TMM** coupling is supported to model multi-layered configuration in general geometry problems.
```

### Comparing `PyAcoustiX-0.9.11/PyAcoustiX.egg-info/SOURCES.txt` & `PyAcoustiX-0.9.9/PyAcoustiX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/README.md` & `PyAcoustiX-0.9.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,46 +6,32 @@
 [![PyPi Version](https://img.shields.io/pypi/v/pyacoustix.svg?style=flat-square)](https://pypi.org/project/PyAcoustiX/)
 
 </center>
 
                                  based on Finite Element Method
                                  contact: Shaoqiwu@outlook.com
 
-**SAcouS** is pure python software based on an Finite Element libraray 'PyacoustiX' (AcoustiX in cpp version found in my git repo https://github.com/Shaoqigit/AcoustiX), mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
+**SAcouS** is pure python software based on an Finite Element libraray 'PyacoustiX' (AcoustiX in cpp version found in my git repo), mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
 
 ## Installation and Usage
 ```bash
 pip install pyacoustix
 ```
-- You can use either as a standalone library or as a part of your project. The following is a simple example to use the library:
+You can use either as a standalone library or as a part of your project. The following is a simple example to use the library:
 ```python
 from SAcouS import *
 ```
-- either used with executable with standard pyacoustix input file format .axi. To do so, you need first install the package as
+either used with executable with standard pyacoustix input file format .axi. To do so, you need first install the package as
 ```bash
 pip install .
 ```
 Then you can run the following command to execute the simulation:
 ```bash
 sacous -i input_file.axi
 ```
-- This software is also a wrap of python interpreter, so you can use it interactively with the comsole by entering:
-```bash
-sacous
-```
-you get into PyacoustiX console, where you can use the library interactively. For example:
-```bash
-Welcome to PyAcoustiX console!
-PyAcoustiX 0.9.10
-base on python 3.10.13 (main, Sep 11 2023, 13:44:35) [GCC 11.2.0] on linux
-Type "help", "copyright" or "license" for more information.
-Author: Shaoqiwu@outlook.com
-(PyAcoustiXInteractiveConsole)
->>> import numpy as np
-```
 
 ## Main special features/architecture of the library compared to other existing lib:
 > * Apart from classical Linear/Quadratic Larange polynomial, **High order (lobatto)** shape functions are supported.
 > * The element type (interpolation order of shape functions) can be **varied** on each element (mesh).
 > * **Extended elements** and double node techinique are used to deal with discontitnuity.
 > * Various common Acoustic materials are supported, including porous rigid, Limp and **Biot-up** models.
 > * FEM-**TMM** coupling is supported to model multi-layered configuration in general geometry problems.
```

### Comparing `PyAcoustiX-0.9.11/SAcouS/__main__.py` & `PyAcoustiX-0.9.9/SAcouS/__main__.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/BCs_impose.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/BCs_impose.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/assembly.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/assembly.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/basis.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/basis.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/dofhandler.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/dofhandler.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/materials.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/materials.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/mesh.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/mesh.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/physic_assembler.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/physic_assembler.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/polynomial.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/polynomial.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/postprocess.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/postprocess.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/precompute_matrices.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/precompute_matrices.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/precompute_matrices_lag.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/precompute_matrices_lag.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/quadratures.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/quadratures.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/solver.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/solver.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxfem/utilities.py` & `PyAcoustiX-0.9.9/SAcouS/acxfem/utilities.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxmor/modal_reduction.py` & `PyAcoustiX-0.9.9/SAcouS/acxmor/modal_reduction.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxmor/myEIM.py` & `PyAcoustiX-0.9.9/SAcouS/acxmor/myEIM.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxmor/myRBSolver.py` & `PyAcoustiX-0.9.9/SAcouS/acxmor/myRBSolver.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxtmm/BC_matrix.py` & `PyAcoustiX-0.9.9/SAcouS/acxtmm/BC_matrix.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxtmm/adm_assembler.py` & `PyAcoustiX-0.9.9/SAcouS/acxtmm/adm_assembler.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxtmm/adm_basis.py` & `PyAcoustiX-0.9.9/SAcouS/acxtmm/adm_basis.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/acxtmm/tmm.py` & `PyAcoustiX-0.9.9/SAcouS/acxtmm/tmm.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/interface/parser.py` & `PyAcoustiX-0.9.9/SAcouS/interface/parser.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/SAcouS/interface/sol_setup.py` & `PyAcoustiX-0.9.9/SAcouS/interface/sol_setup.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/analytical/Biot_sol.py` & `PyAcoustiX-0.9.9/analytical/Biot_sol.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/analytical/Fluid_Biot_sol.py` & `PyAcoustiX-0.9.9/analytical/Fluid_Biot_sol.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/analytical/fluid_sol.py` & `PyAcoustiX-0.9.9/analytical/fluid_sol.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.11/setup.py` & `PyAcoustiX-0.9.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='PyAcoustiX',
-    version='0.9.11',
-    description='A pure Python package/software for acoustic analysis',
+    version='0.9.9',
+    description='A Python package for acoustic analysis',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Shaoqi WU',
     author_email='shaoqiwu@outlook.com',
     url='https://github.com/Shaoqigit/PyXfem',
     entry_points={
         'console_scripts': [
@@ -30,13 +30,13 @@
     ],
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
     ],
     python_requires='>=3.8'
 )
```

