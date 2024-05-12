# Comparing `tmp/sherlock_testabcyuegughriuhgu-0.14.5.tar.gz` & `tmp/sherlock_testabcyuegughriuhgu-0.14.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherlock_testabcyuegughriuhgu-0.14.5.tar", last modified: Sun May 12 01:57:44 2024, max compression
+gzip compressed data, was "sherlock_testabcyuegughriuhgu-0.14.6.tar", last modified: Sun May 12 02:13:00 2024, max compression
```

## Comparing `sherlock_testabcyuegughriuhgu-0.14.5.tar` & `sherlock_testabcyuegughriuhgu-0.14.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:44.328263 sherlock_testabcyuegughriuhgu-0.14.5/
--rw-r--r--   0 paul      (1000) paul      (1000)     1073 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.5/LICENSE
--rw-r--r--   0 paul      (1000) paul      (1000)     9735 2024-05-12 01:57:44.328263 sherlock_testabcyuegughriuhgu-0.14.5/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     7132 2024-05-12 01:17:05.000000 sherlock_testabcyuegughriuhgu-0.14.5/README.md
--rw-r--r--   0 paul      (1000) paul      (1000)     1421 2024-05-12 01:32:16.000000 sherlock_testabcyuegughriuhgu-0.14.5/pyproject.toml
--rw-r--r--   0 paul      (1000) paul      (1000)      166 2024-05-11 04:10:51.000000 sherlock_testabcyuegughriuhgu-0.14.5/requirements.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      133 2024-05-12 01:57:44.329263 sherlock_testabcyuegughriuhgu-0.14.5/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)     1059 2024-05-12 01:54:47.000000 sherlock_testabcyuegughriuhgu-0.14.5/setup.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:44.327263 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:44.328263 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     9735 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)      740 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       43 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/entry_points.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      166 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       63 2024-05-12 01:57:44.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/top_level.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      106 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)      537 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/__main__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     9034 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/notify.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:44.328263 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/resources/
--rw-r--r--   0 paul      (1000) paul      (1000)    87973 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/resources/data.json
--rw-r--r--   0 paul      (1000) paul      (1000)     3228 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/resources/data.schema.json
--rw-r--r--   0 paul      (1000) paul      (1000)     3184 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/result.py
--rw-r--r--   0 paul      (1000) paul      (1000)    32322 2024-05-12 01:57:40.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/sherlock.py
--rw-r--r--   0 paul      (1000) paul      (1000)     9370 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/sites.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 01:57:44.328263 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/
--rw-r--r--   0 paul      (1000) paul      (1000)       87 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7164 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/all.py
--rw-r--r--   0 paul      (1000) paul      (1000)     8588 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/base.py
--rw-r--r--   0 paul      (1000) paul      (1000)      930 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/test_multiple_usernames.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 02:13:00.919101 sherlock_testabcyuegughriuhgu-0.14.6/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1073 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.6/LICENSE
+-rw-r--r--   0 paul      (1000) paul      (1000)     8497 2024-05-12 02:13:00.919101 sherlock_testabcyuegughriuhgu-0.14.6/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     7132 2024-05-12 01:17:05.000000 sherlock_testabcyuegughriuhgu-0.14.6/README.md
+-rw-r--r--   0 paul      (1000) paul      (1000)     1417 2024-05-12 02:12:34.000000 sherlock_testabcyuegughriuhgu-0.14.6/pyproject.toml
+-rw-r--r--   0 paul      (1000) paul      (1000)      166 2024-05-11 04:10:51.000000 sherlock_testabcyuegughriuhgu-0.14.6/requirements.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      133 2024-05-12 02:13:00.920102 sherlock_testabcyuegughriuhgu-0.14.6/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)      473 2024-05-12 02:08:40.000000 sherlock_testabcyuegughriuhgu-0.14.6/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 02:13:00.918101 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 02:13:00.919101 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     8497 2024-05-12 02:13:00.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)      740 2024-05-12 02:13:00.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2024-05-12 02:13:00.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       43 2024-05-12 02:13:00.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/entry_points.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      166 2024-05-12 02:13:00.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       63 2024-05-12 02:13:00.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/top_level.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      106 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      537 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/__main__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     9034 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/notify.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 02:13:00.919101 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/resources/
+-rw-r--r--   0 paul      (1000) paul      (1000)    87973 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/resources/data.json
+-rw-r--r--   0 paul      (1000) paul      (1000)     3228 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/resources/data.schema.json
+-rw-r--r--   0 paul      (1000) paul      (1000)     3184 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/result.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    32322 2024-05-12 02:12:45.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/sherlock.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     9370 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/sites.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2024-05-12 02:13:00.919101 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/tests/
+-rw-r--r--   0 paul      (1000) paul      (1000)       87 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/tests/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7164 2024-05-11 20:01:58.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/tests/all.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     8588 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/tests/base.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      930 2024-04-07 22:08:31.000000 sherlock_testabcyuegughriuhgu-0.14.6/sherlock/tests/test_multiple_usernames.py
```

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/LICENSE` & `sherlock_testabcyuegughriuhgu-0.14.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/PKG-INFO` & `sherlock_testabcyuegughriuhgu-0.14.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,15 @@
 Metadata-Version: 2.1
 Name: Sherlock-testABCYUEGUGHRIUHGU
-Version: 0.14.5
+Version: 0.14.6
 Summary: Hunt down social media accounts by username across social networks
 Home-page: http://sherlock-project.github.io/
 Author: Sherlock Project
 Maintainer: Siddharth Dushantha, Matheus Felipe, Sondre Karlsen Dyrnes, Paul Pfeister
-License: MIT License
-        
-        Copyright (c) 2019 Sherlock Project
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+License: MIT
 Project-URL: Homepage, http://sherlock-project.github.io/
 Project-URL: Repository, https://github.com/sherlock-project/sherlock.git
 Project-URL: Issues, https://github.com/sherlock-project/sherlock/issues
 Keywords: osint,reconnaissance,information gathering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,40 +1,25 @@
-Metadata-Version: 2.1 Name: Sherlock-testABCYUEGUGHRIUHGU Version: 0.14.5
+Metadata-Version: 2.1 Name: Sherlock-testABCYUEGUGHRIUHGU Version: 0.14.6
 Summary: Hunt down social media accounts by username across social networks
 Home-page: http://sherlock-project.github.io/ Author: Sherlock Project
 Maintainer: Siddharth Dushantha, Matheus Felipe, Sondre Karlsen Dyrnes, Paul
-Pfeister License: MIT License Copyright (c) 2019 Sherlock Project Permission is
-hereby granted, free of charge, to any person obtaining a copy of this software
-and associated documentation files (the "Software"), to deal in the Software
-without restriction, including without limitation the rights to use, copy,
-modify, merge, publish, distribute, sublicense, and/or sell copies of the
-Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions: The above copyright notice and this
-permission notice shall be included in all copies or substantial portions of
-the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, http://sherlock-
-project.github.io/ Project-URL: Repository, https://github.com/sherlock-
-project/sherlock.git Project-URL: Issues, https://github.com/sherlock-project/
-sherlock/issues Keywords: osint,reconnaissance,information gathering
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
-:: English Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Topic :: Communications
-Classifier: Topic :: Security Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: certifi>=2019.6.16 Requires-Dist: colorama>=0.4.1
-Requires-Dist: PySocks>=1.7.0 Requires-Dist: requests>=2.22.0 Requires-Dist:
-requests-futures>=1.0.0 Requires-Dist: stem>=1.8.0 Requires-Dist:
-torrequest>=0.1.0 Requires-Dist: pandas>=1.0.0 Requires-Dist: openpyxl<=3.0.10
-Requires-Dist: exrex>=0.11.0
+Pfeister License: MIT Project-URL: Homepage, http://sherlock-project.github.io/
+Project-URL: Repository, https://github.com/sherlock-project/sherlock.git
+Project-URL: Issues, https://github.com/sherlock-project/sherlock/issues
+Keywords: osint,reconnaissance,information gathering Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology Classifier: License ::
+OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Topic :: Communications Classifier: Topic :: Security
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+certifi>=2019.6.16 Requires-Dist: colorama>=0.4.1 Requires-Dist: PySocks>=1.7.0
+Requires-Dist: requests>=2.22.0 Requires-Dist: requests-futures>=1.0.0
+Requires-Dist: stem>=1.8.0 Requires-Dist: torrequest>=0.1.0 Requires-Dist:
+pandas>=1.0.0 Requires-Dist: openpyxl<=3.0.10 Requires-Dist: exrex>=0.11.0
 
   _[_h_t_t_p_s_:_/_/_u_s_e_r_-_i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_2_7_0_6_5_6_4_6_/_5_3_5_5_1_9_6_0_-_a_e_4_d_f_f_8_0_-_3_b_3_a_-
                           _1_1_e_9_-_9_0_7_5_-_c_e_f_7_8_6_c_6_9_3_6_4_._p_n_g_]
       Hunt down social media accounts by username across _s_o_c_i_a_l_ _n_e_t_w_o_r_k_s
      _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e    |    _D_o_c_k_e_r_ _N_o_t_e_s    |    _C_o_n_t_r_i_b_u_t_i_n_g
  [https://user-images.githubusercontent.com/27065646/219638267-a5e11090-aa6e-
                           4e77-87f7-0e95f6ad5978.png]
```

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/README.md` & `sherlock_testabcyuegughriuhgu-0.14.6/README.md`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/pyproject.toml` & `sherlock_testabcyuegughriuhgu-0.14.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     { name = "Siddharth Dushantha" },
     { name = "Matheus Felipe" },
     { name = "Sondre Karlsen Dyrnes" },
     { name = "Paul Pfeister" }
 ]
 description = "Hunt down social media accounts by username across social networks"
 readme = "README.md"
-license = {file = "LICENSE"}
+license = {text = "MIT"}
 dynamic = ["dependencies", "version"]
 keywords = [ "osint", "reconnaissance", "information gathering" ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "License :: OSI Approved :: MIT License",
```

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/PKG-INFO` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,15 @@
 Metadata-Version: 2.1
 Name: Sherlock-testABCYUEGUGHRIUHGU
-Version: 0.14.5
+Version: 0.14.6
 Summary: Hunt down social media accounts by username across social networks
 Home-page: http://sherlock-project.github.io/
 Author: Sherlock Project
 Maintainer: Siddharth Dushantha, Matheus Felipe, Sondre Karlsen Dyrnes, Paul Pfeister
-License: MIT License
-        
-        Copyright (c) 2019 Sherlock Project
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
+License: MIT
 Project-URL: Homepage, http://sherlock-project.github.io/
 Project-URL: Repository, https://github.com/sherlock-project/sherlock.git
 Project-URL: Issues, https://github.com/sherlock-project/sherlock/issues
 Keywords: osint,reconnaissance,information gathering
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

#### html2text {}

```diff
@@ -1,40 +1,25 @@
-Metadata-Version: 2.1 Name: Sherlock-testABCYUEGUGHRIUHGU Version: 0.14.5
+Metadata-Version: 2.1 Name: Sherlock-testABCYUEGUGHRIUHGU Version: 0.14.6
 Summary: Hunt down social media accounts by username across social networks
 Home-page: http://sherlock-project.github.io/ Author: Sherlock Project
 Maintainer: Siddharth Dushantha, Matheus Felipe, Sondre Karlsen Dyrnes, Paul
