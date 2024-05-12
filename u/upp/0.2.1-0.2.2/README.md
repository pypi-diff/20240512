# Comparing `tmp/upp-0.2.1.tar.gz` & `tmp/upp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upp-0.2.1.tar", last modified: Mon Apr  8 15:37:55 2024, max compression
+gzip compressed data, was "upp-0.2.2.tar", last modified: Sun May 12 12:54:25 2024, max compression
```

## Comparing `upp-0.2.1.tar` & `upp-0.2.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.832385 upp-0.2.1/
--rw-r--r--   0 samir     (1000) samir     (1000)     1225 2021-01-04 17:42:38.000000 upp-0.2.1/.gitignore
--rw-r--r--   0 samir     (1000) samir     (1000)    35149 2019-02-20 19:25:43.000000 upp-0.2.1/LICENSE
--rw-r--r--   0 samir     (1000) samir     (1000)     7956 2024-04-08 15:37:55.832385 upp-0.2.1/PKG-INFO
--rw-r--r--   0 samir     (1000) samir     (1000)     7252 2024-03-25 18:35:38.000000 upp-0.2.1/README.md
--rw-r--r--   0 samir     (1000) samir     (1000)       38 2024-04-08 15:37:55.835718 upp-0.2.1/setup.cfg
--rw-r--r--   0 samir     (1000) samir     (1000)     1054 2024-04-08 15:16:53.000000 upp-0.2.1/setup.py
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.829051 upp-0.2.1/src/
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.832385 upp-0.2.1/src/upp/
--rw-r--r--   0 samir     (1000) samir     (1000)        0 2020-03-27 07:44:19.000000 upp-0.2.1/src/upp/__init__.py
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.832385 upp-0.2.1/src/upp/atom_gen/
--rw-r--r--   0 samir     (1000) samir     (1000)     3582 2024-03-25 15:46:08.000000 upp-0.2.1/src/upp/atom_gen/README.md
--rw-r--r--   0 samir     (1000) samir     (1000)        0 2021-08-15 09:31:23.000000 upp-0.2.1/src/upp/atom_gen/__init__.py
--rw-r--r--   0 samir     (1000) samir     (1000)     8599 2024-03-25 16:25:09.000000 upp-0.2.1/src/upp/atom_gen/atombios.py
--rw-r--r--   0 samir     (1000) samir     (1000)    30254 2024-03-25 16:25:20.000000 upp-0.2.1/src/upp/atom_gen/pptable_v1_0.py
--rw-r--r--   0 samir     (1000) samir     (1000)    31364 2024-04-01 12:39:06.000000 upp-0.2.1/src/upp/atom_gen/smu_v11_0_7_navi20.py
--rw-rw-r--   0 samir     (1000) samir     (1000)    25359 2024-03-25 16:25:40.000000 upp-0.2.1/src/upp/atom_gen/smu_v11_0_navi10.py
--rw-r--r--   0 samir     (1000) samir     (1000)    39447 2024-03-25 16:25:49.000000 upp-0.2.1/src/upp/atom_gen/smu_v13_0_7_navi30.py
--rw-rw-r--   0 samir     (1000) samir     (1000)    30177 2024-03-25 16:25:31.000000 upp-0.2.1/src/upp/atom_gen/vega10_pptable.py
--rw-rw-r--   0 samir     (1000) samir     (1000)    22595 2024-03-25 16:25:35.000000 upp-0.2.1/src/upp/atom_gen/vega20_pptable.py
--rw-r--r--   0 samir     (1000) samir     (1000)    38974 2024-04-08 15:10:39.000000 upp-0.2.1/src/upp/decode.py
--rwxr-xr-x   0 samir     (1000) samir     (1000)    16881 2024-03-25 18:27:25.000000 upp-0.2.1/src/upp/upp.py
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.832385 upp-0.2.1/src/upp.egg-info/
--rw-r--r--   0 samir     (1000) samir     (1000)     7956 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/PKG-INFO
--rw-r--r--   0 samir     (1000) samir     (1000)     1231 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/SOURCES.txt
--rw-r--r--   0 samir     (1000) samir     (1000)        1 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/dependency_links.txt
--rw-r--r--   0 samir     (1000) samir     (1000)       37 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/entry_points.txt
--rw-r--r--   0 samir     (1000) samir     (1000)       17 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/requires.txt
--rw-r--r--   0 samir     (1000) samir     (1000)       17 2024-04-08 15:37:55.000000 upp-0.2.1/src/upp.egg-info/top_level.txt
-drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-04-08 15:37:55.832385 upp-0.2.1/test/
--rw-rw-r--   0 samir     (1000) samir     (1000)     8888 2021-06-03 18:56:29.000000 upp-0.2.1/test/AMD.RX480.8192.160603.rom.dump
--rw-rw-r--   0 samir     (1000) samir     (1000)    30539 2024-04-08 14:54:40.000000 upp-0.2.1/test/AMD.RX480.8192.160603.rom.rawdump
--rw-rw-r--   0 samir     (1000) samir     (1000)       91 2021-01-04 17:30:40.000000 upp-0.2.1/test/AMD.RX5700XT.8192.190616.rom.check
--rw-rw-r--   0 samir     (1000) samir     (1000)    17367 2024-04-08 15:13:17.000000 upp-0.2.1/test/AMD.RX5700XT.8192.190616.rom.dump
--rw-rw-r--   0 samir     (1000) samir     (1000)    51669 2024-04-08 15:15:25.000000 upp-0.2.1/test/AMD.RX5700XT.8192.190616.rom.rawdump
--rw-rw-r--   0 samir     (1000) samir     (1000)    25867 2024-04-08 14:58:34.000000 upp-0.2.1/test/AMD.RX6900.16384.201104.rom.dump
--rw-rw-r--   0 samir     (1000) samir     (1000)    76184 2024-04-08 15:04:05.000000 upp-0.2.1/test/AMD.RX6900.16384.201104.rom.rawdump
--rw-r--r--   0 samir     (1000) samir     (1000)    47367 2024-04-08 15:06:00.000000 upp-0.2.1/test/AMD.RX7900XTX.24576.230323.rom.dump
--rw-r--r--   0 samir     (1000) samir     (1000)   127547 2024-04-08 15:07:25.000000 upp-0.2.1/test/AMD.RX7900XTX.24576.230323.rom.rawdump
--rw-rw-r--   0 samir     (1000) samir     (1000)     7718 2021-01-04 17:25:18.000000 upp-0.2.1/test/AMD.RXVega64.8176.170719.rom.dump
--rw-rw-r--   0 samir     (1000) samir     (1000)    25072 2024-04-08 14:55:09.000000 upp-0.2.1/test/AMD.RXVega64.8176.170719.rom.rawdump
--rw-r--r--   0 samir     (1000) samir     (1000)     6722 2022-07-03 10:14:53.000000 upp-0.2.1/test/AMD.RXVegaFrontier.16384.170628.rom.dump
--rw-r--r--   0 samir     (1000) samir     (1000)    22180 2024-04-08 14:55:12.000000 upp-0.2.1/test/AMD.RXVegaFrontier.16384.170628.rom.rawdump
--rw-rw-r--   0 samir     (1000) samir     (1000)    16605 2021-01-04 17:25:18.000000 upp-0.2.1/test/AMD.RadeonVII.16384.190116.rom.dump
--rw-rw-r--   0 samir     (1000) samir     (1000)    48006 2024-04-08 14:51:07.000000 upp-0.2.1/test/AMD.RadeonVII.16384.190116.rom.rawdump
--rw-r--r--   0 samir     (1000) samir     (1000)     2726 2024-03-23 09:43:45.000000 upp-0.2.1/test/navi23.mpt
--rwxrwxr-x   0 samir     (1000) samir     (1000)     3991 2024-03-25 18:46:45.000000 upp-0.2.1/test/test.sh
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-05-12 12:54:25.983810 upp-0.2.2/
+-rw-r--r--   0 samir     (1000) samir     (1000)     1225 2021-01-04 17:42:38.000000 upp-0.2.2/.gitignore
+-rw-r--r--   0 samir     (1000) samir     (1000)    35149 2019-02-20 19:25:43.000000 upp-0.2.2/LICENSE
+-rw-r--r--   0 samir     (1000) samir     (1000)     8116 2024-05-12 12:54:25.983810 upp-0.2.2/PKG-INFO
+-rw-r--r--   0 samir     (1000) samir     (1000)     7361 2024-05-12 12:53:50.000000 upp-0.2.2/README.md
+-rw-r--r--   0 samir     (1000) samir     (1000)       38 2024-05-12 12:54:25.983810 upp-0.2.2/setup.cfg
+-rw-r--r--   0 samir     (1000) samir     (1000)     1104 2024-05-12 12:53:50.000000 upp-0.2.2/setup.py
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-05-12 12:54:25.977143 upp-0.2.2/src/
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-05-12 12:54:25.980476 upp-0.2.2/src/upp/
+-rw-r--r--   0 samir     (1000) samir     (1000)        0 2020-03-27 07:44:19.000000 upp-0.2.2/src/upp/__init__.py
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-05-12 12:54:25.980476 upp-0.2.2/src/upp/atom_gen/
+-rw-r--r--   0 samir     (1000) samir     (1000)     4043 2024-05-12 12:53:50.000000 upp-0.2.2/src/upp/atom_gen/README.md
+-rw-r--r--   0 samir     (1000) samir     (1000)        0 2021-08-15 09:31:23.000000 upp-0.2.2/src/upp/atom_gen/__init__.py
+-rw-r--r--   0 samir     (1000) samir     (1000)     8599 2024-03-25 16:25:09.000000 upp-0.2.2/src/upp/atom_gen/atombios.py
+-rw-r--r--   0 samir     (1000) samir     (1000)    30254 2024-03-25 16:25:20.000000 upp-0.2.2/src/upp/atom_gen/pptable_v1_0.py
+-rw-r--r--   0 samir     (1000) samir     (1000)    31364 2024-04-01 12:39:06.000000 upp-0.2.2/src/upp/atom_gen/smu_v11_0_7_navi20.py
+-rw-r--r--   0 samir     (1000) samir     (1000)    24275 2024-05-12 12:53:50.000000 upp-0.2.2/src/upp/atom_gen/smu_v11_0_arcturus.py
+-rw-rw-r--   0 samir     (1000) samir     (1000)    25359 2024-03-25 16:25:40.000000 upp-0.2.2/src/upp/atom_gen/smu_v11_0_navi10.py
+-rw-r--r--   0 samir     (1000) samir     (1000)    39447 2024-03-25 16:25:49.000000 upp-0.2.2/src/upp/atom_gen/smu_v13_0_7_navi30.py
+-rw-rw-r--   0 samir     (1000) samir     (1000)    30177 2024-03-25 16:25:31.000000 upp-0.2.2/src/upp/atom_gen/vega10_pptable.py
+-rw-rw-r--   0 samir     (1000) samir     (1000)    22595 2024-03-25 16:25:35.000000 upp-0.2.2/src/upp/atom_gen/vega20_pptable.py
+-rw-r--r--   0 samir     (1000) samir     (1000)    39330 2024-05-12 12:53:50.000000 upp-0.2.2/src/upp/decode.py
+-rwxr-xr-x   0 samir     (1000) samir     (1000)    16881 2024-03-25 18:27:25.000000 upp-0.2.2/src/upp/upp.py
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-05-12 12:54:25.983810 upp-0.2.2/src/upp.egg-info/
+-rw-r--r--   0 samir     (1000) samir     (1000)     8116 2024-05-12 12:54:25.000000 upp-0.2.2/src/upp.egg-info/PKG-INFO
+-rw-r--r--   0 samir     (1000) samir     (1000)     1270 2024-05-12 12:54:25.000000 upp-0.2.2/src/upp.egg-info/SOURCES.txt
+-rw-r--r--   0 samir     (1000) samir     (1000)        1 2024-05-12 12:54:25.000000 upp-0.2.2/src/upp.egg-info/dependency_links.txt
+-rw-r--r--   0 samir     (1000) samir     (1000)       37 2024-05-12 12:54:25.000000 upp-0.2.2/src/upp.egg-info/entry_points.txt
+-rw-r--r--   0 samir     (1000) samir     (1000)       17 2024-05-12 12:54:25.000000 upp-0.2.2/src/upp.egg-info/requires.txt
+-rw-r--r--   0 samir     (1000) samir     (1000)       17 2024-05-12 12:54:25.000000 upp-0.2.2/src/upp.egg-info/top_level.txt
+drwxr-xr-x   0 samir     (1000) samir     (1000)        0 2024-05-12 12:54:25.983810 upp-0.2.2/test/
+-rw-rw-r--   0 samir     (1000) samir     (1000)     8888 2021-06-03 18:56:29.000000 upp-0.2.2/test/AMD.RX480.8192.160603.rom.dump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    30539 2024-04-08 14:54:40.000000 upp-0.2.2/test/AMD.RX480.8192.160603.rom.rawdump
+-rw-rw-r--   0 samir     (1000) samir     (1000)       91 2021-01-04 17:30:40.000000 upp-0.2.2/test/AMD.RX5700XT.8192.190616.rom.check
+-rw-rw-r--   0 samir     (1000) samir     (1000)    17367 2024-04-08 15:13:17.000000 upp-0.2.2/test/AMD.RX5700XT.8192.190616.rom.dump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    51669 2024-04-08 15:15:25.000000 upp-0.2.2/test/AMD.RX5700XT.8192.190616.rom.rawdump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    25867 2024-04-08 14:58:34.000000 upp-0.2.2/test/AMD.RX6900.16384.201104.rom.dump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    76184 2024-04-08 15:04:05.000000 upp-0.2.2/test/AMD.RX6900.16384.201104.rom.rawdump
+-rw-r--r--   0 samir     (1000) samir     (1000)    47259 2024-05-12 12:53:50.000000 upp-0.2.2/test/AMD.RX7900XTX.24576.230323.rom.dump
+-rw-r--r--   0 samir     (1000) samir     (1000)   127579 2024-05-12 12:53:50.000000 upp-0.2.2/test/AMD.RX7900XTX.24576.230323.rom.rawdump
+-rw-rw-r--   0 samir     (1000) samir     (1000)     7718 2021-01-04 17:25:18.000000 upp-0.2.2/test/AMD.RXVega64.8176.170719.rom.dump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    25072 2024-04-08 14:55:09.000000 upp-0.2.2/test/AMD.RXVega64.8176.170719.rom.rawdump
+-rw-r--r--   0 samir     (1000) samir     (1000)     6722 2022-07-03 10:14:53.000000 upp-0.2.2/test/AMD.RXVegaFrontier.16384.170628.rom.dump
+-rw-r--r--   0 samir     (1000) samir     (1000)    22180 2024-04-08 14:55:12.000000 upp-0.2.2/test/AMD.RXVegaFrontier.16384.170628.rom.rawdump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    16605 2021-01-04 17:25:18.000000 upp-0.2.2/test/AMD.RadeonVII.16384.190116.rom.dump
+-rw-rw-r--   0 samir     (1000) samir     (1000)    48006 2024-04-08 14:51:07.000000 upp-0.2.2/test/AMD.RadeonVII.16384.190116.rom.rawdump
+-rw-r--r--   0 samir     (1000) samir     (1000)     2726 2024-03-23 09:43:45.000000 upp-0.2.2/test/navi23.mpt
+-rwxr-xr-x   0 samir     (1000) samir     (1000)     4997 2024-05-12 12:53:50.000000 upp-0.2.2/test/test.sh
```

### Comparing `upp-0.2.1/.gitignore` & `upp-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/LICENSE` & `upp-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/PKG-INFO` & `upp-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: upp
-Version: 0.2.1
+Version: 0.2.2
 Summary: Uplift Power Play
 Home-page: https://github.com/sibradzic/upp
 Author: Samir Ibradžić
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: setuptools
@@ -48,23 +49,27 @@
 This tool currently supports parsing and modifying PowerPlay tables found
 on the following AMD GPU families:
 
 * Polaris
 * Vega
 * Radeon VII
 * Navi 10
