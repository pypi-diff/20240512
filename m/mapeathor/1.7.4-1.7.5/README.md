# Comparing `tmp/mapeathor-1.7.4.tar.gz` & `tmp/mapeathor-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapeathor-1.7.4.tar", last modified: Sat May 11 09:55:35 2024, max compression
+gzip compressed data, was "mapeathor-1.7.5.tar", last modified: Sun May 12 11:27:55 2024, max compression
```

## Comparing `mapeathor-1.7.4.tar` & `mapeathor-1.7.5.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.403584 mapeathor-1.7.4/
--rw-r--r--   0 runner     (501) staff       (20)    11349 2024-05-11 09:55:29.000000 mapeathor-1.7.4/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-11 09:55:29.000000 mapeathor-1.7.4/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    18422 2024-05-11 09:55:35.403424 mapeathor-1.7.4/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     3535 2024-05-11 09:55:29.000000 mapeathor-1.7.4/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1828 2024-05-11 09:55:29.000000 mapeathor-1.7.4/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      125 2024-05-11 09:55:35.404396 mapeathor-1.7.4/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1507 2024-05-11 09:55:29.000000 mapeathor-1.7.4/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.365467 mapeathor-1.7.4/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.368810 mapeathor-1.7.4/src/mapeathor/
--rw-r--r--   0 runner     (501) staff       (20)     1795 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)       22 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/_version.py
--rw-r--r--   0 runner     (501) staff       (20)     3881 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/api.py
--rw-r--r--   0 runner     (501) staff       (20)     1206 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/global_config.py
--rw-r--r--   0 runner     (501) staff       (20)    13044 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/mapping_generator.py
--rw-r--r--   0 runner     (501) staff       (20)    13026 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/mapping_writer.py
--rw-r--r--   0 runner     (501) staff       (20)      782 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/source.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.365901 mapeathor-1.7.4/src/mapeathor/templates/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.372872 mapeathor-1.7.4/src/mapeathor/templates/r2rml/
--rw-r--r--   0 runner     (501) staff       (20)       26 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Base.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       11 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Function.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      318 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Join.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      375 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/POM.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Prefix.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       54 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Source.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       98 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/SourceQuery.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      102 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/Subject.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       34 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/TriplesMap.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      384 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/config.json
--rw-r--r--   0 runner     (501) staff       (20)      758 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/r2rml/structure.json
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.392098 mapeathor-1.7.4/src/mapeathor/templates/rml/
--rw-r--r--   0 runner     (501) staff       (20)       26 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Base.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      189 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Function.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/FunctionMap.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      122 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/FunctionPOM.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      145 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/FunctionSource.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      279 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Join.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      388 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/POM.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Prefix.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Source.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      103 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/SourceQuery.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      108 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/Subject.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/TriplesMap.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      444 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/config.json
--rw-r--r--   0 runner     (501) staff       (20)      209 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/rmlMapping.json
--rw-r--r--   0 runner     (501) staff       (20)     1146 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml/structure.json
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.397686 mapeathor-1.7.4/src/mapeathor/templates/rml2014/
--rw-r--r--   0 runner     (501) staff       (20)       26 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Base.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      186 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Function.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/FunctionMap.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      122 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/FunctionPOM.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      145 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/FunctionSource.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      268 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Join.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      375 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/POM.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Prefix.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      123 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Source.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       99 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/SourceQuery.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      102 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/Subject.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       34 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/TriplesMap.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      442 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/config.json
--rw-r--r--   0 runner     (501) staff       (20)      209 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/rmlMapping.json
--rw-r--r--   0 runner     (501) staff       (20)     1250 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/rml2014/structure.json
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.401823 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/
--rw-r--r--   0 runner     (501) staff       (20)       25 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Base.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       12 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Function.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      198 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Join.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      234 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/POM.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      107 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Prefix.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       70 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Source.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       83 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/SourceQuery.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       36 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/Subject.tmpl
--rw-r--r--   0 runner     (501) staff       (20)       13 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/TriplesMap.tmpl
--rw-r--r--   0 runner     (501) staff       (20)      415 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/config.json
--rw-r--r--   0 runner     (501) staff       (20)     1218 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/templates/yarrrml/structure.json
--rw-r--r--   0 runner     (501) staff       (20)     3711 2024-05-11 09:55:29.000000 mapeathor-1.7.4/src/mapeathor/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-11 09:55:35.402243 mapeathor-1.7.4/src/mapeathor.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)    18422 2024-05-11 09:55:35.000000 mapeathor-1.7.4/src/mapeathor.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2773 2024-05-11 09:55:35.000000 mapeathor-1.7.4/src/mapeathor.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-11 09:55:35.000000 mapeathor-1.7.4/src/mapeathor.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-11 09:55:35.000000 mapeathor-1.7.4/src/mapeathor.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2024-05-11 09:55:35.000000 mapeathor-1.7.4/src/mapeathor.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 11:27:55.705613 mapeathor-1.7.5/
+-rw-r--r--   0 runner     (501) staff       (20)    11349 2024-05-12 11:27:49.000000 mapeathor-1.7.5/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-12 11:27:49.000000 mapeathor-1.7.5/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    18422 2024-05-12 11:27:55.705515 mapeathor-1.7.5/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3535 2024-05-12 11:27:49.000000 mapeathor-1.7.5/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1828 2024-05-12 11:27:49.000000 mapeathor-1.7.5/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      125 2024-05-12 11:27:55.705842 mapeathor-1.7.5/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1507 2024-05-12 11:27:49.000000 mapeathor-1.7.5/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 11:27:55.692497 mapeathor-1.7.5/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 11:27:55.694604 mapeathor-1.7.5/src/mapeathor/
+-rw-r--r--   0 runner     (501) staff       (20)     1795 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)       22 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/_version.py
+-rw-r--r--   0 runner     (501) staff       (20)     3881 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/api.py
+-rw-r--r--   0 runner     (501) staff       (20)     1206 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/global_config.py
+-rw-r--r--   0 runner     (501) staff       (20)    13044 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/mapping_generator.py
+-rw-r--r--   0 runner     (501) staff       (20)    13026 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/mapping_writer.py
+-rw-r--r--   0 runner     (501) staff       (20)      782 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/source.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 11:27:55.692806 mapeathor-1.7.5/src/mapeathor/templates/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 11:27:55.698676 mapeathor-1.7.5/src/mapeathor/templates/r2rml/
+-rw-r--r--   0 runner     (501) staff       (20)       26 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/Base.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       11 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/Function.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      318 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/Join.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      375 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/POM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/Prefix.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       54 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/Source.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       98 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/SourceQuery.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      102 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/Subject.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       34 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/TriplesMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      384 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/config.json
+-rw-r--r--   0 runner     (501) staff       (20)      758 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/r2rml/structure.json
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 11:27:55.701004 mapeathor-1.7.5/src/mapeathor/templates/rml/
+-rw-r--r--   0 runner     (501) staff       (20)       26 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/Base.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      189 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/Function.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/FunctionMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      122 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/FunctionPOM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      145 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/FunctionSource.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      279 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/Join.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      388 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/POM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/Prefix.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/Source.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      103 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/SourceQuery.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      108 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/Subject.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/TriplesMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      444 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/config.json
+-rw-r--r--   0 runner     (501) staff       (20)      209 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/rmlMapping.json
+-rw-r--r--   0 runner     (501) staff       (20)     1145 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml/structure.json
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 11:27:55.703263 mapeathor-1.7.5/src/mapeathor/templates/rml2014/
+-rw-r--r--   0 runner     (501) staff       (20)       26 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/Base.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      186 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/Function.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       90 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/FunctionMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      122 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/FunctionPOM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      145 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/FunctionSource.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      268 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/Join.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      375 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/POM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/Prefix.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      123 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/Source.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       99 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/SourceQuery.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      102 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/Subject.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       34 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/TriplesMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      442 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/config.json
+-rw-r--r--   0 runner     (501) staff       (20)      209 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/rmlMapping.json
+-rw-r--r--   0 runner     (501) staff       (20)     1249 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/rml2014/structure.json
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 11:27:55.704934 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/
+-rw-r--r--   0 runner     (501) staff       (20)       25 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/Base.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       12 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/Function.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      198 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/Join.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      234 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/POM.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      107 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/Prefix.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       70 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/Source.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       83 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/SourceQuery.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       36 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/Subject.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)       13 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/TriplesMap.tmpl
+-rw-r--r--   0 runner     (501) staff       (20)      417 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/config.json
+-rw-r--r--   0 runner     (501) staff       (20)     1218 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/templates/yarrrml/structure.json
+-rw-r--r--   0 runner     (501) staff       (20)     3711 2024-05-12 11:27:49.000000 mapeathor-1.7.5/src/mapeathor/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-12 11:27:55.705170 mapeathor-1.7.5/src/mapeathor.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)    18422 2024-05-12 11:27:55.000000 mapeathor-1.7.5/src/mapeathor.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2773 2024-05-12 11:27:55.000000 mapeathor-1.7.5/src/mapeathor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-12 11:27:55.000000 mapeathor-1.7.5/src/mapeathor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-12 11:27:55.000000 mapeathor-1.7.5/src/mapeathor.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       10 2024-05-12 11:27:55.000000 mapeathor-1.7.5/src/mapeathor.egg-info/top_level.txt
```

### Comparing `mapeathor-1.7.4/LICENSE` & `mapeathor-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/PKG-INFO` & `mapeathor-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapeathor
-Version: 1.7.4
+Version: 1.7.5
 Summary: Mapeathor translates your mapping rules specified in spreadsheets to a mapping language.
 Home-page: https://github.com/oeg-upm/Mapeathor
 Author: Ana Iglesias-Molina
 Author-email: Ana Iglesias-Molina <ana.iglesiasm@upm.es>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `mapeathor-1.7.4/README.md` & `mapeathor-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/pyproject.toml` & `mapeathor-1.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/setup.py` & `mapeathor-1.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/src/mapeathor/__init__.py` & `mapeathor-1.7.5/src/mapeathor/__init__.py`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/src/mapeathor/api.py` & `mapeathor-1.7.5/src/mapeathor/api.py`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/src/mapeathor/global_config.py` & `mapeathor-1.7.5/src/mapeathor/global_config.py`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/src/mapeathor/mapping_generator.py` & `mapeathor-1.7.5/src/mapeathor/mapping_generator.py`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/src/mapeathor/mapping_writer.py` & `mapeathor-1.7.5/src/mapeathor/mapping_writer.py`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/src/mapeathor/source.py` & `mapeathor-1.7.5/src/mapeathor/source.py`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/src/mapeathor/templates/r2rml/structure.json` & `mapeathor-1.7.5/src/mapeathor/templates/r2rml/structure.json`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/src/mapeathor/templates/rml/structure.json` & `mapeathor-1.7.5/src/mapeathor/templates/rml/structure.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'variable'": "{1: {'after': '    \\n.\\n'}}"}*

