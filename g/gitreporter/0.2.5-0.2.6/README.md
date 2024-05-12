# Comparing `tmp/gitreporter-0.2.5.tar.gz` & `tmp/gitreporter-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitreporter-0.2.5.tar", last modified: Sun Apr 21 10:06:13 2024, max compression
+gzip compressed data, was "gitreporter-0.2.6.tar", last modified: Sun May 12 09:18:15 2024, max compression
```

## Comparing `gitreporter-0.2.5.tar` & `gitreporter-0.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-21 10:06:13.088718 gitreporter-0.2.5/
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)    35149 2023-12-11 09:15:58.000000 gitreporter-0.2.5/LICENSE
--rw-r--r--   0 michgutt  (1000) michgutt  (1000)      946 2024-04-21 10:06:13.088718 gitreporter-0.2.5/PKG-INFO
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      456 2024-02-29 18:25:07.000000 gitreporter-0.2.5/README.md
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      681 2024-04-21 10:05:57.000000 gitreporter-0.2.5/pyproject.toml
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       38 2024-04-21 10:06:13.088718 gitreporter-0.2.5/setup.cfg
-drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-21 10:06:13.080718 gitreporter-0.2.5/src/
-drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-21 10:06:13.084718 gitreporter-0.2.5/src/gitreporter/
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)        0 2024-02-02 20:03:19.000000 gitreporter-0.2.5/src/gitreporter/__init__.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5089 2024-04-21 10:05:50.000000 gitreporter-0.2.5/src/gitreporter/__main__.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5841 2023-12-10 10:14:49.000000 gitreporter-0.2.5/src/gitreporter/commit.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     1139 2023-12-10 10:14:49.000000 gitreporter-0.2.5/src/gitreporter/commit_statistic.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     3448 2024-02-29 17:34:10.000000 gitreporter-0.2.5/src/gitreporter/config.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     7874 2024-02-24 11:52:10.000000 gitreporter-0.2.5/src/gitreporter/diff.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     4726 2024-02-22 20:01:42.000000 gitreporter-0.2.5/src/gitreporter/file.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      814 2024-03-03 19:40:52.000000 gitreporter-0.2.5/src/gitreporter/progressbar.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     8672 2024-04-21 09:55:34.000000 gitreporter-0.2.5/src/gitreporter/report.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5858 2024-03-14 16:43:21.000000 gitreporter-0.2.5/src/gitreporter/repository.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     4386 2024-01-27 18:05:26.000000 gitreporter-0.2.5/src/gitreporter/repository_statistic.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     6099 2023-12-10 10:14:49.000000 gitreporter-0.2.5/src/gitreporter/statistic_values.py
-drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-21 10:06:13.088718 gitreporter-0.2.5/src/gitreporter/templates/
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)    15110 2024-01-31 19:01:49.000000 gitreporter-0.2.5/src/gitreporter/templates/report_template.mustache
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     2281 2024-02-22 19:46:43.000000 gitreporter-0.2.5/src/gitreporter/textline.py
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      689 2024-01-31 19:01:49.000000 gitreporter-0.2.5/src/gitreporter/types.py
-drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-04-21 10:06:13.088718 gitreporter-0.2.5/src/gitreporter.egg-info/
--rw-r--r--   0 michgutt  (1000) michgutt  (1000)      946 2024-04-21 10:06:13.000000 gitreporter-0.2.5/src/gitreporter.egg-info/PKG-INFO
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      727 2024-04-21 10:06:13.000000 gitreporter-0.2.5/src/gitreporter.egg-info/SOURCES.txt
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)        1 2024-04-21 10:06:13.000000 gitreporter-0.2.5/src/gitreporter.egg-info/dependency_links.txt
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       58 2024-04-21 10:06:13.000000 gitreporter-0.2.5/src/gitreporter.egg-info/entry_points.txt
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       78 2024-04-21 10:06:13.000000 gitreporter-0.2.5/src/gitreporter.egg-info/requires.txt
--rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       12 2024-04-21 10:06:13.000000 gitreporter-0.2.5/src/gitreporter.egg-info/top_level.txt
+drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-05-12 09:18:15.784143 gitreporter-0.2.6/
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)    35149 2023-12-11 09:15:58.000000 gitreporter-0.2.6/LICENSE
+-rw-r--r--   0 michgutt  (1000) michgutt  (1000)      946 2024-05-12 09:18:15.784143 gitreporter-0.2.6/PKG-INFO
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      456 2024-02-29 18:25:07.000000 gitreporter-0.2.6/README.md
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      681 2024-05-12 09:13:41.000000 gitreporter-0.2.6/pyproject.toml
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       38 2024-05-12 09:18:15.784143 gitreporter-0.2.6/setup.cfg
+drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-05-12 09:18:15.780142 gitreporter-0.2.6/src/
+drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-05-12 09:18:15.780142 gitreporter-0.2.6/src/gitreporter/
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)        0 2024-02-02 20:03:19.000000 gitreporter-0.2.6/src/gitreporter/__init__.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5125 2024-05-12 09:14:09.000000 gitreporter-0.2.6/src/gitreporter/__main__.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5841 2023-12-10 10:14:49.000000 gitreporter-0.2.6/src/gitreporter/commit.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     1139 2023-12-10 10:14:49.000000 gitreporter-0.2.6/src/gitreporter/commit_statistic.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     3448 2024-02-29 17:34:10.000000 gitreporter-0.2.6/src/gitreporter/config.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     7874 2024-02-24 11:52:10.000000 gitreporter-0.2.6/src/gitreporter/diff.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     4726 2024-02-22 20:01:42.000000 gitreporter-0.2.6/src/gitreporter/file.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      814 2024-03-03 19:40:52.000000 gitreporter-0.2.6/src/gitreporter/progressbar.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     8689 2024-05-12 09:09:05.000000 gitreporter-0.2.6/src/gitreporter/report.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     5858 2024-03-14 16:43:21.000000 gitreporter-0.2.6/src/gitreporter/repository.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     4402 2024-05-12 09:11:52.000000 gitreporter-0.2.6/src/gitreporter/repository_statistic.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     6099 2023-12-10 10:14:49.000000 gitreporter-0.2.6/src/gitreporter/statistic_values.py
+drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-05-12 09:18:15.784143 gitreporter-0.2.6/src/gitreporter/templates/
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)    15110 2024-01-31 19:01:49.000000 gitreporter-0.2.6/src/gitreporter/templates/report_template.mustache
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)     2281 2024-02-22 19:46:43.000000 gitreporter-0.2.6/src/gitreporter/textline.py
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      689 2024-01-31 19:01:49.000000 gitreporter-0.2.6/src/gitreporter/types.py
+drwxrwxr-x   0 michgutt  (1000) michgutt  (1000)        0 2024-05-12 09:18:15.784143 gitreporter-0.2.6/src/gitreporter.egg-info/
+-rw-r--r--   0 michgutt  (1000) michgutt  (1000)      946 2024-05-12 09:18:15.000000 gitreporter-0.2.6/src/gitreporter.egg-info/PKG-INFO
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)      727 2024-05-12 09:18:15.000000 gitreporter-0.2.6/src/gitreporter.egg-info/SOURCES.txt
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)        1 2024-05-12 09:18:15.000000 gitreporter-0.2.6/src/gitreporter.egg-info/dependency_links.txt
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       58 2024-05-12 09:18:15.000000 gitreporter-0.2.6/src/gitreporter.egg-info/entry_points.txt
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       78 2024-05-12 09:18:15.000000 gitreporter-0.2.6/src/gitreporter.egg-info/requires.txt
+-rw-rw-r--   0 michgutt  (1000) michgutt  (1000)       12 2024-05-12 09:18:15.000000 gitreporter-0.2.6/src/gitreporter.egg-info/top_level.txt
```

### Comparing `gitreporter-0.2.5/LICENSE` & `gitreporter-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/PKG-INFO` & `gitreporter-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitreporter
-Version: 0.2.5
+Version: 0.2.6
 Summary: Git Analysis Tool
 Author-email: Michael Guttmann <michael.guttmann@live.at>
 Project-URL: Homepage, https://github.com/Migutti/GitReporter
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gitreporter-0.2.5/pyproject.toml` & `gitreporter-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitreporter"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Michael Guttmann", email="michael.guttmann@live.at" },
 ]
 description = "Git Analysis Tool"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `gitreporter-0.2.5/src/gitreporter/__main__.py` & `gitreporter-0.2.6/src/gitreporter/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,34 +120,34 @@
         help="check for comments and coding standard (currently only supported for c-like languages)",
         dest="comments-and-coding-standard"
     )
 
     return vars(parser.parse_args(sys.argv[1:] if len(sys.argv) > 1 else ["-h"]))
 
 def main():
-    print("Gitreporter 0.2.5")
+    print("GitReporter 0.2.6")
 
     args = parse_arguments()
     if args["create-config"]:
         if not args["config"]:
             print("error: specify a path to the configuration file with -c.")
             exit(-1)
         try:
-            with open(args["config"], "w") as f:
+            with open(args["config"], "w", encoding='utf-8') as f:
                 json.dump(Config.DEFAULT_CONFIG, f, indent=4)
         except:
             print("error: could not create configuration file.")
             exit(-1)
         print(f"created configuration file at {args['config']}")
         exit(0)
 
     options = copy.copy(Config.DEFAULT_CONFIG)
     if args["config"]:
         try:
-            with open(args["config"], "r") as f:
+            with open(args["config"], "r", encoding='utf-8') as f:
                 config_file = json.load(f)
         except:
             print("error: could not open configuration file.")
             exit(-1)
 
         for key, value in config_file.items():
             if key not in options:
```