+* Arcturus (MI100)
 * Navi 12 (PRO V520)
 * Navi 14
 * Navi 21 (Sienna Cichlid)
 * Navi 22 (Navy Flounder)
 * Navi 23 (Dimgrey Cavefish)
-* Navi 3x *experimental support
+* Navi 3x
 
-Note: iGPUs found in many recent AMD APUs are using completely different
-PowerPlay control methods, this tool does not support them.
+Notes:
+* iGPUs found in many recent AMD APUs are using completely different
+  PowerPlay control methods, this tool does not support them.
+* The kernel driver does not fully implement modifying the PowerPlay tables
+  on runtime for Navi 3x cards
 
 **WARNING**: Authors of this tool are in no way responsible for any damage
 that may happen to your expansive graphics card if you choose to modify
 card voltages, power limits, or any other PowerPlay parameters. Always
 remember that you are doing it entirely on your own risk!
 
 If you have bugs to report or features to request please create an issue on:
```

### Comparing `upp-0.2.1/README.md` & `upp-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,23 +28,27 @@
 This tool currently supports parsing and modifying PowerPlay tables found
 on the following AMD GPU families:
 
 * Polaris
 * Vega
 * Radeon VII
 * Navi 10
+* Arcturus (MI100)
 * Navi 12 (PRO V520)
 * Navi 14
 * Navi 21 (Sienna Cichlid)
 * Navi 22 (Navy Flounder)
 * Navi 23 (Dimgrey Cavefish)
