# Comparing `tmp/sto_oscr-2024.4b20.tar.gz` & `tmp/sto_oscr-2024.5b120.tar.gz`

## Comparing `sto_oscr-2024.4b20.tar` & `sto_oscr-2024.5b120.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/.flake8
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/__init__.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/cli.py
--rw-r--r--   0        0        0    14233 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/combat.py
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/datamodels.py
--rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/detection.py
--rw-r--r--   0        0        0    11062 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/iofunc.py
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/liveparser.py
--rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/main.py
--rw-r--r--   0        0        0    23569 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/parser.py
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/OSCR/utilities.py
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/LICENSE
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/pyproject.toml
--rw-r--r--   0        0        0    41255 2020-02-02 00:00:00.000000 sto_oscr-2024.4b20/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/.flake8
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/__init__.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/cli.py
+-rw-r--r--   0        0        0    14305 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/combat.py
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/datamodels.py
+-rw-r--r--   0        0        0    10460 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/detection.py
+-rw-r--r--   0        0        0    11062 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/iofunc.py
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/liveparser.py
+-rw-r--r--   0        0        0     9636 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/main.py
+-rw-r--r--   0        0        0    23569 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/parser.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/OSCR/utilities.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/LICENSE
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/pyproject.toml
+-rw-r--r--   0        0        0    41256 2020-02-02 00:00:00.000000 sto_oscr-2024.5b120/PKG-INFO
```

### Comparing `sto_oscr-2024.4b20/OSCR/__init__.py` & `sto_oscr-2024.5b120/OSCR/__init__.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.4b20/OSCR/cli.py` & `sto_oscr-2024.5b120/OSCR/cli.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.4b20/OSCR/combat.py` & `sto_oscr-2024.5b120/OSCR/combat.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,16 @@
                 player.heal_share = 0.0
 
             for k, v in Detection.BUILD_DETECTION_ABILITIES.items():
                 for event in player.events:
                     if k in event:
                         player.build = v
                         break
+                if player.build != "Unknown":
+                    break
 
             player.graph_time = tuple(map(lambda x: round(x, 1), player.graph_time))
             DPS_data = numpy.array(player.DMG_graph_data, dtype=numpy.float64).cumsum()
             player.DPS_graph_data = tuple(DPS_data / player.graph_time)
 
     def analyze_critters(self):
         """
```

### Comparing `sto_oscr-2024.4b20/OSCR/datamodels.py` & `sto_oscr-2024.5b120/OSCR/datamodels.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.4b20/OSCR/detection.py` & `sto_oscr-2024.5b120/OSCR/detection.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.4b20/OSCR/iofunc.py` & `sto_oscr-2024.5b120/OSCR/iofunc.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.4b20/OSCR/liveparser.py` & `sto_oscr-2024.5b120/OSCR/liveparser.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.4b20/OSCR/main.py` & `sto_oscr-2024.5b120/OSCR/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .iofunc import get_combat_log_data, reset_temp_folder, save_log, split_log_by_lines
 from .parser import analyze_combat
 from .utilities import datetime_to_display, to_datetime
 
 
 class OSCR():
 
-    version = '2024.04b020'
+    version = '2024.05b120'
 
     def __init__(self, log_path: str = None, settings: dict = None):
         self.log_path = log_path
         self.combats: list[Combat] = list()
         self.combats_pointer = None
         self.excess_log_lines = list()
         self.combatlog_tempfiles = list()
```

### Comparing `sto_oscr-2024.4b20/OSCR/parser.py` & `sto_oscr-2024.5b120/OSCR/parser.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.4b20/OSCR/utilities.py` & `sto_oscr-2024.5b120/OSCR/utilities.py`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.4b20/LICENSE` & `sto_oscr-2024.5b120/LICENSE`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.4b20/pyproject.toml` & `sto_oscr-2024.5b120/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sto_oscr-2024.4b20/PKG-INFO` & `sto_oscr-2024.5b120/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: STO-OSCR
-Version: 2024.4b20
+Version: 2024.5b120
 Summary: Open Source Combatlog Reader for Star Trek Online.
 Project-URL: Homepage, https://github.com/STOCD/OSCR
 Project-URL: Repository, https://github.com/STOCD/OSCR.git
 Project-URL: Bug Tracker, https://github.com/STOCD/OSCR/issues
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