### Comparing `gitreporter-0.2.5/src/gitreporter/commit.py` & `gitreporter-0.2.6/src/gitreporter/commit.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter/commit_statistic.py` & `gitreporter-0.2.6/src/gitreporter/commit_statistic.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter/config.py` & `gitreporter-0.2.6/src/gitreporter/config.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter/diff.py` & `gitreporter-0.2.6/src/gitreporter/diff.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter/file.py` & `gitreporter-0.2.6/src/gitreporter/file.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter/progressbar.py` & `gitreporter-0.2.6/src/gitreporter/progressbar.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter/report.py` & `gitreporter-0.2.6/src/gitreporter/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 dictionary |= {
                     'line-mapping': []
                 }
             self.generate_html(f"files/{file.replace('.', '_').replace('/', '_')}", "report_template", dictionary)
 
     def generate_html(self, html_name, template_name, dictionary):
         template = files('gitreporter.templates').joinpath(f'{template_name}.mustache').read_text()
-        with open(f'gitreport/{html_name}.html', 'w', encoding='utf-8') as g:
+        with open(f'gitreport/{html_name}.html', 'w', encoding='utf-8', errors='ignore') as g:
             g.write(chevron.render(template, dictionary))
 
     def data_with_ref(self, data, reference):
         if reference is None:
             return f'{data}' + 9 * ' '
         return f'{data} ({data / reference * 100 if reference != 0 else 0.0:5.1f}%)'