-* Navi 3x *experimental support
+* Navi 3x
 
-Note: iGPUs found in many recent AMD APUs are using completely different
-PowerPlay control methods, this tool does not support them.
+Notes:
+* iGPUs found in many recent AMD APUs are using completely different
+  PowerPlay control methods, this tool does not support them.
+* The kernel driver does not fully implement modifying the PowerPlay tables
+  on runtime for Navi 3x cards
 
 **WARNING**: Authors of this tool are in no way responsible for any damage
 that may happen to your expansive graphics card if you choose to modify
 card voltages, power limits, or any other PowerPlay parameters. Always
 remember that you are doing it entirely on your own risk!
 
 If you have bugs to report or features to request please create an issue on:
```

### Comparing `upp-0.2.1/setup.py` & `upp-0.2.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='upp',
-    version='0.2.1',
+    version='0.2.2',
     author='Samir Ibradžić',
     description='Uplift Power Play',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sibradzic/upp',
     package_dir={'': 'src'},
     packages=['upp', 'upp/atom_gen'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.7, <4',
     install_requires=[
         'click',
         'setuptools'
```

### Comparing `upp-0.2.1/src/upp/atom_gen/README.md` & `upp-0.2.2/src/upp/atom_gen/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,24 @@
       --clang-args="--include stdint.h \
                     --include linux/drivers/gpu/drm/amd/include/atom-types.h \
                     --include linux/drivers/gpu/drm/amd/include/atomfirmware.h \
                     --include linux/drivers/gpu/drm/amd/pm/swsmu/inc/pmfw_if/smu11_driver_if_navi10.h " \
        linux/drivers/gpu/drm/amd/pm/swsmu/inc/smu_v11_0_pptable.h > smu_v11_0_navi10.py
 
 
+##  smu_v11_0_arcturus.py (MI100)
+
+    clang2py -k 'mste' \
+      --clang-args="--include stdint.h \
+                    --include linux/drivers/gpu/drm/amd/include/atom-types.h \
+                    --include linux/drivers/gpu/drm/amd/include/atomfirmware.h \
+                    --include linux/drivers/gpu/drm/amd/pm/swsmu/inc/pmfw_if/smu11_driver_if_arcturus.h " \
+       linux/drivers/gpu/drm/amd/pm/swsmu/inc/smu_v11_0_pptable.h > smu_v11_0_arcturus.py
+
+
 ##  smu_v11_0_navi20.py (Navi21/22/23)
 
     clang2py -k 'mste' \
       --clang-args="--include stdint.h \
                     --include linux/drivers/gpu/drm/amd/include/atom-types.h \
                     --include linux/drivers/gpu/drm/amd/include/atomfirmware.h \
                     --include linux/drivers/gpu/drm/amd/pm/swsmu/inc/pmfw_if/smu11_driver_if_sienna_cichlid.h " \
```

### Comparing `upp-0.2.1/src/upp/atom_gen/atombios.py` & `upp-0.2.2/src/upp/atom_gen/atombios.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/src/upp/atom_gen/pptable_v1_0.py` & `upp-0.2.2/src/upp/atom_gen/pptable_v1_0.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/src/upp/atom_gen/smu_v11_0_7_navi20.py` & `upp-0.2.2/src/upp/atom_gen/smu_v11_0_7_navi20.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/src/upp/atom_gen/smu_v11_0_navi10.py` & `upp-0.2.2/src/upp/atom_gen/smu_v11_0_navi10.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/src/upp/atom_gen/smu_v13_0_7_navi30.py` & `upp-0.2.2/src/upp/atom_gen/smu_v13_0_7_navi30.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/src/upp/atom_gen/vega10_pptable.py` & `upp-0.2.2/src/upp/atom_gen/vega10_pptable.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/src/upp/atom_gen/vega20_pptable.py` & `upp-0.2.2/src/upp/atom_gen/vega20_pptable.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/src/upp/decode.py` & `upp-0.2.2/src/upp/decode.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 atom_rom_header_v2 = atombios.struct__ATOM_ROM_HEADER_V2_1
 leagcy_vrom_offset = 0x40000
 
 # Base ctypes variables, in order to distinguish from structures and arrays
 primitives = [
     ctypes.c_byte, ctypes.c_ubyte,
     ctypes.c_int16, ctypes.c_uint16,
-    ctypes.c_uint32, ctypes.c_float
+    ctypes.c_int32, ctypes.c_uint32,
+    ctypes.c_float
 ]
 
 # Defined as uint in kernel, but in reality these are float
 float_fields = ['a', 'b', 'c', 'm',
-                'VcBtcPsmA', 'VcBtcPsmB', 'VcBtcVminA', 'VcBtcVminB']
+                'VcBtcPsmA', 'VcBtcPsmB', 'VcBtcVminA', 'VcBtcVminB',
+                'DfllBtcMasterScalerM', 'DfllBtcSlaveScalerM',
+                'DfllBtcMasterScalerB', 'DfllBtcSlaveScalerB']
 float_arrays = ['Fset', 'Vdroop', 'VcBtcPsmA', 'VcBtcPsmB', 'VcBtcVminA',
                 'VcBtcVminB', 'Droop_PWL_F', 'Droop_PWL_a', 'Droop_PWL_b',
                 'Droop_PWL_c']
 
-
 def odict(init_data=None):
     """
     Returns ordered dictionary (for consistent behavior on Python 2.7 & 3.6+)
     """
     if init_data:
         return OrderedDict(init_data)
     else:
@@ -699,14 +701,19 @@
             'overdrive_table': {
                 'prefix': 'SMU_11_0_ODSETTING_',
                 'struct': pp_struct.SMU_11_0_ODSETTING_ID__enumvalues,
                 'cappfx': 'SMU_11_0_ODCAP_',
                 'capstr': pp_struct.SMU_11_0_ODFEATURE_CAP__enumvalues,
             }
         }
