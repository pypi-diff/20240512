# Comparing `tmp/var_print-0.0.8.tar.gz` & `tmp/var_print-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "var_print-0.0.8.tar", last modified: Mon Oct  2 08:02:51 2023, max compression
+gzip compressed data, was "var_print-0.0.9.tar", last modified: Sun May 12 12:26:06 2024, max compression
```

## Comparing `var_print-0.0.8.tar` & `var_print-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-10-02 08:02:51.852552 var_print-0.0.8/
--rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 var_print-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      159 2023-01-07 18:55:43.000000 var_print-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     5750 2023-10-02 08:02:51.851552 var_print-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4986 2023-01-07 18:59:14.000000 var_print-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-10-02 08:02:51.852552 var_print-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1803 2023-10-02 08:02:04.000000 var_print-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-02 08:02:51.838551 var_print-0.0.8/var_print/
--rw-rw-rw-   0        0        0       78 2023-10-02 08:02:00.000000 var_print-0.0.8/var_print/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-02 08:02:51.848551 var_print-0.0.8/var_print/data/
--rw-rw-rw-   0        0        0     6221 2023-01-07 18:45:09.000000 var_print-0.0.8/var_print/data/color_schemes.pickle
--rw-rw-rw-   0        0        0    45043 2023-10-02 08:01:51.000000 var_print-0.0.8/var_print/varPrint.py
-drwxrwxrwx   0        0        0        0 2023-10-02 08:02:51.847552 var_print-0.0.8/var_print.egg-info/
--rw-rw-rw-   0        0        0     5750 2023-10-02 08:02:51.000000 var_print-0.0.8/var_print.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-10-02 08:02:51.000000 var_print-0.0.8/var_print.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-02 08:02:51.000000 var_print-0.0.8/var_print.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-10-02 08:02:51.000000 var_print-0.0.8/var_print.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-10-02 08:02:51.000000 var_print-0.0.8/var_print.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 12:26:06.427477 var_print-0.0.9/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:45:09.000000 var_print-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      159 2023-01-07 18:55:43.000000 var_print-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     5750 2024-05-12 12:26:06.426480 var_print-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4986 2023-01-07 18:59:14.000000 var_print-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-12 12:26:06.427477 var_print-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1803 2024-05-12 12:25:09.000000 var_print-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:26:06.413357 var_print-0.0.9/var_print/
+-rw-rw-rw-   0        0        0       78 2024-05-12 12:25:06.000000 var_print-0.0.9/var_print/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:26:06.423463 var_print-0.0.9/var_print/data/
+-rw-rw-rw-   0        0        0     6221 2023-01-07 18:45:09.000000 var_print-0.0.9/var_print/data/color_schemes.pickle
+-rw-rw-rw-   0        0        0    45722 2024-05-12 12:24:25.000000 var_print-0.0.9/var_print/varPrint.py
+drwxrwxrwx   0        0        0        0 2024-05-12 12:26:06.421363 var_print-0.0.9/var_print.egg-info/
+-rw-rw-rw-   0        0        0     5750 2024-05-12 12:26:06.000000 var_print-0.0.9/var_print.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-05-12 12:26:06.000000 var_print-0.0.9/var_print.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 12:26:06.000000 var_print-0.0.9/var_print.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-12 12:26:06.000000 var_print-0.0.9/var_print.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-12 12:26:06.000000 var_print-0.0.9/var_print.egg-info/top_level.txt
```

### Comparing `var_print-0.0.8/LICENSE` & `var_print-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `var_print-0.0.8/PKG-INFO` & `var_print-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: var_print
-Version: 0.0.8
+Version: 0.0.9
 Summary: Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. 
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `var_print-0.0.8/README.md` & `var_print-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `var_print-0.0.8/setup.py` & `var_print-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 DESCRIPTION = "Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. "
 
 # Setting up
 setup(
     name="var_print",
     version=VERSION,
     author="André Herber",
```

### Comparing `var_print-0.0.8/var_print/data/color_schemes.pickle` & `var_print-0.0.9/var_print/data/color_schemes.pickle`

 * *Files identical despite different names*

### Comparing `var_print-0.0.8/var_print/varPrint.py` & `var_print-0.0.9/var_print/varPrint.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,14 +329,35 @@
             l = len(out.split("\n")) - 1
             for i, line in enumerate(out.split("\n")):
                 if i < l:
                     print(line)
                 else:
                     colored_print(line)
             return out
+        
+    def get_formated_output(self, *vars, colored=None) -> None:
+        if colored != None:
+            prev_colored = self.colored
+            self.colored = colored
+        try:
+            var_names = self.get_var_names()
+        except:
+            var_names = [f"{type(v)}" for v in vars]
+
+        kwargs = {k: vars[i] for (i, k) in enumerate(var_names)}
+
+        if len(kwargs) > 0:
+            out = self.format_vars_and_args(kwargs)
+        else:
+            out = f"Testing varp: {Fore.CYAN} date and time: {Fore.get_rainbow_string(aktuelle_Zeit())}"
+
+        if colored != None:
+            self.colored = prev_colored
+
+        return out
 
     def get_var_names(self, frame=2):
         if frame == 1:
             callFrame = inspect.currentframe().f_back
         elif frame == 2:
             callFrame = inspect.currentframe().f_back.f_back
         elif frame == 3:
```

### Comparing `var_print-0.0.8/var_print.egg-info/PKG-INFO` & `var_print-0.0.9/var_print.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: var-print
-Version: 0.0.8
+Version: 0.0.9
 Summary: Nicer printing with var_print: Colours and structure allow quick reading of the output, at the same time the name of the variable is displayed. 
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

