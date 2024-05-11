# Comparing `tmp/pyiron_ontology-0.1.4.tar.gz` & `tmp/pyiron_ontology-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_ontology-0.1.4.tar", last modified: Thu Jan 18 00:02:01 2024, max compression
+gzip compressed data, was "pyiron_ontology-0.2.7.tar", last modified: Sat May 11 22:27:14 2024, max compression
```

## Comparing `pyiron_ontology-0.1.4.tar` & `pyiron_ontology-0.2.7.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 00:02:01.844179 pyiron_ontology-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 00:02:01.844179 pyiron_ontology-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 00:02:01.844179 pyiron_ontology-0.1.4/pyiron_ontology/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/pyiron_ontology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-01-18 00:02:01.848179 pyiron_ontology-0.1.4/pyiron_ontology/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 00:02:01.844179 pyiron_ontology-0.1.4/pyiron_ontology/atomistics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/pyiron_ontology/atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/pyiron_ontology/atomistics/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/pyiron_ontology/atomistics/reasoning.py
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/pyiron_ontology/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/pyiron_ontology/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 00:02:01.844179 pyiron_ontology-0.1.4/pyiron_ontology/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/pyiron_ontology/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/pyiron_ontology/example/constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/pyiron_ontology/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 00:02:01.844179 pyiron_ontology-0.1.4/pyiron_ontology.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 00:02:01.000000 pyiron_ontology-0.1.4/pyiron_ontology.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-18 00:02:01.000000 pyiron_ontology-0.1.4/pyiron_ontology.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 00:02:01.000000 pyiron_ontology-0.1.4/pyiron_ontology.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-18 00:02:01.000000 pyiron_ontology-0.1.4/pyiron_ontology.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-18 00:02:01.000000 pyiron_ontology-0.1.4/pyiron_ontology.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-18 00:02:01.848179 pyiron_ontology-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-01-18 00:02:01.000000 pyiron_ontology-0.1.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-01-18 00:01:58.000000 pyiron_ontology-0.1.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:27:14.399420 pyiron_ontology-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18424 2024-05-11 22:27:14.399420 pyiron_ontology-0.2.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:27:14.395420 pyiron_ontology-0.2.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    15515 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:27:14.395420 pyiron_ontology-0.2.7/pyiron_ontology/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/pyiron_ontology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-11 22:27:14.399420 pyiron_ontology-0.2.7/pyiron_ontology/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:27:14.395420 pyiron_ontology-0.2.7/pyiron_ontology/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/pyiron_ontology/atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/pyiron_ontology/atomistics/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/pyiron_ontology/atomistics/reasoning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/pyiron_ontology/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/pyiron_ontology/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:27:14.395420 pyiron_ontology-0.2.7/pyiron_ontology/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/pyiron_ontology/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/pyiron_ontology/example/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/pyiron_ontology/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 22:27:14.395420 pyiron_ontology-0.2.7/pyiron_ontology.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18424 2024-05-11 22:27:14.000000 pyiron_ontology-0.2.7/pyiron_ontology.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-11 22:27:14.000000 pyiron_ontology-0.2.7/pyiron_ontology.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 22:27:14.000000 pyiron_ontology-0.2.7/pyiron_ontology.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-11 22:27:14.000000 pyiron_ontology-0.2.7/pyiron_ontology.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-11 22:27:14.000000 pyiron_ontology-0.2.7/pyiron_ontology.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-11 22:27:12.000000 pyiron_ontology-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 22:27:14.399420 pyiron_ontology-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-11 22:25:50.000000 pyiron_ontology-0.2.7/setup.py
```

### Comparing `pyiron_ontology-0.1.4/LICENSE` & `pyiron_ontology-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.4/pyiron_ontology/atomistics/constructor.py` & `pyiron_ontology-0.2.7/pyiron_ontology/atomistics/constructor.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.4/pyiron_ontology/atomistics/reasoning.py` & `pyiron_ontology-0.2.7/pyiron_ontology/atomistics/reasoning.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.4/pyiron_ontology/constructor.py` & `pyiron_ontology-0.2.7/pyiron_ontology/constructor.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.4/pyiron_ontology/dynamic.py` & `pyiron_ontology-0.2.7/pyiron_ontology/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.4/pyiron_ontology/example/constructor.py` & `pyiron_ontology-0.2.7/pyiron_ontology/example/constructor.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.4/pyiron_ontology/workflow.py` & `pyiron_ontology-0.2.7/pyiron_ontology/workflow.py`

 * *Files identical despite different names*

### Comparing `pyiron_ontology-0.1.4/pyiron_ontology.egg-info/SOURCES.txt` & `pyiron_ontology-0.2.7/pyiron_ontology.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 MANIFEST.in
-setup.cfg
+pyproject.toml
 setup.py