+    # Arcturus aka MI100
+    elif pp_ver == (13, 0):
+        gpugen = 'Arcturus'
+        from upp.atom_gen import smu_v11_0_arcturus as pp_struct
+        ctypes_strct = pp_struct.struct_smu_11_0_powerplay_table
     # Navi 12 aka PRO V520
     elif pp_ver == (14, 0):
         gpugen = 'Navi 12'
         from upp.atom_gen import smu_v11_0_navi10 as pp_struct
         ctypes_strct = pp_struct.struct_smu_11_0_powerplay_table
     # Navi 21 (Sienna Cichlid) aka RX6900XT/RX6800(XT)
     # Navi 22 (Navy Flounder) aka RX6700(XT)/RX6800M
```

### Comparing `upp-0.2.1/src/upp/upp.py` & `upp-0.2.2/src/upp/upp.py`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/src/upp.egg-info/PKG-INFO` & `upp-0.2.2/src/upp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: upp
-Version: 0.2.1
+Version: 0.2.2
 Summary: Uplift Power Play
 Home-page: https://github.com/sibradzic/upp
 Author: Samir Ibradžić
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: setuptools
@@ -48,23 +49,27 @@
 This tool currently supports parsing and modifying PowerPlay tables found
 on the following AMD GPU families:
 
 * Polaris
 * Vega
 * Radeon VII
 * Navi 10
+* Arcturus (MI100)
 * Navi 12 (PRO V520)
 * Navi 14
 * Navi 21 (Sienna Cichlid)
 * Navi 22 (Navy Flounder)
 * Navi 23 (Dimgrey Cavefish)
-* Navi 3x *experimental support
+* Navi 3x
 
-Note: iGPUs found in many recent AMD APUs are using completely different
-PowerPlay control methods, this tool does not support them.
+Notes:
+* iGPUs found in many recent AMD APUs are using completely different
+  PowerPlay control methods, this tool does not support them.
+* The kernel driver does not fully implement modifying the PowerPlay tables
+  on runtime for Navi 3x cards
 
 **WARNING**: Authors of this tool are in no way responsible for any damage
 that may happen to your expansive graphics card if you choose to modify
 card voltages, power limits, or any other PowerPlay parameters. Always
 remember that you are doing it entirely on your own risk!
 
 If you have bugs to report or features to request please create an issue on:
```