-Pfeister License: MIT License Copyright (c) 2019 Sherlock Project Permission is
-hereby granted, free of charge, to any person obtaining a copy of this software
-and associated documentation files (the "Software"), to deal in the Software
-without restriction, including without limitation the rights to use, copy,
-modify, merge, publish, distribute, sublicense, and/or sell copies of the
-Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions: The above copyright notice and this
-permission notice shall be included in all copies or substantial portions of
-the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. Project-URL: Homepage, http://sherlock-
-project.github.io/ Project-URL: Repository, https://github.com/sherlock-
-project/sherlock.git Project-URL: Issues, https://github.com/sherlock-project/
-sherlock/issues Keywords: osint,reconnaissance,information gathering
-Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
-:: English Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Topic :: Communications
-Classifier: Topic :: Security Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: certifi>=2019.6.16 Requires-Dist: colorama>=0.4.1
-Requires-Dist: PySocks>=1.7.0 Requires-Dist: requests>=2.22.0 Requires-Dist:
-requests-futures>=1.0.0 Requires-Dist: stem>=1.8.0 Requires-Dist:
-torrequest>=0.1.0 Requires-Dist: pandas>=1.0.0 Requires-Dist: openpyxl<=3.0.10
-Requires-Dist: exrex>=0.11.0
+Pfeister License: MIT Project-URL: Homepage, http://sherlock-project.github.io/
+Project-URL: Repository, https://github.com/sherlock-project/sherlock.git
+Project-URL: Issues, https://github.com/sherlock-project/sherlock/issues
+Keywords: osint,reconnaissance,information gathering Classifier: Development
+Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology Classifier: License ::
+OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Classifier: Topic :: Communications Classifier: Topic :: Security
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+certifi>=2019.6.16 Requires-Dist: colorama>=0.4.1 Requires-Dist: PySocks>=1.7.0
+Requires-Dist: requests>=2.22.0 Requires-Dist: requests-futures>=1.0.0
+Requires-Dist: stem>=1.8.0 Requires-Dist: torrequest>=0.1.0 Requires-Dist:
+pandas>=1.0.0 Requires-Dist: openpyxl<=3.0.10 Requires-Dist: exrex>=0.11.0
 
   _[_h_t_t_p_s_:_/_/_u_s_e_r_-_i_m_a_g_e_s_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_2_7_0_6_5_6_4_6_/_5_3_5_5_1_9_6_0_-_a_e_4_d_f_f_8_0_-_3_b_3_a_-
                           _1_1_e_9_-_9_0_7_5_-_c_e_f_7_8_6_c_6_9_3_6_4_._p_n_g_]
       Hunt down social media accounts by username across _s_o_c_i_a_l_ _n_e_t_w_o_r_k_s
      _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e    |    _D_o_c_k_e_r_ _N_o_t_e_s    |    _C_o_n_t_r_i_b_u_t_i_n_g
  [https://user-images.githubusercontent.com/27065646/219638267-a5e11090-aa6e-
                           4e77-87f7-0e95f6ad5978.png]
```

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/SOURCES.txt` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/Sherlock_testABCYUEGUGHRIUHGU.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/__main__.py` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/__main__.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/notify.py` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/notify.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/resources/data.json` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/resources/data.json`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/resources/data.schema.json` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/resources/data.schema.json`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/result.py` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/result.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/sherlock.py` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/sherlock.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from result import QueryResult
 from notify import QueryNotifyPrint
 from sites import SitesInformation
 from colorama import init
 from argparse import ArgumentTypeError
 
 module_name = "Sherlock: Find Usernames Across Social Networks"
-__version__ = "0.14.5"
+__version__ = "0.14.6"
 
 
 class SherlockFuturesSession(FuturesSession):
     def request(self, method, url, hooks=None, *args, **kwargs):
         """Request URL.
 
         This extends the FuturesSession request method to calculate a response
```

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/sites.py` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/sites.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/all.py` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/tests/all.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/base.py` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/tests/base.py`

 * *Files identical despite different names*

### Comparing `sherlock_testabcyuegughriuhgu-0.14.5/sherlock/tests/test_multiple_usernames.py` & `sherlock_testabcyuegughriuhgu-0.14.6/sherlock/tests/test_multiple_usernames.py`

 * *Files identical despite different names*

