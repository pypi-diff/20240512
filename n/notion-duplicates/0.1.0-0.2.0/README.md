# Comparing `tmp/notion_duplicates-0.1.0.tar.gz` & `tmp/notion_duplicates-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notion_duplicates-0.1.0.tar", max compression
+gzip compressed data, was "notion_duplicates-0.2.0.tar", max compression
```

## Comparing `notion_duplicates-0.1.0.tar` & `notion_duplicates-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4484 2024-05-12 03:48:27.080611 notion_duplicates-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-11 20:49:07.405044 notion_duplicates-0.1.0/notion_duplicates/__init__.py
--rw-r--r--   0        0        0     4128 2024-05-12 03:37:33.989807 notion_duplicates-0.1.0/notion_duplicates/notion_duplicates.py
--rw-r--r--   0        0        0      512 2024-05-12 01:56:55.504331 notion_duplicates-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 notion_duplicates-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4925 2024-05-12 04:13:56.655299 notion_duplicates-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-11 20:49:07.405044 notion_duplicates-0.2.0/notion_duplicates/__init__.py
+-rw-r--r--   0        0        0     4128 2024-05-12 03:37:33.989807 notion_duplicates-0.2.0/notion_duplicates/notion_duplicates.py
+-rw-r--r--   0        0        0      512 2024-05-12 04:16:13.564571 notion_duplicates-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 notion_duplicates-0.2.0/PKG-INFO
```

### Comparing `notion_duplicates-0.1.0/README.md` & `notion_duplicates-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 ## Purpose
 
-Detect the duplicated pages in a Notion database and optionally delete the dupes
+**Detect the duplicated pages in a Notion database and optionally delete the dupes**
+
+### What's a duplicated page?
+It's a page with the both same _title_ and _last_edited_time_ as another document.
+
+### Motivation
+I recently decided to move away from Evernote (after being a subsciber since 2008). 
+My reason? They started to jack up their price to a level that wasn't justifiable to me.
+
+After I imported many pages from Evernote, I ended up with 100s if not 1000s of duplicated pages.
+
+This script solved the problem! 
 
 ## Install
 
 ```sh
 pip install notion-duplicates
 ```
```

### Comparing `notion_duplicates-0.1.0/notion_duplicates/notion_duplicates.py` & `notion_duplicates-0.2.0/notion_duplicates/notion_duplicates.py`

 * *Files identical despite different names*

### Comparing `notion_duplicates-0.1.0/pyproject.toml` & `notion_duplicates-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notion-duplicates"
-version = "0.1.0"
+version = "0.2.0"
 description = "Detect duplicated pages in a Notion database and optionallly delete them"
 authors = ["Jerome Provensal <jeromegit@provensal.com>"]
 readme = "README.md"
 packages = [{include = "notion_duplicates"}]
 
 [tool.poetry.scripts]
 notion_duplicates = 'notion_duplicates.notion_duplicates:main'
```

### Comparing `notion_duplicates-0.1.0/PKG-INFO` & `notion_duplicates-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 Metadata-Version: 2.1
 Name: notion-duplicates
-Version: 0.1.0
+Version: 0.2.0
 Summary: Detect duplicated pages in a Notion database and optionallly delete them
 Author: Jerome Provensal
 Author-email: jeromegit@provensal.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: notion-client (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 ## Purpose
 
-Detect the duplicated pages in a Notion database and optionally delete the dupes
+**Detect the duplicated pages in a Notion database and optionally delete the dupes**
+
+### What's a duplicated page?
+It's a page with the both same _title_ and _last_edited_time_ as another document.
+
+### Motivation
+I recently decided to move away from Evernote (after being a subsciber since 2008). 
+My reason? They started to jack up their price to a level that wasn't justifiable to me.
+
+After I imported many pages from Evernote, I ended up with 100s if not 1000s of duplicated pages.
+
+This script solved the problem! 
 
 ## Install
 
 ```sh
 pip install notion-duplicates
 ```
```