### Comparing `upp-0.2.1/src/upp.egg-info/SOURCES.txt` & `upp-0.2.2/src/upp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/upp.egg-info/requires.txt
 src/upp.egg-info/top_level.txt
 src/upp/atom_gen/README.md
 src/upp/atom_gen/__init__.py
 src/upp/atom_gen/atombios.py
 src/upp/atom_gen/pptable_v1_0.py
 src/upp/atom_gen/smu_v11_0_7_navi20.py
+src/upp/atom_gen/smu_v11_0_arcturus.py
 src/upp/atom_gen/smu_v11_0_navi10.py
 src/upp/atom_gen/smu_v13_0_7_navi30.py
 src/upp/atom_gen/vega10_pptable.py
 src/upp/atom_gen/vega20_pptable.py
 test/AMD.RX480.8192.160603.rom.dump
 test/AMD.RX480.8192.160603.rom.rawdump
 test/AMD.RX5700XT.8192.190616.rom.check
```

### Comparing `upp-0.2.1/test/AMD.RX480.8192.160603.rom.dump` & `upp-0.2.2/test/AMD.RX480.8192.160603.rom.dump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RX480.8192.160603.rom.rawdump` & `upp-0.2.2/test/AMD.RX480.8192.160603.rom.rawdump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RX5700XT.8192.190616.rom.dump` & `upp-0.2.2/test/AMD.RX5700XT.8192.190616.rom.dump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RX5700XT.8192.190616.rom.rawdump` & `upp-0.2.2/test/AMD.RX5700XT.8192.190616.rom.rawdump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RX6900.16384.201104.rom.dump` & `upp-0.2.2/test/AMD.RX6900.16384.201104.rom.dump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RX6900.16384.201104.rom.rawdump` & `upp-0.2.2/test/AMD.RX6900.16384.201104.rom.rawdump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RX7900XTX.24576.230323.rom.dump` & `upp-0.2.2/test/AMD.RX7900XTX.24576.230323.rom.dump`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-ERROR: Unexpected data structure: <class 'int'>
-ERROR: Unexpected data structure: <class 'int'>
 header:
   structuresize: 5424
   format_revision: 20
   content_revision: 0
 table_revision: 3
 padding: 0
 table_size: 832
@@ -775,18 +773,18 @@
       GfxoffSpare 8: 0
       GfxoffSpare 9: 0
       GfxoffSpare 10: 0
       GfxoffSpare 11: 0
       GfxoffSpare 12: 0
       GfxoffSpare 13: 0
       GfxoffSpare 14: 0
-    DfllBtcMasterScalerM: 1065353216
-    DfllBtcMasterScalerB:
-    DfllBtcSlaveScalerM: 1066192077
-    DfllBtcSlaveScalerB:
+    DfllBtcMasterScalerM: 1
+    DfllBtcMasterScalerB: 0
+    DfllBtcSlaveScalerM: 1.1
+    DfllBtcSlaveScalerB: 0
     DfllPccAsWaitCtrl: 6553700
     DfllPccAsStepCtrl: 2065455
     GfxGpoSpare:
       GfxGpoSpare 0: 1066024305
       GfxGpoSpare 1: 0
       GfxGpoSpare 2: 0
       GfxGpoSpare 3: 0
```