```diff
@@ -56,15 +56,15 @@
                     "tabs": 1
                 }
             ],
             "file": "TriplesMap",
             "tabs": 1
         },
         {
-            "after": "    ]\n.\n",
+            "after": "    \n.\n",
             "before": "",
             "childs": [
                 {
                     "after": "",
                     "before": "",
                     "childs": [],
                     "file": "FunctionSource",
```

### Comparing `mapeathor-1.7.4/src/mapeathor/templates/rml2014/structure.json` & `mapeathor-1.7.5/src/mapeathor/templates/rml2014/structure.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'variable'": "{1: {'after': '    \\n.\\n'}}"}*

```diff
@@ -56,15 +56,15 @@
                     "tabs": 1
                 }
             ],
             "file": "TriplesMap",
             "tabs": 1
         },
         {
-            "after": "    ]\n.\n",
+            "after": "    \n.\n",
             "before": "",
             "childs": [
                 {
                     "after": "",
                     "before": "",
                     "childs": [],
                     "file": "FunctionSource",
```

### Comparing `mapeathor-1.7.4/src/mapeathor/templates/yarrrml/structure.json` & `mapeathor-1.7.5/src/mapeathor/templates/yarrrml/structure.json`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/src/mapeathor/utils.py` & `mapeathor-1.7.5/src/mapeathor/utils.py`

 * *Files identical despite different names*

### Comparing `mapeathor-1.7.4/src/mapeathor.egg-info/PKG-INFO` & `mapeathor-1.7.5/src/mapeathor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapeathor
-Version: 1.7.4
+Version: 1.7.5
 Summary: Mapeathor translates your mapping rules specified in spreadsheets to a mapping language.
 Home-page: https://github.com/oeg-upm/Mapeathor
 Author: Ana Iglesias-Molina
 Author-email: Ana Iglesias-Molina <ana.iglesiasm@upm.es>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `mapeathor-1.7.4/src/mapeathor.egg-info/SOURCES.txt` & `mapeathor-1.7.5/src/mapeathor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

