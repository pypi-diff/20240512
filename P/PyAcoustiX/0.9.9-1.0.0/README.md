# Comparing `tmp/PyAcoustiX-0.9.9.tar.gz` & `tmp/PyAcoustiX-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAcoustiX-0.9.9.tar", last modified: Sun May 12 14:12:12 2024, max compression
+gzip compressed data, was "PyAcoustiX-1.0.0.tar", last modified: Sun May  5 19:14:36 2024, max compression
```

## Comparing `PyAcoustiX-0.9.9.tar` & `PyAcoustiX-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,46 @@
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1070 2024-05-05 18:15:22.000000 PyAcoustiX-0.9.9/LICENSE
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4111 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/PKG-INFO
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4111 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/PKG-INFO
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1126 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/SOURCES.txt
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        1 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/dependency_links.txt
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       48 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/entry_points.txt
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       29 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/requires.txt
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       18 2024-05-12 14:12:12.000000 PyAcoustiX-0.9.9/PyAcoustiX.egg-info/top_level.txt
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3486 2024-05-11 20:49:00.000000 PyAcoustiX-0.9.9/README.md
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/SAcouS/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)      256 2024-05-10 19:03:16.000000 PyAcoustiX-0.9.9/SAcouS/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2982 2024-05-12 13:38:16.000000 PyAcoustiX-0.9.9/SAcouS/__main__.py
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/SAcouS/acxfem/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3518 2024-05-11 14:03:42.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/BCs_impose.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        1 2024-05-05 19:02:57.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    16704 2024-05-11 14:04:49.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/assembly.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3944 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/basis.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    13450 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/dofhandler.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    10497 2024-05-11 15:07:27.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/materials.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4557 2024-05-11 19:19:16.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/mesh.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    10565 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/physic_assembler.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     7452 2023-12-23 11:17:09.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/polynomial.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4461 2024-05-11 20:07:37.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/postprocess.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2869 2024-05-11 20:22:08.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/precompute_matrices.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3464 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/precompute_matrices_lag.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    12018 2023-12-23 19:04:28.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/quadratures.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4544 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/solver.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1658 2023-09-11 19:45:03.000000 PyAcoustiX-0.9.9/SAcouS/acxfem/utilities.py
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/SAcouS/acxmor/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:03:30.000000 PyAcoustiX-0.9.9/SAcouS/acxmor/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2510 2024-05-05 19:05:22.000000 PyAcoustiX-0.9.9/SAcouS/acxmor/modal_reduction.py
--rw-------   0 shaoqi    (1000) shaoqi    (1000)     2797 2023-12-02 20:22:21.000000 PyAcoustiX-0.9.9/SAcouS/acxmor/myEIM.py
--rw-------   0 shaoqi    (1000) shaoqi    (1000)     9494 2023-12-02 20:22:26.000000 PyAcoustiX-0.9.9/SAcouS/acxmor/myRBSolver.py
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/SAcouS/acxtmm/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1678 2023-08-25 21:15:58.000000 PyAcoustiX-0.9.9/SAcouS/acxtmm/BC_matrix.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:03:05.000000 PyAcoustiX-0.9.9/SAcouS/acxtmm/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1773 2024-05-11 14:04:55.000000 PyAcoustiX-0.9.9/SAcouS/acxtmm/adm_assembler.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    11062 2023-11-09 20:58:34.000000 PyAcoustiX-0.9.9/SAcouS/acxtmm/adm_basis.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     7867 2023-08-20 17:00:10.000000 PyAcoustiX-0.9.9/SAcouS/acxtmm/tmm.py
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/SAcouS/interface/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-10 19:03:05.000000 PyAcoustiX-0.9.9/SAcouS/interface/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     9860 2024-05-11 20:22:16.000000 PyAcoustiX-0.9.9/SAcouS/interface/parser.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4985 2024-05-12 13:11:48.000000 PyAcoustiX-0.9.9/SAcouS/interface/sol_setup.py
-drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/analytical/
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     5547 2023-07-31 19:01:24.000000 PyAcoustiX-0.9.9/analytical/Biot_sol.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     6372 2024-05-05 19:00:03.000000 PyAcoustiX-0.9.9/analytical/Fluid_Biot_sol.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:07:10.000000 PyAcoustiX-0.9.9/analytical/__init__.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3896 2024-05-11 14:04:27.000000 PyAcoustiX-0.9.9/analytical/fluid_sol.py
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       38 2024-05-12 14:12:12.069730 PyAcoustiX-0.9.9/setup.cfg
--rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1159 2024-05-12 14:07:32.000000 PyAcoustiX-0.9.9/setup.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:14:36.100409 PyAcoustiX-1.0.0/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1070 2024-05-05 18:15:22.000000 PyAcoustiX-1.0.0/LICENSE
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3300 2024-05-05 19:14:36.100409 PyAcoustiX-1.0.0/PKG-INFO
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:14:36.096409 PyAcoustiX-1.0.0/PyAcoustiX.egg-info/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3300 2024-05-05 19:14:36.000000 PyAcoustiX-1.0.0/PyAcoustiX.egg-info/PKG-INFO
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)      984 2024-05-05 19:14:36.000000 PyAcoustiX-1.0.0/PyAcoustiX.egg-info/SOURCES.txt
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        1 2024-05-05 19:14:36.000000 PyAcoustiX-1.0.0/PyAcoustiX.egg-info/dependency_links.txt
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       29 2024-05-05 19:14:36.000000 PyAcoustiX-1.0.0/PyAcoustiX.egg-info/requires.txt
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       18 2024-05-05 19:14:36.000000 PyAcoustiX-1.0.0/PyAcoustiX.egg-info/top_level.txt
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2675 2023-12-02 20:56:23.000000 PyAcoustiX-1.0.0/README.md
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:14:36.096409 PyAcoustiX-1.0.0/SAcouS/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)      232 2024-05-05 19:06:51.000000 PyAcoustiX-1.0.0/SAcouS/__init__.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:14:36.096409 PyAcoustiX-1.0.0/SAcouS/acxfem/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3512 2023-11-02 20:10:00.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/BCs_impose.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        1 2024-05-05 19:02:57.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/__init__.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    16692 2023-09-16 09:17:44.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/assembly.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3944 2024-05-05 19:05:22.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/basis.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    13450 2024-05-05 19:05:22.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/dofhandler.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     9640 2023-09-02 09:51:40.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/materials.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4438 2023-11-14 21:37:38.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/mesh.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    10565 2024-05-05 19:05:22.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/physic_assembler.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     7452 2023-12-23 11:17:09.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/polynomial.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3364 2023-11-22 22:03:10.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/postprocess.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2867 2024-05-05 19:10:57.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/precompute_matrices.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3464 2024-05-05 19:05:22.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/precompute_matrices_lag.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    12018 2023-12-23 19:04:28.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/quadratures.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     4544 2024-05-05 19:05:22.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/solver.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1658 2023-09-11 19:45:03.000000 PyAcoustiX-1.0.0/SAcouS/acxfem/utilities.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:14:36.096409 PyAcoustiX-1.0.0/SAcouS/acxmor/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:03:30.000000 PyAcoustiX-1.0.0/SAcouS/acxmor/__init__.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     2510 2024-05-05 19:05:22.000000 PyAcoustiX-1.0.0/SAcouS/acxmor/modal_reduction.py
+-rw-------   0 shaoqi    (1000) shaoqi    (1000)     2797 2023-12-02 20:22:21.000000 PyAcoustiX-1.0.0/SAcouS/acxmor/myEIM.py
+-rw-------   0 shaoqi    (1000) shaoqi    (1000)     9494 2023-12-02 20:22:26.000000 PyAcoustiX-1.0.0/SAcouS/acxmor/myRBSolver.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:14:36.096409 PyAcoustiX-1.0.0/SAcouS/acxtmm/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1678 2023-08-25 21:15:58.000000 PyAcoustiX-1.0.0/SAcouS/acxtmm/BC_matrix.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:03:05.000000 PyAcoustiX-1.0.0/SAcouS/acxtmm/__init__.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1767 2024-05-05 19:05:22.000000 PyAcoustiX-1.0.0/SAcouS/acxtmm/adm_assembler.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)    11062 2023-11-09 20:58:34.000000 PyAcoustiX-1.0.0/SAcouS/acxtmm/adm_basis.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     7867 2023-08-20 17:00:10.000000 PyAcoustiX-1.0.0/SAcouS/acxtmm/tmm.py
+drwxrwxr-x   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:14:36.100409 PyAcoustiX-1.0.0/analytical/
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     5547 2023-07-31 19:01:24.000000 PyAcoustiX-1.0.0/analytical/Biot_sol.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     6372 2024-05-05 19:00:03.000000 PyAcoustiX-1.0.0/analytical/Fluid_Biot_sol.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)        0 2024-05-05 19:07:10.000000 PyAcoustiX-1.0.0/analytical/__init__.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     3872 2023-08-10 20:12:46.000000 PyAcoustiX-1.0.0/analytical/fluid_sol.py
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)       38 2024-05-05 19:14:36.100409 PyAcoustiX-1.0.0/setup.cfg
+-rw-rw-r--   0 shaoqi    (1000) shaoqi    (1000)     1000 2024-05-05 18:07:34.000000 PyAcoustiX-1.0.0/setup.py
```

### Comparing `PyAcoustiX-0.9.9/LICENSE` & `PyAcoustiX-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/PKG-INFO` & `PyAcoustiX-1.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAcoustiX
-Version: 0.9.9
+Version: 1.0.0
 Summary: A Python package for acoustic analysis
 Home-page: https://github.com/Shaoqigit/PyXfem
 Author: Shaoqi WU
 Author-email: shaoqiwu@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,62 +14,38 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **S**imple **A**coustic **S**imulator(SAcouS)
 [comment]: <> ( - AcoustiX based Sound simulation library)