### Comparing `upp-0.2.1/test/AMD.RX7900XTX.24576.230323.rom.rawdump` & `upp-0.2.2/test/AMD.RX7900XTX.24576.230323.rom.rawdump`

 * *Files 0% similar despite different names*

```diff
@@ -678,18 +678,18 @@
  0x071c (1820) I 00000000 GfxoffSpare                               : 0
  0x0720 (1824) I 00000000 GfxoffSpare                               : 0
  0x0724 (1828) I 00000000 GfxoffSpare                               : 0
  0x0728 (1832) I 00000000 GfxoffSpare                               : 0
  0x072c (1836) I 00000000 GfxoffSpare                               : 0
  0x0730 (1840) I 00000000 GfxoffSpare                               : 0
  0x0734 (1844) I 00000000 GfxoffSpare                               : 0
- 0x0738 (1848) I 0000803f DfllBtcMasterScalerM                      : 1065353216
-ERROR: Unexpected data structure: <class 'int'>
- 0x0740 (1856) I cdcc8c3f DfllBtcSlaveScalerM                       : 1066192077
-ERROR: Unexpected data structure: <class 'int'>
+ 0x0738 (1848) f 0000803f DfllBtcMasterScalerM                      : 1
+ 0x073c (1852) i 00000000 DfllBtcMasterScalerB                      : 0
+ 0x0740 (1856) f cdcc8c3f DfllBtcSlaveScalerM                       : 1.1
+ 0x0744 (1860) i 00000000 DfllBtcSlaveScalerB                       : 0
  0x0748 (1864) I 64006400 DfllPccAsWaitCtrl                         : 6553700
  0x074c (1868) I 2f841f00 DfllPccAsStepCtrl                         : 2065455
  0x0750 (1872) I 713d8a3f GfxGpoSpare                               : 1066024305
  0x0754 (1876) I 00000000 GfxGpoSpare                               : 0
  0x0758 (1880) I 00000000 GfxGpoSpare                               : 0
  0x075c (1884) I 00000000 GfxGpoSpare                               : 0
  0x0760 (1888) I 00000000 GfxGpoSpare                               : 0
```

