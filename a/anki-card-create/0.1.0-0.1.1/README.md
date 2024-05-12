# Comparing `tmp/anki_card_create-0.1.0.tar.gz` & `tmp/anki_card_create-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anki_card_create-0.1.0.tar", max compression
+gzip compressed data, was "anki_card_create-0.1.1.tar", max compression
```

## Comparing `anki_card_create-0.1.0.tar` & `anki_card_create-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      565 2024-05-06 09:06:07.081513 anki_card_create-0.1.0/README.md
--rw-r--r--   0        0        0      947 2024-05-11 09:11:41.634361 anki_card_create-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      220 2024-05-06 01:38:51.729666 anki_card_create-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     1575 2024-05-04 09:24:22.849971 anki_card_create-0.1.0/src/ankicard.py
--rw-r--r--   0        0        0     6242 2024-05-11 02:52:46.669977 anki_card_create-0.1.0/src/card_creator.py
--rw-r--r--   0        0        0     1768 2024-05-02 08:36:19.769201 anki_card_create-0.1.0/src/models.py
--rw-r--r--   0        0        0     2267 2024-05-11 02:52:46.188800 anki_card_create-0.1.0/src/utils.py
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 anki_card_create-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      496 2024-05-12 04:28:01.633979 anki_card_create-0.1.1/README.md
+-rw-r--r--   0        0        0      947 2024-05-12 04:40:49.400235 anki_card_create-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      220 2024-05-06 01:38:51.729666 anki_card_create-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0     1575 2024-05-04 09:24:22.849971 anki_card_create-0.1.1/src/ankicard.py
+-rw-r--r--   0        0        0     6242 2024-05-11 02:52:46.669977 anki_card_create-0.1.1/src/card_creator.py
+-rw-r--r--   0        0        0     1768 2024-05-02 08:36:19.769201 anki_card_create-0.1.1/src/models.py
+-rw-r--r--   0        0        0     2267 2024-05-11 02:52:46.188800 anki_card_create-0.1.1/src/utils.py
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 anki_card_create-0.1.1/PKG-INFO
```

### Comparing `anki_card_create-0.1.0/pyproject.toml` & `anki_card_create-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anki-card-create"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Kuroflectr <ike.kuroflectr@gmail.com>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `anki_card_create-0.1.0/src/ankicard.py` & `anki_card_create-0.1.1/src/ankicard.py`

 * *Files identical despite different names*

### Comparing `anki_card_create-0.1.0/src/card_creator.py` & `anki_card_create-0.1.1/src/card_creator.py`

 * *Files identical despite different names*

### Comparing `anki_card_create-0.1.0/src/models.py` & `anki_card_create-0.1.1/src/models.py`

 * *Files identical despite different names*

### Comparing `anki_card_create-0.1.0/src/utils.py` & `anki_card_create-0.1.1/src/utils.py`

 * *Files identical despite different names*

### Comparing `anki_card_create-0.1.0/PKG-INFO` & `anki_card_create-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anki-card-create
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Kuroflectr
 Author-email: ike.kuroflectr@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: googletrans (==4.0.0rc1)
@@ -18,17 +18,15 @@
 
 Add anki cards with audios (korean vocabulary) simply with only one command: `kanki`.
 
 ## Package setup
 
 Set up the package using: 
 ```
-git clone https://github.com/Kuroflectr/anki-card-create.git
-cd ./anki-card-create
-poetry install
+pip install anki-card-create
 ```
 
 ## Usage
 
 1. Ensure that Anki has been running in the background. 
 
 2. Ensure that anki-connect has been installed.
```

