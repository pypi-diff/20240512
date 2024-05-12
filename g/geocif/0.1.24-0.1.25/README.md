# Comparing `tmp/geocif-0.1.24.tar.gz` & `tmp/geocif-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocif-0.1.24.tar", last modified: Fri May 10 01:09:35 2024, max compression
+gzip compressed data, was "geocif-0.1.25.tar", last modified: Sun May 12 14:58:50 2024, max compression
```

## Comparing `geocif-0.1.24.tar` & `geocif-0.1.25.tar`

### file list

```diff
@@ -1,55 +1,61 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 01:09:35.405721 geocif-0.1.24/
--rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.24/LICENSE
--rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.24/MANIFEST.in
--rw-rw-rw-   0        0        0     1270 2024-05-10 01:09:35.405721 geocif-0.1.24/PKG-INFO
--rw-rw-rw-   0        0        0      589 2024-05-10 00:49:32.000000 geocif-0.1.24/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 01:09:35.232711 geocif-0.1.24/geocif/
--rw-rw-rw-   0        0        0      148 2024-05-09 17:33:59.000000 geocif-0.1.24/geocif/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:09:35.327014 geocif-0.1.24/geocif/agmet/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.24/geocif/agmet/__init__.py
--rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.24/geocif/agmet/geoagmet.py
--rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.24/geocif/agmet/plot.py
--rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.24/geocif/agmet/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:09:35.358308 geocif-0.1.24/geocif/backup/
--rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.24/geocif/backup/__init__.py
--rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.24/geocif/backup/constants.py
--rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.24/geocif/backup/features.py
--rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.24/geocif/backup/geo.py
--rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.24/geocif/backup/geocif.py
--rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.24/geocif/backup/metadata.py
--rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.24/geocif/backup/models.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:09:35.373920 geocif-0.1.24/geocif/cei/
--rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.24/geocif/cei/__init__.py
--rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.24/geocif/cei/definitions.py
--rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.24/geocif/cei/indices.py
--rw-rw-rw-   0        0        0    40714 2024-05-10 01:09:03.000000 geocif-0.1.24/geocif/geocif.py
--rw-rw-rw-   0        0        0     6426 2024-05-09 19:50:03.000000 geocif-0.1.24/geocif/indices_runner.py
--rw-rw-rw-   0        0        0     2267 2024-05-10 00:58:39.000000 geocif-0.1.24/geocif/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:09:35.405721 geocif-0.1.24/geocif/ml/
--rw-rw-rw-   0        0        0        0 2024-05-09 17:32:51.000000 geocif-0.1.24/geocif/ml/__init__.py
--rw-rw-rw-   0        0        0    31393 2024-05-09 15:38:37.000000 geocif-0.1.24/geocif/ml/analysis.py
--rw-rw-rw-   0        0        0    12251 2024-05-09 21:07:36.000000 geocif-0.1.24/geocif/ml/correlations.py
--rw-rw-rw-   0        0        0     5054 2024-05-09 20:41:26.000000 geocif-0.1.24/geocif/ml/embedding.py
--rw-rw-rw-   0        0        0    12505 2024-05-09 22:33:28.000000 geocif-0.1.24/geocif/ml/feature_engineering.py
--rw-rw-rw-   0        0        0     6562 2024-05-09 20:18:20.000000 geocif-0.1.24/geocif/ml/feature_selection.py
--rw-rw-rw-   0        0        0    12461 2024-05-09 15:38:37.000000 geocif-0.1.24/geocif/ml/misc.py
--rw-rw-rw-   0        0        0     9769 2024-05-09 15:38:36.000000 geocif-0.1.24/geocif/ml/outliers.py
--rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.24/geocif/ml/outlook.py
--rw-rw-rw-   0        0        0     3542 2024-05-09 19:16:41.000000 geocif-0.1.24/geocif/ml/output.py
--rw-rw-rw-   0        0        0     8044 2024-05-09 19:16:41.000000 geocif-0.1.24/geocif/ml/stages.py
--rw-rw-rw-   0        0        0     4961 2024-05-09 19:26:37.000000 geocif-0.1.24/geocif/ml/stats.py
--rw-rw-rw-   0        0        0     9718 2024-05-09 21:02:58.000000 geocif-0.1.24/geocif/ml/trainers.py
--rw-rw-rw-   0        0        0     3149 2024-05-09 19:24:05.000000 geocif-0.1.24/geocif/ml/trend.py
--rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.24/geocif/ml/xai.py
--rw-rw-rw-   0        0        0    18531 2024-05-10 00:58:39.000000 geocif-0.1.24/geocif/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:09:35.311381 geocif-0.1.24/geocif.egg-info/
--rw-rw-rw-   0        0        0     1270 2024-05-10 01:09:34.000000 geocif-0.1.24/geocif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1002 2024-05-10 01:09:35.000000 geocif-0.1.24/geocif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 01:09:34.000000 geocif-0.1.24/geocif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.24/geocif.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-05-10 01:09:34.000000 geocif-0.1.24/geocif.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.24/requirements.txt
--rw-rw-rw-   0        0        0      415 2024-05-10 01:09:35.421349 geocif-0.1.24/setup.cfg
--rw-rw-rw-   0        0        0     1620 2024-05-10 01:09:32.000000 geocif-0.1.24/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 01:09:35.405721 geocif-0.1.24/tests/
--rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.24/tests/test_geocif.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:58:50.380838 geocif-0.1.25/
+-rw-rw-rw-   0        0        0     1096 2023-07-27 15:12:03.000000 geocif-0.1.25/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-07-27 15:12:03.000000 geocif-0.1.25/MANIFEST.in
+-rw-rw-rw-   0        0        0     1586 2024-05-12 14:58:50.379839 geocif-0.1.25/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2024-05-12 14:58:37.000000 geocif-0.1.25/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 14:58:50.057218 geocif-0.1.25/geocif/
+-rw-rw-rw-   0        0        0      155 2024-05-10 16:27:36.000000 geocif-0.1.25/geocif/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:58:50.142733 geocif-0.1.25/geocif/agmet/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:42.000000 geocif-0.1.25/geocif/agmet/__init__.py
+-rw-rw-rw-   0        0        0     6201 2024-05-09 16:20:58.000000 geocif-0.1.25/geocif/agmet/geoagmet.py
+-rw-rw-rw-   0        0        0    27060 2024-05-09 16:20:58.000000 geocif-0.1.25/geocif/agmet/plot.py
+-rw-rw-rw-   0        0        0     6907 2023-07-27 16:56:06.000000 geocif-0.1.25/geocif/agmet/utils.py
+-rw-rw-rw-   0        0        0    34217 2024-05-11 02:14:29.000000 geocif-0.1.25/geocif/analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:58:50.211777 geocif-0.1.25/geocif/backup/
+-rw-rw-rw-   0        0        0        0 2024-05-09 16:19:12.000000 geocif-0.1.25/geocif/backup/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-07-27 15:12:03.000000 geocif-0.1.25/geocif/backup/constants.py
+-rw-rw-rw-   0        0        0    10198 2024-05-10 00:43:58.000000 geocif-0.1.25/geocif/backup/features.py
+-rw-rw-rw-   0        0        0     9919 2023-10-24 19:21:13.000000 geocif-0.1.25/geocif/backup/geo.py
+-rw-rw-rw-   0        0        0    17693 2024-05-09 16:20:58.000000 geocif-0.1.25/geocif/backup/geocif.py
+-rw-rw-rw-   0        0        0     1284 2023-10-24 19:33:45.000000 geocif-0.1.25/geocif/backup/metadata.py
+-rw-rw-rw-   0        0        0       65 2023-07-27 16:50:11.000000 geocif-0.1.25/geocif/backup/models.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:58:50.251226 geocif-0.1.25/geocif/cei/
+-rw-rw-rw-   0        0        0       83 2024-05-09 17:30:03.000000 geocif-0.1.25/geocif/cei/__init__.py
+-rw-rw-rw-   0        0        0     5125 2024-05-09 18:11:43.000000 geocif-0.1.25/geocif/cei/definitions.py
+-rw-rw-rw-   0        0        0    27358 2024-05-09 19:45:29.000000 geocif-0.1.25/geocif/cei/indices.py
+-rw-rw-rw-   0        0        0    42331 2024-05-11 03:29:36.000000 geocif-0.1.25/geocif/geocif.py
+-rw-rw-rw-   0        0        0     6709 2024-05-12 14:57:40.000000 geocif-0.1.25/geocif/indices_runner.py
+-rw-rw-rw-   0        0        0     2274 2024-05-10 01:57:37.000000 geocif-0.1.25/geocif/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:58:50.344544 geocif-0.1.25/geocif/ml/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.25/geocif/ml/__init__.py
+-rw-rw-rw-   0        0        0    12171 2024-05-11 02:34:09.000000 geocif-0.1.25/geocif/ml/correlations.py
+-rw-rw-rw-   0        0        0     5054 2024-05-09 20:41:26.000000 geocif-0.1.25/geocif/ml/embedding.py
+-rw-rw-rw-   0        0        0    12671 2024-05-12 03:53:54.000000 geocif-0.1.25/geocif/ml/feature_engineering.py
+-rw-rw-rw-   0        0        0     7015 2024-05-12 03:04:01.000000 geocif-0.1.25/geocif/ml/feature_selection.py
+-rw-rw-rw-   0        0        0     9769 2024-05-09 15:38:36.000000 geocif-0.1.25/geocif/ml/outliers.py
+-rw-rw-rw-   0        0        0      526 2024-03-31 02:56:14.000000 geocif-0.1.25/geocif/ml/outlook.py
+-rw-rw-rw-   0        0        0     3671 2024-05-10 17:25:05.000000 geocif-0.1.25/geocif/ml/output.py
+-rw-rw-rw-   0        0        0     8286 2024-05-12 14:57:40.000000 geocif-0.1.25/geocif/ml/stages.py
+-rw-rw-rw-   0        0        0     8119 2024-05-12 03:17:46.000000 geocif-0.1.25/geocif/ml/stats.py
+-rw-rw-rw-   0        0        0     9718 2024-05-10 14:56:22.000000 geocif-0.1.25/geocif/ml/trainers.py
+-rw-rw-rw-   0        0        0     3149 2024-05-09 19:24:05.000000 geocif-0.1.25/geocif/ml/trend.py
+-rw-rw-rw-   0        0        0     2831 2024-05-09 19:24:05.000000 geocif-0.1.25/geocif/ml/xai.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:58:50.357282 geocif-0.1.25/geocif/playground/
+-rw-rw-rw-   0        0        0        0 2024-05-10 19:03:20.000000 geocif-0.1.25/geocif/playground/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-10 18:55:55.000000 geocif-0.1.25/geocif/playground/automl.py
+-rw-rw-rw-   0        0        0    13665 2024-05-11 01:04:25.000000 geocif-0.1.25/geocif/playground/misc.py
+-rw-rw-rw-   0        0        0    18744 2024-05-12 14:57:40.000000 geocif-0.1.25/geocif/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:58:50.361240 geocif-0.1.25/geocif/viz/
+-rw-rw-rw-   0        0        0       83 2024-05-10 16:27:36.000000 geocif-0.1.25/geocif/viz/__init__.py
+-rw-rw-rw-   0        0        0    15867 2024-05-10 17:06:33.000000 geocif-0.1.25/geocif/viz/plot.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:58:50.107461 geocif-0.1.25/geocif.egg-info/
+-rw-rw-rw-   0        0        0     1586 2024-05-12 14:58:49.000000 geocif-0.1.25/geocif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1107 2024-05-12 14:58:49.000000 geocif-0.1.25/geocif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 14:58:49.000000 geocif-0.1.25/geocif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-10-22 16:27:17.000000 geocif-0.1.25/geocif.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-05-12 14:58:49.000000 geocif-0.1.25/geocif.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:05:13.000000 geocif-0.1.25/requirements.txt
+-rw-rw-rw-   0        0        0      415 2024-05-12 14:58:50.389350 geocif-0.1.25/setup.cfg
+-rw-rw-rw-   0        0        0     1617 2024-05-12 14:57:56.000000 geocif-0.1.25/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 14:58:50.378840 geocif-0.1.25/tests/
+-rw-rw-rw-   0        0        0      355 2024-05-09 16:20:58.000000 geocif-0.1.25/tests/test_geocif.py
```

### Comparing `geocif-0.1.24/LICENSE` & `geocif-0.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/PKG-INFO` & `geocif-0.1.25/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.24
+Version: 0.1.25
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -27,14 +27,22 @@
 **Models to visualize and forecast crop conditions and yields**
 
 
 -   Free software: MIT license
 -   Documentation: https://ritviksahajpal.github.io/yield_forecasting/
 
 
-## Features
+### Upload package to pypi
+1. Update requirements.txt
+2. Update version="A.B.C" in setup.py
+3. Navigate to the directory containing `setup.py` and run the following command:
+```python
+pipreqs . --force --savepath requirements.txt
+mamba env export > environment.yml
+python setup.py sdist
+twine upload dist/geocif-A.B.C.tar.gz
+```
 
--   TODO
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geocif-0.1.24/geocif/agmet/geoagmet.py` & `geocif-0.1.25/geocif/agmet/geoagmet.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/agmet/plot.py` & `geocif-0.1.25/geocif/agmet/plot.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/agmet/utils.py` & `geocif-0.1.25/geocif/agmet/utils.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/backup/features.py` & `geocif-0.1.25/geocif/backup/features.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/backup/geo.py` & `geocif-0.1.25/geocif/backup/geo.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/backup/geocif.py` & `geocif-0.1.25/geocif/backup/geocif.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/backup/metadata.py` & `geocif-0.1.25/geocif/backup/metadata.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/cei/definitions.py` & `geocif-0.1.25/geocif/cei/definitions.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/cei/indices.py` & `geocif-0.1.25/geocif/cei/indices.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/geocif.py` & `geocif-0.1.25/geocif/geocif.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,33 @@
 import geopandas as gp
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import sklearn
 from tqdm import tqdm
 
+from geocif import logger as log
 from .cei import definitions as di
 from .ml import correlations
 from .ml import feature_engineering as fe
 from .ml import feature_selection as fs
-from geocif import logger as log
 from .ml import output
 from .ml import stages
 from .ml import stats
 from .ml import trainers
 from .ml import trend
 from .ml import xai
 
 plt.style.use("default")
 sklearn.set_config(transform_output="pandas")
 
+import warnings
+
+warnings.simplefilter(action="ignore", category=FutureWarning)
+
 
 class TimeFilter:
     def __init__(self, threshold=1):  # Time threshold in seconds
         self.threshold = threshold
 
     def __call__(self, frame):
         return frame.time() > self.threshold
@@ -53,17 +57,17 @@
         default_factory=lambda: ["Index", "Country", "Region", "Crop", "Season"]
     )
     metrics: List[str] = field(default_factory=lambda: ["$r^2$", "RMSE", "MAE", "MAPE"])
     logger: log = None
     parser: ConfigParser = field(default_factory=ConfigParser)
 
     def __post_init__(self):
-        self.out_dir = Path(self.parser.get("PATHS", "dir_output"))
+        self.dir_output = Path(self.parser.get("PATHS", "dir_output"))
         self.dir_condition = Path(self.parser.get("PATHS", "dir_condition"))
-        os.makedirs(self.out_dir / "ml", exist_ok=True)
+        os.makedirs(self.dir_output / "ml", exist_ok=True)
 
         self.country: str = None
         self.crop: str = None
         self.forecast_season: int = None
         self.all_stages: list = []
         self.all_seasons: list = []
         self.all_seasons_with_yield: list = []
@@ -72,55 +76,69 @@
         self.selected_features: list = []
         self.num_cpus = mp.cpu_count()
 
         self._date = ar.utcnow().to("America/New_York")
         self.today = self._date.format("MMMM_DD_YYYY")
         self.today_year = self._date.year
         self.today_doy = int(self._date.format("DDD"))
-        self.today_full = self._date.format("MMMM_DD_YYYY HH:mm")
+        self.today_full = self._date.format("MMMM_DD_YYYY_HH_mm")
 
         self.df_forecast = pd.DataFrame()
         """
         ====================================================================
                                 Config file: Default
         ====================================================================
         """
         self.method = self.parser.get("DEFAULT", "method")
         self.db_forecasts = self.parser.get("DEFAULT", "db")
         self.countries = ast.literal_eval(self.parser.get("DEFAULT", "countries"))
         self.do_parallel = self.parser.getboolean("DEFAULT", "do_parallel")
         self.update_input_file = self.parser.getboolean("DEFAULT", "update_input_file")
-        self.national_correlation = self.parser.getboolean("DEFAULT", "national_correlation")
-        self.correlation_plot_groupby = self.parser.get("DEFAULT", "correlation_plot_groupby")
+        self.national_correlation = self.parser.getboolean(
+            "DEFAULT", "national_correlation"
+        )
+        self.correlation_plot_groupby = self.parser.get(
+            "DEFAULT", "correlation_plot_groupby"
+        )
         self.run_ml = self.parser.getboolean("DEFAULT", "run_ml")
 
         """
         ====================================================================
                                 Config file: ML
         ====================================================================
         """
         self.model_type = self.parser.get("ML", "model_type")
         self.fraction_simulate = self.parser.getint("ML", "fraction_simulate")
         self.analogous_year_yield_as_feature = self.parser.getboolean(
             "ML", "analogous_year_yield_as_feature"
         )
-        self.last_year_yield_as_feature = self.parser.getboolean("ML", "last_year_yield_as_feature")
+        self.last_year_yield_as_feature = self.parser.getboolean(
+            "ML", "last_year_yield_as_feature"
+        )
         self.panel_model = self.parser.getboolean("ML", "panel_model")
         self.panel_model_region = self.parser.get("ML", "panel_model_region")
-        self.use_outlook_as_feature = self.parser.getboolean("ML", "use_outlook_as_feature")
+        self.use_outlook_as_feature = self.parser.getboolean(
+            "ML", "use_outlook_as_feature"
+        )
         self.lag_yield_as_feature = self.parser.getboolean("ML", "lag_yield_as_feature")
         self.number_median_years = self.parser.getint("ML", "median_years")
-        self.median_yield_as_feature = self.parser.getboolean("ML", "median_yield_as_feature")
+        self.median_yield_as_feature = self.parser.getboolean(
+            "ML", "median_yield_as_feature"
+        )
         self.number_lag_years = self.parser.getint("ML", "lag_years")
         self.cluster_strategy = self.parser.get("ML", "cluster_strategy")
         self.feature_selection = self.parser.get("ML", "feature_selection")
         self.check_yield_trend = self.parser.getboolean("ML", "check_yield_trend")
-        self.run_latest_time_period = self.parser.getboolean("ML", "run_latest_time_period")
+        self.run_latest_time_period = self.parser.getboolean(
+            "ML", "run_latest_time_period"
+        )
         self.run_every_time_period = self.parser.get("ML", "run_every_time_period")
-        self.cat_features: list = ast.literal_eval(self.parser.get("ML", "cat_features"))
+        self.cat_features: list = ast.literal_eval(
+            self.parser.get("ML", "cat_features")
+        )
 
         """
         ====================================================================
                                 Variables, Paths
         ====================================================================
         """
         # If ML model is run for individual region or cluster, then Region_ID is the same for each region
@@ -132,15 +150,15 @@
             "Country",
             "Region",
             "Crop",
             "Area",
             "Season",
             "Harvest Year",
         ]
-        self.target_column: str = "Yield (tn per ha)"
+        self.target: str = "Yield (tn per ha)"
         self.statistics_columns: list = [
             "Area (ha)",
             "Production (tn)",
         ]
 
         self.combined_dict = {
             **di.dict_indices,
@@ -148,24 +166,24 @@
             **di.dict_gcvi,
             **di.dict_esi4wk,
             **di.dict_hindex,
         }
 
         self.combined_keys = list(self.combined_dict.keys())
 
-        self.ml_dir = self.out_dir / "ml"
-        self.db_dir = self.ml_dir / "db"
-        self.analysis_dir = self.ml_dir / "analysis" / self.today
+        self.dir_ml = self.dir_output / "ml"
+        self.dir_db = self.dir_ml / "db"
+        self.dir_analysis = self.dir_ml / "analysis" / self.today
         dir_input = Path(self.parser.get("PATHS", "dir_input"))
         self.dir_shapefiles = dir_input / "Global_Datasets" / "Regions" / "Shps"
 
