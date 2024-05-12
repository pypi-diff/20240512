# Comparing `tmp/lexwolf-0.1.4.tar.gz` & `tmp/lexwolf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexwolf-0.1.4.tar", last modified: Sat Mar  9 23:29:49 2024, max compression
+gzip compressed data, was "lexwolf-0.2.0.tar", last modified: Sun May 12 11:52:56 2024, max compression
```

## Comparing `lexwolf-0.1.4.tar` & `lexwolf-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-03-09 23:29:49.053921 lexwolf-0.1.4/
--rwxrwxrwx   0 allem     (1000) allem     (1000)     1098 2023-11-24 20:23:52.000000 lexwolf-0.1.4/LICENSE
--rwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-02-20 19:13:22.000000 lexwolf-0.1.4/MANIFEST.in
--rwxrwxrwx   0 allem     (1000) allem     (1000)      721 2024-03-09 23:29:49.051921 lexwolf-0.1.4/PKG-INFO
--rwxrwxrwx   0 allem     (1000) allem     (1000)        9 2024-03-09 12:21:49.000000 lexwolf-0.1.4/README.md
-drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-03-09 23:29:48.987921 lexwolf-0.1.4/lexwolf/
--rwxrwxrwx   0 allem     (1000) allem     (1000)     6592 2024-03-09 23:17:16.000000 lexwolf-0.1.4/lexwolf/__init__.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     2730 2024-03-09 23:18:09.000000 lexwolf-0.1.4/lexwolf/bitBoard.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     2993 2024-03-08 11:29:43.000000 lexwolf-0.1.4/lexwolf/core.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)    15853 2024-03-08 11:29:43.000000 lexwolf-0.1.4/lexwolf/genetic.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)      459 2024-03-08 11:29:43.000000 lexwolf-0.1.4/lexwolf/interfpsql.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     4349 2024-03-09 23:18:43.000000 lexwolf-0.1.4/lexwolf/minmax.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     2881 2024-03-08 11:29:43.000000 lexwolf-0.1.4/lexwolf/structEl.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     3546 2024-03-09 23:07:24.000000 lexwolf-0.1.4/lexwolf/tests.py
--rwxrwxrwx   0 allem     (1000) allem     (1000)     1086 2024-03-08 11:29:43.000000 lexwolf-0.1.4/lexwolf/weights.py
-drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-03-09 23:29:49.040921 lexwolf-0.1.4/lexwolf.egg-info/
--rwxrwxrwx   0 allem     (1000) allem     (1000)      721 2024-03-09 23:29:48.000000 lexwolf-0.1.4/lexwolf.egg-info/PKG-INFO
--rwxrwxrwx   0 allem     (1000) allem     (1000)      363 2024-03-09 23:29:48.000000 lexwolf-0.1.4/lexwolf.egg-info/SOURCES.txt
--rwxrwxrwx   0 allem     (1000) allem     (1000)        1 2024-03-09 23:29:48.000000 lexwolf-0.1.4/lexwolf.egg-info/dependency_links.txt
--rwxrwxrwx   0 allem     (1000) allem     (1000)        6 2024-03-09 23:29:48.000000 lexwolf-0.1.4/lexwolf.egg-info/requires.txt
--rwxrwxrwx   0 allem     (1000) allem     (1000)        8 2024-03-09 23:29:48.000000 lexwolf-0.1.4/lexwolf.egg-info/top_level.txt
--rwxrwxrwx   0 allem     (1000) allem     (1000)       38 2024-03-09 23:29:49.054922 lexwolf-0.1.4/setup.cfg
--rwxrwxrwx   0 allem     (1000) allem     (1000)     1410 2024-03-09 23:29:37.000000 lexwolf-0.1.4/setup.py
+drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-05-12 11:52:56.979297 lexwolf-0.2.0/
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     1098 2023-11-24 20:23:52.000000 lexwolf-0.2.0/LICENSE
+-rwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-02-20 19:13:22.000000 lexwolf-0.2.0/MANIFEST.in
+-rwxrwxrwx   0 allem     (1000) allem     (1000)      873 2024-05-12 11:52:56.970312 lexwolf-0.2.0/PKG-INFO
+-rwxrwxrwx   0 allem     (1000) allem     (1000)        9 2024-03-09 12:21:49.000000 lexwolf-0.2.0/README.md
+drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-05-12 11:52:56.813219 lexwolf-0.2.0/lexwolf/
+-rwxrwxrwx   0 allem     (1000) allem     (1000)    88811 2024-05-12 11:46:37.000000 lexwolf-0.2.0/lexwolf/__init__.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     5709 2024-03-30 15:39:12.000000 lexwolf-0.2.0/lexwolf/adaptativeminmax.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)    42088 2024-04-05 16:19:22.000000 lexwolf-0.2.0/lexwolf/bitBoard.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     3471 2024-03-29 16:05:20.000000 lexwolf-0.2.0/lexwolf/core.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     1613 2024-03-29 16:00:17.000000 lexwolf-0.2.0/lexwolf/dEvalTest.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)    15853 2024-03-08 11:29:43.000000 lexwolf-0.2.0/lexwolf/genetic.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)      459 2024-03-08 11:29:43.000000 lexwolf-0.2.0/lexwolf/interfpsql.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)    12724 2024-04-05 15:31:20.000000 lexwolf-0.2.0/lexwolf/minmax.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)    18762 2024-03-21 17:08:34.000000 lexwolf-0.2.0/lexwolf/structEl.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     3592 2024-04-01 17:23:48.000000 lexwolf-0.2.0/lexwolf/tests.py
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     2173 2024-03-31 13:07:22.000000 lexwolf-0.2.0/lexwolf/weights.py
+drwxrwxrwx   0 allem     (1000) allem     (1000)        0 2024-05-12 11:52:56.957296 lexwolf-0.2.0/lexwolf.egg-info/
+-rwxrwxrwx   0 allem     (1000) allem     (1000)      873 2024-05-12 11:52:56.000000 lexwolf-0.2.0/lexwolf.egg-info/PKG-INFO
+-rwxrwxrwx   0 allem     (1000) allem     (1000)      412 2024-05-12 11:52:56.000000 lexwolf-0.2.0/lexwolf.egg-info/SOURCES.txt
+-rwxrwxrwx   0 allem     (1000) allem     (1000)        1 2024-05-12 11:52:56.000000 lexwolf-0.2.0/lexwolf.egg-info/dependency_links.txt
+-rwxrwxrwx   0 allem     (1000) allem     (1000)       47 2024-05-12 11:52:56.000000 lexwolf-0.2.0/lexwolf.egg-info/requires.txt
+-rwxrwxrwx   0 allem     (1000) allem     (1000)        8 2024-05-12 11:52:56.000000 lexwolf-0.2.0/lexwolf.egg-info/top_level.txt
+-rwxrwxrwx   0 allem     (1000) allem     (1000)       38 2024-05-12 11:52:56.980298 lexwolf-0.2.0/setup.cfg
+-rwxrwxrwx   0 allem     (1000) allem     (1000)     1498 2024-05-12 11:51:00.000000 lexwolf-0.2.0/setup.py
```

### Comparing `lexwolf-0.1.4/LICENSE` & `lexwolf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lexwolf-0.1.4/PKG-INFO` & `lexwolf-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 Metadata-Version: 2.1
 Name: lexwolf
