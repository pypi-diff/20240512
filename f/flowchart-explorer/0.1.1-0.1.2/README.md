# Comparing `tmp/flowchart_explorer-0.1.1.tar.gz` & `tmp/flowchart_explorer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchart_explorer-0.1.1.tar", max compression
+gzip compressed data, was "flowchart_explorer-0.1.2.tar", max compression
```

## Comparing `flowchart_explorer-0.1.1.tar` & `flowchart_explorer-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      100 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     1055 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/LICENSE
--rw-r--r--   0        0        0      229 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/README.md
--rw-r--r--   0        0        0       22 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/__init__.py
--rw-r--r--   0        0        0     2274 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/chartpath.py
--rw-r--r--   0        0        0     5238 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/explorer.py
--rw-r--r--   0        0        0        0 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/flowchartdiagrams/__init__.py
--rw-r--r--   0        0        0     2488 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/flowchartdiagrams/nodes.py
--rw-r--r--   0        0        0        0 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/graph/__init__.py
--rw-r--r--   0        0        0    11225 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/graph/drawio.py
--rw-r--r--   0        0        0     1823 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/flowchart_explorer/methods.py
--rw-r--r--   0        0        0     2680 2024-05-06 02:05:08.980983 flowchart_explorer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 flowchart_explorer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      100 2024-05-12 07:57:00.299538 flowchart_explorer-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1055 2024-05-12 07:57:00.299538 flowchart_explorer-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4600 2024-05-12 07:57:00.299538 flowchart_explorer-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-12 07:57:00.303538 flowchart_explorer-0.1.2/flowchart_explorer/__init__.py
+-rw-r--r--   0        0        0     2274 2024-05-12 07:57:00.303538 flowchart_explorer-0.1.2/flowchart_explorer/chartpath.py
+-rw-r--r--   0        0        0     5238 2024-05-12 07:57:00.303538 flowchart_explorer-0.1.2/flowchart_explorer/explorer.py
+-rw-r--r--   0        0        0        0 2024-05-12 07:57:00.303538 flowchart_explorer-0.1.2/flowchart_explorer/flowchartdiagrams/__init__.py
+-rw-r--r--   0        0        0     2488 2024-05-12 07:57:00.303538 flowchart_explorer-0.1.2/flowchart_explorer/flowchartdiagrams/nodes.py
+-rw-r--r--   0        0        0        0 2024-05-12 07:57:00.303538 flowchart_explorer-0.1.2/flowchart_explorer/graph/__init__.py
+-rw-r--r--   0        0        0    11225 2024-05-12 07:57:00.303538 flowchart_explorer-0.1.2/flowchart_explorer/graph/drawio.py
+-rw-r--r--   0        0        0     1823 2024-05-12 07:57:00.307538 flowchart_explorer-0.1.2/flowchart_explorer/methods.py
+-rw-r--r--   0        0        0     2680 2024-05-12 07:57:00.307538 flowchart_explorer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5355 1970-01-01 00:00:00.000000 flowchart_explorer-0.1.2/PKG-INFO
```

### Comparing `flowchart_explorer-0.1.1/LICENSE` & `flowchart_explorer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchart_explorer-0.1.1/flowchart_explorer/chartpath.py` & `flowchart_explorer-0.1.2/flowchart_explorer/chartpath.py`

 * *Files identical despite different names*

### Comparing `flowchart_explorer-0.1.1/flowchart_explorer/explorer.py` & `flowchart_explorer-0.1.2/flowchart_explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `flowchart_explorer-0.1.1/flowchart_explorer/flowchartdiagrams/nodes.py` & `flowchart_explorer-0.1.2/flowchart_explorer/flowchartdiagrams/nodes.py`

 * *Files identical despite different names*

### Comparing `flowchart_explorer-0.1.1/flowchart_explorer/graph/drawio.py` & `flowchart_explorer-0.1.2/flowchart_explorer/graph/drawio.py`

 * *Files identical despite different names*

### Comparing `flowchart_explorer-0.1.1/flowchart_explorer/methods.py` & `flowchart_explorer-0.1.2/flowchart_explorer/methods.py`

 * *Files identical despite different names*

### Comparing `flowchart_explorer-0.1.1/pyproject.toml` & `flowchart_explorer-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flowchart_explorer"
-version = "0.1.1"
+version = "0.1.2"
 description = "FlowChart Explorer is a GitHub-integrated tool that analyzes all execution paths in a flowchart. It helps identify bottlenecks and redundancies in your codebase, providing a new level of clarity and control."
 authors = ["sabi2345"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sabi2345/flowchart-explorer"
 
 include = ["CHANGELOG.md"]
```