-versioneer.py
+docs/README.md
 pyiron_ontology/__init__.py
 pyiron_ontology/_version.py
 pyiron_ontology/constructor.py
 pyiron_ontology/dynamic.py
 pyiron_ontology/workflow.py
 pyiron_ontology.egg-info/PKG-INFO
 pyiron_ontology.egg-info/SOURCES.txt
```

### Comparing `pyiron_ontology-0.1.4/setup.py` & `pyiron_ontology-0.2.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-"""
-Setuptools based setup module
-"""
-from setuptools import setup, find_packages
-import versioneer
-
-setup(
-    name='pyiron_ontology',
-    version=versioneer.get_version(),
-    description='pyiron_ontology - module extension to pyiron.',
-    long_description='http://pyiron.org',
-
-    url='https://github.com/pyiron/pyiron_ontology',
-    author='Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department',
-    author_email='liamhuber@greyhavensolutions.com',
-    license='BSD',
-
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Topic :: Scientific/Engineering :: Physics',
-        'License :: OSI Approved :: BSD License',
-        'Intended Audience :: Science/Research',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ],
-
-    keywords='pyiron',
-    packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
-    install_requires=[
-        'numpy>=1.26.3',
-        'owlready2>=0.45',
-        'pandas>=2.1.4',
-        'pint>=0.23',
-    ],
-    cmdclass=versioneer.get_cmdclass(),
+[build-system]
+requires = [ "numpy", "owlready2", "pandas", "pint", "setuptools", "versioneer[toml]==0.29",]
+build-backend = "setuptools.build_meta"
 
-    )
+[project]
+name = "pyiron_ontology"
+description = "pyiron_ontology - module extension to pyiron."
+readme = "docs/README.md"
+keywords = [ "pyiron",]
+requires-python = ">=3.9, <3.13"
+classifiers = [ "Development Status :: 5 - Production/Stable", "Topic :: Scientific/Engineering :: Physics", "License :: OSI Approved :: BSD License", "Intended Audience :: Science/Research", "Operating System :: OS Independent", "Programming Language :: Python :: 3.9", "Programming Language :: Python :: 3.10", "Programming Language :: Python :: 3.11", "Programming Language :: Python :: 3.12",]
+dependencies = [ "numpy>=1.26.3,<1.27.0", "owlready2==0.46", "pandas>=2.1.4,<2.3.0", "pint==0.23",]
+dynamic = [ "version",]
+[[project.authors]]
+name = "Liam Huber"
+email = "liamhuber@greyhavensolutions.com"
+
+[project.license]
+file = "LICENSE"
+
+[project.urls]
+Homepage = "https://github.com/pyiron/pyiron_ontology"
+Documentation = "https://pyiron-ontology.readthedocs.io"
+Repository = "https://github.com/pyiron/pyiron_ontology"
+
+[tool.versioneer]
+VCS = "git"
+style = "pep440-pre"
+versionfile_source = "pyiron_ontology/_version.py"
+parentdir_prefix = "pyiron_ontology"
+tag_prefix = "pyiron_ontology-"
+
+[tool.setuptools.packages.find]
+include = [ "pyiron_ontology*",]
+
+[tool.setuptools.dynamic.version]
+attr = "pyiron_ontology.__version__"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