-Version: 0.1.4
+Version: 0.2.0
 Summary: The LexWolf chess artificial intelligences.
-Home-page: UNKNOWN
+Home-page: 
 Author: Alexandre Le Mercier
 Author-email: alexandre.le.mercier@ulb.be
 License: MIT
-Description: # lexwolf
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: chess
+Requires-Dist: numpy
+Requires-Dist: math
+Requires-Dist: random
+Requires-Dist: time
+Requires-Dist: pandas
+Requires-Dist: IPython
+Requires-Dist: os
+
+# lexwolf
```

### Comparing `lexwolf-0.1.4/lexwolf/core.py` & `lexwolf-0.2.0/lexwolf/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from time import time
 
 import chess
 from random import shuffle, seed, randrange, choices, random
+from lexwolf.bitBoard import bitBoard
 import numpy as np
 
 
 class LexWolfCore():
     """
     Parent class for all LexWolf chess models.
     """
 
-    def __init__(self, max_depth=3, max_thinking_time=3600.0, random_seed=None, verbose=0):
+    def __init__(self, max_depth=3, max_thinking_time=3600.0, random_seed=None, verbose=0, bruteForce = False,incrementalEvaluation=True):
+        self.incrEval = incrementalEvaluation
+        self.bF = bruteForce
+        self.bitBrd = bitBoard(bruteForce=bruteForce)
         self.is_playing = False
         self.is_defeated = False
         self.is_winner = False
         self.combinations_count = 0
         self.max_depth = max_depth  # None = infinite
         self.verbose = verbose
         self.max_thinking_time = max_thinking_time  # Number of seconds before plays the move
