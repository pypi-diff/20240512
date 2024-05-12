# Comparing `tmp/FiveMCipherFinder-2.6.2.tar.gz` & `tmp/fivemcipherfinder-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FiveMCipherFinder-2.6.2.tar", last modified: Tue Feb 13 12:09:53 2024, max compression
+gzip compressed data, was "fivemcipherfinder-2.6.3.tar", last modified: Sun May 12 13:47:07 2024, max compression
```

## Comparing `FiveMCipherFinder-2.6.2.tar` & `fivemcipherfinder-2.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:09:53.378989 FiveMCipherFinder-2.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:09:53.378989 FiveMCipherFinder-2.6.2/FiveMCipherFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-02-13 12:09:53.000000 FiveMCipherFinder-2.6.2/FiveMCipherFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-02-13 12:09:53.000000 FiveMCipherFinder-2.6.2/FiveMCipherFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 12:09:53.000000 FiveMCipherFinder-2.6.2/FiveMCipherFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-13 12:09:53.000000 FiveMCipherFinder-2.6.2/FiveMCipherFinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-13 12:09:53.000000 FiveMCipherFinder-2.6.2/FiveMCipherFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-13 12:09:53.000000 FiveMCipherFinder-2.6.2/FiveMCipherFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-02-13 12:09:53.378989 FiveMCipherFinder-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:09:53.378989 FiveMCipherFinder-2.6.2/cipherFinder/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/cipherFinder/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3776 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/cipherFinder/de_obfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/cipherFinder/deleter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13428 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/cipherFinder/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/cipherFinder/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/cipherFinder/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-02-13 12:09:53.378989 FiveMCipherFinder-2.6.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 12:09:53.378989 FiveMCipherFinder-2.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/tests/test_de_obfs.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/tests/test_deleter.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-13 12:09:43.000000 FiveMCipherFinder-2.6.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:47:07.655090 fivemcipherfinder-2.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:47:07.655090 fivemcipherfinder-2.6.3/FiveMCipherFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-05-12 13:47:07.000000 fivemcipherfinder-2.6.3/FiveMCipherFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-12 13:47:07.000000 fivemcipherfinder-2.6.3/FiveMCipherFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 13:47:07.000000 fivemcipherfinder-2.6.3/FiveMCipherFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-12 13:47:07.000000 fivemcipherfinder-2.6.3/FiveMCipherFinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 13:47:07.000000 fivemcipherfinder-2.6.3/FiveMCipherFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 13:47:07.000000 fivemcipherfinder-2.6.3/FiveMCipherFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-05-12 13:47:07.655090 fivemcipherfinder-2.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:47:07.655090 fivemcipherfinder-2.6.3/cipherFinder/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/cipherFinder/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3827 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/cipherFinder/de_obfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/cipherFinder/deleter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13428 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/cipherFinder/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/cipherFinder/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/cipherFinder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-12 13:47:07.655090 fivemcipherfinder-2.6.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 13:47:07.655090 fivemcipherfinder-2.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/tests/test_de_obfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/tests/test_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/tests/test_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-12 13:47:03.000000 fivemcipherfinder-2.6.3/tests/test_utils.py
```

### Comparing `FiveMCipherFinder-2.6.2/FiveMCipherFinder.egg-info/PKG-INFO` & `fivemcipherfinder-2.6.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,36 @@
-Metadata-Version: 2.1
-Name: FiveMCipherFinder
-Version: 2.6.2
-Summary: Finds Cipher in lua scripts.
-Home-page: https://github.com/exersalza/FivemCipherFinder
-Author: exersalza
-License: MIT
-Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
-Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: chardet
-
-# FivemCipherFinder (v2.6.2)
+# FivemCipherFinder (v2.6.3)
 
 <div align="center">
     <h2> Visitors </h2>
     <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint and Flake8](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
 [![PyTest](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![](https://tokei.rs/b1/github/exersalza/fivemcipherfinder)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/fivemcipherfinder?label=pypi%20downloads)
 
 
-- [Installation](#installation)
-- [Usage](#Usage)
-- [Troubleshooting](#Troubleshooting)
-- [Plugins](#Plugins)
-- [Contributing](#Contributing)
-- [Todo](#todo)
-- [Disclaimer](#Disclaimer)
-- [Prevention](#Prevention)
-- [Contact](#Contact)
-- [Credits](#Credits)
+- [FivemCipherFinder (v2.6.3)](#fivemcipherfinder-v263)
+  - [Installation](#installation)
+    - [New version](#new-version)
+    - [Old Version](#old-version)
+  - [Usage](#usage)
+  - [Troubleshooting](#troubleshooting)
+  - [Known False Positives](#known-false-positives)
+  - [Plugins](#plugins)
+  - [Contributing](#contributing)
+  - [Todo](#todo)
+  - [Disclaimer](#disclaimer)
+  - [Prevention](#prevention)
+  - [Contact](#contact)
+  - [Star History](#star-history)
+  - [Credits](#credits)
 
 
 FivemCipherFinder is a tool designed to assist in the removal of Ciphers from your scripts. It is a console-based tool that can be used by anyone, regardless of their coding experience. The main purpose of FivemCipherFinder is to find and identify Ciphers in your script files.
 
 ## Installation
 
 To install FivemCipherFinder, follow these steps:
@@ -142,28 +129,31 @@
 [DISCLAIMER](DISCLAIMER.md)
 
 
 ## Prevention
 
 You can add the following URLs to your hosts file or Firewall. See [here](https://docs.rackspace.com/docs/modify-your-hosts-file) if you're not sure how to edit the hosts file.
 
+Also read [here](https://github.com/ProjecteEndCipher/Cipher-Panel) and [here](https://github.com/ericstolly/cipher) for further information.
+
 ```
-172.0.0.1       cipher-panel.me
-172.0.0.1       ciphercheats.com
-172.0.0.1       keyx.club
-172.0.0.1       dark-utilities.xyz
-172.0.0.1       ketamin.cc
-172.0.0.1       pqzskjptss.shop
-172.0.0.1       admin-panel.sbs
-172.0.0.1       malware-panel.io
-172.0.0.1       docsfivem.com
-172.0.0.1       thedreamofficeem.com
-172.0.0.1       thedreamoffivem.com
-172.0.0.1       rpserveur.fr
-172.0.0.1       abxcgraovp.pics
+127.0.0.1       cipher-panel.me
+127.0.0.1       ciphercheats.com
+127.0.0.1       keyx.club
+127.0.0.1       dark-utilities.xyz
+127.0.0.1       ketamin.cc
+127.0.0.1       pqzskjptss.shop
+127.0.0.1       admin-panel.sbs
+127.0.0.1       malware-panel.io
+127.0.0.1       docsfivem.com
+127.0.0.1       thedreamofficeem.com
+127.0.0.1       thedreamoffivem.com
+127.0.0.1       rpserveur.fr
+127.0.0.1       abxcgraovp.pics
+127.0.0.1       sayebrouhk.com
 ```
 
 Change default ports like RDP (3389), Ftp (21), SSH (22) and MySql (3306)
 
 ## Contact
 
 If you have any questions or need assistance that can't be resolved with the [Troubleshooting](#troubleshooting) page, you can reach out on Discord:
```

### Comparing `FiveMCipherFinder-2.6.2/FiveMCipherFinder.egg-info/SOURCES.txt` & `fivemcipherfinder-2.6.3/FiveMCipherFinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.6.2/LICENSE` & `fivemcipherfinder-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.6.2/PKG-INFO` & `fivemcipherfinder-2.6.3/FiveMCipherFinder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FiveMCipherFinder
-Version: 2.6.2
+Version: 2.6.3
 Summary: Finds Cipher in lua scripts.
 Home-page: https://github.com/exersalza/FivemCipherFinder
 Author: exersalza
 License: MIT
 Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
 Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
 Classifier: Intended Audience :: Developers
@@ -13,37 +13,43 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: chardet
 
-# FivemCipherFinder (v2.6.2)
+# FivemCipherFinder (v2.6.3)
 
 <div align="center">
     <h2> Visitors </h2>
     <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint and Flake8](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
 [![PyTest](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![](https://tokei.rs/b1/github/exersalza/fivemcipherfinder)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/fivemcipherfinder?label=pypi%20downloads)
 
 
-- [Installation](#installation)
-- [Usage](#Usage)
-- [Troubleshooting](#Troubleshooting)
-- [Plugins](#Plugins)
-- [Contributing](#Contributing)
-- [Todo](#todo)
-- [Disclaimer](#Disclaimer)
-- [Prevention](#Prevention)
-- [Contact](#Contact)
-- [Credits](#Credits)
+- [FivemCipherFinder (v2.6.3)](#fivemcipherfinder-v263)
+  - [Installation](#installation)
+    - [New version](#new-version)
+    - [Old Version](#old-version)
+  - [Usage](#usage)
+  - [Troubleshooting](#troubleshooting)
+  - [Known False Positives](#known-false-positives)
+  - [Plugins](#plugins)
+  - [Contributing](#contributing)
+  - [Todo](#todo)
+  - [Disclaimer](#disclaimer)
+  - [Prevention](#prevention)
+  - [Contact](#contact)
+  - [Star History](#star-history)
+  - [Credits](#credits)
 
 
 FivemCipherFinder is a tool designed to assist in the removal of Ciphers from your scripts. It is a console-based tool that can be used by anyone, regardless of their coding experience. The main purpose of FivemCipherFinder is to find and identify Ciphers in your script files.
 
 ## Installation
 
 To install FivemCipherFinder, follow these steps:
@@ -142,28 +148,31 @@
 [DISCLAIMER](DISCLAIMER.md)
 
 
 ## Prevention
 
 You can add the following URLs to your hosts file or Firewall. See [here](https://docs.rackspace.com/docs/modify-your-hosts-file) if you're not sure how to edit the hosts file.
 
+Also read [here](https://github.com/ProjecteEndCipher/Cipher-Panel) and [here](https://github.com/ericstolly/cipher) for further information.
+
 ```
-172.0.0.1       cipher-panel.me
-172.0.0.1       ciphercheats.com
-172.0.0.1       keyx.club
-172.0.0.1       dark-utilities.xyz
-172.0.0.1       ketamin.cc
-172.0.0.1       pqzskjptss.shop
-172.0.0.1       admin-panel.sbs
-172.0.0.1       malware-panel.io
-172.0.0.1       docsfivem.com
-172.0.0.1       thedreamofficeem.com
-172.0.0.1       thedreamoffivem.com
-172.0.0.1       rpserveur.fr
-172.0.0.1       abxcgraovp.pics
+127.0.0.1       cipher-panel.me
+127.0.0.1       ciphercheats.com
+127.0.0.1       keyx.club
+127.0.0.1       dark-utilities.xyz
+127.0.0.1       ketamin.cc
+127.0.0.1       pqzskjptss.shop
+127.0.0.1       admin-panel.sbs
+127.0.0.1       malware-panel.io
+127.0.0.1       docsfivem.com
+127.0.0.1       thedreamofficeem.com
+127.0.0.1       thedreamoffivem.com
+127.0.0.1       rpserveur.fr
+127.0.0.1       abxcgraovp.pics
+127.0.0.1       sayebrouhk.com
 ```
 
 Change default ports like RDP (3389), Ftp (21), SSH (22) and MySql (3306)
 
 ## Contact
 
 If you have any questions or need assistance that can't be resolved with the [Troubleshooting](#troubleshooting) page, you can reach out on Discord:
```

### Comparing `FiveMCipherFinder-2.6.2/README.md` & `fivemcipherfinder-2.6.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,55 @@
-# FivemCipherFinder (v2.6.2)
+Metadata-Version: 2.1
+Name: FiveMCipherFinder
+Version: 2.6.3
+Summary: Finds Cipher in lua scripts.
+Home-page: https://github.com/exersalza/FivemCipherFinder
+Author: exersalza
+License: MIT
+Project-URL: Source, https://github.com/exersalza/FivemCipherFinder
+Project-URL: Issues, https://github.com/exersalza/FivemCipherFinder/issues
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: chardet
+
+# FivemCipherFinder (v2.6.3)
 
 <div align="center">
     <h2> Visitors </h2>
     <img src="https://profile-counter.glitch.me/FivemCipherFinder/count.svg" />
 </div>
 
 [![Pylint and Flake8](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pylint.yml)
 [![PyTest](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml/badge.svg)](https://github.com/exersalza/FivemCipherFinder/actions/workflows/pytest.yml)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![](https://tokei.rs/b1/github/exersalza/fivemcipherfinder)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/fivemcipherfinder?label=pypi%20downloads)
 
 
-- [Installation](#installation)
-- [Usage](#Usage)
-- [Troubleshooting](#Troubleshooting)
-- [Plugins](#Plugins)
-- [Contributing](#Contributing)
-- [Todo](#todo)
-- [Disclaimer](#Disclaimer)
-- [Prevention](#Prevention)
-- [Contact](#Contact)
-- [Credits](#Credits)
+- [FivemCipherFinder (v2.6.3)](#fivemcipherfinder-v263)
+  - [Installation](#installation)
+    - [New version](#new-version)
+    - [Old Version](#old-version)
+  - [Usage](#usage)
+  - [Troubleshooting](#troubleshooting)
+  - [Known False Positives](#known-false-positives)
+  - [Plugins](#plugins)
+  - [Contributing](#contributing)
+  - [Todo](#todo)
+  - [Disclaimer](#disclaimer)
+  - [Prevention](#prevention)
+  - [Contact](#contact)
+  - [Star History](#star-history)
+  - [Credits](#credits)
 
 
 FivemCipherFinder is a tool designed to assist in the removal of Ciphers from your scripts. It is a console-based tool that can be used by anyone, regardless of their coding experience. The main purpose of FivemCipherFinder is to find and identify Ciphers in your script files.
 
 ## Installation
 
 To install FivemCipherFinder, follow these steps:
@@ -123,28 +148,31 @@
 [DISCLAIMER](DISCLAIMER.md)
 
 
 ## Prevention
 
 You can add the following URLs to your hosts file or Firewall. See [here](https://docs.rackspace.com/docs/modify-your-hosts-file) if you're not sure how to edit the hosts file.
 
+Also read [here](https://github.com/ProjecteEndCipher/Cipher-Panel) and [here](https://github.com/ericstolly/cipher) for further information.
+
 ```
-172.0.0.1       cipher-panel.me
-172.0.0.1       ciphercheats.com
-172.0.0.1       keyx.club
-172.0.0.1       dark-utilities.xyz
-172.0.0.1       ketamin.cc
-172.0.0.1       pqzskjptss.shop
-172.0.0.1       admin-panel.sbs
-172.0.0.1       malware-panel.io
-172.0.0.1       docsfivem.com
-172.0.0.1       thedreamofficeem.com
-172.0.0.1       thedreamoffivem.com
-172.0.0.1       rpserveur.fr
-172.0.0.1       abxcgraovp.pics
+127.0.0.1       cipher-panel.me
+127.0.0.1       ciphercheats.com
+127.0.0.1       keyx.club
+127.0.0.1       dark-utilities.xyz
+127.0.0.1       ketamin.cc
+127.0.0.1       pqzskjptss.shop
+127.0.0.1       admin-panel.sbs
+127.0.0.1       malware-panel.io
+127.0.0.1       docsfivem.com
+127.0.0.1       thedreamofficeem.com
+127.0.0.1       thedreamoffivem.com
+127.0.0.1       rpserveur.fr
+127.0.0.1       abxcgraovp.pics
+127.0.0.1       sayebrouhk.com
 ```
 
 Change default ports like RDP (3389), Ftp (21), SSH (22) and MySql (3306)
 
 ## Contact
 
 If you have any questions or need assistance that can't be resolved with the [Troubleshooting](#troubleshooting) page, you can reach out on Discord:
```

### Comparing `FiveMCipherFinder-2.6.2/cipherFinder/de_obfs.py` & `fivemcipherfinder-2.6.3/cipherFinder/de_obfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         names.append(name)
         line = line.replace(i.strip(), name)
 
     for v, t in de_obfs_char(ret):
         line = line.replace(t.strip('"'), v)
 
     # Prevent false positives, at least we hope it does
-    if not (table := get_table_contents(line)):
+    if not (table := get_table_contents(line)) or not names:
         return line
 
     t_re = rf"({names[0]}\[\d+\])"
     omfg = set(do_regex(line, t_re))  # as the name tells, it was annoying
 
     for i, c in enumerate(sorted(omfg)):
         line = line.replace(c, table[i])
@@ -169,15 +169,17 @@
     for j in found:
         t = ""
         # Get rid of the x and backslashes.
         for i in (j[0].strip('"').replace("\\", "")).split("x"):
             if not i:
                 continue
 
-            t += chr(int(i, 16))
+            if i not in ["u20"]:
+                t += chr(int(i, 16))
+
         temp.append((t, j[0]))
 
     return temp
 
 
 def de_obfs(ret: list, line: str) -> str:
     """Just another way to entry the de-obfuscation
```

### Comparing `FiveMCipherFinder-2.6.2/cipherFinder/deleter.py` & `fivemcipherfinder-2.6.3/cipherFinder/deleter.py`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.6.2/cipherFinder/finder.py` & `fivemcipherfinder-2.6.3/cipherFinder/finder.py`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.6.2/cipherFinder/plugins.py` & `fivemcipherfinder-2.6.3/cipherFinder/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     "https://raw.githubusercontent.com/exersalza/"
     "FivemCipherFinder/main/plugins/sendWebhook.py",
 ]
 
 VALID_HOOKS = [
     "Init",
     "GetValidatedLines",
-    "GetGibberishCheckMatches",
     "GetLoggingValues",
     "GetFileContents",
     "GetRawFileContents",
     "GetLogFilename",
 ]
```

### Comparing `FiveMCipherFinder-2.6.2/cipherFinder/utils.py` & `fivemcipherfinder-2.6.3/cipherFinder/utils.py`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.6.2/setup.cfg` & `fivemcipherfinder-2.6.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FiveMCipherFinder
-version = 2.6.2
+version = 2.6.3
 description = Finds Cipher in lua scripts.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 author = exersalza
 url = https://github.com/exersalza/FivemCipherFinder
 project_urls =
```

### Comparing `FiveMCipherFinder-2.6.2/tests/test_de_obfs.py` & `fivemcipherfinder-2.6.3/tests/test_de_obfs.py`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.6.2/tests/test_finder.py` & `fivemcipherfinder-2.6.3/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `FiveMCipherFinder-2.6.2/tests/test_utils.py` & `fivemcipherfinder-2.6.3/tests/test_utils.py`

 * *Files identical despite different names*