### Comparing `upp-0.2.1/test/AMD.RXVega64.8176.170719.rom.dump` & `upp-0.2.2/test/AMD.RXVega64.8176.170719.rom.dump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RXVega64.8176.170719.rom.rawdump` & `upp-0.2.2/test/AMD.RXVega64.8176.170719.rom.rawdump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RXVegaFrontier.16384.170628.rom.dump` & `upp-0.2.2/test/AMD.RXVegaFrontier.16384.170628.rom.dump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RXVegaFrontier.16384.170628.rom.rawdump` & `upp-0.2.2/test/AMD.RXVegaFrontier.16384.170628.rom.rawdump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RadeonVII.16384.190116.rom.dump` & `upp-0.2.2/test/AMD.RadeonVII.16384.190116.rom.dump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/AMD.RadeonVII.16384.190116.rom.rawdump` & `upp-0.2.2/test/AMD.RadeonVII.16384.190116.rom.rawdump`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/navi23.mpt` & `upp-0.2.2/test/navi23.mpt`

 * *Files identical despite different names*

### Comparing `upp-0.2.1/test/test.sh` & `upp-0.2.2/test/test.sh`

 * *Files 19% similar despite different names*

```diff
@@ -13,46 +13,72 @@
 ROM_RX5700=212120/AMD.RX5700XT.8192.190616.rom
 # RX 6800 16 GB Reference
 ROM_RX6800=226802/AMD.RX6800.16384.201007.rom
 # RX 6900 16 GB Reference
 ROM_RX6900=227070/AMD.RX6900.16384.201104.rom
 # RX 7900 XTX 24GB Reference
 ROM_RX7900=262809/AMD.RX7900XTX.24576.230323.rom
+# MI100
+ROM_MI100=MI100_000.000.000.000.016113_113-D3431401-100.rom
 
-TEST_ROMS="${ROM_RX480} ${ROM_VEGA64} ${ROM_VEGAFRONTIER} ${ROM_RADEON7} ${ROM_RX5700} ${ROM_RX6900} ${ROM_RX7900}"
+# Fetch ROMs not available at TechPowerUp from these links:
+ROM_LINKSs="
+https://github.com/sibradzic/upp/files/15254133/arcturus_vbios.zip
+"
+
+# ROMs to be tested:
+TEST_ROMS="${ROM_RX480} ${ROM_VEGA64} ${ROM_VEGAFRONTIER} ${ROM_RADEON7} ${ROM_RX5700} ${ROM_RX6900} ${ROM_RX7900} ${ROM_MI100}"
 TEST_ROOT=${PWD}
 ROM_DIR=${PWD}/ROMs
 TMP_DIR=${PWD}/tmp
 
 [ ! -d ${ROM_DIR} ] && mkdir ${ROM_DIR}
 [ ! -d ${TMP_DIR} ] && mkdir ${TMP_DIR}
 
 pushd ../src
 
+# Fetch non TehcPowerUp ROMs
+for VBIOS in ${ROM_LINKSs}; do
+  if [ ! -r ${ROM_DIR}/${VBIOS##*/} ]; then
+    wget -P ${ROM_DIR} ${VBIOS}
+    if [[ "${VBIOS##*.}" == "zip" ]]; then
+      unzip ${ROM_DIR}/${VBIOS##*/} -d ${ROM_DIR}
+    fi
+  fi
+done
+
+# Fetch TehcPowerUp ROMs and test all ROMs
 for VBIOS in ${TEST_ROMS}; do
   if [ ! -r ${ROM_DIR}/${VBIOS#*/} ]; then
     wget -P ${ROM_DIR} ${TPU_VBIOS_URL}/${VBIOS}
   fi
   python3 -m upp.upp -p ${TMP_DIR}/${VBIOS#*/}.pp_table extract -r ${ROM_DIR}/${VBIOS#*/}
   python3 -m upp.upp -p ${TMP_DIR}/${VBIOS#*/}.pp_table dump > ${TMP_DIR}/${VBIOS#*/}.dump
   python3 -m upp.upp -p ${TMP_DIR}/${VBIOS#*/}.pp_table dump -r > ${TMP_DIR}/${VBIOS#*/}.rawdump
   diff -s ${TEST_ROOT}/${VBIOS#*/}.dump ${TMP_DIR}/${VBIOS#*/}.dump
   if [ $? -ne "0" ]; then
     echo "ERROR in ${TMP_DIR}/${VBIOS#*/}.dump:"
     diff -u ${TEST_ROOT}/${VBIOS#*/}.dump ${TMP_DIR}/${VBIOS#*/}.dump
+    printf "\033[1m${VBIOS#*/} dump check \033[1;31mERROR\033[0m\n"
     exit 2
+  else
+    printf "\033[1m${VBIOS#*/} dump check \033[1;32mOK\033[0m\n\n"
   fi
   diff -s ${TEST_ROOT}/${VBIOS#*/}.rawdump ${TMP_DIR}/${VBIOS#*/}.rawdump
   if [ $? -ne "0" ]; then
     echo "ERROR in ${TMP_DIR}/${VBIOS#*/}.rawdump:"
     diff -u ${TEST_ROOT}/${VBIOS#*/}.rawdump ${TMP_DIR}/${VBIOS#*/}.rawdump
+    printf "\033[1m${VBIOS#*/} raw dump check \033[1;31mERROR\033[0m\n"
     exit 2
+  else
+    printf "\033[1m${VBIOS#*/} raw dump check \033[1;32mOK\033[0m\n\n"
   fi
 done
 
+# Value write test
 python3 -m upp.upp -p ${TMP_DIR}/${ROM_RX5700#*/}.pp_table set --write \
   smc_pptable/SocketPowerLimitAc/0=110        \
   smc_pptable/SocketPowerLimitDc/0=110        \
   smc_pptable/FanStartTemp=100                \
   smc_pptable/MinVoltageGfx=2800              \
   smc_pptable/MaxVoltageGfx=3900              \
   smc_pptable/MinVoltageSoc=2800              \
@@ -94,9 +120,12 @@
   smc_pptable/FreqTableUclk/3           \
   >  ${TMP_DIR}/${ROM_RX5700#*/}.check
 
 diff -s ${TEST_ROOT}/${ROM_RX5700#*/}.check ${TMP_DIR}/${ROM_RX5700#*/}.check
 if [ $? -ne "0" ]; then
   echo "ERROR in ${TMP_DIR}/${ROM_RX5700#*/}.check:"
   diff -u ${TEST_ROOT}/${ROM_RX5700#*/}.check ${TMP_DIR}/${ROM_RX5700#*/}.check
+  printf "\033[1m${ROM_RX5700#*/} value write check \033[1;31mERROR\033[0m\n"
   exit 2
+else
+  printf "\033[1m${ROM_RX5700#*/} value write check \033[1;32mOK\033[0m\n\n"
 fi
```