-        os.makedirs(self.db_dir, exist_ok=True)
-        os.makedirs(self.analysis_dir, exist_ok=True)
+        os.makedirs(self.dir_db, exist_ok=True)
+        os.makedirs(self.dir_analysis, exist_ok=True)
 
-        self.db_path = self.db_dir / self.db_forecasts
+        self.db_path = self.dir_db / self.db_forecasts
         output.config_to_db(self.db_path, self.parser, self.today_full)
 
         # self.pickle_file = self.base_dir / self.parser.get("outlook", "pickle_file")
         # obj_pickle = outlook.Outlook(self.pickle_file)
         # self.df_outlook = obj_pickle.read_outlook_file()
 
     def train(self, df_region, scaler=None):
@@ -177,49 +195,58 @@
 
         Returns:
 
         """
 
         """ Perform feature selection """
         target_col = (
-            f"Detrended {self.target_column}" if self.check_yield_trend else self.target_column
+            f"Detrended {self.target}" if self.check_yield_trend else self.target
         )
 
         X_train = df_region[self.feature_names]
         # Drop any columns with NaNs
         X_train = X_train.dropna(axis=1, how="any")
         y_train = df_region[target_col]
 
         if self.ml_model:
+            self.logger.info(f"Selecting features for {self.country} {self.crop}")
             selector, _, self.selected_features = fs.select_features(
                 X_train, y_train, method=self.feature_selection
             )
+            self.logger.info(f"Selected features: {self.selected_features}")
 
             """ Update model to include conformal estimates """
             X_train = df_region[self.selected_features + self.cat_features]
+            dir_output = (
+                self.dir_analysis / self.country / self.crop / self.model_name / str(self.forecast_season)
+            )
 
+            region_id = df_region["Region_ID"].unique()[0]
+            X_train.to_csv(dir_output / f"X_train_{region_id}.csv", index=False)
             if scaler:
                 X_train_nocat = X_train.drop(
-                    columns=[item for item in self.cat_features if item != "Harvest Year"]
+                    columns=[
+                        item for item in self.cat_features if item != "Harvest Year"
+                    ]
                 )
                 X_train_scaled = scaler.fit_transform(X_train_nocat)
             else:
                 X_train_scaled = X_train
 
             """ Train model """
             self.best_hyperparams, self.model = trainers.auto_train(
                 self.cluster_strategy,
                 self.model_name,
                 False,
                 "Harvest Year",
-                df_region[self.selected_features + self.cat_features + [self.target_column]],
+                df_region[self.selected_features + self.cat_features + [self.target]],
                 X_train_scaled,
                 y_train,
                 feature_names=self.selected_features,
-                target_col=self.target_column,
+                target_col=self.target,
                 optimize=self.optimize,
                 fraction_loocv=self.fraction_loocv,
                 cat_features=self.cat_features,
                 monotonic_fatures=[],
                 seed=0,
             )
 
@@ -268,31 +295,35 @@
         """
         Predict yield for the current stage
         :param df_region:
         :param scaler:
         """
         """ Select dataframe for prediction"""
         X_test = df_region[self.selected_features + self.cat_features]
-        y_test = df_region[self.target_column].values
+        y_test = df_region[self.target].values
 
         """ Do prediction based on model type"""
         if not self.ml_model:
             best_hyperparameters = np.nan
             if self.model_name == "analog":
                 y_pred = np.full(len(X_test), df_region["Analogous Year Yield"].values)
             elif self.model_name == "median":
-                y_pred = np.full(len(X_test), df_region[f"Median {self.target_column}"].values)
+                y_pred = np.full(len(X_test), df_region[f"Median {self.target}"].values)
             elif self.model_name == "last_year":
-                y_pred = np.full(len(X_test), df_region[f"Last Year {self.target_column}"].values)
+                y_pred = np.full(
+                    len(X_test), df_region[f"Last Year {self.target}"].values
+                )
         else:
             best_hyperparameters = self.model.get_params().copy()
             if self.model_name in ["linear", "gam"]:
                 # Drop cat_features from X_test
                 X_test = X_test.drop(
-                    columns=[item for item in self.cat_features if item != "Harvest Year"]
+                    columns=[
+                        item for item in self.cat_features if item != "Harvest Year"
+                    ]
                 )
                 X_test = scaler.transform(X_test)
                 best_hyperparameters = {}
 
             if self.estimate_ci:
                 if self.estimate_ci_for_all or self.forecast_season == self.today_year:
                     y_pred, y_pred_ci = self.model.predict(X_test, alpha=0.1)
@@ -306,27 +337,27 @@
         if self.check_yield_trend:
             # Get information for retrending
             for idx, region in enumerate(df_region["Region"].unique()):
                 mask_region = self.df_train["Region"] == df_region["Region"].unique()[0]
                 df_tmp = self.df_train[mask_region]
 
                 obj_trend = trend.DetrendedData(
-                    df_tmp[f"Detrended {self.target_column}"],
+                    df_tmp[f"Detrended {self.target}"],
                     df_tmp["Detrend Model"],
                     df_tmp["Detrend Model Type"],
                 )
 
                 # Retrend the predicted yield
                 y_pred[idx] += trend.compute_trend(
                     obj_trend, df_region.iloc[idx][["Harvest Year"]]
                 )[0]
 
         # Create a dataframe with forecast results
         shp = len(X_test)
-        experiment_id = f"{self.country}_{self.crop}"
+        experiment_id = f"{self.country}-{self.crop}"
         now = ar.utcnow().to("America/New_York").format("MMMM-DD-YYYY HH:mm:ss")
         selected_features = self.selected_features + self.cat_features
         df = pd.DataFrame(
             {
                 "Experiment_ID": np.full(shp, experiment_id),
                 "Date": np.full(shp, self.today),
                 "Time": np.full(shp, now),
@@ -342,23 +373,23 @@
                 "Starting Stage": np.full(shp, self.stage_info["Starting Stage"]),
                 "Ending Stage": np.full(shp, self.stage_info["Ending Stage"]),
                 "Model": np.full(shp, self.model_name),
                 "Area (ha)": df_region["Area (ha)"].values,
                 "Region_ID": df_region["Region_ID"].values,
                 "Region": df_region["Region"].values,
                 "Harvest Year": df_region["Harvest Year"].values,
-                f"Observed {self.target_column}": np.around(y_test, 3).ravel(),
-                f"Predicted {self.target_column}": np.around(y_pred, 3).ravel(),
+                f"Observed {self.target}": np.around(y_test, 3).ravel(),
+                f"Predicted {self.target}": np.around(y_pred, 3).ravel(),
             }
         )
 
         if self.median_yield_as_feature:
             # Add median yield to dataframe
-            df.loc[:, f"Median {self.target_column}"] = np.around(
-                df_region[f"Median {self.target_column}"].values, 3
+            df.loc[:, f"Median {self.target}"] = np.around(
+                df_region[f"Median {self.target}"].values, 3
             )
 
         if self.estimate_ci:
             if self.estimate_ci_for_all or self.forecast_season == self.today_year:
                 # Iterate over each element in y_pred_ci
                 for idx, ci in enumerate(y_pred_ci):
                     # Flatten the list
@@ -369,27 +400,30 @@
 
         if self.check_yield_trend:
             df.loc[:, "Detrended Model Type"] = df_region["Detrended Model Type"].values
             df.loc[:, "Detrended Model"] = df_region["Detrended Model"].values
 
         if self.last_year_yield_as_feature:
             # Add last year yield to dataframe
-            df.loc[:, f"Last Year {self.target_column}"] = np.around(
-                df_region[f"Last Year {self.target_column}"].values, 3
+            df.loc[:, f"Last Year {self.target}"] = np.around(
+                df_region[f"Last Year {self.target}"].values, 3
             )
 
         if self.analogous_year_yield_as_feature:
-            # Add analogous year and yield to dataframe
-            df.loc[:, "Analogous Year"] = df_region["Analogous Year"].values
-            df.loc[:, "Analogous Year Yield"] = np.around(
-                df_region["Analogous Year Yield"].values, 3
-            )
+            try:
+                # Add analogous year and yield to dataframe
+                df.loc[:, "Analogous Year"] = df_region["Analogous Year"].values
+                df.loc[:, "Analogous Year Yield"] = np.around(
+                    df_region["Analogous Year Yield"].values, 3
+                )
+            except:
+                breakpoint()
 
         for col in [
-            f"Median {self.target_column}",
+            f"Median {self.target}",
             "Analogous Year",
             "Analogous Year Yield",
             "Detrended Model Type",
             "Detrended Model",
         ]:
             if col not in df.columns:
                 df.loc[:, col] = np.NaN
@@ -399,15 +433,17 @@
             "Model",
             "Country",
             "Region",
             "Crop",
             "Harvest Year",
             "Stage Name",
         ]
-        df.index = df.apply(lambda row: "_".join([str(row[col]) for col in index_columns]), axis=1)
+        df.index = df.apply(
+            lambda row: "_".join([str(row[col]) for col in index_columns]), axis=1
+        )
 
         # name the index level
         df.index.set_names(["Index"], inplace=True)
 
         return experiment_id, df
 
     def create_feature_names(self, stages_features, selected_features):
@@ -423,15 +459,17 @@
         # Clear out feature names
         self.feature_names = []
 
         """ Select stages that will be used for ML
          1. method = "latest" - Select the latest stage
          2. method = "fraction" - Select a fraction (1-100) of all stages
         """
-        stages_features = stages.select_stages_for_ml(stages_features, method="fraction", n=30)
+        stages_features = stages.select_stages_for_ml(
+            stages_features, method="fraction", n=30
+        )
 
         for stage in stages_features:
             # Convert each element of stage to str and join with _
             _stage = "_".join([str(x) for x in stage])
 
             # Create a list appending _stage to each element of combined_keys
             _tmp = [f"{col}_{_stage}" for col in self.combined_keys]
@@ -450,20 +488,20 @@
 
                     if tmp_col in self.df_train.columns:
                         self.feature_names.append(tmp_col)
 
         self.feature_names = list(set(self.feature_names))
 
         if self.median_yield_as_feature:
-            self.feature_names.append(f"Median {self.target_column}")
+            self.feature_names.append(f"Median {self.target}")
 
         if self.lag_yield_as_feature:
             # For the number of years specified in self.number_lag_years
             for i in range(1, self.number_lag_years + 1):
-                self.feature_names.append(f"t -{i} {self.target_column}")
+                self.feature_names.append(f"t -{i} {self.target}")
 
         if self.analogous_year_yield_as_feature:
             self.feature_names.append("Analogous Year")
             self.feature_names.append("Analogous Year Yield")
 
         if self.use_outlook_as_feature:
             self.feature_names.append("FCST")
@@ -488,115 +526,120 @@
         """ Train, Predict, Explain and Store results for each region """
         pbar = tqdm(self.df_train["Region_ID"].unique(), leave=False)
         for idx, region in enumerate(pbar):
             if self.model_name in ["linear", "gam"]:
                 self.create_feature_names(stages, dict_best_cei[region][0:3].tolist())
             elif self.ml_model:
                 self.create_feature_names(stages, dict_selected_features[region])
+            elif self.model_name in ["median"]:
+                self.feature_names = [f"Median {self.target}"]
+                self.last_year_yield_as_feature = False
+                self.analogous_year_yield_as_feature = False
+            elif self.model_name in ["analog"]:
+                self.feature_names = [f"Analogous Year", f"Analogous Year Yield"]
+                self.last_year_yield_as_feature = False
+                self.median_yield_as_feature = False
 
             mask_train = self.df_train["Region_ID"] == region
             mask_test = self.df_test["Region_ID"] == region
 
             num_regions_in_cluster = self.df_train[mask_train]["Region"].unique()
 
             if self.cluster_strategy == "individual":
                 region_name = self.df_train["Region"].unique()[idx]
-                pbar.set_description(f"ML {region_name}")
+                pbar.set_description(f"Fit/Predict for {region_name}")
                 pbar.update()
             elif self.cluster_strategy in ["auto_detect", "single"]:
                 pbar.set_description(f"Fit/Predict for group {idx + 1}")
                 pbar.update()
 
             common_columns = (
-                [self.target_column] + self.statistics_columns + self.feature_names + ["Region_ID"]
+                [self.target]
+                + self.statistics_columns
+                + self.feature_names
+                + ["Region_ID"]
             )
             if self.check_yield_trend:
                 common_columns += ["Detrended Model Type", "Detrended Model"]
 
             if self.last_year_yield_as_feature:
-                common_columns += [f"Last Year {self.target_column}"]
+                common_columns += [f"Last Year {self.target}"]
 
             """ Train """
             # Filter dataframe based on region and self.feature_names
             df_region_train = self.df_train[mask_train]
             df_region_train = df_region_train[self.fixed_columns + common_columns]
             self.train(df_region_train, scaler)
 
-            try:
-                self.model_name in ["linear", "gam"] or self.model.is_fitted()
-            except:
-                breakpoint()
-
-            # Check if the model is fitted
-            if self.model_name in ["linear", "gam"] or self.model.is_fitted():
-                """Predict"""
-                df_region_test = self.df_test[mask_test]
-                df_region_test = df_region_test[self.fixed_columns + common_columns]
-                experiment_id, df = self.predict(df_region_test, scaler)
-                # df.reset_index(inplace=True)
-
-                if self.do_xai:
-                    assert not self.estimate_ci, "Cannot perform XAI if estimate_ci is True"
-
-                    kwargs = {
-                        "cluster_strategy": self.cluster_strategy,
-                        "model": self.model,
-                        "forecast_season": self.forecast_season,
-                        "crop": self.crop,
-                        "country": self.country,
-                        "analysis_dir": self.analysis_dir,
-                    }
-                    df_xai = xai.explain(df_region_train, df_region_test, **kwargs)
-                    # df.set_index("Index", inplace=True)
-
-                """ Output results to database """
-                if not self.ml_model:
-                    model = self.model_name
-                elif self.estimate_ci:
-                    model = self.model.estimator_
-                else:
-                    model = self.model
-                output.store(self.db_path, experiment_id, df, model, self.model_name)
+            """ Predict """
+            df_region_test = self.df_test[mask_test]
+            df_region_test = df_region_test[self.fixed_columns + common_columns]
+            experiment_id, df = self.predict(df_region_test, scaler)
+            # df.reset_index(inplace=True)
+
+            """ XAI """
+            if self.do_xai:
+                assert not self.estimate_ci, "Cannot perform XAI if estimate_ci is True"
+
+                kwargs = {
+                    "cluster_strategy": self.cluster_strategy,
+                    "model": self.model,
+                    "forecast_season": self.forecast_season,
+                    "crop": self.crop,
+                    "country": self.country,
+                    "analysis_dir": self.dir_analysis,
+                }
+                df_xai = xai.explain(df_region_train, df_region_test, **kwargs)
+                # df.set_index("Index", inplace=True)
+
+            """ Output results to database """
+            if not self.ml_model:
+                model = self.model_name
+            elif self.estimate_ci:
+                model = self.model.estimator_
+            else:
+                model = self.model
+            output.store(self.db_path, experiment_id, df, model, self.model_name)
 
     def create_ml_dataframe(self, df):
         """
         Create ML ready dataframe
         :param df:
         """
         _str = f"{self.country} {self.crop}"
         self.logger.info(f"Creating ML dataframe {_str}")
 
         # Convert from long to wide format
         df = df[
             ["Index", "Stage_ID", "CEI"]
             + self.fixed_columns
-            + [self.target_column]
+            + [self.target]
             + self.statistics_columns
         ]
 
         # For each combination of Index and Stage_ID, new columns have been
         # created and filled with the corresponding CEI value from the original dataframe
         # The new column names are a combination of the original Index and Stage_ID values
         # Use pivot_table to create the new columns and flatten the multi-index columns
         # HACK: Set missing values in self.target_col and self.statistics_columns to -1
-        df.loc[:, [self.target_column] + self.statistics_columns] = df[
-            [self.target_column] + self.statistics_columns
+        df.loc[:, [self.target] + self.statistics_columns] = df[
+            [self.target] + self.statistics_columns
         ].fillna(-1)
 
         # HACK, replace later
         df.loc[:, "Area"] = df["Area"].fillna(-1)
         df = df.pivot_table(
-            index=self.fixed_columns + [self.target_column] + self.statistics_columns,
+            index=self.fixed_columns + [self.target] + self.statistics_columns,
             columns=["Index", "Stage_ID"],
             values="CEI",
         ).reset_index()
 
         # Reset self.target_col and self.statistics_columns to NaN
-        df[[self.target_column] + self.statistics_columns] = df[
-            [self.target_column] + self.statistics_columns
+        df[[self.target] + self.statistics_columns] = df[
+            [self.target] + self.statistics_columns
         ].replace(-1, np.nan)
 
         # Flatten the multi-index columns
         df.columns = [f"{i}_{j}" if j != "" else f"{i}" for i, j in df.columns]
 
         # HACK: Get feature name with GD4 in it to extract first and last stage id and name
         GD4_column = df[df.columns[df.columns.str.contains("GD4")]].columns
@@ -608,28 +651,32 @@
         # e.g. 'vDTR_7_6_5_4_3_2_1_37_36_35_34_33_32_31' to 'vDTR Mar 1-Oct 27'
         df = stages.update_feature_names(df, self.method)
 
         # Get all the columns apart from the fixed columns, target column and stats columns
         all_cei_columns = [
             col
             for col in df.columns
-            if col not in self.fixed_columns + [self.target_column] + self.statistics_columns
+            if col not in self.fixed_columns + [self.target] + self.statistics_columns
         ]
 
         # Fill in any missing values with 0
         df.loc[:, all_cei_columns].fillna(0, inplace=True)
 
         if self.last_year_yield_as_feature:
             df = fe.compute_last_year_yield(df)
 
         if self.median_yield_as_feature:
-            df = fe.compute_median_yield(df, self.all_seasons_with_yield, self.number_median_years)
+            df = fe.compute_median_yield(
+                df, self.all_seasons_with_yield, self.number_median_years
+            )
 
         if self.lag_yield_as_feature:
-            df = fe.compute_lag_yield(df, self.all_seasons_with_yield, self.number_lag_years)
+            df = fe.compute_lag_yield(
+                df, self.all_seasons_with_yield, self.number_lag_years
+            )
 
         if self.analogous_year_yield_as_feature:
             df = fe.compute_analogous_yield(
                 df, self.all_seasons_with_yield, self.number_median_years
             )
 
         # Create Region_ID column based on Region column category code
@@ -662,18 +709,20 @@
             _stages.append(stage)
 
         mask = self.df_results["Stage_ID"].isin(_stages)
         df = self.df_results[mask]
 
         """ Convert this dataframe into an ML ready format and save to disk """
         df = self.create_ml_dataframe(df)
-        out_dir = self.analysis_dir / self.country / self.crop / str(self.forecast_season)
-        os.makedirs(out_dir, exist_ok=True)
+        dir_output = (
+            self.dir_analysis / self.country / self.crop / str(self.forecast_season)
+        )
+        os.makedirs(dir_output, exist_ok=True)
         df.to_csv(
-            out_dir / f"{self.country}_{self.crop}_{self.forecast_season}.csv",
+            dir_output / f"{self.country}_{self.crop}_{self.forecast_season}.csv",
             index=False,
         )
 
         # cat_features should be converted to category type
         df[self.cat_features] = df[self.cat_features].astype("category")
 
         """  Heatmap of correlation of various features with yield at each time step"""
@@ -692,18 +741,24 @@
             df[["Country Region", self.correlation_plot_groupby]],
             on="Country Region",
             how="outer",
         )
 
         dict_kwargs = {}
         dict_kwargs["all_stages"] = self.all_stages
-        dict_kwargs["target_col"] = self.target_column
+        dict_kwargs["target_col"] = self.target
         dict_kwargs["country"] = self.country
         dict_kwargs["crop"] = self.crop
-        dict_kwargs["analysis_dir"] = self.analysis_dir
+        dict_kwargs["dir_output"] = (
+            self.dir_analysis
+            / self.country
+            / self.crop
+            / self.model_name
+            / str(self.forecast_season)
+        )
         dict_kwargs["forecast_season"] = self.forecast_season
         dict_kwargs["method"] = self.method
         dict_kwargs["national_correlation"] = self.national_correlation
         dict_kwargs["groupby"] = self.correlation_plot_groupby
         dict_kwargs["dg_country"] = self.dg_country
         dict_kwargs["combined_dict"] = self.combined_dict
 
@@ -715,31 +770,37 @@
 
         """ Separate into train and test datasets based on forecast_season """
         mask = df["Harvest Year"] == self.forecast_season
         self.df_train = df[~mask]
         self.df_test = df[mask]
 
         # Drop rows with missing values for self.target_col in df_train
-        self.df_train = self.df_train.dropna(subset=[self.target_column])
+        self.df_train = self.df_train.dropna(subset=[self.target])
 
         """ Groupby Region column and compute detrended yield """
-        self.df_train[f"Detrended {self.target_column}"] = np.NaN
+        self.df_train[f"Detrended {self.target}"] = np.NaN
         self.df_train["Detrend Model"] = np.NaN
         self.df_train["Detrend Model Type"] = np.NaN
         if self.check_yield_trend:
             group_by = ["Region"]
             groups = self.df_train.groupby(group_by)
             for key, group in groups:
-                if group[self.target_column].any():
-                    detrended_data = trend.detrend_dataframe(group, column_name=self.target_column)
+                if group[self.target].any():
+                    detrended_data = trend.detrend_dataframe(
+                        group, column_name=self.target
+                    )
                     self.df_train.loc[
-                        group.index, f"Detrended {self.target_column}"
+                        group.index, f"Detrended {self.target}"
                     ] = detrended_data.detrended_series
-                    self.df_train.loc[group.index, "Detrend Model"] = detrended_data.trend_model
-                    self.df_train.loc[group.index, "Detrend Model Type"] = detrended_data.model_type
+                    self.df_train.loc[
+                        group.index, "Detrend Model"
+                    ] = detrended_data.trend_model
+                    self.df_train.loc[
+                        group.index, "Detrend Model Type"
+                    ] = detrended_data.model_type
 
         # 6. Exclude years without yields from df_train
         # self.df_train = self.df_train[
         #     self.df_train["Harvest Year"].isin(self.all_seasons_with_yield)
         # ]
 
         """ Run ML code for each stage """
@@ -749,15 +810,17 @@
             if self.run_latest_time_period:
                 # setup_stages = stages.select_stages_for_ml(setup_stages, method="latest")
                 setup_stages = [setup_stages[-1]]
 
             num_regions = len(self.df_train["Region_ID"].unique())
             pbar = tqdm(setup_stages)
             for stage in pbar:
-                pbar.set_description(f"ML {num_regions} regions, {len(setup_stages)} stages")
+                pbar.set_description(
+                    f"ML {num_regions} regions, {len(setup_stages)} stages"
+                )
                 pbar.update()
 
                 self.loop_ml(stage, dict_selected_features, dict_best_cei)
 
     def setup(self, forecast_season, model):
         """
 
