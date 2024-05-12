# Comparing `tmp/pki_tools-1.0.0.tar.gz` & `tmp/pki_tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pki_tools-1.0.0.tar", max compression
+gzip compressed data, was "pki_tools-1.0.1.tar", max compression
```

## Comparing `pki_tools-1.0.0.tar` & `pki_tools-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1096 2024-04-13 12:56:09.562684 pki_tools-1.0.0/LICENSE
--rw-r--r--   0        0        0     1967 2024-04-13 12:56:09.562684 pki_tools-1.0.0/README.md
--rw-r--r--   0        0        0     1321 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/__init__.py
--rw-r--r--   0        0        0     1798 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/crl.py
--rw-r--r--   0        0        0     1397 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/exceptions.py
--rw-r--r--   0        0        0       70 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/funcs/__init__.py
--rw-r--r--   0        0        0     5448 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/funcs/check_revocation.py
--rw-r--r--   0        0        0     5227 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/ocsp.py
--rw-r--r--   0        0        0     1637 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/types/__init__.py
--rw-r--r--   0        0        0    14191 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/types/certificate.py
--rw-r--r--   0        0        0     4652 2024-04-13 12:56:09.570684 pki_tools-1.0.0/pki_tools/types/certificates.py
--rw-r--r--   0        0        0     3158 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/chain.py
--rw-r--r--   0        0        0     7794 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/crl.py
--rw-r--r--   0        0        0     7023 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/crypto_parser.py
--rw-r--r--   0        0        0     6351 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/csr.py
--rw-r--r--   0        0        0      462 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/enums.py
--rw-r--r--   0        0        0    50236 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/extensions.py
--rw-r--r--   0        0        0    26475 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/key_pair.py
--rw-r--r--   0        0        0     4292 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/name.py
--rw-r--r--   0        0        0    12326 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/ocsp.py
--rw-r--r--   0        0        0     9779 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/signature_algorithm.py
--rw-r--r--   0        0        0     1940 2024-04-13 12:56:09.574684 pki_tools-1.0.0/pki_tools/types/utils.py
--rw-r--r--   0        0        0     1800 2024-04-13 12:56:18.318687 pki_tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 pki_tools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-12 19:18:58.214255 pki_tools-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1967 2024-05-12 19:18:58.214255 pki_tools-1.0.1/README.md
+-rw-r--r--   0        0        0     1321 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/__init__.py
+-rw-r--r--   0        0        0     1798 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/crl.py
+-rw-r--r--   0        0        0     1397 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/exceptions.py
+-rw-r--r--   0        0        0       70 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/funcs/__init__.py
+-rw-r--r--   0        0        0     5448 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/funcs/check_revocation.py
+-rw-r--r--   0        0        0     5227 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/ocsp.py
+-rw-r--r--   0        0        0     1637 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/__init__.py
+-rw-r--r--   0        0        0    14191 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/certificate.py
+-rw-r--r--   0        0        0     4652 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/certificates.py
+-rw-r--r--   0        0        0     3158 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/chain.py
+-rw-r--r--   0        0        0     7794 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/crl.py
+-rw-r--r--   0        0        0     7023 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/crypto_parser.py
+-rw-r--r--   0        0        0     6351 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/csr.py
+-rw-r--r--   0        0        0      462 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/enums.py
+-rw-r--r--   0        0        0    50236 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/extensions.py
+-rw-r--r--   0        0        0    26475 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/key_pair.py
+-rw-r--r--   0        0        0     4292 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/name.py
+-rw-r--r--   0        0        0    12326 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/ocsp.py
+-rw-r--r--   0        0        0     9779 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/signature_algorithm.py
+-rw-r--r--   0        0        0     1940 2024-05-12 19:18:58.222255 pki_tools-1.0.1/pki_tools/types/utils.py
+-rw-r--r--   0        0        0     1798 2024-05-12 19:19:04.202203 pki_tools-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 pki_tools-1.0.1/PKG-INFO
```

### Comparing `pki_tools-1.0.0/LICENSE` & `pki_tools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/README.md` & `pki_tools-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/__init__.py` & `pki_tools-1.0.1/pki_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/crl.py` & `pki_tools-1.0.1/pki_tools/crl.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/exceptions.py` & `pki_tools-1.0.1/pki_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/funcs/check_revocation.py` & `pki_tools-1.0.1/pki_tools/funcs/check_revocation.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/ocsp.py` & `pki_tools-1.0.1/pki_tools/ocsp.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/__init__.py` & `pki_tools-1.0.1/pki_tools/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/certificate.py` & `pki_tools-1.0.1/pki_tools/types/certificate.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/certificates.py` & `pki_tools-1.0.1/pki_tools/types/certificates.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/chain.py` & `pki_tools-1.0.1/pki_tools/types/chain.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/crl.py` & `pki_tools-1.0.1/pki_tools/types/crl.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/crypto_parser.py` & `pki_tools-1.0.1/pki_tools/types/crypto_parser.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/csr.py` & `pki_tools-1.0.1/pki_tools/types/csr.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/extensions.py` & `pki_tools-1.0.1/pki_tools/types/extensions.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/key_pair.py` & `pki_tools-1.0.1/pki_tools/types/key_pair.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/name.py` & `pki_tools-1.0.1/pki_tools/types/name.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/ocsp.py` & `pki_tools-1.0.1/pki_tools/types/ocsp.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/signature_algorithm.py` & `pki_tools-1.0.1/pki_tools/types/signature_algorithm.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pki_tools/types/utils.py` & `pki_tools-1.0.1/pki_tools/types/utils.py`

 * *Files identical despite different names*

### Comparing `pki_tools-1.0.0/pyproject.toml` & `pki_tools-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pki-tools"
-version = "1.0.0"
+version = "1.0.1"
 description = "PKI tools for e.g. checking certificate CRL/OCSP revocation"
 authors = ["Michal Sadowski <misad90@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
@@ -18,38 +18,38 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/fulder/pki-tools/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 cryptography = ">=39.0.1,<43.0.0"
 loguru = "^0.7.2"
-pydantic = "^2.7.0"
+pydantic = "^2.7.1"
 httpx = "^0.27.0"
 pyyaml = "^6.0.1"
 pytz = "^2024.1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "^8.1.1"
+pytest = "^8.2.0"
 pytest-mock = "^3.14.0"
-pytest-xdist = "^3.5.0"
+pytest-xdist = "^3.6.1"
 pytest-cov = "^5.0.0"
 smokeshow = "^0.4.0"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
-ruff = ">=0.0.289,<0.3.8"
+ruff = ">=0.0.289,<0.4.4"
 
 [tool.poetry.group.dev.dependencies]
-mkdocstrings = {extras = ["python"], version = "^0.24.3"}
-pymdown-extensions = "^10.7.1"
+mkdocstrings = {extras = ["python"], version = "^0.25.1"}
+pymdown-extensions = "^10.8"
 
 [tool.poetry.group.apitest.dependencies]
 httpx = "^0.27.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

### Comparing `pki_tools-1.0.0/PKG-INFO` & `pki_tools-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pki-tools
-Version: 1.0.0
+Version: 1.0.1
 Summary: PKI tools for e.g. checking certificate CRL/OCSP revocation
 Home-page: https://github.com/fulder/pki-tools
 License: MIT
 Author: Michal Sadowski
 Author-email: misad90@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security :: Cryptography
 Requires-Dist: cryptography (>=39.0.1,<43.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: pydantic (>=2.7.0,<3.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Project-URL: Bug Tracker, https://github.com/fulder/pki-tools/issues
 Project-URL: Repository, https://github.com/fulder/pki-tools
 Description-Content-Type: text/markdown
 
 [![Python Badge](https://img.shields.io/badge/python-3.8%2B-7393B3.svg?logo=python&logoColor=white)](https://devguide.python.org/versions/)
```

