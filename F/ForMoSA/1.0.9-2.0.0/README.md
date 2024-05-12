# Comparing `tmp/ForMoSA-1.0.9.tar.gz` & `tmp/formosa-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ForMoSA-1.0.9.tar", last modified: Wed Mar 29 11:52:05 2023, max compression
+gzip compressed data, was "formosa-2.0.0.tar", last modified: Sat May 11 18:24:42 2024, max compression
```

## Comparing `ForMoSA-1.0.9.tar` & `formosa-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,31 @@
-drwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2023-03-29 11:52:05.351916 ForMoSA-1.0.9/
-drwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2023-03-29 11:52:05.348829 ForMoSA-1.0.9/ForMoSA/
--rw-r--r--   0 ppalmabifani   (501) staff       (20)      120 2023-03-29 11:49:12.000000 ForMoSA-1.0.9/ForMoSA/__init__.py
--rw-r--r--   0 ppalmabifani   (501) staff       (20)     2289 2023-02-28 12:22:12.000000 ForMoSA-1.0.9/ForMoSA/main.py
--rw-r--r--   0 ppalmabifani   (501) staff       (20)     5514 2023-03-16 08:56:55.000000 ForMoSA-1.0.9/ForMoSA/main_utilities.py
-drwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2023-03-29 11:52:05.351512 ForMoSA-1.0.9/ForMoSA.egg-info/
--rw-r--r--   0 ppalmabifani   (501) staff       (20)      318 2023-03-29 11:52:05.000000 ForMoSA-1.0.9/ForMoSA.egg-info/PKG-INFO
--rw-r--r--   0 ppalmabifani   (501) staff       (20)      272 2023-03-29 11:52:05.000000 ForMoSA-1.0.9/ForMoSA.egg-info/SOURCES.txt
--rw-r--r--   0 ppalmabifani   (501) staff       (20)        1 2023-03-29 11:52:05.000000 ForMoSA-1.0.9/ForMoSA.egg-info/dependency_links.txt
--rw-r--r--   0 ppalmabifani   (501) staff       (20)        1 2023-03-29 11:52:05.000000 ForMoSA-1.0.9/ForMoSA.egg-info/not-zip-safe
--rw-r--r--   0 ppalmabifani   (501) staff       (20)      127 2023-03-29 11:52:05.000000 ForMoSA-1.0.9/ForMoSA.egg-info/requires.txt
--rw-r--r--   0 ppalmabifani   (501) staff       (20)        8 2023-03-29 11:52:05.000000 ForMoSA-1.0.9/ForMoSA.egg-info/top_level.txt
--rw-r--r--   0 ppalmabifani   (501) staff       (20)     1324 2022-11-25 14:21:38.000000 ForMoSA-1.0.9/LICENSE
--rw-r--r--   0 ppalmabifani   (501) staff       (20)      318 2023-03-29 11:52:05.351740 ForMoSA-1.0.9/PKG-INFO
--rw-r--r--   0 ppalmabifani   (501) staff       (20)      805 2023-03-29 03:44:38.000000 ForMoSA-1.0.9/README.md
--rw-r--r--   0 ppalmabifani   (501) staff       (20)       38 2023-03-29 11:52:05.351967 ForMoSA-1.0.9/setup.cfg
--rw-r--r--   0 ppalmabifani   (501) staff       (20)      694 2023-03-29 11:48:48.000000 ForMoSA-1.0.9/setup.py
+drwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2024-05-11 18:24:42.731312 formosa-2.0.0/
+drwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2024-05-11 18:24:42.720469 formosa-2.0.0/ForMoSA/
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)       83 2024-05-11 17:42:55.000000 formosa-2.0.0/ForMoSA/__init__.py
+drwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2024-05-11 18:24:42.725284 formosa-2.0.0/ForMoSA/adapt/
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2024-01-31 14:10:20.000000 formosa-2.0.0/ForMoSA/adapt/__init__.py
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)    19666 2024-05-10 08:16:06.000000 formosa-2.0.0/ForMoSA/adapt/adapt_grid.py
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)     7384 2024-05-10 08:16:06.000000 formosa-2.0.0/ForMoSA/adapt/adapt_obs_mod.py
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)    30158 2024-05-10 08:16:06.000000 formosa-2.0.0/ForMoSA/adapt/extraction_functions.py
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)     2400 2024-05-10 08:16:06.000000 formosa-2.0.0/ForMoSA/main.py
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)     9554 2024-05-10 08:16:06.000000 formosa-2.0.0/ForMoSA/main_utilities.py
+drwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2024-05-11 18:24:42.728328 formosa-2.0.0/ForMoSA/nested_sampling/
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2024-01-31 14:10:20.000000 formosa-2.0.0/ForMoSA/nested_sampling/__init__.py
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)     4177 2024-05-10 08:16:06.000000 formosa-2.0.0/ForMoSA/nested_sampling/nested_logL_functions.py
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)    27477 2024-05-10 08:16:06.000000 formosa-2.0.0/ForMoSA/nested_sampling/nested_modif_spec.py
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)     1083 2024-03-08 14:41:15.000000 formosa-2.0.0/ForMoSA/nested_sampling/nested_prior_function.py
+-rwxr-xr-x   0 ppalmabifani   (501) staff       (20)    40559 2024-05-10 08:16:06.000000 formosa-2.0.0/ForMoSA/nested_sampling/nested_sampling.py
+drwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2024-05-11 18:24:42.729350 formosa-2.0.0/ForMoSA/plotting/
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)        0 2024-01-31 14:10:20.000000 formosa-2.0.0/ForMoSA/plotting/__init__.py
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)    47703 2024-05-10 08:16:06.000000 formosa-2.0.0/ForMoSA/plotting/plotting_class.py
+drwxr-xr-x   0 ppalmabifani   (501) staff       (20)        0 2024-05-11 18:24:42.730048 formosa-2.0.0/ForMoSA.egg-info/
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)      674 2024-05-11 18:24:42.000000 formosa-2.0.0/ForMoSA.egg-info/PKG-INFO
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)      681 2024-05-11 18:24:42.000000 formosa-2.0.0/ForMoSA.egg-info/SOURCES.txt
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)        1 2024-05-11 18:24:42.000000 formosa-2.0.0/ForMoSA.egg-info/dependency_links.txt
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)        1 2024-05-11 18:24:42.000000 formosa-2.0.0/ForMoSA.egg-info/not-zip-safe
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)      139 2024-05-11 18:24:42.000000 formosa-2.0.0/ForMoSA.egg-info/requires.txt
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)        8 2024-05-11 18:24:42.000000 formosa-2.0.0/ForMoSA.egg-info/top_level.txt
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)     1324 2024-01-31 14:10:20.000000 formosa-2.0.0/LICENSE
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)      674 2024-05-11 18:24:42.731052 formosa-2.0.0/PKG-INFO
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)     3705 2024-03-08 15:11:31.000000 formosa-2.0.0/README.md
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)       38 2024-05-11 18:24:42.731371 formosa-2.0.0/setup.cfg
+-rw-r--r--   0 ppalmabifani   (501) staff       (20)      779 2024-05-11 17:49:26.000000 formosa-2.0.0/setup.py
```

### Comparing `ForMoSA-1.0.9/ForMoSA/main.py` & `formosa-2.0.0/ForMoSA/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,66 @@
-'''
-ForMoSA run script
-
-Here we open the config file and extract all the needed information.
-Easy to understand and simple access for the new users.
-
-@authors: S. Petrus & P. Palma-Bifani 
-'''
-# ----------------------------------------------------------------------------------------------------------------------
-## IMPORTS
-import sys
-
-# Import ForMoSA
-#base_path = '/Users/ppalmabifani/Desktop/exoAtm/c0_ForMoSA/ForMoSA/'     # Give the path to ForMoSA to be able to import it. No need when this will be a pip package
-#sys.path.insert(1, base_path)
-from main_utilities import yesno
-from main_utilities import GlobFile
-from adapt.adapt_obs_mod import launch_adapt
-from nested_sampling.nested_sampling import launch_nested_sampling
-
-# ----------------------------------------------------------------------------------------------------------------------
-## USER configuration path
-print()
-print('- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -')
-print('-> Configuration of environment')
-if len(sys.argv) == 1:
-    print('Where is your configuration file?')
-    config_file_path = input()
-else:
-    config_file_path = sys.argv[1]
-print()
-
-# ----------------------------------------------------------------------------------------------------------------------
-## CONFIG_FILE reading and defining global parameters
-global_params = GlobFile(config_file_path)                          # To access any param.: global_params.parameter_name
-
-# ----------------------------------------------------------------------------------------------------------------------
-## Run ForMoSA
-print('- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -')
-print('-> Initializing ForMoSA')
-print()
-
-if len(sys.argv) == 1:
-    y_n_par = yesno('Do you want to adapt the grid too your data? (y/n)')
-else:
-    y_n_par = sys.argv[2]
-
-if y_n_par == 'y':
-    launch_adapt(global_params, justobs='no')
-else:
-    launch_adapt(global_params, justobs='yes')
-
-print()
-print('- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -')
-print('-> Nested sampling')
-print()
-# Run S5 for Nested Sampling
-launch_nested_sampling(global_params)
-
-print()
-print('- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -')
-print('-> Voilà, on est prêt')
+'''
+ForMoSA run script
+
+Here we open the config file and extract all the needed information.
+Easy to understand and simple access for the new users.
+
+@authors: S. Petrus & P. Palma-Bifani 
+'''
+# ----------------------------------------------------------------------------------------------------------------------
+## IMPORTS
+import os
+os.environ["OMP_NUM_THREADS"] = "1"
+import sys
+
+# Import ForMoSA
+#base_path = '/Users/ppalmabifani/Desktop/exoAtm/c0_ForMoSA/ForMoSA/'     # Give the path to ForMoSA to be able to import it. No need when this will be a pip package
+#sys.path.insert(1, base_path)
+from main_utilities import yesno
+from main_utilities import GlobFile
+from adapt.adapt_obs_mod import launch_adapt
+from nested_sampling.nested_sampling import launch_nested_sampling
+
+# ----------------------------------------------------------------------------------------------------------------------
+## USER configuration path
+print()
+print('- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -')
+print('-> Configuration of environment')
+if len(sys.argv) == 1:
+    print('Where is your configuration file?')
+    config_file_path = input()
+else:
+    config_file_path = sys.argv[1]
+print()
+
+# ----------------------------------------------------------------------------------------------------------------------
+## CONFIG_FILE reading and defining global parameters
+global_params = GlobFile(config_file_path)                          # To access any param.: global_params.parameter_name
+
+# ----------------------------------------------------------------------------------------------------------------------
+## Run ForMoSA
+print('- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -')
+print('-> Initializing ForMoSA')
+print()
+
+
+if len(sys.argv) == 1:
+    y_n_par = yesno('Do you want to adapt the grid to your data? (y/n)')
+else:
+    y_n_par = sys.argv[2]
+
+if y_n_par == 'y':
+    launch_adapt(global_params, justobs='no')
+else:
+    launch_adapt(global_params, justobs='yes')
+
+print()
+print('- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -')
+print('-> Nested sampling')
+print()
+# Run S5 for Nested Sampling
+launch_nested_sampling(global_params)
+
+print()
+print('- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -')
+print('-> Voilà, on est prêt')
 print()
```

### Comparing `ForMoSA-1.0.9/LICENSE` & `formosa-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ForMoSA-1.0.9/setup.py` & `formosa-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 def get_requires():
     reqs = []
     for line in open('requirements.txt', 'r').readlines():
         reqs.append(line)
     return reqs
 
 setup(name='ForMoSA',
-      version='1.0.9',
+      version='2.0.0',
       description='ForMoSA: Forward Modeling Tool for Spectral Analysis',
       url='https://github.com/exoAtmospheres/ForMoSA',
-      author='P. Palma-Bifani, S. Petrus',
+      author='P. Palma-Bifani, S. Petrus, M. Ravet, A. Denis, M. Bonnefoy, G. Chauvin',
       author_email='paulina.palma-bifani@oca.eu',
       license='BSD 2-Clause License',
-      packages=['ForMoSA'],
+      packages=['ForMoSA', 'ForMoSA.adapt', 'ForMoSA.nested_sampling', 'ForMoSA.plotting'],
       install_requires=get_requires(),
       include_package_data = True,
-      zip_safe=False,
-      python_requires='==3.7')
+      zip_safe=False
+      )
```