@@ -782,21 +845,23 @@
             self.do_xai = False
             self.estimate_ci = False
             self.check_yield_trend = False
             self.estimate_ci_for_all = False
         else:
             self.do_xai = self.parser.getboolean("ML", "do_xai")
             self.estimate_ci = self.parser.getboolean("ML", "estimate_ci")
-            self.estimate_ci_for_all = self.parser.getboolean("ML", "estimate_ci_for_all")
+            self.estimate_ci_for_all = self.parser.getboolean(
+                "ML", "estimate_ci_for_all"
+            )
             self.check_yield_trend = self.parser.getboolean("ML", "check_yield_trend")
 
         # 1. Get all seasons with yield, these are the seasons for which Yield is available
-        self.all_seasons_with_yield = self.df_results[self.df_results[self.target_column].notna()][
-            "Harvest Year"
-        ].unique()
+        self.all_seasons_with_yield = self.df_results[
+            self.df_results[self.target].notna()
+        ]["Harvest Year"].unique()
 
         if self.method.endswith("_r"):
             if self.forecast_season == self.today_year:
                 mask = self.df_results["Harvest Year"] == self.forecast_season
                 self.all_stages = self.df_results[mask]["Stage_ID"].unique()
             else:
                 self.all_stages = self.df_results["Stage_ID"].unique()
@@ -826,29 +891,35 @@
         self.dg = gp.read_file(
             self.dir_shapefiles / self.name_shapefile,
             engine="pyogrio",
         )
 
         if "ADMIN0" in self.dg.columns:
             # Hack rename Tanzania to United Republic of Tanzania
-            self.dg["ADMIN0"] = self.dg["ADMIN0"].replace("Tanzania", "United Republic of Tanzania")
+            self.dg["ADMIN0"] = self.dg["ADMIN0"].replace(
+                "Tanzania", "United Republic of Tanzania"
+            )
 
         # Rename ADMIN0 to ADM0_NAME and ADMIN1 to ADM1_NAME and ADMIN2 to ADM2_NAME
         self.dg = self.dg.rename(
             columns={
                 "ADMIN0": "ADM0_NAME",
                 "ADMIN1": "ADM1_NAME",
                 "ADMIN2": "ADM2_NAME",
             }
         )
 
         if self.admin_zone == "admin_1":
-            self.dg["Country Region"] = self.dg["ADM0_NAME"] + " " + self.dg["ADM1_NAME"]
+            self.dg["Country Region"] = (
+                self.dg["ADM0_NAME"] + " " + self.dg["ADM1_NAME"]
+            )
         else:
-            self.dg["Country Region"] = self.dg["ADM0_NAME"] + " " + self.dg["ADM2_NAME"]
+            self.dg["Country Region"] = (
+                self.dg["ADM0_NAME"] + " " + self.dg["ADM2_NAME"]
+            )
         self.dg["Country Region"] = self.dg["Country Region"].str.lower()
         self.dg_country = self.dg[
             self.dg["ADM0_NAME"].str.lower().str.replace(" ", "_") == self.country
         ]
 
     def read_data(self, country, crop, season):
         """
@@ -867,35 +938,47 @@
         self.crop = crop
 
         """Figure out path to file containing CEI data"""
         admin_zone = self.parser.get(country, "admin_zone")
         country_str = country.title().replace("_", " ")
         crop_str = crop.title().replace("_", " ")
 
-        statistics_dir = self.out_dir / "cei" / "indices" / self.method / "global"
-        os.makedirs(statistics_dir, exist_ok=True)
-        file = statistics_dir / f"{country_str}_{crop_str}_statistics_s1_{self.method}.csv"
+        dir_statistics = self.dir_output / "cei" / "indices" / self.method / "global"
+        os.makedirs(dir_statistics, exist_ok=True)
+        file = (
+            dir_statistics / f"{country_str}_{crop_str}_statistics_s1_{self.method}.csv"
+        )
 
         """ Add area, yield and prod stats from either GEOGLAM or FEWSNET warehouse database"""
         if not os.path.exists(file) or self.update_input_file:
-            _country_dir = self.out_dir / "cei" / "indices" / self.method / admin_zone / country / crop
+            _dir_country = (
+                self.dir_output
+                / "cei"
+                / "indices"
+                / self.method
+                / admin_zone
+                / country
+                / crop
+            )
             file_name = f"{country}_{crop}_s1*.csv"
-            all_files = _country_dir.glob(file_name)
+            all_files = _dir_country.glob(file_name)
             # TODO ignore file with _2000 in its name
             all_files = [f for f in all_files if "_2000" not in f.name]
 
-            self.df_results = pd.concat((pd.read_csv(f) for f in all_files), ignore_index=True)
+            self.df_results = pd.concat(
+                (pd.read_csv(f) for f in all_files), ignore_index=True
+            )
 
             self.df_results = stats.add_statistics(
                 self.dir_condition / "yield",
                 self.df_results,
                 country_str,
                 crop_str,
                 admin_zone,
-                self.statistics_columns + [self.target_column],
+                self.statistics_columns + [self.target],
                 self.method,
             )
             """ Add information on starting and ending time period for each stage"""
             self.df_results = stages.add_stage_information(self.df_results, self.method)
 
             self.df_results.to_csv(file, index=False)
         else:
```

### Comparing `geocif-0.1.24/geocif/indices_runner.py` & `geocif-0.1.25/geocif/indices_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from tqdm import tqdm
 
 warnings.filterwarnings("ignore")
 
 from .cei import indices
 from geoprepare import base
 
+
 def remove_duplicates(lst):
     """
 
     :param lst:
     :return:
     """
     return list(set([i for i in lst]))
@@ -58,15 +59,19 @@
             - path: full path to file
             - filename: name of file
         :return: Return the dataframe created above
         """
         import geopandas as gp
 
         dg_shp = gp.read_file(
-            self.dir_input / "Global_Datasets" / "Regions" / "Shps" / "adm_shapefile.shp",
+            self.dir_input
+            / "Global_Datasets"
+            / "Regions"
+            / "Shps"
+            / "adm_shapefile.shp",
             engine="pyogrio",
         )
 
         # Collect all the files which contain EO information
         df_files = pd.DataFrame(columns=["directory", "path", "filename", "admin_zone"])
         for filepath in self.base_dir.rglob("*.csv"):
             country = filepath.parents[0].name
@@ -110,15 +115,17 @@
         :param method:
         :return:
         """
         combinations = []
 
         for index, row in tqdm(df.iterrows()):
             combinations.extend(
-                list(itertools.product([row[0]], [row[1]], [row[2]], [row[3]], [method]))
+                list(
+                    itertools.product([row[0]], [row[1]], [row[2]], [row[3]], [method])
+                )
             )
 
         combinations = remove_duplicates(combinations)
 
         return combinations
 
     def main(self, method):
@@ -133,15 +140,25 @@
         combinations = self.process_combinations(df_files, method)
 
         # Add an element to the tuple to indicate the season
         # Last element is redo flag which is True if the analysis is to be redone
         # and False otherwise. Analysis is always redone for the current year
         # and last year whether file exists or not
         combinations = [
-            (self.parser, status, path, filename, admin_zone, category, year, "ndvi", True)
+            (
+                self.parser,
+                status,
+                path,
+                filename,
+                admin_zone,
+                category,
+                year,
+                "ndvi",
+                True,
+            )
             for year in range(2001, ar.utcnow().year + 1)
             for status, path, filename, admin_zone, category in combinations
         ]
 
         # Only keep those entries in combinations where the third elemt is
         # mozambique, south_africa, angola or dem_people's_rep_of_korea
         # This is done to test the code for these countries
@@ -162,15 +179,17 @@
                 for i, _ in enumerate(p.imap_unordered(indices.process, combinations)):
                     pass
         else:
             # Use the code below if you want to test without parallelization or
             # if you want to debug by using pdb
             pbar = tqdm(combinations)
             for i, val in enumerate(pbar):
-                pbar.set_description(f"Main loop {combinations[i][2]} {combinations[i][5]}")
+                pbar.set_description(
+                    f"Main loop {combinations[i][2]} {combinations[i][5]}"
+                )
                 indices.process(val)
 
 
 def run(path_config_files=[]):
     """
 
     Args:
@@ -179,15 +198,15 @@
     Returns:
 
     """
     """ Check dictionary keys to have no spaces"""
     indices.validate_index_definitions()
 
     for method in [
-        "biweekly_r",  # "dekad_r"  # "dekad_r"
+        "monthly_r",  # "dekad_r"  # "dekad_r"
     ]:  # , "full_season", "phenological_stages", "fraction_season"]:
         obj = cei_runner(path_config_files)
         obj.main(method)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `geocif-0.1.24/geocif/logger.py` & `geocif-0.1.25/geocif/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # DEBUG	          10
     # NOTSET	       0
     def __init__(
         self,
         dir_log,  # Path to the directory where the log file will be saved
         project="geoprepare",  # Name of the project, this will be created as a subdirectory in dir_log
         file="logger.txt",  # Name of the log file
-        level=logging.INFO  # Logging level (see above)
+        level=logging.INFO,  # Logging level (see above)
     ):
         log_format = "[%(asctime)s] %(message)s"
         dir_log = Path(dir_log) / project / ar.now().format("MMMM_DD_YYYY")
         os.makedirs(dir_log, exist_ok=True)
 
         self.logger = logzero.setup_logger(
             name=file,
@@ -67,15 +67,17 @@
     def warning(self, msg):
         self.logger.warning(msg)
 
     def error(self, msg):
         self.logger.error(msg)
 
 
-def setup_logger_parser(path_config_file, name_project="geocif", name_file="ml", level=logging.DEBUG):
+def setup_logger_parser(
+    path_config_file, name_project="geocif", name_file="ml", level=logging.DEBUG
+):
     """
 
     Args:
         path_config_file:
         name_project:
         name_file:
         level:
```

### Comparing `geocif-0.1.24/geocif/ml/analysis.py` & `geocif-0.1.25/geocif/analysis.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,744 +1,828 @@
-import os
-import ast
-
-import sqlite3
-import arrow as ar
-import numpy as np
-import pandas as pd
-import seaborn as sns
-from tqdm import tqdm
-import palettable as pal
-import geopandas as gpd
-from pathlib import Path
-import matplotlib.pyplot as plt
-from dataclasses import dataclass
-
-import always
-import Code.base.plot as plot
-import Code.fao.utils as utils
-import Code.base.constants as cc
-import Code.preprocess.constants_preprocess as constants
-
-
-@dataclass
-class Geoanalysis:
-    path_config_file: Path
-
-    def __post_init__(self):
-        self.country: str = None
-        self.countries: list = None
-        self.crop: str = None
-        self.table: str = None
-        self.forecast_season: int = None
-        self.model_names: list = []
-        self.df_analysis: pd.DataFrame = None
-        self.lag_yield_as_feature: bool = None
-        self.number_lag_years: int = None
-        self.all_seasons_with_yield: list = None
-
-        self.fao_dir = constants.dir_output / "fao" / "output"
-        self.parser = utils.read_config(self.path_config_file)
-        self.today = ar.utcnow().format("MMMM-DD-YYYY")
-
-        self.ml_dir = self.fao_dir / "ml"
-        self.db_dir = self.ml_dir / "db"
-        self.analysis_dir = self.ml_dir / "analysis" / self.today
-        os.makedirs(self.db_dir, exist_ok=True)
-        os.makedirs(self.analysis_dir, exist_ok=True)
-
-        self.db_forecasts = self.parser.get("DEFAULT", "db")
-        self.db_path = self.db_dir / self.db_forecasts
-
-        self.dir_shapefiles = cc.dir_inp / "Global_Datasets" / "Regions" / "Shps"
-
-    def parse_config(self, section="DEFAULT"):
-        """
-
-        Args:
-            section ():
-
-        Returns:
-
-        """
-        self.countries = ast.literal_eval(self.parser.get("DEFAULT", "countries"))
-        self.lag_yield_as_feature = self.parser.getboolean("ML", "lag_yield_as_feature")
-        self.number_lag_years = self.parser.getint("ML", "lag_years")
-
-    def query(self):
-        print("Query")
-        con = sqlite3.connect(self.db_path)
-
-        # Read from database, where country and crop match
-        query = "SELECT * FROM " + self.table
-        try:
-            self.df_analysis = pd.read_sql_query(query, con)
-
-            # Select just Country and Crop
-            self.df_analysis = self.df_analysis[
-                (self.df_analysis["Country"] == self.country)
-                & (self.df_analysis["Crop"] == self.crop)
-                & (self.df_analysis["Model"] == self.model)
-            ]
-        except Exception as e:
-            pass
-
-        con.commit()
-        con.close()
-
-    def annual_metrics(self, df):
-        """
-        Compute metrics for a given dataframe
-        :param df: dataframe containing Observed and Forecast data
-        """
-        import scipy.stats
-        from sklearn.metrics import mean_squared_error, mean_absolute_error
-
-        if len(df) < 3:
-            return pd.Series()
-
-        # Compute metrics
-        rmse = np.sqrt(mean_squared_error(df[self.observed], df[self.predicted]))
-        nse = utils.nse(df[self.observed], df[self.predicted])
-        r2 = scipy.stats.pearsonr(df[self.observed], df[self.predicted])[0] ** 2
-        mae = mean_absolute_error(df[self.observed], df[self.predicted])
-        mape = utils.mape(df[self.observed], df[self.predicted])
-        pbias = utils.pbias(df[self.observed], df[self.predicted])
-
-        # Return as a dictionary
-        dict_results = {
-            "Root Mean Square Error": rmse,
-            "Nash-Sutcliff Efficiency": nse,
-            "$r^2$": r2,
-            "Mean Absolute Error": mae,
-            "Mean Absolute\nPercentage Error": mape,
-            "Percentage Bias": pbias,
-        }
-
-        return pd.Series(dict_results)
-
-    def regional_metrics(self, df):
-        # Compute MAPE for each region, compute within this function
-        # Compute metrics
-
-        actual, predicted = df[self.observed], df[self.predicted]
-        mape = np.mean(np.abs((actual - predicted) / actual)) * 100
-
-        return pd.Series({"Mean Absolute Percentage Error": mape})
-
-    def add_stage_information(self, df):
-        """
-        Create a new column called Dekad which contains the last dekad
-        :param df: dataframe containing the column Stages for which we will compute Dekad information
-        """
-        for i, row in df.iterrows():
-            # Get the latest stage
-            stage = row["Stage Name"].split("-")[0]
-            df.loc[i, "Date"] = stage
-
-        return df
-
-    def select_top_N_years(self, group, N=5):
-        return group.nsmallest(N, "Mean Absolute Percentage Error")
-
-    def analyze(self):
-        print("Analyze")
-        # Remove rows with missing values in Observed Yield (tn per ha)
-        df = self.df_analysis.dropna(subset=["Observed Yield (tn per ha)"])
-
-        if df.empty:
-            return pd.DataFrame(), pd.DataFrame()
-
-        # For each Harvest Year, Stages combination, compute
-        # RMSE, NSE, R2, MAE, MAPE, PBIAS
-        df_metrics = df.groupby(
-            ["Country", "Model", "Harvest Year", "Stage Name", "Stage Range"]
-        ).apply(self.annual_metrics)
-
-        df_metrics = df_metrics.reset_index()
-        # Assign each unique Stage Name a unique integer identifier
-        df_metrics["Stage_ID"] = pd.Categorical(df_metrics["Stage Name"]).codes
-
-        # Order by Harvest Year and Number Stages (ascending)
-        df_metrics = df_metrics.sort_values(by=["Harvest Year", "Stage_ID"], ascending=[True, True])
-
-        # Add columns with the name of the country and crop
-        df_metrics["Country"] = self.country
-        df_metrics["Crop"] = self.crop
-
-        # Add stage information for plotting
-        df_metrics = self.add_stage_information(df_metrics)
-
-        # Rename level_2 to Metric and 0 to Value
-        # df_metrics = df_metrics.rename(columns={"level_2": "Metric", 0: "Value"})
-        # breakpoint()
-        # df_metrics.to_csv(r'D:\Users\ritvik\projects\GEOGLAM\Output\fao\dekad\ml\analysis\February-28-2024\ethiopia_maize\ab1.csv')
-        for metric in [
-            "Root Mean Square Error",
-            # "Nash-Sutcliff Efficiency",
-            "$r^2$",
-            "Mean Absolute Error",
-            "Mean Absolute\nPercentage Error",
-            "Percentage Bias",
-        ]:
-            self.plot_metric(df_metrics, metric)
-
-        # Only select years after 2010
-        # breakpoint()
-        # df = df[df["Harvest Year"].astype(int) >= 2010]
-        # For each Stages combination, compute MAPE
-        df_regional_metrics = (
-            df.groupby(
-                [
-                    "Country",
-                    "Region",
-                    "Harvest Year",
-                    "% of total Area (ha)",
-                    "Model",
-                    "Crop",
-                    "Stage Name",
-                    "Stage Range",
-                ]
-            )
-            .apply(self.regional_metrics)
-            .reset_index()
-        )
-
-        # HACK
-        # For each Country, Region, harvest Year combination, select the 5 years with least MAPE
-        df_regional_metrics = (
-            df_regional_metrics.groupby(["Country", "Region"])
-            .apply(lambda x: self.select_top_N_years(x, 10))
-            .reset_index(drop=True)
-        )
-
-        # Determine average MAPE for each Country, Region, Model, Crop, Stage Name, Stage Range
-        df_regional_metrics = (
-            df_regional_metrics.groupby(
-                [
-                    "Country",
-                    "Region",
-                    "% of total Area (ha)",
-                    "Model",
-                    "Crop",
-                    "Stage Name",
-                    "Stage Range",
-                ]
-            )["Mean Absolute Percentage Error"]
-            .mean()
-            .reset_index()
-        )
-
-        # Create an index based on following columns
-        index_columns = [
-            "Country",
-            "Crop",
-            "Model",
-            "Harvest Year",
-            "Stage Name",
-        ]
-        df_metrics.index = df_metrics.apply(
-            lambda row: "_".join([str(row[col]) for col in index_columns]), axis=1
-        )
-        df_metrics.index.set_names(["Index"], inplace=True)
-
-        index_columns = [
-            "Country",
-            "Region",
-            "Model",
-            "Crop",
-            "Stage Name",
-        ]
-        df_regional_metrics.index = df_regional_metrics.apply(
-            lambda row: "_".join([str(row[col]) for col in index_columns]), axis=1
-        )
-        df_regional_metrics.index.set_names(["Index"], inplace=True)
-
-        # Format with 3 places after the decimal point
-        df_metrics = df_metrics.round(3)
-        df_regional_metrics = df_regional_metrics.round(3)
-
-        # Store results in database
-        con = sqlite3.connect(self.db_path)
-        utils.to_db(self.db_path, f"country_metrics", df_metrics)
-        utils.to_db(self.db_path, f"regional_metrics", df_regional_metrics)
-
-        con.commit()
-        con.close()
-
-    def get_historic_production(self):
-        # Read in historic production data
-        statistics_dir = constants.dir_output / "fao" / "indices" / "biweekly_r" / "global"
-        country = self.country.title().replace("_", " ")
-        crop = self.crop.title().replace("_", " ")
-        file = statistics_dir / f"{country}_{crop}_statistics_s1_biweekly_r.csv"
-        df_historic = pd.read_csv(file)
-
-        df_historic = df_historic[["Region", "Harvest Year", "Yield (tn per ha)"]]
-
-        # Drop rows with NaN values
-        df_historic = df_historic.dropna()
-
-        # Determine unique years
-        years = df_historic["Harvest Year"].unique()
-
-        # Subset dataframe to only include the last years of the dataset
-        df_historic = df_historic[df_historic["Harvest Year"].isin(years[-5:])]
-
-        # For each region, compute the % of the total production
-        df_historic = (
-            df_historic.groupby("Region")["Yield (tn per ha)"]
-            .sum()
-            .pipe(lambda x: x / x.sum() * 100)
-            .to_frame(name="% of total Area (ha)")
-            .reset_index()
-        )
-        # Find median yield for each region
-        # df_historic = (
-        #     df_historic.groupby("Region")["Yield (tn per ha)"]
-        #     .median()
-        #     .to_frame(name="Median Yield (tn per ha)")
-        #     .reset_index()
-        # )
-
-        return df_historic
-
-    def preprocess(self):
-        if self.df_analysis.empty:
-            return
-
-        # Add a column called N year average that contains the average of the yield of the last 10 years
-        # this will be the same for each dekad in any year
-        df_lag_yield = self.df_analysis.copy()
-
-        df_lag_yield = (
-            df_lag_yield.groupby("Region")["Median Yield (tn per ha)"].median().reset_index()
-        )
-        df_lag_yield.columns = ["Region", f"{self.number_lag_years} year average"]
-
-        self.df_analysis = self.df_analysis.merge(df_lag_yield, on="Region", how="left")
-
-        df_historic = self.get_historic_production()
-        self.df_analysis = self.df_analysis.merge(df_historic, on="Region", how="left")
-
-        # Add a column called anomaly that is the ratio between the predicted yield and the N year average
-        self.df_analysis["Anomaly"] = (
-            self.df_analysis[self.predicted] * 100.0 / self.df_analysis["Median Yield (tn per ha)"]
-        )
-
-        # Compute the yield from the last year
-        # Add a column called Ratio Last Year that is the ratio between the predicted yield and the last year yield
-        # self.df_analysis["Ratio Last Year"] = (
-        #     self.df_analysis[self.predicted]
-        #     * 100.0
-        #     / self.df_analysis[f"Last Year Yield (tn per ha)"]
-        # )
-
-        return self.df_analysis
-
-    def map_regional(self):
-        con = sqlite3.connect(self.db_path)
-
-        # Read from database, where country and crop match
-        query = "SELECT * FROM country_metrics"
-        df_country = pd.read_sql_query(query, con)
-        query = "SELECT * FROM regional_metrics"
-        df_regional = pd.read_sql_query(query, con)
-
-        # Plot a histogram of the MAPE, different color for each country
-        # Plotting the histograms with KDE for each country
-        df_regional["Country"] = df_regional["Country"].str.replace("_", " ").str.title()
-        df_regional["Model"] = df_regional["Model"].str.title()
-
-        # Plotting the histogram with a smaller bin size for greater detail
-        # Plotting the KDE for each country, ensuring each step works
-        models = df_regional["Model"].unique()
-        for model in models:
-            df_model = df_regional[df_regional["Model"] == model]
-
-            # HACK: Drop rows where '% of total Area (ha)' is less than 1% and Mean Absolute Percentage Error is > 50%
-            # or where the Mean Absolute Percentage Error is greater than 50% if the '% of total Area (ha)' is greater than 1%
-            df_tmp = df_model[
-                (df_model["% of total Area (ha)"] < 1)
-                & (df_model["Mean Absolute Percentage Error"] > 50)
-                & (df_model["Country"].isin(["Angola", "United Republic Of Tanzania"]))
-            ]
-
-            # Remove df_tmp from df_model
-            df_model = df_model.drop(df_tmp.index)
-
-            # Plot the histogram of MAPE
-            # Create bins for '% of total Area (ha)' and 'MAPE'
-            df_model["Area Bins"] = pd.cut(
-                df_model["% of total Area (ha)"],
-                bins=[0, 2, 4, 6, 8, 10, 20, max(df_model["% of total Area (ha)"])],
-                precision=0,
-            )
-            df_model["MAPE Bins"] = pd.cut(
-                df_model["Mean Absolute Percentage Error"],
-                bins=6,  # [0, 5, 10, 15, 20, 25, 30, 50, max(df_model["Mean Absolute Percentage Error"])],
-                right=False,
-                precision=1,
-            )
-
-            # Count occurrences of MAPE values for each area bin
-            area_mape_counts = (
-                df_model.groupby(["Area Bins", "MAPE Bins"]).size().unstack(fill_value=0)
-            )
-
-            # Create the heatmap
-            plt.figure(figsize=(10, 8))
-            ax = sns.heatmap(
-                area_mape_counts,
-                annot=True,
-                square=True,
-                cmap=pal.scientific.sequential.Bamako_20_r.mpl_colormap,
-                fmt="d",
-            )
-            # Do not color or annotate cells with 0
-            for text in ax.texts:
-                if text.get_text() == "0":
-                    text.set_text("")
-                    text.set_color("white")
-
-            # plt.title("Heatmap of MAPE Bins vs % Total Area Bins")
-            plt.ylabel("% of Total Area (ha) Bins")
-            plt.xlabel("MAPE Bins")
-
-            # Adjust y-axis labels to horizontal
-            ax.set_yticklabels(ax.get_yticklabels(), rotation=0)
-
-            # Invert y-axis to have the highest bin at the top
-            ax.invert_yaxis()
-            plt.savefig(self.analysis_dir / f"heatmap_{model}.png", dpi=250)
-            plt.close()
-
-            # Plot the KDE of MAPE
-            plt.figure(figsize=(12, 8))
-            for label, group_data in df_model.groupby("Country"):
-                sns.kdeplot(
-                    group_data["Mean Absolute Percentage Error"],
-                    label=label,
-                    clip=(0, None),
-                    # bins=len(group_data),
-                    # kde=True,
-                )
-
-            # Add minor ticks on the x-axis
-            plt.minorticks_on()
-
-            # Setting the title and labels
-            plt.title(
-                f"Kernel Density Estimation of Mean Absolute Percentage Error by Country - {model}"
-            )
-            plt.xlabel("Mean Absolute Percentage Error (%)")
-            plt.ylabel("Density")
-            plt.legend(title="Country", title_fontsize="13")
-
-            plt.savefig(self.analysis_dir / f"mape_histogram_{model}.png", dpi=250)
-            plt.close()
-
-            # Map MAPE at regional level
-            df_model["Country Region"] = (
-                df_model["Country"].str.lower().str.replace("_", " ")
-                + " "
-                + df_model["Region"].str.lower()
-            )
-
-            fname = f"mape_{self.crop}_{model}.png"
-            col = "Mean Absolute Percentage Error"
-            countries = df_model["Country"].unique().tolist()
-            # make it title case and replace _ with space
-            countries = [country.title().replace("_", " ") for country in countries]
-            plot.plot_df_shpfile(
-                self.dg,  # dataframe containing adm1 name and polygon
-                df_model,  # dataframe containing information that will be mapped
-                merge_col="Country Region",  # Column on which to merge
-                name_country=countries,
-                name_col=col,  # Which column to plot
-                dir_out=self.analysis_dir,  # Output directory
-                fname=fname,  # Output file name
-                label=f"Mean Absolute Percentage Error",
-                vmin=df_model[col].min(),
-                vmax=50,  # df_model[col].max(),
-                cmap=pal.scientific.sequential.Bamako_20_r,
-                series="sequential",
-                show_bg=False,
-                annotate_regions=False,
-                loc_legend="lower left",
-            )
-
-        con.commit()
-        con.close()
-
-    def map(self, df_plot):
-        # df_plot = self.df_analysis.copy()
-        models = df_plot["Model"].unique()
-
-        for model in models:
-            df_model = df_plot[df_plot["Model"] == model]
-
-            countries = df_model["Country"].unique().tolist()
-            countries = [country.title().replace("_", " ") for country in countries]
-            df_model["Country Region"] = (
-                df_model["Country"].str.lower().str.replace("_", " ")
-                + " "
-                + df_model["Region"].str.lower()
-            )
-
-            # Change Harvest year to type int
-            df_model["Harvest Year"] = df_model["Harvest Year"].astype(int)
-            annotate_region_column = "ADM1_NAME" if self.admin_zone == "admin_1" else "ADM2_NAME"
-            analysis_years = df_model["Harvest Year"].unique()
-            for idx, year in enumerate(tqdm(analysis_years, desc="Map")):
-                df_harvest_year = df_model[df_model["Harvest Year"] == year]
-
-                for dekad in tqdm(df_harvest_year["Stage Name"].unique(), desc="Map"):
-                    df_dekad = df_harvest_year[df_harvest_year["Stage Name"] == dekad]
-
-                    """ % of total area """
-                    # if idx == 0:
-                    #     fname = f"{self.country}_{self.crop}_perc_area.png"
-                    #     col = "% of total Area (ha)"
-                    #     plot.plot_df_shpfile(
-                    #         self.dg,  # dataframe containing adm1 name and polygon
-                    #         df_model,  # dataframe containing information that will be mapped
-                    #         merge_col="Country Region",  # Column on which to merge
-                    #         name_country=countries,  # Plot global map
-                    #         name_col=col,  # Which column to plot
-                    #         dir_out=self.plot_dir / str(year),  # Output directory
-                    #         fname=fname,  # Output file name
-                    #         label=f"% of Total Area (ha)\n{self.crop.title()}",
-                    #         vmin=df_model[col].min(),
-                    #         vmax=df_model[col].max(),
-                    #         cmap=pal.scientific.sequential.Bamako_20_r,
-                    #         series="sequential",
-                    #         show_bg=False,
-                    #         annotate_regions=True,
-                    #         annotate_region_column=annotate_region_column,
-                    #         loc_legend="lower left",
-                    #     )
-                    #
-                    #     """ Unique regions """
-                    #     fname = f"{self.country}_{self.crop}_region_ID.png"
-                    #     col = "Region_ID"
-                    #     df_model[col] = df_model[col].astype(int) + 1
-                    #     if len(df_model["Region_ID"].unique() > 1):
-                    #         # Create a dictionary with each region assigned a unique integer identifier and name
-                    #         dict_region = {
-                    #             int(key): key for key in df_dekad["Region_ID"].unique()
-                    #         }
-                    #         plot.plot_df_shpfile(
-                    #             self.dg,  # dataframe containing adm1 name and polygon
-                    #             df_model,  # dataframe containing information that will be mapped
-                    #             dict_lup=dict_region,
-                    #             merge_col="Country Region",  # Column on which to merge
-                    #             name_country=countries,  # Plot global map
-                    #             name_col=col,  # Which column to plot
-                    #             dir_out=self.plot_dir / str(year),  # Output directory
-                    #             fname=fname,  # Output file name
-                    #             label=f"Region Cluster\n{self.crop.title()}",
-                    #             vmin=df_model[col].min(),
-                    #             vmax=df_model[col].max(),
-                    #             cmap=pal.tableau.Tableau_20.mpl_colors,
-                    #             series="qualitative",
-                    #             show_bg=False,
-                    #             alpha_feature=1,
-                    #             use_key=True,
-                    #             annotate_regions=True,
-                    #             annotate_region_column=annotate_region_column,
-                    #             loc_legend="lower left",
-                    #         )
-
-                    """ Anomaly """
-                    fname = f"{self.country}_{self.crop}_{dekad}_{year}_anomaly.png"
-                    # country = self.country.title().replace("_", " ")
-                    # print(df_dekad[["Region", "Anomaly"]])
-                    plot.plot_df_shpfile(
-                        self.dg,  # dataframe containing adm1 name and polygon
-                        df_harvest_year,  # dataframe containing information that will be mapped
-                        merge_col="Country Region",  # Column on which to merge
-                        name_country=countries,  # Plot global map
-                        name_col="Anomaly",  # Which column to plot
-                        dir_out=self.plot_dir / str(year),  # Output directory
-                        fname=fname,  # Output file name
-                        label=f"% of {self.number_lag_years}-year Median Yield\n{self.crop.title()}, {year}",
-                        vmin=df_harvest_year["Anomaly"].min(),
-                        vmax=110,  # df_harvest_year["Anomaly"].max(),
-                        cmap=pal.cartocolors.diverging.Geyser_5_r,
-                        series="sequential",
-                        show_bg=False,
-                        annotate_regions=False,
-                        annotate_region_column=annotate_region_column,
-                        loc_legend="lower left",
-                    )
-
-                    """ Predicted Yield """
-                    fname = f"{self.country}_{self.crop}_{dekad}_{year}_predicted_yield.png"
-                    plot.plot_df_shpfile(
-                        self.dg,  # dataframe containing adm1 name and polygon
-                        df_harvest_year,  # dataframe containing information that will be mapped
-                        merge_col="Country Region",  # Column on which to merge
-                        name_country=countries,  # Plot global map
-                        name_col="Predicted Yield (tn per ha)",  # Which column to plot
-                        dir_out=self.plot_dir / str(year),  # Output directory
-                        fname=fname,  # Output file name
-                        label=f"{self.predicted}\n{self.crop.title()}, {year}",
-                        vmin=df_harvest_year[self.predicted].min(),
-                        vmax=df_harvest_year[self.predicted].max(),
-                        cmap=pal.scientific.sequential.Bamako_20_r,
-                        series="sequential",
-                        show_bg=False,
-                        annotate_regions=False,
-                        annotate_region_column=annotate_region_column,
-                        loc_legend="lower left",
-                    )
-
-                    """ Ratio of Predicted to last Year Yield """
-                    fname = f"{self.country}_{self.crop}_{dekad}_{year}_ratio_last_year_yield.png"
-                    plot.plot_df_shpfile(
-                        self.dg,  # dataframe containing adm1 name and polygon
-                        df_dekad,  # dataframe containing information that will be mapped
-                        merge_col="Country Region",  # Column on which to merge
-                        name_country=countries,  # Plot global map
-                        name_col="Ratio Last Year",  # Which column to plot
-                        dir_out=self.plot_dir / str(year),  # Output directory
-                        fname=fname,  # Output file name
-                        label=f"Ratio Last Year to {self.predicted}\n{self.crop.title()}, {dekad} {year}",
-                        vmin=df_dekad["Ratio Last Year"].min(),
-                        vmax=df_dekad["Ratio Last Year"].max(),
-                        cmap=pal.scientific.sequential.Bamako_20_r,
-                        series="sequential",
-                        show_bg=False,
-                        annotate_regions=False,
-                        annotate_region_column=annotate_region_column,
-                        loc_legend="lower left",
-                    )
-                    break
-
-                    # Area
-                    # breakpoint()
-                    # if df_dekad["Area (ha)"].notna().all():
-                    #     fname = f"{self.country}_{self.crop}_{year}_area.png"
-                    #     plot.plot_df_shpfile(
-                    #         self.dg,  # dataframe containing adm1 name and polygon
-                    #         df_dekad,  # dataframe containing information that will be mapped
-                    #         merge_col="Country Region",  # Column on which to merge
-                    #         name_country=country,  # Plot global map
-                    #         name_col="Area (ha)",  # Which column to plot
-                    #         dir_out=self.plot_dir / str(year),  # Output directory
-                    #         fname=fname,  # Output file name
-                    #         label=f"{self.predicted}\n{self.crop.title()}, {dekad}",
-                    #         vmin=df_dekad[self.predicted].min(),
-                    #         vmax=df_dekad[self.predicted].max(),
-                    #         cmap=pal.scientific.sequential.Bamako_20_r,
-                    #         series="sequential",
-                    #         show_bg=False,
-                    #         annotate_regions=True,
-                    #         loc_legend="lower left",
-                    #     )
-
-    def plot_metric(self, df, metric="$r^2$"):
-        with plt.style.context("science"):
-            fig, ax = plt.subplots(figsize=(10, 5))
-            ax = sns.lineplot(data=df, x="Date", y=metric, ax=ax)  # "$r^2$"
-            ax.set_xlabel("")
-            ax.set_ylabel(metric)
-            plt.xticks(rotation=0)
-            plt.tight_layout()
-
-            # If metric is $r^2$ or NSE, do not plot values below 0
-            if metric in ["$r^2$", "Nash-Sutcliff Efficiency"]:
-                plt.ylim(0, 1)
-
-            # Replace \n in metric
-            metric = metric.replace("\n", " ")
-            fname = f"{self.country}_{self.crop}_{metric}.png"
-
-            plt.savefig(self.plot_dir / fname, dpi=250)
-            plt.close()
-
-    def run(self):
-        self.query()
-        aa = self.preprocess()
-        self.analyze()
-
-        return aa
-
-    def setup(self, country, crop, model):
-        """
-
-        Args:
-            country:
-            crop:
-            model:
-
-        Returns:
-
-        """
-        print(f"Setup {country}")
-        self.country = country
-        self.crop = crop
-        self.model = model
-        self.table = f"{self.country}_{self.crop}"
-        self.observed = "Observed Yield (tn per ha)"
-        self.predicted = "Predicted Yield (tn per ha)"
-
-        self.name_shapefile = self.parser.get(self.country, "boundary_file")
-        self.admin_zone = self.parser.get(self.country, "admin_zone")
-
-        # Plot directory
-        self.plot_dir = self.analysis_dir / self.country / self.crop
-        os.makedirs(self.plot_dir, exist_ok=True)
-
-
-def main():
-    obj = Geoanalysis(path_config_file=Path("../config/geocif.txt"))
-    obj.parse_config()
-
-    obj.dg = gpd.read_file(
-        obj.dir_shapefiles / "adm_shapefile.shp",
-        engine="pyogrio",
-    )
-
-    # Hack rename Tanzania to United Republic of Tanzania
-    obj.dg["ADMIN0"] = obj.dg["ADMIN0"].replace("Tanzania", "United Republic of Tanzania")
-
-    # Rename ADMIN0 to ADM0_NAME and ADMIN1 to ADM1_NAME and ADMIN2 to ADM2_NAME
-    obj.dg = obj.dg.rename(
-        columns={
-            "ADMIN0": "ADM0_NAME",
-            "ADMIN1": "ADM1_NAME",
-            "ADMIN2": "ADM2_NAME",
-        }
-    )
-
-    # Create a new column called Country Region that is the concatenation of ADM0_NAME and ADM1_NAME
-    # however if ADM2_NAME is not null, then it is the concatenation of ADM0_NAME and ADM2_NAME
-    obj.dg["Country Region"] = obj.dg["ADM0_NAME"]
-    obj.dg["Country Region"] = obj.dg["Country Region"].str.cat(obj.dg["ADM1_NAME"], sep=" ")
-    obj.dg.loc[obj.dg["ADM2_NAME"].notna(), "Country Region"] = (
-        obj.dg["ADM0_NAME"] + " " + obj.dg["ADM2_NAME"]
-    )
-    # Make it lower case
-    obj.dg["Country Region"] = obj.dg["Country Region"].str.lower()
-    frames = []
-    for country in obj.countries:
-        crops = ast.literal_eval(obj.parser.get(country, "crops"))
-
-        for crop in crops:
-            models = ast.literal_eval(obj.parser.get(country, "models"))
-
-            for model in models:
-                obj.setup(country, crop, model)
-                gg = obj.run()
-                frames.append(gg)
-
-    dk = pd.concat(frames)
-
-    # Map the metrics
-    # obj.map_regional()
-    obj.map(dk)
-
-
-if __name__ == "__main__":
-    main()
+import ast
+import os
+import sqlite3
+import warnings
+from configparser import ConfigParser
+from dataclasses import dataclass, field
+from pathlib import Path
+from typing import List
+
+import arrow as ar
+import geopandas as gpd
+import matplotlib.pyplot as plt
+import numpy as np
+import palettable as pal
+import pandas as pd
+import seaborn as sns
+from tqdm import tqdm
+
+from geocif import logger as log
+from geocif import utils
+from .viz import plot
+
+warnings.simplefilter(action="ignore", category=FutureWarning)
+
+
+@dataclass
+class Geoanalysis:
+    path_config_files: List[Path] = field(default_factory=list)
+    logger: log = None
+    parser: ConfigParser = field(default_factory=ConfigParser)
+
+    def __post_init__(self):
+        self.country: str = None
+        self.countries: list = None
+        self.crop: str = None
+        self.table: str = None
+        self.forecast_season: int = None
+        self.model_names: list = []
+        self.df_analysis: pd.DataFrame = None
+        self.lag_yield_as_feature: bool = None
+        self.number_lag_years: int = None
+        self.all_seasons_with_yield: list = None
+
+        self.dir_out = Path(self.parser.get("PATHS", "dir_output"))
+        self._date = ar.utcnow().to("America/New_York")
+        self.today = self._date.format("MMMM_DD_YYYY")
+
+        self.dir_ml = self.dir_out / "ml"
+        self.dir_db = self.dir_ml / "db"
+        self.dir_analysis = self.dir_ml / "analysis" / self.today
+        os.makedirs(self.dir_db, exist_ok=True)
+        os.makedirs(self.dir_analysis, exist_ok=True)
+
+        self.db_forecasts = self.parser.get("DEFAULT", "db")
+        self.db_path = self.dir_db / self.db_forecasts
+
+        dir_input = Path(self.parser.get("PATHS", "dir_input"))
+        self.dir_shapefiles = dir_input / "Global_Datasets" / "Regions" / "Shps"
+
+    def table_exists(self, db_path, table_name):
+        # Create a connection to the SQLite database
+        with sqlite3.connect(db_path) as con:
+            # Create a cursor object using the cursor() method
+            cursor = con.cursor()
+
+            # Define the query to find the table
+            query = f"SELECT name FROM sqlite_master WHERE type='table' AND name=?"
+
+            # Execute the prepared query passing the table_name as a parameter
+            cursor.execute(query, (table_name,))
+
+            # Fetch the result
+            result = cursor.fetchone()
+
+            # Close the cursor
+            cursor.close()
+
+        # Return True if a result is found, False otherwise
+        return result is not None
+
+    def query(self):
+        self.logger.info(f"Query {self.country} {self.crop}")
+        con = sqlite3.connect(self.db_path)
+
+        # Read from database, where country and crop match
+        query = "SELECT * FROM " + self.table
+        try:
+            self.df_analysis = pd.read_sql_query(query, con)
+
+            # Select just Country and Crop
+            self.df_analysis = self.df_analysis[
+                (self.df_analysis["Country"] == self.country)
+                & (self.df_analysis["Crop"] == self.crop)
+                & (self.df_analysis["Model"] == self.model)
+            ]
+        except Exception as e:
+            pass
+
+        con.commit()
+        con.close()
+
+    def annual_metrics(self, df):
+        """
+        Compute metrics for a given dataframe
+        :param df: dataframe containing Observed and Forecast data
+        """
+        import scipy.stats
+        from sklearn.metrics import mean_squared_error, mean_absolute_error
+
+        if len(df) < 3:
+            return pd.Series()
+
+        # Compute metrics
+        rmse = np.sqrt(mean_squared_error(df[self.observed], df[self.predicted]))
+        nse = utils.nse(df[self.observed], df[self.predicted])
+        r2 = scipy.stats.pearsonr(df[self.observed], df[self.predicted])[0] ** 2
+        mae = mean_absolute_error(df[self.observed], df[self.predicted])
+        mape = utils.mape(df[self.observed], df[self.predicted])
+        pbias = utils.pbias(df[self.observed], df[self.predicted])
+
+        # Return as a dictionary
+        dict_results = {
+            "Root Mean Square Error": rmse,
+            "Nash-Sutcliff Efficiency": nse,
+            "$r^2$": r2,
+            "Mean Absolute Error": mae,
+            "Mean Absolute\nPercentage Error": mape,
+            "Percentage Bias": pbias,
+        }
+
+        return pd.Series(dict_results)
+
+    def regional_metrics(self, df):
+        # Compute MAPE for each region, compute within this function
+        # Compute metrics
+
+        actual, predicted = df[self.observed], df[self.predicted]
+        mape = np.mean(np.abs((actual - predicted) / actual)) * 100
+
+        return pd.Series({"Mean Absolute Percentage Error": mape})
+
+    def add_stage_information(self, df):
+        """
+        Create a new column called Dekad which contains the last dekad
+        :param df: dataframe containing the column Stages for which we will compute Dekad information
+        """
+        for i, row in df.iterrows():
+            # Get the latest stage
+            stage = row["Stage Name"].split("-")[0]
+            df.loc[i, "Date"] = stage
+
+        return df
+
+    def select_top_N_years(self, group, N=5):
+        return group.nsmallest(N, "Mean Absolute Percentage Error")
+
+    def analyze(self):
+        self.logger.info(f"Analyze {self.country} {self.crop}")
+        # Remove rows with missing values in Observed Yield (tn per ha)
+        df = self.df_analysis.dropna(subset=["Observed Yield (tn per ha)"])
+
+        if df.empty:
+            return pd.DataFrame(), pd.DataFrame()
+
+        # For each Harvest Year, Stages combination, compute
+        # RMSE, NSE, R2, MAE, MAPE, PBIAS
+        df_metrics = df.groupby(
+            ["Country", "Model", "Harvest Year", "Stage Name", "Stage Range"]
+        ).apply(self.annual_metrics)
+
+        df_metrics = df_metrics.reset_index()
+        # Assign each unique Stage Name a unique integer identifier
+        df_metrics["Stage_ID"] = pd.Categorical(df_metrics["Stage Name"]).codes
+
+        # Order by Harvest Year and Number Stages (ascending)
+        df_metrics = df_metrics.sort_values(
+            by=["Harvest Year", "Stage_ID"], ascending=[True, True]
+        )
+
+        # Add columns with the name of the country and crop
+        df_metrics["Country"] = self.country
+        df_metrics["Crop"] = self.crop
+
+        # Add stage information for plotting
+        df_metrics = self.add_stage_information(df_metrics)
+
+        # Rename level_2 to Metric and 0 to Value
+        # df_metrics = df_metrics.rename(columns={"level_2": "Metric", 0: "Value"})
+        # breakpoint()
+        # df_metrics.to_csv(r'D:\Users\ritvik\projects\GEOGLAM\Output\fao\dekad\ml\analysis\February-28-2024\ethiopia_maize\ab1.csv')
+        for metric in [
+            "Root Mean Square Error",
+            # "Nash-Sutcliff Efficiency",
+            "$r^2$",
+            "Mean Absolute Error",
+            "Mean Absolute\nPercentage Error",
+            "Percentage Bias",
+        ]:
+            self.plot_metric(df_metrics, metric)
+
+        cols = [
+            "Country",
+            "Region",
+            "% of total Area (ha)",
+            "Model",
+            "Crop",
+            "Stage Name",
+            "Stage Range",
+        ]
+
+        # For each Stages combination, compute MAPE
+        df_regional_metrics = (
+            df.groupby(cols + ["Harvest Year"])
+            .apply(self.regional_metrics)
+            .reset_index()
+        )
+
+        # HACK
+        # For each Country, Region, harvest Year combination, select the 10 years with least MAPE
+        df_regional_metrics = (
+            df_regional_metrics.groupby(["Country", "Region"])
+            .apply(lambda x: self.select_top_N_years(x, 10))
+            .reset_index(drop=True)
+        )
+
+        # Determine average MAPE for each Country, Region, Model, Crop, Stage Name, Stage Range
+        df_regional_metrics = (
+            df_regional_metrics.groupby(cols)["Mean Absolute Percentage Error"]
+            .mean()
+            .reset_index()
+        )
+
+        # Create an index based on following columns
+        cols = [
+            "Country",
+            "Crop",
+            "Model",
+            "Harvest Year",
+            "Stage Name",
+        ]
+        df_metrics.index = df_metrics.apply(
+            lambda row: "_".join([str(row[col]) for col in cols]), axis=1
+        )
+        df_metrics.index.set_names(["Index"], inplace=True)
+
+        cols = [
+            "Country",
+            "Region",
+            "Model",
+            "Crop",
+            "Stage Name",
+        ]
+        df_regional_metrics.index = df_regional_metrics.apply(
+            lambda row: "_".join([str(row[col]) for col in cols]), axis=1
+        )
+        df_regional_metrics.index.set_names(["Index"], inplace=True)
+
+        # Format with 3 places after the decimal point
+        df_metrics = df_metrics.round(3)
+        df_regional_metrics = df_regional_metrics.round(3)
+
+        # Store results in database
+        con = sqlite3.connect(self.db_path)
+        utils.to_db(self.db_path, f"country_metrics", df_metrics)
+        utils.to_db(self.db_path, f"regional_metrics", df_regional_metrics)
+
+        con.commit()
+        con.close()
+
+    def get_historic_production(self):
+        # Read in historic production data
+        dir_output = Path(self.parser.get("PATHS", "dir_output"))
+        dir_statistics = dir_output / "cei" / "indices" / self.method / "global"
+        country = self.country.title().replace("_", " ")
+        crop = self.crop.title().replace("_", " ")
+        file = dir_statistics / f"{country}_{crop}_statistics_s1_{self.method}.csv"
+        df_historic = pd.read_csv(file)
+
+        df_historic = df_historic[["Region", "Harvest Year", "Yield (tn per ha)"]]
+
+        # Drop rows with NaN values
+        df_historic = df_historic.dropna()
+
+        # Determine unique years
+        years = df_historic["Harvest Year"].unique()
+
+        # Subset dataframe to only include the last years of the dataset
+        df_historic = df_historic[df_historic["Harvest Year"].isin(years[-5:])]
+
+        # For each region, compute the % of the total production
+        df_historic = (
+            df_historic.groupby("Region")["Yield (tn per ha)"]
+            .sum()
+            .pipe(lambda x: x / x.sum() * 100)
+            .to_frame(name="% of total Area (ha)")
+            .reset_index()
+        )
+        # Find median yield for each region
+        # df_historic = (
+        #     df_historic.groupby("Region")["Yield (tn per ha)"]
+        #     .median()
+        #     .to_frame(name="Median Yield (tn per ha)")
+        #     .reset_index()
+        # )
+
+        return df_historic
+
+    def preprocess(self):
+        if self.df_analysis.empty:
+            return
+
+        # Add a column called N year average that contains the average of the yield of the last 10 years
+        # this will be the same for each dekad in any year
+        df_lag_yield = self.df_analysis.copy()
+
+        df_lag_yield = (
+            df_lag_yield.groupby("Region")["Median Yield (tn per ha)"]
+            .median()
+            .reset_index()
+        )
+        df_lag_yield.columns = ["Region", f"{self.number_lag_years} year average"]
+
+        self.df_analysis = self.df_analysis.merge(df_lag_yield, on="Region", how="left")
+
+        df_historic = self.get_historic_production()
+        self.df_analysis = self.df_analysis.merge(df_historic, on="Region", how="left")
+
+        # Add a column called anomaly that is the ratio between the predicted yield and the N year average
+        self.df_analysis["Anomaly"] = (
+            self.df_analysis[self.predicted]
+            * 100.0
+            / self.df_analysis["Median Yield (tn per ha)"]
+        )
+
+        # Compute the yield from the last year
+        # Add a column called Ratio Last Year that is the ratio between the predicted yield and the last year yield
+        # self.df_analysis["Ratio Last Year"] = (
+        #     self.df_analysis[self.predicted]
+        #     * 100.0
+        #     / self.df_analysis[f"Last Year Yield (tn per ha)"]
+        # )
+
+        return self.df_analysis
+
+    def map_regional(self):
+        con = sqlite3.connect(self.db_path)
+
+        # Read from database, where country and crop match
+        query = "SELECT * FROM country_metrics"
+        df_country = pd.read_sql_query(query, con)
+        query = "SELECT * FROM regional_metrics"
+        df_regional = pd.read_sql_query(query, con)
+
+        # Plot a histogram of the MAPE, different color for each country
+        # Plotting the histograms with KDE for each country
+        df_regional["Country"] = (
+            df_regional["Country"].str.replace("_", " ").str.title()
+        )
+        df_regional["Model"] = df_regional["Model"].str.title()
+
+        # Plotting the histogram with a smaller bin size for greater detail
+        # Plotting the KDE for each country, ensuring each step works
+        models = df_regional["Model"].unique()
+        for model in models:
+            df_model = df_regional[df_regional["Model"] == model]
+
+            # HACK: Drop rows where '% of total Area (ha)' is less than 1% and Mean Absolute Percentage Error is > 50%
+            # or where the Mean Absolute Percentage Error is greater than 50% if the '% of total Area (ha)' is greater than 1%
+            df_tmp = df_model[
+                (df_model["% of total Area (ha)"] < 1)
+                & (df_model["Mean Absolute Percentage Error"] > 50)
+                & (df_model["Country"].isin(["Angola", "United Republic Of Tanzania"]))
+            ]
+
+            # Remove df_tmp from df_model
+            df_model = df_model.drop(df_tmp.index)
+
+            # Plot the histogram of MAPE
+            # Create bins for '% of total Area (ha)' and 'MAPE'
+            df_model["Area Bins"] = pd.cut(
+                df_model["% of total Area (ha)"],
+                bins=[0, 2, 4, 6, 8, 10, 20, max(df_model["% of total Area (ha)"])],
+                precision=0,
+            )
+            df_model["MAPE Bins"] = pd.cut(
+                df_model["Mean Absolute Percentage Error"],
+                bins=6,  # [0, 5, 10, 15, 20, 25, 30, 50, max(df_model["Mean Absolute Percentage Error"])],
+                right=False,
+                precision=1,
+            )
+
+            # Count occurrences of MAPE values for each area bin
+            area_mape_counts = (
+                df_model.groupby(["Area Bins", "MAPE Bins"])
+                .size()
+                .unstack(fill_value=0)
+            )
+
+            # Create the heatmap
+            plt.figure(figsize=(10, 8))
+            ax = sns.heatmap(
+                area_mape_counts,
+                annot=True,
+                square=True,
+                cmap=pal.scientific.sequential.Bamako_20_r.mpl_colormap,
+                fmt="d",
+            )
+            # Do not color or annotate cells with 0
+            for text in ax.texts:
+                if text.get_text() == "0":
+                    text.set_text("")
+                    text.set_color("white")
+
+            # plt.title("Heatmap of MAPE Bins vs % Total Area Bins")
+            plt.ylabel("% of Total Area (ha) Bins")
+            plt.xlabel("MAPE Bins")
+
+            # Adjust y-axis labels to horizontal
+            ax.set_yticklabels(ax.get_yticklabels(), rotation=0)
+
+            # Invert y-axis to have the highest bin at the top
+            ax.invert_yaxis()
+            plt.savefig(self.dir_analysis / f"heatmap_{model}.png", dpi=250)
+            plt.close()
+
+            # Plot the KDE of MAPE
+            plt.figure(figsize=(12, 8))
+            for label, group_data in df_model.groupby("Country"):
+                sns.kdeplot(
+                    group_data["Mean Absolute Percentage Error"],
+                    label=label,
+                    clip=(0, None),
+                    # bins=len(group_data),
+                    # kde=True,
+                )
+
+            # Add minor ticks on the x-axis
+            plt.minorticks_on()
+
+            # Setting the title and labels
+            plt.title(
+                f"Kernel Density Estimation of Mean Absolute Percentage Error by Country - {model}"
+            )
+            plt.xlabel("Mean Absolute Percentage Error (%)")
+            plt.ylabel("Density")
+            plt.legend(title="Country", title_fontsize="13")
+
+            plt.savefig(self.dir_analysis / f"mape_histogram_{model}.png", dpi=250)
+            plt.close()
+
+            # Map MAPE at regional level
+            df_model["Country Region"] = (
+                df_model["Country"].str.lower().str.replace("_", " ")
+                + " "
+                + df_model["Region"].str.lower()
+            )
+
+            fname = f"mape_{self.crop}_{model}.png"
+            col = "Mean Absolute Percentage Error"
+            countries = df_model["Country"].unique().tolist()
+            # make it title case and replace _ with space
+            countries = [country.title().replace("_", " ") for country in countries]
+            plot.plot_df_shpfile(
+                self.dg,  # dataframe containing adm1 name and polygon
+                df_model,  # dataframe containing information that will be mapped
+                merge_col="Country Region",  # Column on which to merge
+                name_country=countries,
+                name_col=col,  # Which column to plot
+                dir_out=self.dir_analysis,  # Output directory
+                fname=fname,  # Output file name
+                label=f"Mean Absolute Percentage Error",
+                vmin=df_model[col].min(),
+                vmax=50,  # df_model[col].max(),
+                cmap=pal.scientific.sequential.Bamako_20_r,
+                series="sequential",
+                show_bg=False,
+                annotate_regions=False,
+                loc_legend="lower left",
+            )
+
+        con.commit()
+        con.close()
+
+    def map(self, df_plot):
+        # df_plot = self.df_analysis.copy()
+        models = df_plot["Model"].unique()
+
+        for model in models:
+            df_model = df_plot[df_plot["Model"] == model]
+
+            countries = df_model["Country"].unique().tolist()
+            if len(countries) > 1:
+                self.dir_plot = self.dir_analysis
+                fname_prefix = f"{len(countries)}_countries"
+            else:
+                self.dir_plot = self.dir_analysis / self.country / self.crop
+                fname_prefix = f"{self.country}"
+            countries = [country.title().replace("_", " ") for country in countries]
+            df_model["Country Region"] = (
+                df_model["Country"].str.lower().str.replace("_", " ")
+                + " "
+                + df_model["Region"].str.lower().str.replace("_", " ")
+            )
+
+            # Change Harvest year to type int
+            df_model["Harvest Year"] = df_model["Harvest Year"].astype(int)
+            annotate_region_column = (
+                "ADM1_NAME" if self.admin_zone == "admin_1" else "ADM2_NAME"
+            )
+            analysis_years = df_model["Harvest Year"].unique()
+            for idx, year in enumerate(tqdm(analysis_years, desc="Map")):
+                df_harvest_year = df_model[df_model["Harvest Year"] == year]
+
+                for time_period in tqdm(
+                    df_harvest_year["Stage Name"].unique(), desc="Map"
+                ):
+                    df_time_period = df_harvest_year[
+                        df_harvest_year["Stage Name"] == time_period
+                    ]
+
+                    """ % of total area """
+                    # if idx == 0:
+                    #     fname = f"{self.country}_{self.crop}_perc_area.png"
+                    #     col = "% of total Area (ha)"
+                    #     plot.plot_df_shpfile(
+                    #         self.dg,  # dataframe containing adm1 name and polygon
+                    #         df_model,  # dataframe containing information that will be mapped
+                    #         merge_col="Country Region",  # Column on which to merge
+                    #         name_country=countries,  # Plot global map
+                    #         name_col=col,  # Which column to plot
+                    #         dir_out=self.plot_dir / str(year),  # Output directory
+                    #         fname=fname,  # Output file name
+                    #         label=f"% of Total Area (ha)\n{self.crop.title()}",
+                    #         vmin=df_model[col].min(),
+                    #         vmax=df_model[col].max(),
+                    #         cmap=pal.scientific.sequential.Bamako_20_r,
+                    #         series="sequential",
+                    #         show_bg=False,
+                    #         annotate_regions=True,
+                    #         annotate_region_column=annotate_region_column,
+                    #         loc_legend="lower left",
+                    #     )
+                    #
+                    #     """ Unique regions """
+                    #     fname = f"{self.country}_{self.crop}_region_ID.png"
+                    #     col = "Region_ID"
+                    #     df_model[col] = df_model[col].astype(int) + 1
+                    #     if len(df_model["Region_ID"].unique() > 1):
+                    #         # Create a dictionary with each region assigned a unique integer identifier and name
+                    #         dict_region = {
+                    #             int(key): key for key in df_time_period["Region_ID"].unique()
+                    #         }
+                    #         plot.plot_df_shpfile(
+                    #             self.dg,  # dataframe containing adm1 name and polygon
+                    #             df_model,  # dataframe containing information that will be mapped
+                    #             dict_lup=dict_region,
+                    #             merge_col="Country Region",  # Column on which to merge
+                    #             name_country=countries,  # Plot global map
+                    #             name_col=col,  # Which column to plot
+                    #             dir_out=self.plot_dir / str(year),  # Output directory
+                    #             fname=fname,  # Output file name
+                    #             label=f"Region Cluster\n{self.crop.title()}",
+                    #             vmin=df_model[col].min(),
+                    #             vmax=df_model[col].max(),
+                    #             cmap=pal.tableau.Tableau_20.mpl_colors,
+                    #             series="qualitative",
+                    #             show_bg=False,
+                    #             alpha_feature=1,
+                    #             use_key=True,
+                    #             annotate_regions=True,
+                    #             annotate_region_column=annotate_region_column,
+                    #             loc_legend="lower left",
+                    #         )
+
+                    """ Anomaly """
+                    fname = (
+                        f"{fname_prefix}_{self.crop}_{time_period}_{year}_anomaly.png"
+                    )
+                    plot.plot_df_shpfile(
+                        self.dg,  # dataframe containing adm1 name and polygon
+                        df_harvest_year,  # dataframe containing information that will be mapped
+                        merge_col="Country Region",  # Column on which to merge
+                        name_country=countries,  # Plot global map
+                        name_col="Anomaly",  # Which column to plot
+                        dir_out=self.dir_plot / str(year),  # Output directory
+                        fname=fname,  # Output file name
+                        label=f"% of {self.number_lag_years}-year Median Yield\n{self.crop.title()}, {year}",
+                        vmin=df_harvest_year["Anomaly"].min(),
+                        vmax=110,  # df_harvest_year["Anomaly"].max(),
+                        cmap=pal.cartocolors.diverging.Geyser_5_r,
+                        series="sequential",
+                        show_bg=False,
+                        annotate_regions=False,
+                        annotate_region_column=annotate_region_column,
+                        loc_legend="lower left",
+                    )
+
+                    """ Predicted Yield """
+                    fname = f"{fname_prefix}_{self.crop}_{time_period}_{year}_predicted_yield.png"
+                    plot.plot_df_shpfile(
+                        self.dg,  # dataframe containing adm1 name and polygon
+                        df_harvest_year,  # dataframe containing information that will be mapped
+                        merge_col="Country Region",  # Column on which to merge
+                        name_country=countries,  # Plot global map
+                        name_col="Predicted Yield (tn per ha)",  # Which column to plot
+                        dir_out=self.dir_plot / str(year),  # Output directory
+                        fname=fname,  # Output file name
+                        label=f"{self.predicted}\n{self.crop.title()}, {year}",
+                        vmin=df_harvest_year[self.predicted].min(),
+                        vmax=df_harvest_year[self.predicted].max(),
+                        cmap=pal.scientific.sequential.Bamako_20_r,
+                        series="sequential",
+                        show_bg=False,
+                        annotate_regions=False,
+                        annotate_region_column=annotate_region_column,
+                        loc_legend="lower left",
+                    )
+
+                    """ Ratio of Predicted to last Year Yield """
+                    # fname = f"{self.country}_{self.crop}_{time_period}_{year}_ratio_last_year_yield.png"
+                    # plot.plot_df_shpfile(
+                    #     self.dg,  # dataframe containing adm1 name and polygon
+                    #     df_time_period,  # dataframe containing information that will be mapped
+                    #     merge_col="Country Region",  # Column on which to merge
+                    #     name_country=countries,  # Plot global map
+                    #     name_col="Ratio Last Year",  # Which column to plot
+                    #     dir_out=self.plot_dir / str(year),  # Output directory
+                    #     fname=fname,  # Output file name
+                    #     label=f"Ratio Last Year to {self.predicted}\n{self.crop.title()}, {time_period} {year}",
+                    #     vmin=df_time_period["Ratio Last Year"].min(),
+                    #     vmax=df_time_period["Ratio Last Year"].max(),
+                    #     cmap=pal.scientific.sequential.Bamako_20_r,
+                    #     series="sequential",
+                    #     show_bg=False,
+                    #     annotate_regions=False,
+                    #     annotate_region_column=annotate_region_column,
+                    #     loc_legend="lower left",
+                    # )
+
+                    # Area
+                    # breakpoint()
+                    # if df_time_period["Area (ha)"].notna().all():
+                    #     fname = f"{self.country}_{self.crop}_{year}_area.png"
+                    #     plot.plot_df_shpfile(
+                    #         self.dg,  # dataframe containing adm1 name and polygon
+                    #         df_time_period,  # dataframe containing information that will be mapped
+                    #         merge_col="Country Region",  # Column on which to merge
+                    #         name_country=country,  # Plot global map
+                    #         name_col="Area (ha)",  # Which column to plot
+                    #         dir_out=self.plot_dir / str(year),  # Output directory
+                    #         fname=fname,  # Output file name
+                    #         label=f"{self.predicted}\n{self.crop.title()}, {time_period}",
+                    #         vmin=df_time_period[self.predicted].min(),
+                    #         vmax=df_time_period[self.predicted].max(),
+                    #         cmap=pal.scientific.sequential.Bamako_20_r,
+                    #         series="sequential",
+                    #         show_bg=False,
+                    #         annotate_regions=True,
+                    #         loc_legend="lower left",
+                    #     )
+
+    def plot_metric(self, df, metric="$r^2$"):
+        with plt.style.context("science"):
+            fig, ax = plt.subplots(figsize=(10, 5))
+            ax = sns.lineplot(data=df, x="Date", y=metric, ax=ax)  # "$r^2$"
+            ax.set_xlabel("")
+            ax.set_ylabel(metric)
+            plt.xticks(rotation=0)
+            plt.tight_layout()
+
+            # If metric is $r^2$ or NSE, do not plot values below 0
+            if metric in ["$r^2$", "Nash-Sutclwiiff Efficiency"]:
+                plt.ylim(0, 1)
+
+            # Replace \n in metric
+            metric = metric.replace("\n", " ")
+            fname = f"{self.country}_{self.crop}_{metric}.png"
+
+            plt.savefig(self.dir_analysis / fname, dpi=250)
+            plt.close()
+
+    def execute(self):
+        self.query()
+        aa = self.preprocess()
+        self.analyze()
+
+        return aa
+
+    def get_config_data(self):
+        try:
+            with sqlite3.connect(self.db_path) as con:
+                # Find names of all tables starting with 'config'
+                query = "SELECT name FROM sqlite_master WHERE type='table' AND name LIKE 'config%'"
+                df = pd.read_sql_query(query, con)
+
+                if df.empty:
+                    raise ValueError("No configuration tables found")
+
+                # Extract datetime from the table names
+                re = "(\d{4} \d{2}:\d{2})$"
+                df["datetime"] = pd.to_datetime(
+                    df["name"].str.extract(re)[0], format="%Y %H:%M"
+                )
+
+                # Sort the DataFrame by datetime in descending order and get the latest config file
+                latest_config = df.sort_values(by="datetime", ascending=False).iloc[0][
+                    "name"
+                ]
+
+                self.logger.info("=====================================")
+                self.logger.info(f"\t{latest_config}")
+                self.logger.info("=====================================")
+                # Read the latest config file
+                query = f"SELECT * FROM {latest_config}"
+                self.df_config = pd.read_sql_query(query, con)
+        except Exception as e:
+            self.logger.error(f"Failed to get configuration data: {e}")
+
+    def setup(self):
+        """
+
+        Args:
+            country:
+            crop:
+            model:
+
+        Returns:
+
+        """
+        self.dict_config = {}
+        self.get_config_data()
+
+        self.observed = "Observed Yield (tn per ha)"
+        self.predicted = "Predicted Yield (tn per ha)"
+
+        # Get the ML section
+        df_ml = self.df_config[self.df_config["Section"] == "ML"]
+
+        self.countries = ast.literal_eval(
+            df_ml[df_ml["Option"] == "countries"]["Value"].values[0]
+        )
+        for country in self.countries:
+            df = self.df_config[self.df_config["Section"] == country]
+
+            method = df[df["Option"] == "method"]["Value"].values[0]
+            crops = ast.literal_eval(df[df["Option"] == "crops"]["Value"].values[0])
+            models = ast.literal_eval(df[df["Option"] == "models"]["Value"].values[0])
+            admin_zone = df[df["Option"] == "admin_zone"]["Value"].values[0]
+            name_shapefile = df[df["Option"] == "boundary_file"]["Value"].values[0]
+
+            for crop in crops:
+                # Does a table with the name {country}-{crop} exist in the database?
+                table = f"{country}-{crop}"
+                if self.table_exists(self.db_path, table):
+                    self.dict_config[f"{country}-{crop}"] = {
+                        "method": method,
+                        "crops": crop,
+                        "models": models,
+                        "admin_zone": admin_zone,
+                        "name_shapefile": name_shapefile,
+                    }
+
+        self.dg = gpd.read_file(
+            self.dir_shapefiles / "adm_shapefile.shp",
+            engine="pyogrio",
+        )
+
+        # Hack rename Tanzania to United Republic of Tanzania
+        self.dg["ADMIN0"] = self.dg["ADMIN0"].replace(
+            "Tanzania", "United Republic of Tanzania"
+        )
+
+        # Rename ADMIN0 to ADM0_NAME and ADMIN1 to ADM1_NAME and ADMIN2 to ADM2_NAME
+        self.dg = self.dg.rename(
+            columns={
+                "ADMIN0": "ADM0_NAME",
+                "ADMIN1": "ADM1_NAME",
+                "ADMIN2": "ADM2_NAME",
+            }
+        )
+
+        # Create a new column called Country Region that is the concatenation of ADM0_NAME and ADM1_NAME
+        # however if ADM2_NAME is not null, then it is the concatenation of ADM0_NAME and ADM2_NAME
+        self.dg["Country Region"] = self.dg["ADM0_NAME"]
+        self.dg["Country Region"] = self.dg["Country Region"].str.cat(
+            self.dg["ADM1_NAME"], sep=" "
+        )
+        self.dg.loc[self.dg["ADM2_NAME"].notna(), "Country Region"] = (
+            self.dg["ADM0_NAME"] + " " + self.dg["ADM2_NAME"]
+        )
+        # Make it lower case
+        self.dg["Country Region"] = self.dg["Country Region"].str.lower()
+
+
+def run(path_config_files=[Path("../config/geocif.txt")]):
+    logger, parser = log.setup_logger_parser(path_config_files)
+    obj = Geoanalysis(path_config_files, logger, parser)
+    obj.setup()
+
+    """ Loop over each country, crop, model combination in dict_config """
+    frames = []
+    for country_crop, value in obj.dict_config.items():
+        obj.country = country_crop.split("-")[0]
+        obj.crop = country_crop.split("-")[1]
+
+        obj.admin_zone = value["admin_zone"]
+        obj.boundary_file = value["name_shapefile"]
+        obj.method = value["method"]
+        obj.number_lag_years = value["number_lag_years"]
+
+        obj.table = f"{obj.country}-{obj.crop}"
+        breakpoint()
+        models = value["models"]
+        for model in models:
+            obj.model = model
+
+            df_tmp = obj.execute()
+            frames.append(df_tmp)
+
+    dk = pd.concat(frames)
+
+    # Map the metrics
+    # obj.map_regional()
+    obj.map(dk)
+
+
+if __name__ == "__main__":
+    run()
```

### Comparing `geocif-0.1.24/geocif/ml/correlations.py` & `geocif-0.1.25/geocif/ml/correlations.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     df_most_corr_feature_by_time = pd.concat(frames)
 
 
 def plot_feature_corr_by_time(df, **kwargs):
     country = kwargs.get("country")
     crop = kwargs.get("crop")
