# Comparing `tmp/bibla-2.0.2.tar.gz` & `tmp/bibla-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibla-2.0.2.tar", last modified: Sat May 11 21:24:20 2024, max compression
+gzip compressed data, was "bibla-2.0.3.tar", last modified: Sun May 12 10:52:18 2024, max compression
```

## Comparing `bibla-2.0.2.tar` & `bibla-2.0.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.892944 bibla-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-11 21:24:12.000000 bibla-2.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.884945 bibla-2.0.2/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-11 21:24:12.000000 bibla-2.0.2/.idea/biblint.iml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.884945 bibla-2.0.2/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-11 21:24:12.000000 bibla-2.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-11 21:24:12.000000 bibla-2.0.2/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 21:24:12.000000 bibla-2.0.2/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-11 21:24:12.000000 bibla-2.0.2/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-11 21:24:12.000000 bibla-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-11 21:24:12.000000 bibla-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-11 21:24:20.892944 bibla-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-11 21:24:12.000000 bibla-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.888944 bibla-2.0.2/bibla/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/bibla.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.888944 bibla-2.0.2/bibla/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/database_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/entry_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/field_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/specification_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/rules/text_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-11 21:24:12.000000 bibla-2.0.2/bibla/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.892944 bibla-2.0.2/bibla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 21:24:20.000000 bibla-2.0.2/bibla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 21:24:20.892944 bibla-2.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1581 2024-05-11 21:24:12.000000 bibla-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.888944 bibla-2.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:12.000000 bibla-2.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-11 21:24:12.000000 bibla-2.0.2/test/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:20.892944 bibla-2.0.2/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/.bibla.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/authorNameFormatting.bib
--rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/bibLaTeX.bib
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/dateFormat.bib
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/emptyEntries.bib
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/mit.bib
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/noHomepages.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/nodirectives.bib
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/nokeys.bib
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/originalOverAlias.bib
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/pages.bib
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/required.bib
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/shouldUseDateInsteadOfYearMonthDay.bib
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/syntax.bib
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/unique.bib
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/wrongDateFormat.bib
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-11 21:24:12.000000 bibla-2.0.2/test_data/wrongFormatKey.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:52:18.547110 bibla-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-12 10:52:14.000000 bibla-2.0.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:52:18.539110 bibla-2.0.3/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-12 10:52:14.000000 bibla-2.0.3/.idea/biblint.iml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:52:18.539110 bibla-2.0.3/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-12 10:52:14.000000 bibla-2.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-12 10:52:14.000000 bibla-2.0.3/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-12 10:52:14.000000 bibla-2.0.3/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-12 10:52:14.000000 bibla-2.0.3/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-12 10:52:14.000000 bibla-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-12 10:52:14.000000 bibla-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-12 10:52:18.547110 bibla-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-12 10:52:14.000000 bibla-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:52:18.539110 bibla-2.0.3/bibla/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/bibla.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:52:18.543110 bibla-2.0.3/bibla/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/rules/database_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/rules/entry_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/rules/field_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/rules/specification_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/rules/text_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-12 10:52:14.000000 bibla-2.0.3/bibla/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:52:18.547110 bibla-2.0.3/bibla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-05-12 10:52:18.000000 bibla-2.0.3/bibla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-12 10:52:18.000000 bibla-2.0.3/bibla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 10:52:18.000000 bibla-2.0.3/bibla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-12 10:52:18.000000 bibla-2.0.3/bibla.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-12 10:52:18.000000 bibla-2.0.3/bibla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 10:52:18.000000 bibla-2.0.3/bibla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 10:52:18.547110 bibla-2.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1575 2024-05-12 10:52:14.000000 bibla-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:52:18.543110 bibla-2.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:52:14.000000 bibla-2.0.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-12 10:52:14.000000 bibla-2.0.3/test/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 10:52:18.547110 bibla-2.0.3/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/.bibla.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/authorNameFormatting.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/bibLaTeX.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/dateFormat.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/emptyEntries.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/mit.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/noHomepages.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/nodirectives.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/nokeys.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/originalOverAlias.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/pages.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/required.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/shouldUseDateInsteadOfYearMonthDay.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/syntax.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/unique.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/wrongDateFormat.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-12 10:52:14.000000 bibla-2.0.3/test_data/wrongFormatKey.bib
```

### Comparing `bibla-2.0.2/.idea/biblint.iml` & `bibla-2.0.3/.idea/biblint.iml`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/LICENSE` & `bibla-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/PKG-INFO` & `bibla-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bibla
-Version: 2.0.2
-Summary: A minimalistic bibLaTeX linter based by Tristan Cuvelier.
+Version: 2.0.3
+Summary: A minimalistic bibLaTeX linter by Tristan Cuvelier.
 Home-page: https://github.com/MrClassicT/bibla
 Author: Tristan Cuvelier
 Author-email: tristan.cuvelier@student.hogent.be
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bibla-2.0.2/README.md` & `bibla-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/__main__.py` & `bibla-2.0.3/bibla/__main__.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/bibla.yml` & `bibla-2.0.3/bibla/bibla.yml`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/config.py` & `bibla-2.0.3/bibla/config.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/lint.py` & `bibla-2.0.3/bibla/lint.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/rule.py` & `bibla-2.0.3/bibla/rule.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/rules/database_rules.py` & `bibla-2.0.3/bibla/rules/database_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/rules/entry_rules.py` & `bibla-2.0.3/bibla/rules/entry_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/rules/field_rules.py` & `bibla-2.0.3/bibla/rules/field_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/rules/specification_rules.py` & `bibla-2.0.3/bibla/rules/specification_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/rules/text_rules.py` & `bibla-2.0.3/bibla/rules/text_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla/text_utils.py` & `bibla-2.0.3/bibla/text_utils.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/bibla.egg-info/PKG-INFO` & `bibla-2.0.3/bibla.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bibla
-Version: 2.0.2
-Summary: A minimalistic bibLaTeX linter based by Tristan Cuvelier.
+Version: 2.0.3
+Summary: A minimalistic bibLaTeX linter by Tristan Cuvelier.
 Home-page: https://github.com/MrClassicT/bibla
 Author: Tristan Cuvelier
 Author-email: tristan.cuvelier@student.hogent.be
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bibla-2.0.2/bibla.egg-info/SOURCES.txt` & `bibla-2.0.3/bibla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/setup.py` & `bibla-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = readme.read()
 
 from bibla import __version__
 
 setup(
     name='bibla',
     version=__version__,
-    description='A minimalistic bibLaTeX linter based by Tristan Cuvelier.',
+    description='A minimalistic bibLaTeX linter by Tristan Cuvelier.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/MrClassicT/bibla',
     author='Tristan Cuvelier',
     author_email='tristan.cuvelier@student.hogent.be',
     packages=['bibla', 'bibla.rules'],
     license="MIT",
```

### Comparing `bibla-2.0.2/test_data/bibLaTeX.bib` & `bibla-2.0.3/test_data/bibLaTeX.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/test_data/mit.bib` & `bibla-2.0.3/test_data/mit.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/test_data/nodirectives.bib` & `bibla-2.0.3/test_data/nodirectives.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/test_data/originalOverAlias.bib` & `bibla-2.0.3/test_data/originalOverAlias.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.2/test_data/wrongDateFormat.bib` & `bibla-2.0.3/test_data/wrongDateFormat.bib`

 * *Files identical despite different names*