@@ -23,14 +27,17 @@
             np.random.seed(random_seed)
         if max_depth is None:
             self.max_depth = float('inf')
 
     def find_optimal_move(self, board=chess.Board()):
         pass
 
+    def find_optimal_move_incremental(self, board=chess.Board()):
+        pass
+
     def verbose_message(self, message):
         if self.verbose:
             print(message)
 
     def count_controlled_squares(self, board, color):
         """
         Counts the squares controlled by each piece type for the specified color.
@@ -78,7 +85,12 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def find_optimal_move(self, board=chess.Board()):
         legal_moves = list(board.legal_moves)
         shuffle(legal_moves)
         return legal_moves[0]
+
+    def find_optimal_move_incremental(self, board=chess.Board()):
+        legal_moves = list(board.legal_moves)
+        shuffle(legal_moves)
+        return legal_moves[0]
```

### Comparing `lexwolf-0.1.4/lexwolf/genetic.py` & `lexwolf-0.2.0/lexwolf/genetic.py`

 * *Files identical despite different names*

### Comparing `lexwolf-0.1.4/lexwolf/tests.py` & `lexwolf-0.2.0/lexwolf/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
 from lexwolf import Game
 from lexwolf.core import DummyLexWolf
 from lexwolf.minmax import MinmaxLexWolf
+from lexwolf.adaptativeminmax import AdaptativeMinmaxLexWolf
 from tqdm import tqdm
 
 class TestLexWolf(unittest.TestCase):
 
     def test_stalemate(self):
         SEED = 0
         game = Game(False, False,
@@ -28,15 +29,15 @@
 
     def test_Dummy_vs_Minmax(self):
         win_ratio = 0
         n_games = 100
         for SEED in tqdm(range(n_games)):
             game = Game(False, False,
                             DummyLexWolf(random_seed=SEED),
-                            MinmaxLexWolf(random_seed=SEED, max_depth=2, center_bonus=0), silence=True)
+                            MinmaxLexWolf(random_seed=SEED, max_depth=3), silence=True)
             win_ratio += game.result
             print("Win ratio so far is", round(win_ratio / (SEED + 1), 2)*100, "%")
         print(
             f"Win ratio between DummyLexWolf (white) and MinmaxLexWolf with depth 1 (black) over {n_games} games: {win_ratio}")
 
         # Result: -94 with center and king bonuses (0.1, 0.2)
         #         -94 with center, control and king bonuses (0.1, 0.1, 0.2)
```

### Comparing `lexwolf-0.1.4/lexwolf/weights.py` & `lexwolf-0.2.0/lexwolf/weights.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,46 @@
 WEIGHTS = {
+    'PAWN_VALUE': 1,
+    'KNIGHT_VALUE': 3,
+    'BISHOP_VALUE': 3,
+    'ROOK_VALUE': 5,
+    'QUEEN_VALUE': 9,
+    'PAWN_ADVANCE_A': 2,
+    'PAWN_ADVANCE_B': 4,
+    'PASSED_PAWN_MULT': 5,
+    'DOUBLED_PAWN_PENALTY': 21,
+    'ISOLATED_PAWN_PENALTY': 10,
+    'BACKWARD_PAWN_PENALTY': 3,
+    'WEAK_SQUARE_PENALTY': 7,
+    'PASSED_PAWN_ENEMY_KING_DIST': 5,
+    'KNIGHT_SQ_MULT': 7,
+    'KNIGHT_OUTPOST_MULT': 8,
+    'BISHOP_MOBILITY': 5,
+    'BISHOP_PAIR': 44,
+    'ROOK_ATTACK_KING_FILE': 30,
+    'ROOK_ATTACK_KING_ADJ_FILE': 1,
+    'ROOK_ATTACK_KING_ADJ_FILE_ABGH': 21,
+    'ROOK_7TH_RANK': 32,
+    'ROOK_CONNECTED': 2,
+    'ROOK_MOBILITY': 2,
+    'ROOK_BEHIND_PASSED_PAWN': 48,
+    'ROOK_OPEN_FILE': 12,
+    'ROOK_SEMI_OPEN_FILE': 6,
+    'ROOK_ATCK_WEAK_PAWN_OPEN_COLUMN': 7,
+    'ROOK_COLUMN_MULT': 3,
+    'QUEEN_MOBILITY': 0,
+    'KING_NO_FRIENDLY_PAWN': 27,
+    'KING_NO_FRIENDLY_PAWN_ADJ': 17,
+    'KING_FRIENDLY_PAWN_ADVANCED1': 12,
+    'KING_NO_ENEMY_PAWN': 11,
+    'KING_NO_ENEMY_PAWN_ADJ': 3,
+    'KING_PRESSURE_MULT': 8,
+}
+
+'''WEIGHTS = {
     'PAWN_VALUE': 83,
     'KNIGHT_VALUE': 322,
     'BISHOP_VALUE': 323,
     'ROOK_VALUE': 478,
     'QUEEN_VALUE': 954,
     'PAWN_ADVANCE_A': 2,
     'PAWN_ADVANCE_B': 4,
@@ -30,8 +68,8 @@
     'QUEEN_MOBILITY': 0,
     'KING_NO_FRIENDLY_PAWN': 27,
     'KING_NO_FRIENDLY_PAWN_ADJ': 17,
     'KING_FRIENDLY_PAWN_ADVANCED1': 12,
     'KING_NO_ENEMY_PAWN': 11,
     'KING_NO_ENEMY_PAWN_ADJ': 3,
     'KING_PRESSURE_MULT': 8,
-}
+}'''
```

### Comparing `lexwolf-0.1.4/lexwolf.egg-info/PKG-INFO` & `lexwolf-0.2.0/lexwolf.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 Metadata-Version: 2.1
 Name: lexwolf
-Version: 0.1.4
+Version: 0.2.0
 Summary: The LexWolf chess artificial intelligences.
-Home-page: UNKNOWN
+Home-page: 
 Author: Alexandre Le Mercier
 Author-email: alexandre.le.mercier@ulb.be
 License: MIT
-Description: # lexwolf
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: chess
+Requires-Dist: numpy
+Requires-Dist: math
+Requires-Dist: random
+Requires-Dist: time
+Requires-Dist: pandas
+Requires-Dist: IPython
+Requires-Dist: os
+
+# lexwolf
```

### Comparing `lexwolf-0.1.4/setup.py` & `lexwolf-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 # To use a consistent encoding
 from codecs import open
 from os import path
 
@@ -11,15 +13,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="lexwolf",
-    version="0.1.4",
+    version="0.2.0",
     description="The LexWolf chess artificial intelligences.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Alexandre Le Mercier",
     author_email="alexandre.le.mercier@ulb.be",
     license="MIT",
@@ -32,15 +34,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["lexwolf"],
     include_package_data=True,
-    install_requires=["chess"]
+    install_requires=["chess", "numpy", "math", "random", "time", "pandas", "IPython", "os"]
 )
 
 """
 python setup.py sdist bdist_wheel
 twine check dist/*
 twine upload dist/*
 """
```

