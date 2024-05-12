# Comparing `tmp/cancer_simulation-0.5.tar.gz` & `tmp/cancer_simulation-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cancer_simulation-0.5.tar", last modified: Sun May 12 18:57:41 2024, max compression
+gzip compressed data, was "cancer_simulation-0.6.tar", last modified: Sun May 12 19:00:53 2024, max compression
```

## Comparing `cancer_simulation-0.5.tar` & `cancer_simulation-0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-12 18:57:41.995793 cancer_simulation-0.5/
--rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      152 2024-05-12 18:57:41.995793 cancer_simulation-0.5/PKG-INFO
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     9885 2024-05-12 12:44:46.000000 cancer_simulation-0.5/README.md
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-12 18:57:41.991793 cancer_simulation-0.5/cancer_simulation.egg-info/
--rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      152 2024-05-12 18:57:41.000000 cancer_simulation-0.5/cancer_simulation.egg-info/PKG-INFO
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      390 2024-05-12 18:57:41.000000 cancer_simulation-0.5/cancer_simulation.egg-info/SOURCES.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        1 2024-05-12 18:57:41.000000 cancer_simulation-0.5/cancer_simulation.egg-info/dependency_links.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       34 2024-05-12 18:57:41.000000 cancer_simulation-0.5/cancer_simulation.egg-info/entry_points.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       48 2024-05-12 18:57:41.000000 cancer_simulation-0.5/cancer_simulation.egg-info/requires.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        4 2024-05-12 18:57:41.000000 cancer_simulation-0.5/cancer_simulation.egg-info/top_level.txt
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       38 2024-05-12 18:57:41.995793 cancer_simulation-0.5/setup.cfg
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      340 2024-05-12 18:57:37.000000 cancer_simulation-0.5/setup.py
-drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-12 18:57:41.991793 cancer_simulation-0.5/src/
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       30 2024-05-12 18:56:52.000000 cancer_simulation-0.5/src/__init__.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2983 2024-05-12 12:48:55.000000 cancer_simulation-0.5/src/automaton.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     1625 2024-05-12 17:43:44.000000 cancer_simulation-0.5/src/cell.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      274 2024-05-11 21:25:41.000000 cancer_simulation-0.5/src/constants.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    12357 2024-05-12 18:33:08.000000 cancer_simulation-0.5/src/csimulation.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     8344 2024-05-12 12:58:07.000000 cancer_simulation-0.5/src/entity.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2922 2024-05-12 01:38:20.000000 cancer_simulation-0.5/src/grid.py
--rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     4286 2024-05-12 11:57:53.000000 cancer_simulation-0.5/src/variables.py
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-12 19:00:53.510921 cancer_simulation-0.6/
+-rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      152 2024-05-12 19:00:53.510921 cancer_simulation-0.6/PKG-INFO
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     9885 2024-05-12 12:44:46.000000 cancer_simulation-0.6/README.md
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-12 19:00:53.510921 cancer_simulation-0.6/cancer_simulation.egg-info/
+-rw-r--r--   0 zhukowych  (1000) zhukowych  (1000)      152 2024-05-12 19:00:53.000000 cancer_simulation-0.6/cancer_simulation.egg-info/PKG-INFO
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      390 2024-05-12 19:00:53.000000 cancer_simulation-0.6/cancer_simulation.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        1 2024-05-12 19:00:53.000000 cancer_simulation-0.6/cancer_simulation.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       34 2024-05-12 19:00:53.000000 cancer_simulation-0.6/cancer_simulation.egg-info/entry_points.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       48 2024-05-12 19:00:53.000000 cancer_simulation-0.6/cancer_simulation.egg-info/requires.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)        4 2024-05-12 19:00:53.000000 cancer_simulation-0.6/cancer_simulation.egg-info/top_level.txt
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       38 2024-05-12 19:00:53.510921 cancer_simulation-0.6/setup.cfg
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      340 2024-05-12 19:00:50.000000 cancer_simulation-0.6/setup.py
+drwxrwxr-x   0 zhukowych  (1000) zhukowych  (1000)        0 2024-05-12 19:00:53.510921 cancer_simulation-0.6/src/
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)       30 2024-05-12 18:56:52.000000 cancer_simulation-0.6/src/__init__.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2986 2024-05-12 19:00:27.000000 cancer_simulation-0.6/src/automaton.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     1625 2024-05-12 17:43:44.000000 cancer_simulation-0.6/src/cell.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)      274 2024-05-11 21:25:41.000000 cancer_simulation-0.6/src/constants.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)    12362 2024-05-12 18:59:45.000000 cancer_simulation-0.6/src/csimulation.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     8346 2024-05-12 19:00:17.000000 cancer_simulation-0.6/src/entity.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     2924 2024-05-12 19:00:03.000000 cancer_simulation-0.6/src/grid.py
+-rw-rw-r--   0 zhukowych  (1000) zhukowych  (1000)     4286 2024-05-12 11:57:53.000000 cancer_simulation-0.6/src/variables.py
```

### Comparing `cancer_simulation-0.5/README.md` & `cancer_simulation-0.6/README.md`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.5/src/automaton.py` & `cancer_simulation-0.6/src/automaton.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Finite automaton"""
 
 import numpy as np
 from random import randint
 from math import sqrt
-from grid import Grid
-from variables import Variables
-from entity import *
+from .grid import Grid
+from .variables import Variables
+from .entity import *
 
 
 class CellCounter:
 
     def __init__(self):
         self.immune_cell = 0
         self.tumor_cell = 0
```

