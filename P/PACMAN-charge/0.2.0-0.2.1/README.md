# Comparing `tmp/PACMAN-charge-0.2.0.tar.gz` & `tmp/PACMAN-charge-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PACMAN-charge-0.2.0.tar", last modified: Wed May  8 01:49:10 2024, max compression
+gzip compressed data, was "PACMAN-charge-0.2.1.tar", last modified: Sun May 12 12:13:38 2024, max compression
```

## Comparing `PACMAN-charge-0.2.0.tar` & `PACMAN-charge-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:49:10.650687 PACMAN-charge-0.2.0/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.2.0/LICENSE
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:49:10.532688 PACMAN-charge-0.2.0/PACMANCharge/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.2.0/PACMANCharge/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.2.0/PACMANCharge/atom_init.json
--rwxrwxrwx   0 root         (0) root         (0)    25766 2024-05-07 08:18:34.000000 PACMAN-charge-0.2.0/PACMANCharge/pmcharge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:49:10.602688 PACMAN-charge-0.2.0/PACMAN_charge.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3189 2024-05-08 01:49:10.000000 PACMAN-charge-0.2.0/PACMAN_charge.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      318 2024-05-08 01:49:10.000000 PACMAN-charge-0.2.0/PACMAN_charge.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-08 01:49:10.000000 PACMAN-charge-0.2.0/PACMAN_charge.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-08 01:49:10.000000 PACMAN-charge-0.2.0/PACMAN_charge.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-08 01:49:10.000000 PACMAN-charge-0.2.0/PACMAN_charge.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3189 2024-05-08 01:49:10.648688 PACMAN-charge-0.2.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2799 2024-05-08 01:47:58.000000 PACMAN-charge-0.2.0/README.md
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-08 01:49:10.651689 PACMAN-charge-0.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      986 2024-05-08 01:48:48.000000 PACMAN-charge-0.2.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:49:10.630688 PACMAN-charge-0.2.0/test/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.2.0/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      134 2024-05-06 03:24:19.000000 PACMAN-charge-0.2.0/test/test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 12:13:38.933105 PACMAN-charge-0.2.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2024-03-25 02:54:44.000000 PACMAN-charge-0.2.1/LICENSE
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 12:13:38.817096 PACMAN-charge-0.2.1/PACMANCharge/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-29 12:12:36.000000 PACMAN-charge-0.2.1/PACMANCharge/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    28392 2024-01-10 01:22:23.000000 PACMAN-charge-0.2.1/PACMANCharge/atom_init.json
+-rwxrwxrwx   0 root         (0) root         (0)    25766 2024-05-07 08:18:34.000000 PACMAN-charge-0.2.1/PACMANCharge/pmcharge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 12:13:38.888097 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3191 2024-05-12 12:13:38.000000 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      318 2024-05-12 12:13:38.000000 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-12 12:13:38.000000 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      121 2024-05-12 12:13:38.000000 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-05-12 12:13:38.000000 PACMAN-charge-0.2.1/PACMAN_charge.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3191 2024-05-12 12:13:38.931105 PACMAN-charge-0.2.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2801 2024-05-12 12:13:19.000000 PACMAN-charge-0.2.1/README.md
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-05-12 12:13:38.934105 PACMAN-charge-0.2.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      986 2024-05-12 12:12:57.000000 PACMAN-charge-0.2.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 12:13:38.916105 PACMAN-charge-0.2.1/test/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-25 03:31:56.000000 PACMAN-charge-0.2.1/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      134 2024-05-06 03:24:19.000000 PACMAN-charge-0.2.1/test/test.py
```

### Comparing `PACMAN-charge-0.2.0/LICENSE` & `PACMAN-charge-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.2.0/PACMANCharge/atom_init.json` & `PACMAN-charge-0.2.1/PACMANCharge/atom_init.json`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.2.0/PACMANCharge/pmcharge.py` & `PACMAN-charge-0.2.1/PACMANCharge/pmcharge.py`

 * *Files identical despite different names*

### Comparing `PACMAN-charge-0.2.0/PACMAN_charge.egg-info/PKG-INFO` & `PACMAN-charge-0.2.1/PACMAN_charge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.2.0
+Version: 0.2.1
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 [![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
 
 
 # Usage
 
 ```sh      
 from PACMANCharge import pmcharge
-PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
+pmcharge.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
 ```
 
 * cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
 * charge-type (default: DDE6): DDEC6, Bader or CM5                                        
 * digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
 * atom-type (default: False): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
 * neutral (default: False): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.
```

### Comparing `PACMAN-charge-0.2.0/PKG-INFO` & `PACMAN-charge-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PACMAN-charge
-Version: 0.2.0
+Version: 0.2.1
 Summary: Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)
 Home-page: https://github.com/sxm13/PACMAN
 Author: Guobin Zhao
 Author-email: sxmzhaogb@gmai.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 [![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
 
 
 # Usage
 
 ```sh      
 from PACMANCharge import pmcharge
-PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
+pmcharge.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
 ```
 
 * cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
 * charge-type (default: DDE6): DDEC6, Bader or CM5                                        
 * digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
 * atom-type (default: False): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
 * neutral (default: False): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.
```

### Comparing `PACMAN-charge-0.2.0/README.md` & `PACMAN-charge-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [![Requires Python 3.9](https://img.shields.io/badge/Python-3.9-blue.svg?logo=python&logoColor=white)](https://python.org/downloads) [![Zenodo](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.10822403-blue)](https://doi.org/10.5281/zenodo.10822403)  [![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/sxm13/PACMAN/LICENSE.txt) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sxmzhaogb@gmail.com) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)]() [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)]()          
 
 
 # Usage
 
 ```sh      
 from PACMANCharge import pmcharge
-PACMaN.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
+pmcharge.predict(cif_file="./test/Cu-BTC.cif",charge_type="DDEC6",digits=6,atom_type=False,neutral=False)
 ```
 
 * cif_file: cif file (without partial atomic charges) **[cif path]**                                                            
 * charge-type (default: DDE6): DDEC6, Bader or CM5                                        
 * digits (default: 6): number of decimal places to print for partial atomic charges. ML models were trained on a 6-digit dataset.                                                                     
 * atom-type (default: False): keep the same partial atomic charge for the same atom types (based on the similarity of partial atomic charges up to 2 decimal places).                                                         
 * neutral (default: False): keep the net charge is zero. We use "mean" method to neuralize the system where the excess charges are equally distributed across all atoms.
```

### Comparing `PACMAN-charge-0.2.0/setup.py` & `PACMAN-charge-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from setuptools import setup, find_packages
 
 setup(
     name="PACMAN-charge",
-    version="0.2.0",
+    version="0.2.1",
     packages=find_packages(),
     description="Partial Atomic Charges for Porous Materials based on Graph Convolutional Neural Network (PACMAN)",
     author="Guobin Zhao",
     author_email="sxmzhaogb@gmai.com",
     url="https://github.com/sxm13/PACMAN",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