-[comment]: <> ( - put following badges centre)
-<center>
-  
-[![PyPi Version](https://img.shields.io/pypi/v/pyacoustix.svg?style=flat-square)](https://pypi.org/project/PyAcoustiX/)
-
-</center>
-
-                                 based on Finite Element Method
-                                 contact: Shaoqiwu@outlook.com
-
-**SAcouS** is pure python software based on an Finite Element libraray 'PyacoustiX' (AcoustiX in cpp version found in my git repo), mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
-
-## Installation and Usage
-```bash
-pip install pyacoustix
-```
-You can use either as a standalone library or as a part of your project. The following is a simple example to use the library:
-```python
-from SAcouS import *
-```
-either used with executable with standard pyacoustix input file format .axi. To do so, you need first install the package as
-```bash
-pip install .
-```
-Then you can run the following command to execute the simulation:
-```bash
-sacous -i input_file.axi
-```
+
+                   based on Finite Element Method
+                    contact: Shaoqiwu@outlook.com
+
+**AcoustiX** is Finite Element (FEM) modular Library, mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
 
 ## Main special features/architecture of the library compared to other existing lib:
-> * Apart from classical Linear/Quadratic Larange polynomial, **High order (lobatto)** shape functions are supported.
-> * The element type (interpolation order of shape functions) can be **varied** on each element (mesh).
-> * **Extended elements** and double node techinique are used to deal with discontitnuity.
-> * Various common Acoustic materials are supported, including porous rigid, Limp and **Biot-up** models.
-> * FEM-**TMM** coupling is supported to model multi-layered configuration in general geometry problems.
+* Apart from classical Linear/Quadratic Larange polynomial, **High order (lobatto)** shape functions are supported
+* The element type (interpolation order of shape functions) can be **varied** on each element (mesh)
+* **Extended elements** and double node techinique are used to deal with discontitnuity
+* Various common Acoustic materials are supported, including porous rigid, Limp and **Biot-up** models.
+* FEM-**TMM** coupling is supported to model multi-layered configuration in general geometry problems
 
 
 ### Up to this moment:
 * High order lobatto shape function supported (up to $p=4$)
 * JCA and Limp model to account for porous acoustic materials
 * **Biot equation** modeling for poro-elastic materials
 * Impedence boundary condition supported
 * Weakly enforced essential boundary condition (penalty method and **Nitche's method**)
 * Biot UP and Fluid coupling model (implemented but not fully validated)
 * Modal domain reduction method
 
 ### To do list
-* update to python 3.11
 * MoR for damped systems (RB+EIM algorithme for porous materials)
 * Perfect Matched Layer (PML) for free field boundary condition
 * Infinite Element for free field boundary condition
 * Finite Admittance Method (FAM) for high precision multi-layered configuration
 * TMM embeded for multi-layered configuration
 * higher order shape function and integration ($p=10$)
```

### Comparing `PyAcoustiX-0.9.9/PyAcoustiX.egg-info/PKG-INFO` & `PyAcoustiX-1.0.0/PyAcoustiX.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAcoustiX
-Version: 0.9.9
+Version: 1.0.0
 Summary: A Python package for acoustic analysis
 Home-page: https://github.com/Shaoqigit/PyXfem
 Author: Shaoqi WU
 Author-email: shaoqiwu@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,62 +14,38 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **S**imple **A**coustic **S**imulator(SAcouS)
 [comment]: <> ( - AcoustiX based Sound simulation library)
-[comment]: <> ( - put following badges centre)
-<center>
-  
-[![PyPi Version](https://img.shields.io/pypi/v/pyacoustix.svg?style=flat-square)](https://pypi.org/project/PyAcoustiX/)
-
-</center>
-
-                                 based on Finite Element Method
-                                 contact: Shaoqiwu@outlook.com
-
-**SAcouS** is pure python software based on an Finite Element libraray 'PyacoustiX' (AcoustiX in cpp version found in my git repo), mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
-
-## Installation and Usage
-```bash
-pip install pyacoustix
-```
-You can use either as a standalone library or as a part of your project. The following is a simple example to use the library:
-```python
-from SAcouS import *
-```
-either used with executable with standard pyacoustix input file format .axi. To do so, you need first install the package as
-```bash
-pip install .
-```
-Then you can run the following command to execute the simulation:
-```bash
-sacous -i input_file.axi
-```
+
+                   based on Finite Element Method
+                    contact: Shaoqiwu@outlook.com
+
+**AcoustiX** is Finite Element (FEM) modular Library, mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
 
 ## Main special features/architecture of the library compared to other existing lib:
-> * Apart from classical Linear/Quadratic Larange polynomial, **High order (lobatto)** shape functions are supported.
-> * The element type (interpolation order of shape functions) can be **varied** on each element (mesh).
-> * **Extended elements** and double node techinique are used to deal with discontitnuity.
-> * Various common Acoustic materials are supported, including porous rigid, Limp and **Biot-up** models.
-> * FEM-**TMM** coupling is supported to model multi-layered configuration in general geometry problems.
+* Apart from classical Linear/Quadratic Larange polynomial, **High order (lobatto)** shape functions are supported
+* The element type (interpolation order of shape functions) can be **varied** on each element (mesh)
+* **Extended elements** and double node techinique are used to deal with discontitnuity
+* Various common Acoustic materials are supported, including porous rigid, Limp and **Biot-up** models.
+* FEM-**TMM** coupling is supported to model multi-layered configuration in general geometry problems
 
 
 ### Up to this moment:
 * High order lobatto shape function supported (up to $p=4$)
 * JCA and Limp model to account for porous acoustic materials
 * **Biot equation** modeling for poro-elastic materials
 * Impedence boundary condition supported
 * Weakly enforced essential boundary condition (penalty method and **Nitche's method**)
 * Biot UP and Fluid coupling model (implemented but not fully validated)
 * Modal domain reduction method
 
 ### To do list
-* update to python 3.11
 * MoR for damped systems (RB+EIM algorithme for porous materials)
 * Perfect Matched Layer (PML) for free field boundary condition
 * Infinite Element for free field boundary condition
 * Finite Admittance Method (FAM) for high precision multi-layered configuration
 * TMM embeded for multi-layered configuration
 * higher order shape function and integration ($p=10$)
```

### Comparing `PyAcoustiX-0.9.9/PyAcoustiX.egg-info/SOURCES.txt` & `PyAcoustiX-1.0.0/PyAcoustiX.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 LICENSE
 README.md
 setup.py
 PyAcoustiX.egg-info/PKG-INFO
 PyAcoustiX.egg-info/SOURCES.txt
 PyAcoustiX.egg-info/dependency_links.txt
-PyAcoustiX.egg-info/entry_points.txt
 PyAcoustiX.egg-info/requires.txt
 PyAcoustiX.egg-info/top_level.txt
 SAcouS/__init__.py
-SAcouS/__main__.py
 SAcouS/acxfem/BCs_impose.py
 SAcouS/acxfem/__init__.py
 SAcouS/acxfem/assembly.py
 SAcouS/acxfem/basis.py
 SAcouS/acxfem/dofhandler.py
 SAcouS/acxfem/materials.py
 SAcouS/acxfem/mesh.py
@@ -29,14 +27,11 @@
 SAcouS/acxmor/myEIM.py
 SAcouS/acxmor/myRBSolver.py
 SAcouS/acxtmm/BC_matrix.py
 SAcouS/acxtmm/__init__.py
 SAcouS/acxtmm/adm_assembler.py
 SAcouS/acxtmm/adm_basis.py
 SAcouS/acxtmm/tmm.py
-SAcouS/interface/__init__.py
-SAcouS/interface/parser.py
-SAcouS/interface/sol_setup.py
 analytical/Biot_sol.py
 analytical/Fluid_Biot_sol.py
 analytical/__init__.py
 analytical/fluid_sol.py
```

### Comparing `PyAcoustiX-0.9.9/README.md` & `PyAcoustiX-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,33 @@
 # **S**imple **A**coustic **S**imulator(SAcouS)
 [comment]: <> ( - AcoustiX based Sound simulation library)
-[comment]: <> ( - put following badges centre)
-<center>
-  
-[![PyPi Version](https://img.shields.io/pypi/v/pyacoustix.svg?style=flat-square)](https://pypi.org/project/PyAcoustiX/)
-
-</center>
-
-                                 based on Finite Element Method
-                                 contact: Shaoqiwu@outlook.com
-
-**SAcouS** is pure python software based on an Finite Element libraray 'PyacoustiX' (AcoustiX in cpp version found in my git repo), mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
-
-## Installation and Usage
-```bash
-pip install pyacoustix
-```
-You can use either as a standalone library or as a part of your project. The following is a simple example to use the library:
-```python
-from SAcouS import *
-```
-either used with executable with standard pyacoustix input file format .axi. To do so, you need first install the package as
-```bash
-pip install .
-```
-Then you can run the following command to execute the simulation:
-```bash
-sacous -i input_file.axi
-```
+
+                   based on Finite Element Method
+                    contact: Shaoqiwu@outlook.com
+
+**AcoustiX** is Finite Element (FEM) modular Library, mainly designed for Acoustic simulation but can be used (extended) to other physics. This labrary aims at providing the simplest, clearest and easily conprehensive tool to use FEM for purpose of research, education or industry prototype.
 
 ## Main special features/architecture of the library compared to other existing lib:
-> * Apart from classical Linear/Quadratic Larange polynomial, **High order (lobatto)** shape functions are supported.
-> * The element type (interpolation order of shape functions) can be **varied** on each element (mesh).
-> * **Extended elements** and double node techinique are used to deal with discontitnuity.
-> * Various common Acoustic materials are supported, including porous rigid, Limp and **Biot-up** models.
-> * FEM-**TMM** coupling is supported to model multi-layered configuration in general geometry problems.
+* Apart from classical Linear/Quadratic Larange polynomial, **High order (lobatto)** shape functions are supported
+* The element type (interpolation order of shape functions) can be **varied** on each element (mesh)
+* **Extended elements** and double node techinique are used to deal with discontitnuity
+* Various common Acoustic materials are supported, including porous rigid, Limp and **Biot-up** models.
+* FEM-**TMM** coupling is supported to model multi-layered configuration in general geometry problems
 
 
 ### Up to this moment:
 * High order lobatto shape function supported (up to $p=4$)
 * JCA and Limp model to account for porous acoustic materials
 * **Biot equation** modeling for poro-elastic materials
 * Impedence boundary condition supported
 * Weakly enforced essential boundary condition (penalty method and **Nitche's method**)
 * Biot UP and Fluid coupling model (implemented but not fully validated)
 * Modal domain reduction method
 
 ### To do list
-* update to python 3.11
 * MoR for damped systems (RB+EIM algorithme for porous materials)
 * Perfect Matched Layer (PML) for free field boundary condition
 * Infinite Element for free field boundary condition
 * Finite Admittance Method (FAM) for high precision multi-layered configuration
 * TMM embeded for multi-layered configuration
 * higher order shape function and integration ($p=10$)
```

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/BCs_impose.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/BCs_impose.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.left_hand_side += C_damp
         return C_damp
 
         
     def apply_nature_bc(self, nature_bc, var=None):
         dof_index = self.mesh2dof(nature_bc['position'], var)
 
-        if nature_bc['type']=='fluid_velocity':
+        if nature_bc['type']=='velocity':
             self.right_hand_side[dof_index] += -nature_bc['value']/(1j*self.omega)
         elif nature_bc['type']=='total_displacement':
             self.right_hand_side[dof_index] += nature_bc['value']
         elif nature_bc['type']=='solid_stress':
             self.right_hand_side[dof_index] += nature_bc['value']
         else:
             print("Nature BC type not supported")
```

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/assembly.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/assembly.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     
     def assemble_nature_bc(self, nature_bc):
         """
         nature_bc: dict of nature boundary conditions
         return the global vector contributed from nature boundary conditions
         """
         F = np.zeros(self.nb_dofs, dtype=self.dtype)
-        if nature_bc['type']=='fluid_velocity':
+        if nature_bc['type']=='velocity':
             F[nature_bc['position']] = 1j * self.omega * nature_bc['value']
         elif nature_bc['type']=='total_displacement':
             F[nature_bc['position']] += nature_bc['value']
         else:
             print("Nature BC type not supported")
 
         return F
@@ -375,15 +375,15 @@
     
     def apply_nature_bc(self, nature_bc, var=None):
         dof_index = self.dof_handler.mesh2dof(nature_bc['position'], var)
         if self.F is None:
             right_hand_side = np.zeros(self.nb_dofs, dtype=self.dtype)
         else:
             right_hand_side = self.F
-        if nature_bc['type']=='fluid_velocity':
+        if nature_bc['type']=='velocity':
             right_hand_side[dof_index] += 1j * self.omega * nature_bc['value']
         elif nature_bc['type']=='total_displacement':
             right_hand_side[dof_index] += nature_bc['value']
         else:
             print("Nature BC type not supported")
 
         return right_hand_side
```

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/basis.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/basis.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/dofhandler.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/dofhandler.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/materials.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/materials.py`

 * *Files 6% similar despite different names*

```diff
@@ -288,33 +288,8 @@
         self.rho_f = self.rho_eq_til
         self.c_f = self.c_eq_til
         self.Z_f = self.rho_f*self.c_f
         self.K_f = self.K_eq_til
 
 
 
-# TODO: correct Limp and BiotMaterial class
-
-# write a class to get differennt material class according to the material type
-class MaterialFactory:
-    """material factory class
-    """
-    def __init__(self):
-        pass
-
-    @staticmethod
-    def create_material(material_type, name, *args):
-        if material_type == 'FLUID':
-            return Fluid(name, *args)
-        elif material_type == 'AIR':
-            return Air(name, *args)
-        elif material_type == 'RIGID_POROUS':
-            return EquivalentFluid(name, *args)
-        elif material_type == 'LIMP_POROUS':
-            return LimpPorousMaterial(name, *args)
-        elif material_type == 'ELASTIC':
-            return ElasticMaterial(name, *args)
-        elif material_type == 'PORO_ELASTIC':
-            return PoroElasticMaterial(name, *args)
-        else:
-            raise ValueError('The material type is not defined')
-
+# TODO: correct Limp and BiotMaterial class
```

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/mesh.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/mesh.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,18 +49,14 @@
     def get_mesh(self):
         """dict of element number and nodes coordinates"""
         elems = {}
         for i in range(len(self.elem_connect)):
             elems[i] = np.array([self.nodes[i], self.nodes[i+1]])
         return elems
     
-    def get_min_size(self):
-        """return minimum size of elements"""
-        return min(np.diff(self.nodes))
-    
     def node2elem(self, node):
         """return element number from node number"""
         for i in range(len(self.elem_connect)):
             if node in self.elem_connect[i]:
                 return i
         raise ValueError("node not in mesh")
```

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/physic_assembler.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/physic_assembler.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/polynomial.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/polynomial.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/postprocess.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/postprocess.py`

 * *Files 26% similar despite different names*

```diff
@@ -57,31 +57,22 @@
         return l2_error
 
 class PostProcessField(BasePostProcess):
 
     def __init__(self, x_nodes, title, quantity='Pressure', unit='Pa'):
         super().__init__(title)
         self.x_nodes = x_nodes
-        self.quantity = quantity
-        self.unit = unit
+        self.set_figure('Position(m)', quantity+'('+unit+')')
 
     
-    def plot_sol(self, *sols, file_name=None, save=False):
-        self.set_figure('Position(m)', self.quantity+'('+self.unit+')')
+    def plot_sol(self, *sols):
         for sol in sols:
             self.ax.plot(self.x_nodes, sol[0], label=sol[1], linestyle=sol[2])
         
         self.ax.legend()
-        if save:
-            plt.savefig(file_name)
-
-    def save_sol(self, *sols, file_name):
-        for sol in sols:
-            np.savetxt(file_name, sol[0])
-        
 
     def display_layers(self, *layers_pos):
         for pos in layers_pos:
             self.ax.axvline(x=pos, ls='--', c='k')
 
 
 
@@ -89,51 +80,25 @@
 # frequency response function postprocessor
 class PostProcessFRF(BasePostProcess):  
 
     def __init__(self, freqs, title, acoustic_indicator='SPL'):
         super().__init__(title)
         self.freqs = freqs
         self.operator=acoustic_indicator
-        self.unit = ''
+        unit = ''
         if acoustic_indicator == 'SPL':
-            self.unit = 'dB'
-        
+            unit = 'dB'
+        self.set_figure('Frequency(Hz)', acoustic_indicator+f'({unit})')
 
     def get_operator(self):
         if self.operator == 'SPL(dB)':
             return lambda x: 20*np.log10(np.abs(x))
         elif self.operator == 'SPL(dB) - 2':
             print("Warning: SPL(dB) - 2 is not implemented yet!")
 
 
-    def plot_sol(self, *sols, save=False, file_name=None):
-        self.set_figure('Frequency(Hz)', self.operator+f'({self.unit})')
+    def plot_sol(self, *sols):
         for sol in sols:
             sol_r = self.get_operator()(sol[0])
             self.ax.plot(self.freqs, sol_r, label=sol[1], linestyle=sol[2])
         
         self.ax.legend()
-        if save:
-            plt.savefig(file_name)
-
-    def save_sol(self, *sols, file_name):
-        """
-        output result as a txt file, res.txt
-        {
-        // header, PyacoustiX FRF result file
-        // Frequency(Hz) SPL(dB)
-        100 20.1
-        200 30.7
-        300 40.4
-        400 50.1
-        500 48.7
-        }
-        """
-        with open(file_name, 'w') as file:
-            # write the header
-            file.write('// PyacoustiX FRF result file\n')
-            file.write(f'Frequency(Hz) {self.operator}({self.unit})\n')
-            for sol in sols:
-                file.write(f'\n{sol[1]}')
-                sol_r = self.get_operator()(sol[0])
-                for i in range(len(sol_r)):
-                    file.write(f'{self.freqs[i]} {sol_r[i]}\n')
```

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/precompute_matrices.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/precompute_matrices.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 Ce1Do4 = np.zeros((5,5))
 compute_matrix(Ke1Do4, Me1Do4, Ce1Do4, order)
 
 Ke1D = [Ke1Do1, Ke1Do2, Ke1Do3, Ke1Do4]
 Me1D = [Me1Do1, Me1Do2, Me1Do3, Me1Do4]
 Ce1D = [Ce1Do1, Ce1Do2, Ce1Do3, Ce1Do4]
 
-# print(Ke1Do1)
+print(Ke1Do1)
 # print(Me1Do1)
 # print(Ke1Do2)
 # print(Me1Do2)
 # print(Ke1Do3)
 # print(Me1Do3)
 # print(Ke1Do4)
 # print(Me1Do4)
```

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/precompute_matrices_lag.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/precompute_matrices_lag.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/quadratures.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/quadratures.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/solver.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/solver.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxfem/utilities.py` & `PyAcoustiX-1.0.0/SAcouS/acxfem/utilities.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxmor/modal_reduction.py` & `PyAcoustiX-1.0.0/SAcouS/acxmor/modal_reduction.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxmor/myEIM.py` & `PyAcoustiX-1.0.0/SAcouS/acxmor/myEIM.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxmor/myRBSolver.py` & `PyAcoustiX-1.0.0/SAcouS/acxmor/myRBSolver.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxtmm/BC_matrix.py` & `PyAcoustiX-1.0.0/SAcouS/acxtmm/BC_matrix.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxtmm/adm_assembler.py` & `PyAcoustiX-1.0.0/SAcouS/acxtmm/adm_assembler.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                 adm.admittance()
             self.global_adm[i:i+2, i:i+2] += adm.adm
             
         return self.global_adm.tocsr()
     
     def assemble_nature_bc(self, nature_bc):
         F = np.zeros(self.nb_dofs, dtype=self.dtype)
-        if nature_bc['type']=='fluid_velocity':
+        if nature_bc['type']=='velocity':
             F[nature_bc['position']] = -1*nature_bc['value']/(1j*self.omega)
         elif nature_bc['type'] == 'total_displacement':
             F[nature_bc['position']] = nature_bc['value']
         else:
             print("Nature BC type not supported")
 
         return F
```

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxtmm/adm_basis.py` & `PyAcoustiX-1.0.0/SAcouS/acxtmm/adm_basis.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/SAcouS/acxtmm/tmm.py` & `PyAcoustiX-1.0.0/SAcouS/acxtmm/tmm.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/analytical/Biot_sol.py` & `PyAcoustiX-1.0.0/analytical/Biot_sol.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/analytical/Fluid_Biot_sol.py` & `PyAcoustiX-1.0.0/analytical/Fluid_Biot_sol.py`

 * *Files identical despite different names*

### Comparing `PyAcoustiX-0.9.9/analytical/fluid_sol.py` & `PyAcoustiX-1.0.0/analytical/fluid_sol.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class ImpedenceKundltTube():
 
     def __init__(self, mesh, *args) -> None:
         self.mesh = mesh
         self.mat = args[0]
         self.omega = args[1]
         self.nature_bc = args[2]
-        assert(self.nature_bc['type'] == 'fluid_velocity')
+        assert(self.nature_bc['type'] == 'velocity')
         self.impedence_bc = args[3]
         assert(self.impedence_bc['type'] == 'impedence')
         self.analytical_field()
 
     def analytical_field(self):
         Z_0 = self.mat.Z_f
         Up = self.nature_bc['value']
@@ -36,15 +36,15 @@
     
     def __init__(self, mesh, *args) -> None:
         self.mesh = mesh
         self.mat1 = args[0]
         self.mat2 = args[1]
         self.omega = args[2]
         self.bc = args[3]
-        assert(self.bc['type'] == 'fluid_velocity')
+        assert(self.bc['type'] == 'velocity')
         self.analytical_field()
 
     def analytical_field(self):
         l1, l2 = abs(self.mesh.nodes[0]), abs(self.mesh.nodes[-1])
         l_a = l1
         l_eq= l2
         v_0 = self.bc['value']
@@ -77,17 +77,17 @@
         
 
     def sol_on_nodes(self, ana_sol, sol_type):
         for i, x in enumerate(self.mesh.nodes):
             if x <= 0:
                 if sol_type == 'pressure':
                     sol = self.P_analy[0](x) 
-                elif sol_type=='fluid_velocity':
+                elif sol_type=='velocity':
                     sol = self.v_analy[0](x)
             elif x >= 0:
                 if sol_type == 'pressure':
                     sol = self.P_analy[1](x)
-                elif sol_type=='fluid_velocity':
+                elif sol_type=='velocity':
                     sol = self.v_analy[1](x)
 
             ana_sol[i] = sol
         return ana_sol
```

### Comparing `PyAcoustiX-0.9.9/setup.py` & `PyAcoustiX-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='PyAcoustiX',
-    version='0.9.9',
+    version='1.0.0',
     description='A Python package for acoustic analysis',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Shaoqi WU',
     author_email='shaoqiwu@outlook.com',
     url='https://github.com/Shaoqigit/PyXfem',
-    entry_points={
-        'console_scripts': [
-            'sacous = SAcouS.__main__:main',
-        ],
-    },
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'numba',
         # Add any other dependencies here
     ],
-    install_optional=[
-        'pymls',
-    ],
-
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