### Comparing `cancer_simulation-0.5/src/cell.py` & `cancer_simulation-0.6/src/cell.py`

 * *Files identical despite different names*

### Comparing `cancer_simulation-0.5/src/csimulation.py` & `cancer_simulation-0.6/src/csimulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import sys
 from multiprocessing import Process, Queue, Value
 import pygame
 import pygame_chart as pyc
 
 import pygame
 import argparse
-from automaton import FiniteAutomaton
-from grid import Grid
-from entity import TrueStemCell, ImmuneCell
-from variables import Variables, read_variables
+from .automaton import FiniteAutomaton
+from .grid import Grid
+from .entity import TrueStemCell, ImmuneCell
+from .variables import Variables, read_variables
 
-from constants import (
+from .constants import (
     SCREEN_HEIGHT,
     SCREEN_WIDTH,
 )
 
 # IN GAME constants
 BETWEEN_IND = SCREEN_WIDTH // 170, SCREEN_HEIGHT // 30  # x, y
```

### Comparing `cancer_simulation-0.5/src/entity.py` & `cancer_simulation-0.6/src/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Entities"""
 import math
 import numpy as np
-from variables import Variables
 from random import random, choice
-from cell import Cell
+from .variables import Variables
+from .cell import Cell
 
 
 MAX_PROLIFERATION_POTENTIAL = 30
 MAX_PROLIFERATION_COLOR = np.array([250,0,0])
 LOW_PROLIFERATION_COLOR = np.array([0, 0, 0])
 
 DELTA = ( MAX_PROLIFERATION_COLOR - LOW_PROLIFERATION_COLOR ) / MAX_PROLIFERATION_POTENTIAL
```

### Comparing `cancer_simulation-0.5/src/grid.py` & `cancer_simulation-0.6/src/grid.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Grid and cell"""
 
 from typing import Iterable
 import numpy as np
 from random import randint
 from math import sqrt
-from cell import Cell
-from entity import Entity
+from .cell import Cell
+from .entity import Entity
 
 
 class Grid:
     """Grid"""
 
     def __init__(self, width=1000, height=1000) -> None:
         """Initialize the grid"""
```

### Comparing `cancer_simulation-0.5/src/variables.py` & `cancer_simulation-0.6/src/variables.py`

 * *Files identical despite different names*

