# Comparing `tmp/ftb_snbt_lib-0.2.3.tar.gz` & `tmp/ftb_snbt_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftb_snbt_lib-0.2.3.tar", last modified: Sat May  4 16:51:57 2024, max compression
+gzip compressed data, was "ftb_snbt_lib-0.3.0.tar", last modified: Sun May 12 09:44:06 2024, max compression
```

## Comparing `ftb_snbt_lib-0.2.3.tar` & `ftb_snbt_lib-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:51:57.149058 ftb_snbt_lib-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-04 16:51:57.149058 ftb_snbt_lib-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:51:57.145058 ftb_snbt_lib-0.2.3/ftb_snbt_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/parsetab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:51:57.145058 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/ctokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/yacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/ygen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib/write.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:51:57.145058 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-04 16:51:57.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-04 16:51:57.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:51:57.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 16:51:57.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-04 16:51:57.000000 ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:51:57.149058 ftb_snbt_lib-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-04 16:51:43.000000 ftb_snbt_lib-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:44:06.081214 ftb_snbt_lib-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-12 09:44:06.081214 ftb_snbt_lib-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5630 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:44:06.077214 ftb_snbt_lib-0.3.0/ftb_snbt_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/parsetab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:44:06.081214 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33639 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/ctokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42905 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137736 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/yacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/ygen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib/write.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 09:44:06.081214 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-12 09:44:06.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-12 09:44:06.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 09:44:06.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-12 09:44:06.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 09:44:06.000000 ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 09:44:06.081214 ftb_snbt_lib-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-12 09:44:01.000000 ftb_snbt_lib-0.3.0/setup.py
```

### Comparing `ftb_snbt_lib-0.2.3/LICENSE` & `ftb_snbt_lib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.2.3/PKG-INFO` & `ftb_snbt_lib-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.2.3
+Version: 0.3.0
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ftb_snbt_lib-0.2.3/README.md` & `ftb_snbt_lib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib/parse.py` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,16 +51,16 @@
                 | LBRACKET RBRACKET"""
     if len(p) == 3:
         p[0] = List()
     else:
         p[0] = List(p[2])
 
 def p_array(p):
-    """array : LBRACKET NAME SEMICOLON values RBRACKET
-                | LBRACKET NAME SEMICOLON RBRACKET"""
+    """array : LBRACKET TYPE SEMICOLON values RBRACKET
+                | LBRACKET TYPE SEMICOLON RBRACKET"""
     if len(p) == 4:
         p[0] = Array(p[2], [])
     else:
         p[0] = Array(p[2], p[4])
 
 def p_values(p):
     """values : values value
```

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib/parsetab.py` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib/parsetab.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # parsetab.py
 # This file is automatically generated. Do not edit.
 # pylint: disable=W,C,R
 _tabversion = '3.10'
 
 _lr_method = 'LALR'
 
-_lr_signature = 'BOOL BYTE COLON COMMA DOUBLE FLOAT INTEGER LBRACE LBRACKET LONG NAME RBRACE RBRACKET SEMICOLON SHORT STRINGsnbt : compoundcompound : LBRACE key_value_pairs RBRACE\n                | LBRACE RBRACEkey_value_pairs : key_value_pairs key_value_pair\n                       | key_value_pairs COMMA key_value_pair\n                       | key_value_pairkey_value_pair : NAME COLON value\n                      | STRING COLON valuevalue : compound\n                | list\n                | array\n                | BOOL\n                | BYTE\n                | SHORT\n                | FLOAT\n                | DOUBLE\n                | LONG\n                | INTEGER\n                | STRINGlist : LBRACKET values RBRACKET\n                | LBRACKET RBRACKETarray : LBRACKET NAME SEMICOLON values RBRACKET\n                | LBRACKET NAME SEMICOLON RBRACKETvalues : values value\n              | values COMMA value\n              | value'
+_lr_signature = 'BOOL BYTE COLON COMMA DOUBLE FLOAT INTEGER LBRACE LBRACKET LONG NAME RBRACE RBRACKET SEMICOLON SHORT STRING TYPEsnbt : compoundcompound : LBRACE key_value_pairs RBRACE\n                | LBRACE RBRACEkey_value_pairs : key_value_pairs key_value_pair\n                       | key_value_pairs COMMA key_value_pair\n                       | key_value_pairkey_value_pair : NAME COLON value\n                      | STRING COLON valuevalue : compound\n                | list\n                | array\n                | BOOL\n                | BYTE\n                | SHORT\n                | FLOAT\n                | DOUBLE\n                | LONG\n                | INTEGER\n                | STRINGlist : LBRACKET values RBRACKET\n                | LBRACKET RBRACKETarray : LBRACKET TYPE SEMICOLON values RBRACKET\n                | LBRACKET TYPE SEMICOLON RBRACKETvalues : values value\n              | values COMMA value\n              | value'
     
-_lr_action_items = {'LBRACE':([0,5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[3,-3,-2,3,3,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,3,3,-21,-26,-20,-24,3,3,-25,3,-23,-22,]),'$end':([1,2,5,9,],[0,-1,-3,-2,]),'RBRACE':([3,4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,24,25,26,28,30,33,39,40,],[5,9,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-8,-21,-20,-23,-22,]),'NAME':([3,4,5,6,9,10,11,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,30,33,39,40,],[7,7,-3,-6,-2,-4,7,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,31,-8,-21,-20,-23,-22,]),'STRING':([3,4,5,6,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,32,33,34,35,36,37,38,39,40,],[8,8,-3,-6,-2,-4,8,26,26,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,26,-8,26,-21,-26,-20,-24,26,26,-25,26,-23,-22,]),'COMMA':([4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,24,25,26,28,29,30,32,33,34,37,38,39,40,],[11,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-8,35,-21,-26,-20,-24,-25,35,-23,-22,]),'RBRACKET':([5,9,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,36,37,38,39,40,],[-3,-2,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,30,33,-21,-26,-20,-24,39,-25,40,-23,-22,]),'BOOL':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,19,19,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,19,19,-21,-26,-20,-24,19,19,-25,19,-23,-22,]),'BYTE':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,20,20,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,20,20,-21,-26,-20,-24,20,20,-25,20,-23,-22,]),'SHORT':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,21,21,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,21,21,-21,-26,-20,-24,21,21,-25,21,-23,-22,]),'FLOAT':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,22,22,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,22,22,-21,-26,-20,-24,22,22,-25,22,-23,-22,]),'DOUBLE':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,23,23,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,23,23,-21,-26,-20,-24,23,23,-25,23,-23,-22,]),'LONG':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,24,24,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,24,24,-21,-26,-20,-24,24,24,-25,24,-23,-22,]),'INTEGER':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,25,25,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,25,25,-21,-26,-20,-24,25,25,-25,25,-23,-22,]),'LBRACKET':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,27,27,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,27,27,-21,-26,-20,-24,27,27,-25,27,-23,-22,]),'COLON':([7,8,],[12,13,]),'SEMICOLON':([31,],[36,]),}
+_lr_action_items = {'LBRACE':([0,5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[3,-3,-2,3,3,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,3,3,-21,-26,-20,-24,3,3,-25,3,-23,-22,]),'$end':([1,2,5,9,],[0,-1,-3,-2,]),'RBRACE':([3,4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,24,25,26,28,30,33,39,40,],[5,9,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-8,-21,-20,-23,-22,]),'NAME':([3,4,5,6,9,10,11,14,15,16,17,18,19,20,21,22,23,24,25,26,28,30,33,39,40,],[7,7,-3,-6,-2,-4,7,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-8,-21,-20,-23,-22,]),'STRING':([3,4,5,6,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,32,33,34,35,36,37,38,39,40,],[8,8,-3,-6,-2,-4,8,26,26,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,26,-8,26,-21,-26,-20,-24,26,26,-25,26,-23,-22,]),'COMMA':([4,5,6,9,10,14,15,16,17,18,19,20,21,22,23,24,25,26,28,29,30,32,33,34,37,38,39,40,],[11,-3,-6,-2,-4,-5,-7,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,-8,35,-21,-26,-20,-24,-25,35,-23,-22,]),'RBRACKET':([5,9,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,36,37,38,39,40,],[-3,-2,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,30,33,-21,-26,-20,-24,39,-25,40,-23,-22,]),'BOOL':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,19,19,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,19,19,-21,-26,-20,-24,19,19,-25,19,-23,-22,]),'BYTE':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,20,20,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,20,20,-21,-26,-20,-24,20,20,-25,20,-23,-22,]),'SHORT':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,21,21,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,21,21,-21,-26,-20,-24,21,21,-25,21,-23,-22,]),'FLOAT':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,22,22,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,22,22,-21,-26,-20,-24,22,22,-25,22,-23,-22,]),'DOUBLE':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,23,23,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,23,23,-21,-26,-20,-24,23,23,-25,23,-23,-22,]),'LONG':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,24,24,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,24,24,-21,-26,-20,-24,24,24,-25,24,-23,-22,]),'INTEGER':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,25,25,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,25,25,-21,-26,-20,-24,25,25,-25,25,-23,-22,]),'LBRACKET':([5,9,12,13,16,17,18,19,20,21,22,23,24,25,26,27,29,30,32,33,34,35,36,37,38,39,40,],[-3,-2,27,27,-9,-10,-11,-12,-13,-14,-15,-16,-17,-18,-19,27,27,-21,-26,-20,-24,27,27,-25,27,-23,-22,]),'COLON':([7,8,],[12,13,]),'TYPE':([27,],[31,]),'SEMICOLON':([31,],[36,]),}
 
 _lr_action = {}
 for _k, _v in _lr_action_items.items():
    for _x,_y in zip(_v[0],_v[1]):
       if not _x in _lr_action:  _lr_action[_x] = {}
       _lr_action[_x][_k] = _y
 del _lr_action_items
@@ -44,13 +44,13 @@
   ('value -> FLOAT','value',1,'p_value','parse.py',42),
   ('value -> DOUBLE','value',1,'p_value','parse.py',43),
   ('value -> LONG','value',1,'p_value','parse.py',44),
   ('value -> INTEGER','value',1,'p_value','parse.py',45),
   ('value -> STRING','value',1,'p_value','parse.py',46),
   ('list -> LBRACKET values RBRACKET','list',3,'p_list','parse.py',50),
   ('list -> LBRACKET RBRACKET','list',2,'p_list','parse.py',51),
-  ('array -> LBRACKET NAME SEMICOLON values RBRACKET','array',5,'p_array','parse.py',58),
-  ('array -> LBRACKET NAME SEMICOLON RBRACKET','array',4,'p_array','parse.py',59),
+  ('array -> LBRACKET TYPE SEMICOLON values RBRACKET','array',5,'p_array','parse.py',58),
+  ('array -> LBRACKET TYPE SEMICOLON RBRACKET','array',4,'p_array','parse.py',59),
   ('values -> values value','values',2,'p_values','parse.py',66),
   ('values -> values COMMA value','values',3,'p_values','parse.py',67),
   ('values -> value','values',1,'p_values','parse.py',68),
 ]
```

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/cpp.py` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/ctokens.py` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/lex.py` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/lex.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/yacc.py` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib/ply/ygen.py` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib/tag.py` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib/tag.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib/token.py` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,48 +11,34 @@
     "SHORT",
     "FLOAT",
     "DOUBLE",
     "LONG",
     "INTEGER",
     "STRING",
     "NAME",
+    "TYPE",
     "COLON",
     "SEMICOLON",
     "COMMA",
 )
 
 t_ignore = ' \t\r'
 
-def t_newline(t):
-    r'\n'
-    t.lexer.lineno += 1
-
-def t_LBRACE(t):
-    r'\{'
-    t.lexer.level += 1
-    return t
-
-def t_RBRACE(t):
-    r'\}'
-    t.lexer.level -= 1
-    return t
-
-def t_LBRACKET(t):
-    r'\['
-    t.lexer.level += 1
+def t_BOOL(t):
+    r'true|false'
+    t.value = Bool(t.value == "true")
     return t
 
-def t_RBRACKET(t):
-    r'\]'
-    t.lexer.level -= 1
+def t_NAME(t):    
+    r'[a-zA-Z0-9._+-]+(?=:)'
     return t
 
-def t_BOOL(t):
-    r'true|false'
-    t.value = Bool(t.value == "true")
+def t_STRING(t):
+    r'\"[^\"\\]*(?:\\.[^\"\\]*)*\"'
+    t.value = String(t.value[1:-1].replace(r'\"', '"').replace(r'\\', '\\'))
     return t
 
 def t_BYTE(t):
     r'\-?[0-9]+b'
     t.value = Byte(t.value[:-1])
     return t
 
@@ -77,21 +63,40 @@
     return t
 
 def t_INTEGER(t):
     r'\-?[0-9]+'
     t.value = Integer(t.value)
     return t
 
-def t_STRING(t):
-    r'\"[^\"\\]*(?:\\.[^\"\\]*)*\"'
-    t.value = String(t.value[1:-1].replace(r'\"', '"').replace(r'\\', '\\'))
+def t_TYPE(t):
+    r'[BIL]+(?=;)'
     return t
 
-def t_NAME(t):    
-    r'[a-zA-Z0-9._+-]+'
+def t_newline(t):
+    r'\n'
+    t.lexer.lineno += 1
+
+def t_LBRACE(t):
+    r'\{'
+    t.lexer.level += 1
+    return t
+
+def t_RBRACE(t):
+    r'\}'
+    t.lexer.level -= 1
+    return t
+
+def t_LBRACKET(t):
+    r'\['
+    t.lexer.level += 1
+    return t
+
+def t_RBRACKET(t):
+    r'\]'
+    t.lexer.level -= 1
     return t
 
 def t_COLON(t):
     r'\:'
     return t
 
 def t_SEMICOLON(t):
```

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib/write.py` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib/write.py`

 * *Files identical despite different names*

### Comparing `ftb_snbt_lib-0.2.3/ftb_snbt_lib.egg-info/PKG-INFO` & `ftb_snbt_lib-0.3.0/ftb_snbt_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftb-snbt-lib
-Version: 0.2.3
+Version: 0.3.0
 Summary: A python library to parse, edit, and save FTB snbt tag, which is a variant of the "vanilla" snbt tag.
 Author-email: peunsu <peunsu55@gmail.com>
 Project-URL: homepage, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: repository, https://github.com/peunsu/ftb-snbt-lib
 Project-URL: documentation, https://github.com/peunsu/ftb-snbt-lib
 Keywords: minecraft,ftb,snbt,parser,library
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ftb_snbt_lib-0.2.3/pyproject.toml` & `ftb_snbt_lib-0.3.0/pyproject.toml`

 * *Files identical despite different names*

