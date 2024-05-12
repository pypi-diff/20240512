# Comparing `tmp/hplc_data_analysis-1.0.4.tar.gz` & `tmp/hplc_data_analysis-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hplc_data_analysis-1.0.4.tar", last modified: Fri Feb 16 20:27:46 2024, max compression
+gzip compressed data, was "hplc_data_analysis-1.0.5.tar", last modified: Fri Feb 16 20:31:59 2024, max compression
```

## Comparing `hplc_data_analysis-1.0.4.tar` & `hplc_data_analysis-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-02-16 20:27:46.859527 hplc_data_analysis-1.0.4/
--rw-rw-rw-   0        0        0     3529 2024-02-16 20:27:46.855541 hplc_data_analysis-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2857 2024-02-15 15:07:23.000000 hplc_data_analysis-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-16 20:27:46.828616 hplc_data_analysis-1.0.4/hplc_data_analysis/
--rw-rw-rw-   0        0        0       25 2024-01-30 22:54:45.000000 hplc_data_analysis-1.0.4/hplc_data_analysis/__init__.py
--rw-rw-rw-   0        0        0   101726 2024-02-16 20:26:05.000000 hplc_data_analysis-1.0.4/hplc_data_analysis/main.py
-drwxrwxrwx   0        0        0        0 2024-02-16 20:27:46.851554 hplc_data_analysis-1.0.4/hplc_data_analysis.egg-info/
--rw-rw-rw-   0        0        0     3529 2024-02-16 20:27:46.000000 hplc_data_analysis-1.0.4/hplc_data_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-02-16 20:27:46.000000 hplc_data_analysis-1.0.4/hplc_data_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-16 20:27:46.000000 hplc_data_analysis-1.0.4/hplc_data_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-02-16 20:27:46.000000 hplc_data_analysis-1.0.4/hplc_data_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-02-16 20:27:46.000000 hplc_data_analysis-1.0.4/hplc_data_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-16 20:27:46.860524 hplc_data_analysis-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1428 2024-02-15 16:25:06.000000 hplc_data_analysis-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-16 20:31:59.002211 hplc_data_analysis-1.0.5/
+-rw-rw-rw-   0        0        0     5190 2024-02-16 20:31:58.995242 hplc_data_analysis-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4518 2024-02-16 20:29:22.000000 hplc_data_analysis-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-02-16 20:31:58.956041 hplc_data_analysis-1.0.5/hplc_data_analysis/
+-rw-rw-rw-   0        0        0       25 2024-01-30 22:54:45.000000 hplc_data_analysis-1.0.5/hplc_data_analysis/__init__.py
+-rw-rw-rw-   0        0        0   101726 2024-02-16 20:26:05.000000 hplc_data_analysis-1.0.5/hplc_data_analysis/main.py
+drwxrwxrwx   0        0        0        0 2024-02-16 20:31:58.990259 hplc_data_analysis-1.0.5/hplc_data_analysis.egg-info/
+-rw-rw-rw-   0        0        0     5190 2024-02-16 20:31:58.000000 hplc_data_analysis-1.0.5/hplc_data_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-02-16 20:31:58.000000 hplc_data_analysis-1.0.5/hplc_data_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-16 20:31:58.000000 hplc_data_analysis-1.0.5/hplc_data_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-02-16 20:31:58.000000 hplc_data_analysis-1.0.5/hplc_data_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-02-16 20:31:58.000000 hplc_data_analysis-1.0.5/hplc_data_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-16 20:31:59.004204 hplc_data_analysis-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1428 2024-02-16 20:31:41.000000 hplc_data_analysis-1.0.5/setup.py
```

### Comparing `hplc_data_analysis-1.0.4/hplc_data_analysis/main.py` & `hplc_data_analysis-1.0.5/hplc_data_analysis/main.py`

 * *Files identical despite different names*

### Comparing `hplc_data_analysis-1.0.4/setup.py` & `hplc_data_analysis-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", 'r', encoding="utf-8") as f:
     description = f.read()
 
 setup(
     name='hplc_data_analysis',  # Replace with your own package name
-    version='1.0.4',  # Start with a small version number and increment it with each release
+    version='1.0.5',  # Start with a small version number and increment it with each release
     author='Matteo Pecchi',  # Replace with your name
     # author_email='your.email@example.com',  # Replace with your email
     description='Tool for automatic analysis of multiple HPLC results',  # Provide a short description
     long_description=description,  # This will read your README file to use as the long description
     long_description_content_type='text/markdown',  # This is the format of your README file
     url='https://github.com/mpecchi/hplc_data_analysis/tree/main',  # Replace with the URL of your project
     packages=find_packages(),  # This function will find all the packages in your project
```

