# Comparing `tmp/cycling_dynamics-0.0.8.tar.gz` & `tmp/cycling_dynamics-0.0.9.tar.gz`

## Comparing `cycling_dynamics-0.0.8.tar` & `cycling_dynamics-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/qodana.yaml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/requirements.txt
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/ruff.toml
--rw-r--r--   0        0        0   660177 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/note_books/Critical Power.ipynb
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/note_books/Surface.ipynb
--rw-r--r--   0        0        0   290283 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/note_books/examples.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/__init__.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/calc.py
--rw-r--r--   0        0        0    12441 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/critical_power.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/load_data.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/models.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/plots.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/stats.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/src/cycling_dynamics/surface.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_critical_power.py
--rw-r--r--   0        0        0   140591 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT ROAM 3FF5-53-0.fit
--rw-r--r--   0        0        0   140591 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT_ROAM_3FF5-53-0.fit
--rw-r--r--   0        0        0   152253 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT ROAM 3FF5-54-0.fit
--rw-r--r--   0        0        0   152253 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT_ROAM_3FF5-54-0.fit
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/power_profile_2.csv
--rw-r--r--   0        0        0   197110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/vincent_lap_1_24HOP_14012433014_ACTIVITY.fit
--rw-r--r--   0        0        0   186596 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/vincent_lap_2_24HOP_14010180820_ACTIVITY.fit
--rw-r--r--   0        0        0   431114 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/tests/test_data/vincent_mtb_id_surface_14517623900_ACTIVITY.fit
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/LICENSE.md
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/README.md
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/qodana.yaml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/ruff.toml
+-rw-r--r--   0        0        0   660177 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/note_books/Critical Power.ipynb
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/note_books/Surface.ipynb
+-rw-r--r--   0        0        0   290283 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/note_books/examples.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/src/cycling_dynamics/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/src/cycling_dynamics/__init__.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/src/cycling_dynamics/calc.py
+-rw-r--r--   0        0        0    12441 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/src/cycling_dynamics/critical_power.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/src/cycling_dynamics/load_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/src/cycling_dynamics/models.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/src/cycling_dynamics/plots.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/src/cycling_dynamics/stats.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/src/cycling_dynamics/surface.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/tests/test_critical_power.py
+-rw-r--r--   0        0        0   140591 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT ROAM 3FF5-53-0.fit
+-rw-r--r--   0        0        0   140591 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT_ROAM_3FF5-53-0.fit
+-rw-r--r--   0        0        0   152253 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT ROAM 3FF5-54-0.fit
+-rw-r--r--   0        0        0   152253 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT_ROAM_3FF5-54-0.fit
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/tests/test_data/power_profile_2.csv
+-rw-r--r--   0        0        0   197110 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/tests/test_data/vincent_lap_1_24HOP_14012433014_ACTIVITY.fit
+-rw-r--r--   0        0        0   186596 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/tests/test_data/vincent_lap_2_24HOP_14010180820_ACTIVITY.fit
+-rw-r--r--   0        0        0   431114 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/tests/test_data/vincent_mtb_id_surface_14517623900_ACTIVITY.fit
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/README.md
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 cycling_dynamics-0.0.9/PKG-INFO
```

### Comparing `cycling_dynamics-0.0.8/qodana.yaml` & `cycling_dynamics-0.0.9/qodana.yaml`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/ruff.toml` & `cycling_dynamics-0.0.9/ruff.toml`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/note_books/Critical Power.ipynb` & `cycling_dynamics-0.0.9/note_books/Critical Power.ipynb`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/note_books/Surface.ipynb` & `cycling_dynamics-0.0.9/note_books/Surface.ipynb`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/note_books/examples.ipynb` & `cycling_dynamics-0.0.9/note_books/examples.ipynb`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/src/cycling_dynamics/calc.py` & `cycling_dynamics-0.0.9/src/cycling_dynamics/calc.py`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/src/cycling_dynamics/critical_power.py` & `cycling_dynamics-0.0.9/src/cycling_dynamics/critical_power.py`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/src/cycling_dynamics/load_data.py` & `cycling_dynamics-0.0.9/src/cycling_dynamics/load_data.py`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/src/cycling_dynamics/plots.py` & `cycling_dynamics-0.0.9/src/cycling_dynamics/plots.py`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/src/cycling_dynamics/stats.py` & `cycling_dynamics-0.0.9/src/cycling_dynamics/stats.py`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/tests/test_critical_power.py` & `cycling_dynamics-0.0.9/tests/test_critical_power.py`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT ROAM 3FF5-53-0.fit` & `cycling_dynamics-0.0.9/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT ROAM 3FF5-53-0.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT_ROAM_3FF5-53-0.fit` & `cycling_dynamics-0.0.9/tests/test_data/alex_24HOP_2024-02-17-185919-ELEMNT_ROAM_3FF5-53-0.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT ROAM 3FF5-54-0.fit` & `cycling_dynamics-0.0.9/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT ROAM 3FF5-54-0.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT_ROAM_3FF5-54-0.fit` & `cycling_dynamics-0.0.9/tests/test_data/alex_24HOP_2024-02-18-002255-ELEMNT_ROAM_3FF5-54-0.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/tests/test_data/power_profile_2.csv` & `cycling_dynamics-0.0.9/tests/test_data/power_profile_2.csv`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/tests/test_data/vincent_lap_1_24HOP_14012433014_ACTIVITY.fit` & `cycling_dynamics-0.0.9/tests/test_data/vincent_lap_1_24HOP_14012433014_ACTIVITY.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/tests/test_data/vincent_lap_2_24HOP_14010180820_ACTIVITY.fit` & `cycling_dynamics-0.0.9/tests/test_data/vincent_lap_2_24HOP_14010180820_ACTIVITY.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/tests/test_data/vincent_mtb_id_surface_14517623900_ACTIVITY.fit` & `cycling_dynamics-0.0.9/tests/test_data/vincent_mtb_id_surface_14517623900_ACTIVITY.fit`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/.gitignore` & `cycling_dynamics-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/LICENSE.md` & `cycling_dynamics-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/README.md` & `cycling_dynamics-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cycling_dynamics-0.0.8/pyproject.toml` & `cycling_dynamics-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
-dependencies = ["numpy==1.26.4",
+dependencies = ["numpy>=1.26.4",
     "pandas>=2.2",
     "pyarrow>=16.0",
     "matplotlib>=3.8.3",
-    "garmin-fit-sdk==21.133.0",
+    "garmin-fit-sdk>=21.133.0",
     "plotly>=5.20.0",
 ]
 
 [project.urls]
 Documentation = "https://github.com/vincentdavis/cycling-dynamics#readme"
 Issues = "https://github.com/vincentdavis/cycling-dynamics/issues"
 Source = "https://github.com/vincentdavis/cycling-dynamics"
```