```

### Comparing `gitreporter-0.2.5/src/gitreporter/repository.py` & `gitreporter-0.2.6/src/gitreporter/repository.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter/repository_statistic.py` & `gitreporter-0.2.6/src/gitreporter/repository_statistic.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,20 +79,22 @@
 
                 self.totals[RepoCategory.SURVIVED_LINES][line.get_type()] += 1
                 total[RepoCategory.SURVIVED_LINES][line.get_type()] += 1
 
                 self.authors[email][RepoCategory.SURVIVED_LINES][line.get_type()] += 1
                 self.authors_per_file[email][filename][RepoCategory.SURVIVED_LINES][line.get_type()] += 1
 
+    """
     def create_json(self, write_to_file=False):
         results = {
             "Options": self.config.get_options_with_datetime_string(),
             "Totals": self.totals,
             "Totals Authors": self.authors,
             "Totals per File": self.totals_per_file,
             "Authors per File": self.authors_per_file
         }
         if write_to_file:
             with open('report.json', 'w') as f:
                 f.write(json.dumps(results, indent=4))
 
         return results
+    """
```

### Comparing `gitreporter-0.2.5/src/gitreporter/statistic_values.py` & `gitreporter-0.2.6/src/gitreporter/statistic_values.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter/templates/report_template.mustache` & `gitreporter-0.2.6/src/gitreporter/templates/report_template.mustache`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter/textline.py` & `gitreporter-0.2.6/src/gitreporter/textline.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter/types.py` & `gitreporter-0.2.6/src/gitreporter/types.py`

 * *Files identical despite different names*

### Comparing `gitreporter-0.2.5/src/gitreporter.egg-info/PKG-INFO` & `gitreporter-0.2.6/src/gitreporter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitreporter
-Version: 0.2.5
+Version: 0.2.6
 Summary: Git Analysis Tool
 Author-email: Michael Guttmann <michael.guttmann@live.at>
 Project-URL: Homepage, https://github.com/Migutti/GitReporter
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gitreporter-0.2.5/src/gitreporter.egg-info/SOURCES.txt` & `gitreporter-0.2.6/src/gitreporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