-    analysis_dir = kwargs.get("analysis_dir")
+    dir_output = kwargs.get("dir_output")
     forecast_season = kwargs.get("forecast_season")
     national_correlation = kwargs.get("national_correlation")
     group_by = kwargs.get("groupby")
 
     # Setup the figure and gridspec
     fig = plt.figure(figsize=(10, 5))
     gs = fig.add_gridspec(
@@ -149,17 +149,16 @@
     if not national_correlation:
         fname = f"{country}_{crop}_{id}_corr_feature_by_time.png"
     else:
         fname = f"{country}_{crop}_corr_feature_by_time.png"
     ax_heatmap.set_title(f"{_country}\n{_crop}")
 
     # plt.tight_layout()
-    out_dir = analysis_dir / country / crop / str(forecast_season)
-    os.makedirs(out_dir, exist_ok=True)
-    plt.savefig(out_dir / fname, dpi=250)
+    os.makedirs(dir_output, exist_ok=True)
+    plt.savefig(dir_output / fname, dpi=250)
     plt.close()
 
 
 def _all_correlated_feature_by_time(df, **kwargs):
     """
 
     Args:
@@ -255,15 +254,15 @@
                 df_tmp = df_corr[df_corr.columns[(df_corr.mean() > 0.1)]]
                 dict_selected_features[region_id] = df_tmp.columns
 
                 df_tmp2 = df_tmp.median(axis=0).abs().sort_values(ascending=False).reset_index()
                 df_tmp2.columns = ["Metric", "Value"]
                 # Add another column based on Type of Metric
                 for idx, row in df_tmp2.iterrows():
-                    df_tmp2.loc[df_tmp2.index[idx], "Type"] = combined_dict[row[0]][0]
+                    df_tmp2.loc[idx, "Type"] = combined_dict[row[0]][0]
 
                 # Compute median of each CEI and sort the dataframe based on the absolute value of the median
                 dict_best_cei[region_id] = (
                     df_tmp2.groupby("Type")
                     .max()
                     .reset_index()
                     .sort_values("Value", ascending=False)["Metric"]
```

### Comparing `geocif-0.1.24/geocif/ml/embedding.py` & `geocif-0.1.25/geocif/ml/embedding.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/ml/feature_engineering.py` & `geocif-0.1.25/geocif/ml/feature_engineering.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,16 +103,14 @@
     # For the number of years specified in self.number_lag_years, add the yield of that number of years
     # ago to the dataframe
     # For example, if number_lag_years is 3, then the yield of each year upto 3 years ago will be added
     # to the dataframe
     # The yield of the previous year is already added to the dataframe
     # Ensure 'Harvest Year' is treated as integer for accurate comparisons
     df["Harvest Year"] = df["Harvest Year"].astype(int)
-    # Initialize the new column with NaNs
-    df[f"Median {target_col}"] = np.nan
 
     for region, group in tqdm(df.groupby("Region"), desc="Lag yields", leave=False):
         unique_years = group["Harvest Year"].unique()
 
         # Check if the target column is empty for the current group
         if group[target_col].isnull().all():
             continue
@@ -277,17 +275,23 @@
 
     # Determine an appropriate number of clusters using the Elbow Method
     inertia = []
     range_of_clusters = range(
         1, len(df_yield_pivot)
     )  # Assuming up to 15 clusters for demonstration
 
+    # Replace inf or NaN values with column median
+    df_yield_pivot = df_yield_pivot.replace([np.inf, -np.inf], np.nan)
+    df_yield_pivot = df_yield_pivot.fillna(df_yield_pivot.median())
     for n_clusters in range_of_clusters:
         kmeans = KMeans(n_clusters=n_clusters, random_state=42)
-        kmeans.fit(df_yield_pivot)
+        try:
+            kmeans.fit(df_yield_pivot)
+        except:
+            breakpoint()
         inertia.append(kmeans.inertia_)
 
     # Use KneeLocator to find the elbow point automatically
     knee_locator = KneeLocator(range_of_clusters, inertia, curve="convex", direction="decreasing")
 
     # # Plot the Elbow Method for visual confirmation
     # plt.figure(figsize=(10, 6))
```

### Comparing `geocif-0.1.24/geocif/ml/feature_selection.py` & `geocif-0.1.25/geocif/ml/feature_selection.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,27 @@
         X_new = selector.fit_transform(X, y)
 
         # Get the selected feature indices
         selected_features = selector.get_support(indices=True)
 
         # Get the selected feature names
         selected_features = X.columns[selected_features].tolist()
+    elif method == "feature_engine":
+        from feature_engine.selection import SmartCorrelatedSelection
+
+        selector = SmartCorrelatedSelection(
+            method="pearson",
+            threshold=0.7,
+            selection_method="model_performance",
+            estimator=forest,
+            scoring="neg_mean_squared_error",
+        )
+
+        X_filtered = selector.fit_transform(X, y)
+        selected_features = X_filtered.columns.tolist()
     elif method == "RFECV":
         from sklearn.feature_selection import RFECV
         from sklearn.model_selection import KFold
 
         # Initialize a k-fold cross-validation strategy
         cv = KFold(n_splits=5)
```

### Comparing `geocif-0.1.24/geocif/ml/misc.py` & `geocif-0.1.25/geocif/playground/misc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,365 +1,408 @@
-import pandas as pd
-import matplotlib.pyplot as plt
-import matplotlib.patches as patches
-
-
-from matplotlib.cm import ScalarMappable
-from matplotlib.colors import ListedColormap, Normalize
-import matplotlib.pyplot as plt
-import matplotlib as mpl
-
-import matplotlib.pyplot as plt
-from matplotlib.colors import ListedColormap, Normalize
-from matplotlib.cm import ScalarMappable
-
-fig, ax = plt.subplots(figsize=(3, 0.5))
-
-colors = ["red", "cyan", "darkgreen"]
-cmap = ListedColormap(colors)
-norm = Normalize(vmin=2.5, vmax=5.5)
-cb = fig.colorbar(
-    mappable=ScalarMappable(norm=norm, cmap=cmap),
-    cax=ax,
-    ticks=[3.5, 4.5],
-    ticklocation="top",
-    orientation="horizontal",
-    drawedges=True,
-)
-cb.solids.set(edgecolor="white", linewidth=5)
-cb.outline.set_visible(False)
-cb.dividers.set(linewidth=1, alpha=0.6)
-cb.ax.tick_params(width=1, length=10, color="k")
-plt.setp(cb.ax.xaxis.get_ticklines(), alpha=0.6)
-cb.set_ticklabels([3.5, 4.5], alpha=0.6, color="k", fontsize=15, fontfamily="Arial")
-plt.savefig(r"D:\Users\ritvik\projects\GEOGLAM\Output\fao\output\ml\db\aa.png")
-breakpoint()
-fig, ax = plt.subplots(figsize=(6, 1), layout="constrained")
-cmap = ListedColormap(["red", "cyan", "slategrey"])
-norm = mpl.colors.Normalize(vmin=5, vmax=10)
-sm = ScalarMappable(norm=Normalize(2.5, 5.5), cmap=cmap)
-fig.colorbar(sm, cmap=cmap, ticks=[3.5, 4.5], cax=ax, orientation="horizontal", label="Colorbar")
-plt.show()
-cb = plt.colorbar(
-    sm, cmap=cmap, ticks=[3.5, 4.5], cax=ax, orientation="horizontal", label="Colorbar"
-)
-
-# Add number on top of the colorbar
-
-breakpoint()
-df = pd.read_csv(
-    r"D:\Users\ritvik\projects\GEOGLAM\Output\fao\output\ml\analysis\April-16-2024\aa.csv"
-)
-# Initialize the Matplotlib figure and axis
-fig, ax = plt.subplots(figsize=(14, 10))
-
-# Plot the predicted yield as a dot and the CI as a vertical line for each region
-for i in range(len(df)):
-    ax.plot([i, i], [df["Lower CI"][i], df["Upper CI"][i]], color="gray")  # CI line
-    ax.plot(i, df["Predicted"][i], "ko")  # Predicted yield dot
-    ax.plot(i, df["Median"][i], "ro")  # Median yield differently colored dot
-
-# Add labels and title
-ax.set_xticks(range(len(df)))
-ax.set_xticklabels(df["Region"], rotation=90)
-ax.set_ylabel("Yield (tn per ha)")
-ax.set_title("Predicted and Median Yields with Confidence Intervals per Region")
-
-# Show the plot with a tight layout
-plt.tight_layout()
-plt.show()
-breakpoint()
-
-from osgeo import ogr
-
-driver = ogr.GetDriverByName("FileGDB")
-
-ds = driver.Open(r"C:\Users\ritvik\Downloads\Admin_1_Regions.gdb", 0)
-
-breakpoint()
-
-
-import numpy as np
-
-import geopandas as gpd
-
-dg_ewcm_geoglam = gpd.read_file(
-    r"D:\Users\ritvik\projects\GEOGLAM\Input\Global_Datasets\Regions\Shps\EWCM_Level_1.shp",
-    engine="pyogrio",
-)
-
-dg_ewcm_fewsnet = gpd.read_file(
-    r"D:\Users\ritvik\projects\GEOGLAM\Input\Global_Datasets\Regions\Shps\hvstat_shape (1).gpkg",
-    engine="pyogrio",
-)
-
-# Only select thiose rows in dg_ewcm_fewsnet where ADMIN2 is not None
-dg_ewcm_fewsnet = dg_ewcm_fewsnet[dg_ewcm_fewsnet["ADMIN2"].notnull()]
-
-# Find countries in dg_ewcm_fewsnet
-countries = dg_ewcm_fewsnet[dg_ewcm_fewsnet["ADMIN0"].notnull()]["ADMIN0"].unique()
-
-# Restrict dg_ewcm_geoglam to countries in dg_ewcm_fewsnet
-dg_ewcm_geoglam = dg_ewcm_geoglam[dg_ewcm_geoglam["ADM0_NAME"].isin(countries)]
-# Find polygons that exist in dg_ewcm_geoglam but not in dg_ewcm_fewsnet
-# print("GEOGLAM but not in FEWSNET", dg_ewcm_geoglam[~dg_ewcm_geoglam.geometry.isin(dg_ewcm_fewsnet.geometry)])
-a1 = dg_ewcm_geoglam[~dg_ewcm_geoglam.geometry.isin(dg_ewcm_fewsnet.geometry)]
-# Find polygons that exist in dg_ewcm_fewsnet but not in dg_ewcm_geoglam
-# print("FEWSNET but not in GEOGLAM", dg_ewcm_fewsnet[~dg_ewcm_fewsnet.geometry.isin(dg_ewcm_geoglam.geometry)])
-a2 = dg_ewcm_fewsnet[~dg_ewcm_fewsnet.geometry.isin(dg_ewcm_geoglam.geometry)]
-
-# Remove geometry from a1 and a2
-a1 = a1.drop(columns=["geometry"])
-a2 = a2.drop(columns=["geometry"])
-
-# Output to disk
-a1.to_csv(r"D:\Users\ritvik\projects\GEOGLAM\in_geoglam_but_not_in_fewsnet.csv", index=False)
-a2.to_csv(r"D:\Users\ritvik\projects\GEOGLAM\in_fewsnet_but_not_in_geoglam.csv", index=False)
-breakpoint()
-
-
-def compute_h_index(values):
-    # Sort the citations array in descending order
-    sorted_value = np.sort(values)[::-1]
-    # Iterate through the sorted citations to find the h-index
-    h_index = 0
-    for i, value in enumerate(sorted_value, start=1):
-        if value >= i:
-            h_index = value
-        else:
-            break
-
-    return h_index
-
-
-# Example usage
-citations = np.array([3.1, 0.56, 10.02, 2.35, 5.60])
-h_index = compute_h_index(citations)
-print(f"The h-index is: {h_index}")
-
-breakpoint()
-import numpy as np
-import pandas as pd
-from sklearn.ensemble import RandomForestClassifier
-from sklearn.model_selection import train_test_split
-import shap
-import matplotlib.pyplot as plt
-
-# Generate synthetic data
-np.random.seed(0)
-X = np.random.normal(size=(100, 4))
-y = np.random.binomial(1, 0.5, size=100)
-
-# Split the data
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
-
-# Train a simple RandomForest model
-model = RandomForestClassifier(n_estimators=10, max_depth=3, random_state=42)
-model.fit(X_train, y_train)
-
-# Compute SHAP values
-explainer = shap.TreeExplainer(model)
-shap_values = explainer.shap_values(X_test)
-
-# Plot with default font sizes
-# Beeswarm plot
-shap.summary_plot(shap_values[1], X_test, plot_type="dot")
-
-# Waterfall plot for a single prediction
-sample_idx = 0  # Example index for demonstration
-shap.plots.waterfall(shap_values[1][sample_idx], max_display=10)
-
-# Adjust font sizes globally for subsequent plots
-plt.rcParams.update({"font.size": 8})  # Adjust the font size as needed
-
-# Beeswarm plot with adjusted font size
-shap.summary_plot(shap_values[1], X_test, plot_type="dot")
-
-# Waterfall plot with adjusted font size for a single prediction
-shap.plots.waterfall(shap_values[1][sample_idx], max_display=10)
-
-# Reset matplotlib font settings to default if needed
-plt.rcParams.update(plt.rcParamsDefault)
-
-breakpoint()
-
-
-def plot_dekads():
-    # Correcting the generation of dekad start dates
-    start_date = pd.Timestamp(year=2021, month=1, day=1)
-    dekad_starts = []
-
-    for month in range(1, 13):  # Loop through each month
-        for day in [1, 11, 21]:
-            dekad_date = pd.Timestamp(year=2021, month=month, day=day)
-            dekad_starts.append(dekad_date)
-
-    # Remove the extra dekad start if it goes beyond the year
-    if dekad_starts[-1] > pd.Timestamp(year=2021, month=12, day=31):
-        dekad_starts.pop()
-
-    fig, ax = plt.subplots(figsize=(20, 3))
-
-    color_nov_to_apr = "lightblue"  # Light blue for Nov 1 to Apr 30
-    color_default = "lightgray"  # Light gray for the rest of the year
-
-    for i, date in enumerate(dekad_starts):
-        if date.month >= 11 or date.month <= 4:
-            facecolor = color_nov_to_apr
-        else:
-            facecolor = color_default
-
-        # Adding squares with specified face color and white border
-        ax.add_patch(
-            patches.Rectangle((i, 0.5), 1, 1, edgecolor="white", facecolor=facecolor, linewidth=2)
-        )
-
-        # Non-rotated annotations, slightly increased size
-        annotation = f"D{i + 1}"
-        ax.text(
-            i + 0.5,
-            0.35,
-            annotation,
-            ha="center",
-            va="top",
-            fontsize=10,
-            fontweight="bold",
-        )
-
-    ax.set_xlim(0, len(dekad_starts))
-    ax.set_ylim(0, 1.75)
-    ax.set_aspect("equal")
-    ax.axis("off")
-    ax.set_facecolor("whitesmoke")
-    # plt.title('Dekad Start Dates with White Borders', fontsize=12, fontweight='bold')
-    plt.tight_layout()
-    plt.show()
-
-
-def plot_dekads_with_arrows():
-    # Correctly generating dekad start dates
-    start_date = pd.Timestamp(year=2021, month=1, day=1)
-    dekad_starts = []
-
-    for month in range(1, 13):  # Loop through each month
-        for day in [1, 11, 21]:
-            dekad_date = pd.Timestamp(year=2021, month=month, day=day)
-            dekad_starts.append(dekad_date)
-
-    # Adjust if the last date exceeds the year
-    if dekad_starts[-1] > pd.Timestamp(year=2021, month=12, day=31):
-        dekad_starts.pop()
-
-    # Plotting with annotations, colored squares, and arrows
-    fig, ax = plt.subplots(figsize=(20, 4))  # Increased figure height to accommodate arrows
-
-    color_nov_to_apr = "lightblue"  # Light blue for Nov 1 to Apr 30
-    color_default = "lightgray"  # Light gray for the rest of the year
-
-    for i, date in enumerate(dekad_starts):
-        facecolor = color_nov_to_apr if date.month >= 11 or date.month <= 4 else color_default
-        # Draw the rectangles with specified face color and white border
-        ax.add_patch(
-            patches.Rectangle((i, 0.5), 1, 1, edgecolor="white", facecolor=facecolor, linewidth=2)
-        )
-        # Add annotation
-        ax.text(
-            i + 0.5,
-            0.35,
-            f"D{i + 1}",
-            ha="center",
-            va="top",
-            fontsize=10,
-            fontweight="bold",
-        )
-
-    # Drawing arrows from center to center, maintaining vertical positions
-    # The vertical positions remain the same as before (-0.2, -0.6, -1.0) for visual consistency
-    arrow_starts_ends = [
-        (7.5, -0.2, 6.5, -0.2),
-        (7.5, -0.6, 5.5, -0.6),
-        (7.5, -1.0, 4.5, -1.0),
-    ]
-
-    for x_start, y_start, x_end, y_end in arrow_starts_ends:
-        ax.annotate(
-            "",
-            xy=(x_end, y_end),
-            xycoords="data",
-            xytext=(x_start, y_start),
-            textcoords="data",
-            arrowprops=dict(arrowstyle="->", color="black", lw=1.5),
-        )
-
-    ax.set_xlim(0, len(dekad_starts))
-    ax.set_ylim(-1.25, 1.75)  # Adjusted to accommodate arrows
-    ax.set_aspect("equal")
-    ax.axis("off")
-    ax.set_facecolor("whitesmoke")
-    # plt.title('Dekad Start Dates with Centered Arrows', fontsize=12, fontweight='bold')
-    plt.tight_layout()
-    plt.show()
-
-
-def plot_dekads_v2():
-    # Correctly generating dekad start dates
-    start_date = pd.Timestamp(year=2021, month=1, day=1)
-    dekad_starts = []
-
-    for month in range(1, 13):  # Loop through each month
-        for day in [1, 11, 21]:
-            dekad_date = pd.Timestamp(year=2021, month=month, day=day)
-            dekad_starts.append(dekad_date)
-
-    # Adjust if the last date exceeds the year
-    if dekad_starts[-1] > pd.Timestamp(year=2021, month=12, day=31):
-        dekad_starts.pop()
-
-    # Plotting with increased space for annotations
-    fig, ax = plt.subplots(
-        figsize=(20, 4)
-    )  # Adjusted figure size for clarity and additional spacing
-
-    color_nov_to_apr = "lightblue"  # Light blue for Nov 1 to Apr 30
-    color_default = "lightgray"  # Light gray for the rest of the year
-
-    for i, date in enumerate(dekad_starts):
-        facecolor = color_nov_to_apr if date.month >= 11 or date.month <= 4 else color_default
-        # Draw the rectangles with specified face color and white border
-        ax.add_patch(
-            patches.Rectangle((i, 0.5), 1, 1, edgecolor="white", facecolor=facecolor, linewidth=2)
-        )
-        # Add "D" annotation
-        ax.text(
-            i + 0.5,
-            0.35,
-            f"D{i + 1}",
-            ha="center",
-            va="top",
-            fontsize=10,
-            fontweight="bold",
-        )
-        # Further increase space and then add date annotation
-        ax.text(
-            i + 0.5,
-            0.1,
-            date.strftime("%b %d"),
-            ha="center",
-            va="top",
-            fontsize=8,
-            fontstyle="italic",
-        )
-
-    ax.set_xlim(0, len(dekad_starts))
-    ax.set_ylim(-0.5, 1.75)  # Adjusted to better accommodate the increased spacing
-    ax.set_aspect("equal")
-    ax.axis("off")
-    ax.set_facecolor("whitesmoke")
-    # plt.title('Dekad Start Dates with Increased Space for Annotations', fontsize=12, fontweight='bold')
-    plt.tight_layout()
-    plt.show()
-
-
-if __name__ == "__main__":
-    plot_dekads()
-    plot_dekads_v2()
-    plot_dekads_with_arrows()
+import pandas as pd
+import matplotlib.pyplot as plt
+import matplotlib.patches as patches
+
+import matplotlib.pyplot as plt
+import cartopy.crs as ccrs
+import cartopy.feature as cfeature
+
+from cartopy.mpl.gridliner import LONGITUDE_FORMATTER, LATITUDE_FORMATTER
+
+import matplotlib.pyplot as plt
+import cartopy.crs as ccrs
+import cartopy.feature as cfeature
+def create_map_with_ticks():
+    fig, ax = plt.subplots(figsize=(10, 5), subplot_kw={'projection': ccrs.PlateCarree()})
+
+    # Add features to the map
+    ax.add_feature(cfeature.LAND, edgecolor='black')
+    ax.add_feature(cfeature.COASTLINE)
+
+    # Set the extent (min_lon, max_lon, min_lat, max_lat)
+    ax.set_extent([-120, -70, 25, 50], crs=ccrs.PlateCarree())
+
+    # Customize ticks to mimic GMT style
+    from cartopy.mpl.ticker import LongitudeFormatter, LatitudeFormatter
+    import matplotlib.ticker as mticker
+
+    ax.set_xticks([-120, -110, -100, -90, -80, -70], crs=ccrs.PlateCarree())
+    ax.set_yticks([25, 30, 35, 40, 45, 50], crs=ccrs.PlateCarree())
+
+    lon_formatter = LongitudeFormatter(number_format='g', degree_symbol='', dateline_direction_label=True)
+    lat_formatter = LatitudeFormatter(number_format='g', degree_symbol='')
+
+    ax.xaxis.set_major_formatter(lon_formatter)
+    ax.yaxis.set_major_formatter(lat_formatter)
+
+    # Adding gridlines
+    gl = ax.gridlines(crs=ccrs.PlateCarree(), draw_labels=False, linewidth=1, color='gray', alpha=0.5, linestyle='--')
+    gl.xlocator = mticker.FixedLocator([-120, -110, -100, -90, -80, -70])
+    gl.ylocator = mticker.FixedLocator([25, 30, 35, 40, 45, 50])
+
+    # Display the map
+    plt.show()
+
+
+create_map_with_ticks()
+
+breakpoint()
+from matplotlib.cm import ScalarMappable
+from matplotlib.colors import ListedColormap, Normalize
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+
+import matplotlib.pyplot as plt
+from matplotlib.colors import ListedColormap, Normalize
+from matplotlib.cm import ScalarMappable
+
+fig, ax = plt.subplots(figsize=(3, 0.5))
+
+colors = ["red", "cyan", "darkgreen"]
+cmap = ListedColormap(colors)
+norm = Normalize(vmin=2.5, vmax=5.5)
+cb = fig.colorbar(
+    mappable=ScalarMappable(norm=norm, cmap=cmap),
+    cax=ax,
+    ticks=[3.5, 4.5],
+    ticklocation="top",
+    orientation="horizontal",
+    drawedges=True,
+)
+cb.solids.set(edgecolor="white", linewidth=5)
+cb.outline.set_visible(False)
+cb.dividers.set(linewidth=1, alpha=0.6)
+cb.ax.tick_params(width=1, length=10, color="k")
+plt.setp(cb.ax.xaxis.get_ticklines(), alpha=0.6)
+cb.set_ticklabels([3.5, 4.5], alpha=0.6, color="k", fontsize=15, fontfamily="Arial")
+plt.savefig(r"D:\Users\ritvik\projects\GEOGLAM\Output\fao\output\ml\db\aa.png")
+breakpoint()
+fig, ax = plt.subplots(figsize=(6, 1), layout="constrained")
+cmap = ListedColormap(["red", "cyan", "slategrey"])
+norm = mpl.colors.Normalize(vmin=5, vmax=10)
+sm = ScalarMappable(norm=Normalize(2.5, 5.5), cmap=cmap)
+fig.colorbar(sm, cmap=cmap, ticks=[3.5, 4.5], cax=ax, orientation="horizontal", label="Colorbar")
+plt.show()
+cb = plt.colorbar(
+    sm, cmap=cmap, ticks=[3.5, 4.5], cax=ax, orientation="horizontal", label="Colorbar"
+)
+
+# Add number on top of the colorbar
+
+breakpoint()
+df = pd.read_csv(
+    r"D:\Users\ritvik\projects\GEOGLAM\Output\fao\output\ml\analysis\April-16-2024\aa.csv"
+)
+# Initialize the Matplotlib figure and axis
+fig, ax = plt.subplots(figsize=(14, 10))
+
+# Plot the predicted yield as a dot and the CI as a vertical line for each region
+for i in range(len(df)):
+    ax.plot([i, i], [df["Lower CI"][i], df["Upper CI"][i]], color="gray")  # CI line
+    ax.plot(i, df["Predicted"][i], "ko")  # Predicted yield dot
+    ax.plot(i, df["Median"][i], "ro")  # Median yield differently colored dot
+
+# Add labels and title
+ax.set_xticks(range(len(df)))
+ax.set_xticklabels(df["Region"], rotation=90)
+ax.set_ylabel("Yield (tn per ha)")
+ax.set_title("Predicted and Median Yields with Confidence Intervals per Region")
+
+# Show the plot with a tight layout
+plt.tight_layout()
+plt.show()
+breakpoint()
+
+from osgeo import ogr
+
+driver = ogr.GetDriverByName("FileGDB")
+
+ds = driver.Open(r"C:\Users\ritvik\Downloads\Admin_1_Regions.gdb", 0)
+
+breakpoint()
+
+
+import numpy as np
+
+import geopandas as gpd
+
+dg_ewcm_geoglam = gpd.read_file(
+    r"D:\Users\ritvik\projects\GEOGLAM\Input\Global_Datasets\Regions\Shps\EWCM_Level_1.shp",
+    engine="pyogrio",
+)
+
+dg_ewcm_fewsnet = gpd.read_file(
+    r"D:\Users\ritvik\projects\GEOGLAM\Input\Global_Datasets\Regions\Shps\hvstat_shape (1).gpkg",
+    engine="pyogrio",
+)
+
+# Only select thiose rows in dg_ewcm_fewsnet where ADMIN2 is not None
+dg_ewcm_fewsnet = dg_ewcm_fewsnet[dg_ewcm_fewsnet["ADMIN2"].notnull()]
+
+# Find countries in dg_ewcm_fewsnet
+countries = dg_ewcm_fewsnet[dg_ewcm_fewsnet["ADMIN0"].notnull()]["ADMIN0"].unique()
+
+# Restrict dg_ewcm_geoglam to countries in dg_ewcm_fewsnet
+dg_ewcm_geoglam = dg_ewcm_geoglam[dg_ewcm_geoglam["ADM0_NAME"].isin(countries)]
+# Find polygons that exist in dg_ewcm_geoglam but not in dg_ewcm_fewsnet
+# print("GEOGLAM but not in FEWSNET", dg_ewcm_geoglam[~dg_ewcm_geoglam.geometry.isin(dg_ewcm_fewsnet.geometry)])
+a1 = dg_ewcm_geoglam[~dg_ewcm_geoglam.geometry.isin(dg_ewcm_fewsnet.geometry)]
+# Find polygons that exist in dg_ewcm_fewsnet but not in dg_ewcm_geoglam
+# print("FEWSNET but not in GEOGLAM", dg_ewcm_fewsnet[~dg_ewcm_fewsnet.geometry.isin(dg_ewcm_geoglam.geometry)])
+a2 = dg_ewcm_fewsnet[~dg_ewcm_fewsnet.geometry.isin(dg_ewcm_geoglam.geometry)]
+
+# Remove geometry from a1 and a2
+a1 = a1.drop(columns=["geometry"])
+a2 = a2.drop(columns=["geometry"])
+
+# Output to disk
+a1.to_csv(r"D:\Users\ritvik\projects\GEOGLAM\in_geoglam_but_not_in_fewsnet.csv", index=False)
+a2.to_csv(r"D:\Users\ritvik\projects\GEOGLAM\in_fewsnet_but_not_in_geoglam.csv", index=False)
+breakpoint()
+
+
+def compute_h_index(values):
+    # Sort the citations array in descending order
+    sorted_value = np.sort(values)[::-1]
+    # Iterate through the sorted citations to find the h-index
+    h_index = 0
+    for i, value in enumerate(sorted_value, start=1):
+        if value >= i:
+            h_index = value
+        else:
+            break
+
+    return h_index
+
+
+# Example usage
+citations = np.array([3.1, 0.56, 10.02, 2.35, 5.60])
+h_index = compute_h_index(citations)
+print(f"The h-index is: {h_index}")
+
+breakpoint()
+import numpy as np
+import pandas as pd
+from sklearn.ensemble import RandomForestClassifier
+from sklearn.model_selection import train_test_split
+import shap
+import matplotlib.pyplot as plt
+
+# Generate synthetic data
+np.random.seed(0)
+X = np.random.normal(size=(100, 4))
+y = np.random.binomial(1, 0.5, size=100)
+
+# Split the data
+X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
+
+# Train a simple RandomForest model
+model = RandomForestClassifier(n_estimators=10, max_depth=3, random_state=42)
+model.fit(X_train, y_train)
+
+# Compute SHAP values
+explainer = shap.TreeExplainer(model)
+shap_values = explainer.shap_values(X_test)
+
+# Plot with default font sizes
+# Beeswarm plot
+shap.summary_plot(shap_values[1], X_test, plot_type="dot")
+
+# Waterfall plot for a single prediction
+sample_idx = 0  # Example index for demonstration
+shap.plots.waterfall(shap_values[1][sample_idx], max_display=10)
+
+# Adjust font sizes globally for subsequent plots
+plt.rcParams.update({"font.size": 8})  # Adjust the font size as needed
+
+# Beeswarm plot with adjusted font size
+shap.summary_plot(shap_values[1], X_test, plot_type="dot")
+
+# Waterfall plot with adjusted font size for a single prediction
+shap.plots.waterfall(shap_values[1][sample_idx], max_display=10)
+
+# Reset matplotlib font settings to default if needed
+plt.rcParams.update(plt.rcParamsDefault)
+
+breakpoint()
+
+
+def plot_dekads():
+    # Correcting the generation of dekad start dates
+    start_date = pd.Timestamp(year=2021, month=1, day=1)
+    dekad_starts = []
+
+    for month in range(1, 13):  # Loop through each month
+        for day in [1, 11, 21]:
+            dekad_date = pd.Timestamp(year=2021, month=month, day=day)
+            dekad_starts.append(dekad_date)
+
+    # Remove the extra dekad start if it goes beyond the year
+    if dekad_starts[-1] > pd.Timestamp(year=2021, month=12, day=31):
+        dekad_starts.pop()
+
+    fig, ax = plt.subplots(figsize=(20, 3))
+
+    color_nov_to_apr = "lightblue"  # Light blue for Nov 1 to Apr 30
+    color_default = "lightgray"  # Light gray for the rest of the year
+
+    for i, date in enumerate(dekad_starts):
+        if date.month >= 11 or date.month <= 4:
+            facecolor = color_nov_to_apr
+        else:
+            facecolor = color_default
+
+        # Adding squares with specified face color and white border
+        ax.add_patch(
+            patches.Rectangle((i, 0.5), 1, 1, edgecolor="white", facecolor=facecolor, linewidth=2)
+        )
+
+        # Non-rotated annotations, slightly increased size
+        annotation = f"D{i + 1}"
+        ax.text(
+            i + 0.5,
+            0.35,
+            annotation,
+            ha="center",
+            va="top",
+            fontsize=10,
+            fontweight="bold",
+        )
+
+    ax.set_xlim(0, len(dekad_starts))
+    ax.set_ylim(0, 1.75)
+    ax.set_aspect("equal")
+    ax.axis("off")
+    ax.set_facecolor("whitesmoke")
+    # plt.title('Dekad Start Dates with White Borders', fontsize=12, fontweight='bold')
+    plt.tight_layout()
+    plt.show()
+
+
+def plot_dekads_with_arrows():
+    # Correctly generating dekad start dates
+    start_date = pd.Timestamp(year=2021, month=1, day=1)
+    dekad_starts = []
+
+    for month in range(1, 13):  # Loop through each month
+        for day in [1, 11, 21]:
+            dekad_date = pd.Timestamp(year=2021, month=month, day=day)
+            dekad_starts.append(dekad_date)
+
+    # Adjust if the last date exceeds the year
+    if dekad_starts[-1] > pd.Timestamp(year=2021, month=12, day=31):
+        dekad_starts.pop()
+
+    # Plotting with annotations, colored squares, and arrows
+    fig, ax = plt.subplots(figsize=(20, 4))  # Increased figure height to accommodate arrows
+
+    color_nov_to_apr = "lightblue"  # Light blue for Nov 1 to Apr 30
+    color_default = "lightgray"  # Light gray for the rest of the year
+
+    for i, date in enumerate(dekad_starts):
+        facecolor = color_nov_to_apr if date.month >= 11 or date.month <= 4 else color_default
+        # Draw the rectangles with specified face color and white border
+        ax.add_patch(
+            patches.Rectangle((i, 0.5), 1, 1, edgecolor="white", facecolor=facecolor, linewidth=2)
+        )
+        # Add annotation
+        ax.text(
+            i + 0.5,
+            0.35,
+            f"D{i + 1}",
+            ha="center",
+            va="top",
+            fontsize=10,
+            fontweight="bold",
+        )
+
+    # Drawing arrows from center to center, maintaining vertical positions
+    # The vertical positions remain the same as before (-0.2, -0.6, -1.0) for visual consistency
+    arrow_starts_ends = [
+        (7.5, -0.2, 6.5, -0.2),
+        (7.5, -0.6, 5.5, -0.6),
+        (7.5, -1.0, 4.5, -1.0),
+    ]
+
+    for x_start, y_start, x_end, y_end in arrow_starts_ends:
+        ax.annotate(
+            "",
+            xy=(x_end, y_end),
+            xycoords="data",
+            xytext=(x_start, y_start),
+            textcoords="data",
+            arrowprops=dict(arrowstyle="->", color="black", lw=1.5),
+        )
+
+    ax.set_xlim(0, len(dekad_starts))
+    ax.set_ylim(-1.25, 1.75)  # Adjusted to accommodate arrows
+    ax.set_aspect("equal")
+    ax.axis("off")
+    ax.set_facecolor("whitesmoke")
+    # plt.title('Dekad Start Dates with Centered Arrows', fontsize=12, fontweight='bold')
+    plt.tight_layout()
+    plt.show()
+
+
+def plot_dekads_v2():
+    # Correctly generating dekad start dates
+    start_date = pd.Timestamp(year=2021, month=1, day=1)
+    dekad_starts = []
+
+    for month in range(1, 13):  # Loop through each month
+        for day in [1, 11, 21]:
+            dekad_date = pd.Timestamp(year=2021, month=month, day=day)
+            dekad_starts.append(dekad_date)
+
+    # Adjust if the last date exceeds the year
+    if dekad_starts[-1] > pd.Timestamp(year=2021, month=12, day=31):
+        dekad_starts.pop()
+
+    # Plotting with increased space for annotations
+    fig, ax = plt.subplots(
+        figsize=(20, 4)
+    )  # Adjusted figure size for clarity and additional spacing
+
+    color_nov_to_apr = "lightblue"  # Light blue for Nov 1 to Apr 30
+    color_default = "lightgray"  # Light gray for the rest of the year
+
+    for i, date in enumerate(dekad_starts):
+        facecolor = color_nov_to_apr if date.month >= 11 or date.month <= 4 else color_default
+        # Draw the rectangles with specified face color and white border
+        ax.add_patch(
+            patches.Rectangle((i, 0.5), 1, 1, edgecolor="white", facecolor=facecolor, linewidth=2)
+        )
+        # Add "D" annotation
+        ax.text(
+            i + 0.5,
+            0.35,
+            f"D{i + 1}",
+            ha="center",
+            va="top",
+            fontsize=10,
+            fontweight="bold",
+        )
+        # Further increase space and then add date annotation
+        ax.text(
+            i + 0.5,
+            0.1,
+            date.strftime("%b %d"),
+            ha="center",
+            va="top",
+            fontsize=8,
+            fontstyle="italic",
+        )
+
+    ax.set_xlim(0, len(dekad_starts))
+    ax.set_ylim(-0.5, 1.75)  # Adjusted to better accommodate the increased spacing
+    ax.set_aspect("equal")
+    ax.axis("off")
+    ax.set_facecolor("whitesmoke")
+    # plt.title('Dekad Start Dates with Increased Space for Annotations', fontsize=12, fontweight='bold')
+    plt.tight_layout()
+    plt.show()
+
+
+if __name__ == "__main__":
+    plot_dekads()
+    plot_dekads_v2()
+    plot_dekads_with_arrows()
```

### Comparing `geocif-0.1.24/geocif/ml/outliers.py` & `geocif-0.1.25/geocif/ml/outliers.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/ml/outlook.py` & `geocif-0.1.25/geocif/ml/outlook.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/ml/output.py` & `geocif-0.1.25/geocif/ml/output.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,26 @@
     utils.to_db(db_path, f"config_{today}", df_parser)
 
     con.commit()
     con.close()
 
 
 def store(db_path, experiment_id, df, model, model_name):
+    """
+
+    Args:
+        db_path:
+        experiment_id:
+        df:
+        model:
+        model_name:
+
+    Returns:
+
+    """
     con = sqlite3.connect(db_path)
 
     # Convert any categorical columns to the values else we get the error
     # Exception: 'Categorical' with dtype category does not support reduction 'all'
     for col in df.columns:
         if isinstance(df[col], pd.CategoricalDtype):
             df[col] = df[col].astype(str)
```

### Comparing `geocif-0.1.24/geocif/ml/stages.py` & `geocif-0.1.25/geocif/ml/stages.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
     # Create a column called Stage Names that applies utils.dict_growth_stages
     # to the Starting Stage and Ending Stage
     if "dekad" in method:
         dict = utils.dict_growth_stages
     elif "biweekly" in method:
         dict = utils.dict_growth_stages_biweekly
+    elif "monthly" in method:
+        dict = utils.dict_growth_stages_monthly
     df["Stage Names"] = df["Starting Stage"].map(dict) + " - " + df["Ending Stage"].map(dict)
 
     # Group by Region, Harvest Year
     # For each group, add a column called Percentage Season
     # that is the percentage of the season that has passed based on the number of rows
     # in the group
     grouped = df.groupby(["Region", "Harvest Year"])
@@ -192,14 +194,16 @@
     stage_info["Starting Stage"] = int(start_stage)
     stage_info["Ending Stage"] = int(end_stage)
 
     if "dekad" in method:
         dict = utils.dict_growth_stages
     elif "biweekly" in method:
         dict = utils.dict_growth_stages_biweekly
+    elif "monthly" in method:
+        dict = utils.dict_growth_stages_monthly
 
     stage_info["Stage Name"] = dict[int(start_stage)] + "-" + dict[int(end_stage)]
 
     return stage_info
 
 
 def update_feature_names(df, method):
@@ -233,14 +237,16 @@
         end_stage = numeric_parts[-1]
 
         # Convert starting and ending stage using utils.dict_growth_stages
         if "dekad" in method:
             dict = utils.dict_growth_stages
         elif "biweekly" in method:
             dict = utils.dict_growth_stages_biweekly
+        elif "monthly" in method:
+            dict = utils.dict_growth_stages_monthly
         start_stage = dict[int(start_stage)]
         end_stage = dict[int(end_stage)]
 
         new_column_name = f"{cei} {start_stage}-{end_stage}"
 
         # Saving the result in the dictionary
         stages_info[element] = (cei, start_stage, end_stage, new_column_name)
```

### Comparing `geocif-0.1.24/geocif/ml/trainers.py` & `geocif-0.1.25/geocif/ml/trainers.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                 params = {
                     "depth": trial.suggest_int("depth", 1, 7),
                     "learning_rate": trial.suggest_float("learning_rate", 0.01, 0.1),
                     "iterations": trial.suggest_int("iterations", low=1000, high=5000, step=500),
                     "subsample": trial.suggest_float("subsample", 1.0, 1.0),
                     "random_strength": trial.suggest_float("random_strength", 0.3, 1.0),
                     "reg_lambda": trial.suggest_float("reg_lambda", 1e-8, 1.0),
-                    "loss_function": "RMSE",
+                    "loss_function": "MAPE",
                     "early_stopping_rounds": 50,
                     "random_seed": seed,
                     "verbose": False,
                 }
 
                 # Fit the optuna model
                 optuna_model = CatBoostRegressor(**params, cat_features=cat_features)
@@ -187,15 +187,15 @@
         hyperparams = {
             "depth": 6,
             "learning_rate": 0.01,
             "iterations": 10,
             "subsample": 1.0,
             "random_strength": 0.5,
             "reg_lambda": 0.001,
-            "loss_function": "RMSE",
+            "loss_function": "MAPE",
             "early_stopping_rounds": 50,
             "random_seed": seed,
             "verbose": False,
         }
 
     # Model Initialization & Training
     if model_name == "catboost":
```

### Comparing `geocif-0.1.24/geocif/ml/trend.py` & `geocif-0.1.25/geocif/ml/trend.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/ml/xai.py` & `geocif-0.1.25/geocif/ml/xai.py`

 * *Files identical despite different names*

### Comparing `geocif-0.1.24/geocif/utils.py` & `geocif-0.1.25/geocif/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import logging
 
 import sqlite3
 import numpy as np
 import pandas as pd
 import arrow as ar
 from tqdm.auto import tqdm
 import matplotlib.pyplot as plt
@@ -76,14 +75,30 @@
     24: "Nov 18",
     25: "Dec 2",
     26: "Dec 16",
     27: "Dec 31",
 }
 
 
+dict_growth_stages_monthly = {
+    1: "Jan 1",
+    2: "Feb 1",
+    3: "Mar 1",
+    4: "Apr 1",
+    5: "May 1",
+    6: "Jun 1",
+    7: "Jul 1",
+    8: "Aug 1",
+    9: "Sep 1",
+    10: "Oct 1",
+    11: "Nov 1",
+    12: "Dec 1",
+}
+
+
 def remove_last_part(s):
     # Function to remove the part after the last underscore, including the last underscore
     # e.g. 'MIN_ESI4WK_33' will return 'MIN_ESI4WK'
     # 'TNx_33' will return 'TNx'
     return "_".join(s.split("_")[:-1])
 
 
@@ -313,17 +328,15 @@
     :param method:
     :param admin_zone:
     :param country:
     :param crop:
 
     :return:
     """
-    dir_output = (
-        path_output / "fao" / "indices" / method / admin_zone / country / crop
-    )
+    dir_output = path_output / "fao" / "indices" / method / admin_zone / country / crop
     os.makedirs(dir_output, exist_ok=True)
 
     return dir_output
 
 
 def to_db(db_path, table_name, df):
     """
@@ -636,15 +649,15 @@
     Args:
     - row (pd.Series): A row from the DataFrame containing 'year' and 'doy' columns.
 
     Returns:
     - int: The biweekly period index (starting from 1).
     """
     # Calculate the day of the year, adjusting to start from 0
-    day_of_year_zero_indexed = int(row['Doy']) - 1
+    day_of_year_zero_indexed = int(row["Doy"]) - 1
     # Compute the biweekly index, adjusting so the first period is index 1
     biweekly_index = (day_of_year_zero_indexed // 14) + 1
 
     return biweekly_index
 
 
 def is_leap_year(year):
@@ -663,27 +676,29 @@
     - year: The year for the Doy values, used to handle leap years.
 
     Returns:
     - A tuple with starting and ending periods for the specified period type.
     """
     # Adjust the origin based on whether the year is a leap year
     df = df_inp.copy()
-    df['Date'] = pd.to_datetime(df['Doy'], unit='D', origin=pd.Timestamp(f'{year}-01-01'))
+    df["Date"] = pd.to_datetime(
+        df["Doy"], unit="D", origin=pd.Timestamp(f"{year}-01-01")
+    )
 
-    if period_type.startswith('dekad'):
-        df['Period'] = ((df['Date'].dt.dayofyear - 1) // 10) + 1
-    elif period_type.startswith('biweekly'):
-        df['Period'] = ((df['Date'].dt.dayofyear - 1) // 14) + 1
-    elif period_type.startswith('monthly'):
-        df['Period'] = df['Month']
+    if period_type.startswith("dekad"):
+        df["Period"] = ((df["Date"].dt.dayofyear - 1) // 10) + 1
+    elif period_type.startswith("biweekly"):
+        df["Period"] = ((df["Date"].dt.dayofyear - 1) // 14) + 1
+    elif period_type.startswith("monthly"):
+        df["Period"] = df["Month"]
     else:
         return "Invalid period type. Choose 'dekad', 'biweekly', or 'monthly'."
 
-    start_period = df.iloc[0]['Period']
-    end_period = df.iloc[-1]['Period']
+    start_period = df.iloc[0]["Period"]
+    end_period = df.iloc[-1]["Period"]
 
     return start_period, end_period
 
 
 def compute_h_index(values):
     # Sort the array in descending order
     sorted_value = np.sort(values)[::-1]
```

### Comparing `geocif-0.1.24/geocif.egg-info/PKG-INFO` & `geocif-0.1.25/geocif.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocif
-Version: 0.1.24
+Version: 0.1.25
 Summary: Models to visualize and forecast crop conditions and yields
 Home-page: https://ritviksahajpal.github.io/yield_forecasting/
 Author: Ritvik Sahajpal
 Author-email: ritvik@umd.edu
 License: MIT license
 Keywords: geocif
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -27,14 +27,22 @@
 **Models to visualize and forecast crop conditions and yields**
 
 
 -   Free software: MIT license
 -   Documentation: https://ritviksahajpal.github.io/yield_forecasting/
 
 
-## Features
+### Upload package to pypi
+1. Update requirements.txt
+2. Update version="A.B.C" in setup.py
+3. Navigate to the directory containing `setup.py` and run the following command:
+```python
+pipreqs . --force --savepath requirements.txt
+mamba env export > environment.yml
+python setup.py sdist
+twine upload dist/geocif-A.B.C.tar.gz
+```
 
--   TODO
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
```

### Comparing `geocif-0.1.24/geocif.egg-info/SOURCES.txt` & `geocif-0.1.25/geocif.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 geocif/__init__.py
+geocif/analysis.py
 geocif/geocif.py
 geocif/indices_runner.py
 geocif/logger.py
 geocif/utils.py
 geocif.egg-info/PKG-INFO
 geocif.egg-info/SOURCES.txt
 geocif.egg-info/dependency_links.txt
@@ -25,22 +26,25 @@
 geocif/backup/geocif.py
 geocif/backup/metadata.py
 geocif/backup/models.py
 geocif/cei/__init__.py
 geocif/cei/definitions.py
 geocif/cei/indices.py
 geocif/ml/__init__.py
-geocif/ml/analysis.py
 geocif/ml/correlations.py
 geocif/ml/embedding.py
 geocif/ml/feature_engineering.py
 geocif/ml/feature_selection.py
-geocif/ml/misc.py
 geocif/ml/outliers.py
 geocif/ml/outlook.py
 geocif/ml/output.py
 geocif/ml/stages.py
 geocif/ml/stats.py
 geocif/ml/trainers.py
 geocif/ml/trend.py
 geocif/ml/xai.py
+geocif/playground/__init__.py
+geocif/playground/automl.py
+geocif/playground/misc.py
+geocif/viz/__init__.py
+geocif/viz/plot.py
 tests/test_geocif.py
```

### Comparing `geocif-0.1.24/setup.py` & `geocif-0.1.25/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,54 +2,54 @@
 
 """The setup script."""
 
 import io
 from os import path as op
 from setuptools import setup, find_packages
 
-with open('README.md') as readme_file:
+with open("README.md") as readme_file:
     readme = readme_file.read()
 
 here = op.abspath(op.dirname(__file__))
 
 # get the dependencies and installs
 with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
     all_reqs = f.read().split("\n")
 
 install_requires = [x.strip() for x in all_reqs if "git+" not in x]
 dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
 
-requirements = [ ]
+requirements = []
 
-setup_requirements = [ ]
+setup_requirements = []
 
-test_requirements = [ ]
+test_requirements = []
 
 setup(
     author="Ritvik Sahajpal",
-    author_email='ritvik@umd.edu',
-    python_requires='>=3.9',
+    author_email="ritvik@umd.edu",
+    python_requires=">=3.9",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.9',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
     ],
     description="Models to visualize and forecast crop conditions and yields",
     install_requires=install_requires,
     dependency_links=dependency_links,
     license="MIT license",
     long_description=readme,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     include_package_data=True,
-    keywords='geocif',
-    name='geocif',
-    packages=find_packages(include=['geocif', 'geocif.*']),
+    keywords="geocif",
+    name="geocif",
+    packages=find_packages(include=["geocif", "geocif.*"]),
     setup_requires=setup_requirements,
-    test_suite='tests',
+    test_suite="tests",
     tests_require=test_requirements,
-    url='https://ritviksahajpal.github.io/yield_forecasting/',
-    version='0.1.24',
+    url="https://ritviksahajpal.github.io/yield_forecasting/",
+    version="0.1.25",
     zip_safe=False,
 )
```