### Comparing `cycling_dynamics-0.0.8/PKG-INFO` & `cycling_dynamics-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: cycling-dynamics
-Version: 0.0.8
+Version: 0.0.9
 Summary: Cycling (Bicycling) models of motion, air drag, rolling resistance, power calculations.
 Project-URL: Documentation, https://github.com/vincentdavis/cycling-dynamics#readme
 Project-URL: Issues, https://github.com/vincentdavis/cycling-dynamics/issues
 Project-URL: Source, https://github.com/vincentdavis/cycling-dynamics
 Author-email: Vincent Davis <v@heteroskedastic.org>
 License-Expression: MIT
 License-File: LICENSE.md
 Keywords: Air Resistance,Calculations,Marginal Gains,Rolling Resistance,bicycle,cycling,dynamics,speed
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.12
-Requires-Dist: garmin-fit-sdk==21.133.0
+Requires-Dist: garmin-fit-sdk>=21.133.0
 Requires-Dist: matplotlib>=3.8.3
-Requires-Dist: numpy==1.26.4
+Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2
 Requires-Dist: plotly>=5.20.0
 Requires-Dist: pyarrow>=16.0
 Description-Content-Type: text/markdown
 
 # Cycling Dynamics
 Cycling (Bicycling) models of motion, air drag, rolling resistance, power calculations.
```

