# Comparing `tmp/abses-0.6.2.tar.gz` & `tmp/abses-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abses-0.6.2.tar", max compression
+gzip compressed data, was "abses-0.6.3.tar", max compression
```

## Comparing `abses-0.6.2.tar` & `abses-0.6.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.2/LICENSE
-drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.2/LICENSES/
--rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.2/README.md
--rw-r--r--   0        0        0     1076 2024-05-12 02:38:47.595508 abses-0.6.2/abses/__init__.py
--rw-r--r--   0        0        0     2651 2024-05-11 09:28:11.068165 abses-0.6.2/abses/_bases/bases.py
--rw-r--r--   0        0        0     3124 2024-05-11 09:28:11.068264 abses-0.6.2/abses/_bases/components.py
--rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.2/abses/_bases/dynamic.py
--rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.2/abses/_bases/errors.py
--rw-r--r--   0        0        0      347 2024-05-11 09:28:11.068990 abses-0.6.2/abses/_bases/logging.py
--rw-r--r--   0        0        0     6280 2024-05-11 09:28:11.069510 abses-0.6.2/abses/_bases/modules.py
--rw-r--r--   0        0        0     3075 2024-05-11 09:28:11.069838 abses-0.6.2/abses/_bases/objects.py
--rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.2/abses/_bases/states.py
--rw-r--r--   0        0        0     9572 2024-05-11 09:28:11.070216 abses-0.6.2/abses/actor.py
--rw-r--r--   0        0        0     4979 2024-05-11 09:28:11.070565 abses-0.6.2/abses/cells.py
--rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.2/abses/conf/__init__.py
--rw-r--r--   0        0        0      297 2024-05-11 14:21:43.684047 abses-0.6.2/abses/conf/default.yaml
--rw-r--r--   0        0        0    17526 2024-05-11 09:28:11.070970 abses-0.6.2/abses/container.py
--rw-r--r--   0        0        0      969 2024-05-11 09:28:11.071255 abses-0.6.2/abses/data.py
--rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.2/abses/decision.py
--rw-r--r--   0        0        0    14654 2024-05-11 09:28:11.071603 abses-0.6.2/abses/experiment.py
--rw-r--r--   0        0        0     3930 2024-05-11 09:28:11.071776 abses-0.6.2/abses/human.py
--rw-r--r--   0        0        0    19386 2024-05-11 09:28:11.072342 abses-0.6.2/abses/links.py
--rw-r--r--   0        0        0    13666 2024-05-11 09:28:11.072495 abses-0.6.2/abses/main.py
--rw-r--r--   0        0        0     8375 2024-05-11 09:28:11.072683 abses-0.6.2/abses/move.py
--rw-r--r--   0        0        0    12561 2024-05-11 14:49:37.222743 abses-0.6.2/abses/nature.py
--rw-r--r--   0        0        0    28816 2024-05-12 01:34:57.898417 abses-0.6.2/abses/patch.py
--rw-r--r--   0        0        0     6802 2024-05-11 09:28:11.073646 abses-0.6.2/abses/random.py
--rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.2/abses/selection.py
--rw-r--r--   0        0        0    11768 2024-05-11 09:28:11.073845 abses-0.6.2/abses/sequences.py
--rw-r--r--   0        0        0    14598 2024-05-11 09:28:11.073992 abses-0.6.2/abses/time.py
--rw-r--r--   0        0        0     5391 2024-05-12 02:43:42.296709 abses-0.6.2/abses/tools/func.py
--rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.2/abses/tools/regex.py
--rw-r--r--   0        0        0      918 2024-05-11 09:28:11.074248 abses-0.6.2/abses/viz/viz_actors.py
--rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.2/abses/viz/viz_model.py
--rw-r--r--   0        0        0     4620 2024-05-11 09:28:11.074600 abses-0.6.2/abses/viz/viz_nature.py
--rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.2/data/.DS_Store
--rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.2/data/YR_cities.zip
--rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.2/data/farmland.tif
--rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.2/data/irr_lands.csv
--rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.2/data/precipitation.nc
--rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.2/icons/fa-regular-400.otf
--rw-r--r--   0        0        0     2760 2024-05-12 02:44:03.634683 abses-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 abses-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.3/LICENSE
+drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.3/LICENSES/
+-rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.3/README.md
+-rw-r--r--   0        0        0     1076 2024-05-12 12:07:53.904095 abses-0.6.3/abses/__init__.py
+-rw-r--r--   0        0        0     2651 2024-05-11 09:28:11.068165 abses-0.6.3/abses/_bases/bases.py
+-rw-r--r--   0        0        0     3124 2024-05-11 09:28:11.068264 abses-0.6.3/abses/_bases/components.py
+-rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.3/abses/_bases/dynamic.py
+-rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.3/abses/_bases/errors.py
+-rw-r--r--   0        0        0      347 2024-05-11 09:28:11.068990 abses-0.6.3/abses/_bases/logging.py
+-rw-r--r--   0        0        0     6280 2024-05-11 09:28:11.069510 abses-0.6.3/abses/_bases/modules.py
+-rw-r--r--   0        0        0     3075 2024-05-11 09:28:11.069838 abses-0.6.3/abses/_bases/objects.py
+-rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.3/abses/_bases/states.py
+-rw-r--r--   0        0        0     9572 2024-05-11 09:28:11.070216 abses-0.6.3/abses/actor.py
+-rw-r--r--   0        0        0     4979 2024-05-11 09:28:11.070565 abses-0.6.3/abses/cells.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.3/abses/conf/__init__.py
+-rw-r--r--   0        0        0      297 2024-05-11 14:21:43.684047 abses-0.6.3/abses/conf/default.yaml
+-rw-r--r--   0        0        0    17526 2024-05-11 09:28:11.070970 abses-0.6.3/abses/container.py
+-rw-r--r--   0        0        0      969 2024-05-11 09:28:11.071255 abses-0.6.3/abses/data.py
+-rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.3/abses/decision.py
+-rw-r--r--   0        0        0    15662 2024-05-12 12:06:53.545831 abses-0.6.3/abses/experiment.py
+-rw-r--r--   0        0        0     3930 2024-05-11 09:28:11.071776 abses-0.6.3/abses/human.py
+-rw-r--r--   0        0        0    19386 2024-05-11 09:28:11.072342 abses-0.6.3/abses/links.py
+-rw-r--r--   0        0        0    13666 2024-05-11 09:28:11.072495 abses-0.6.3/abses/main.py
+-rw-r--r--   0        0        0     8375 2024-05-11 09:28:11.072683 abses-0.6.3/abses/move.py
+-rw-r--r--   0        0        0    12561 2024-05-11 14:49:37.222743 abses-0.6.3/abses/nature.py
+-rw-r--r--   0        0        0    28830 2024-05-12 03:13:27.744826 abses-0.6.3/abses/patch.py
+-rw-r--r--   0        0        0     6802 2024-05-11 09:28:11.073646 abses-0.6.3/abses/random.py
+-rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.3/abses/selection.py
+-rw-r--r--   0        0        0    11768 2024-05-11 09:28:11.073845 abses-0.6.3/abses/sequences.py
+-rw-r--r--   0        0        0    14598 2024-05-11 09:28:11.073992 abses-0.6.3/abses/time.py
+-rw-r--r--   0        0        0     5391 2024-05-12 02:43:42.296709 abses-0.6.3/abses/tools/func.py
+-rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.3/abses/tools/regex.py
+-rw-r--r--   0        0        0      918 2024-05-11 09:28:11.074248 abses-0.6.3/abses/viz/viz_actors.py
+-rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.3/abses/viz/viz_model.py
+-rw-r--r--   0        0        0     4620 2024-05-11 09:28:11.074600 abses-0.6.3/abses/viz/viz_nature.py
+-rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.3/data/.DS_Store
+-rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.3/data/YR_cities.zip
+-rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.3/data/farmland.tif
+-rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.3/data/irr_lands.csv
+-rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.3/data/precipitation.nc
+-rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.3/icons/fa-regular-400.otf
+-rw-r--r--   0        0        0     2760 2024-05-12 12:08:01.980157 abses-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 abses-0.6.3/PKG-INFO
```

### Comparing `abses-0.6.2/LICENSE` & `abses-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/README.md` & `abses-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/__init__.py` & `abses-0.6.3/abses/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "PatchCell",
     "perception",
     "alive_required",
     "time_condition",
     "Experiment",
     "load_data",
 ]
-__version__ = "v0.6.2"
+__version__ = "v0.6.3"
 
 from .actor import Actor, alive_required, perception
 from .container import ActorsList
 from .data import load_data
 from .decision import Decision
 from .experiment import Experiment
 from .human import BaseHuman
```

### Comparing `abses-0.6.2/abses/_bases/bases.py` & `abses-0.6.3/abses/_bases/bases.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/_bases/components.py` & `abses-0.6.3/abses/_bases/components.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/_bases/dynamic.py` & `abses-0.6.3/abses/_bases/dynamic.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/_bases/modules.py` & `abses-0.6.3/abses/_bases/modules.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/_bases/objects.py` & `abses-0.6.3/abses/_bases/objects.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/_bases/states.py` & `abses-0.6.3/abses/_bases/states.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/actor.py` & `abses-0.6.3/abses/actor.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/cells.py` & `abses-0.6.3/abses/cells.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/container.py` & `abses-0.6.3/abses/container.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/data.py` & `abses-0.6.3/abses/data.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/decision.py` & `abses-0.6.3/abses/decision.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/experiment.py` & `abses-0.6.3/abses/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,20 +90,21 @@
 
 class Experiment:
     """Repeated Experiment."""
 
     _instance = None
     folder: Path = Path(os.getcwd())
     hydra_config: DictConfig = DictConfig({})
-    results: List[Dict[str, Any]] = []
     name: Optional[str] = None
+    final_vars: List[Dict[str, Any]] = []
+    model_vars: List[pd.DataFrame] = []
 
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
-            cls._instance = super(Experiment, cls).__new__(cls)
+            cls._instance = super().__new__(cls)
         return cls._instance
 
     def __init__(
         self,
         model_cls: Optional[Type[MainModel]] = None,
     ):
         self._n_runs = 0
@@ -214,38 +215,50 @@
             return HydraConfig.get().cfg
         with initialize(version_base=None, config_path=str(cfg_path.parent)):
             cfg = compose(config_name=cfg_path.stem, overrides=overrides)
         return cfg
 
     def run(
         self, cfg: DictConfig, repeat_id: int, outpath: Optional[Path] = None
-    ) -> Dict[str, Any]:
+    ) -> Tuple[Dict[str, Any], pd.DataFrame]:
         """运行模型一次"""
         if not self._model or not issubclass(self._model, MainModel):
             raise TypeError(f"The model class {self._model} is not valid.")
         model = self._model(parameters=cfg, run_id=repeat_id, outpath=outpath)
         model.run_model()
-        return model.final_report()
+        if model.datacollector.model_reporters:
+            df = model.datacollector.get_model_vars_dataframe()
+        else:
+            df = pd.DataFrame()
+        return model.final_report(), df
 
     def _update_result(
         self,
         repeat_id: int,
         reports: Optional[Dict[str, Any]] = None,
+        model_df: Optional[pd.DataFrame] = None,
     ) -> None:
         """Updating in each run."""
         if reports is None:
             reports = {}
         reports.update(
             {
                 "job_id": self.job_id,
                 "repeat_id": repeat_id,
             }
         )
         reports |= self.overrides
-        self.results.append(reports)
+        self.final_vars.append(reports)
+        if model_df is None:
+            return
+        model_df = model_df.reset_index()
+        model_df = model_df.rename({"index": "tick"}, axis=1)
+        model_df.insert(0, "repeat_id", repeat_id)
+        model_df.insert(0, "job_id", self.job_id)
+        self.model_vars.append(model_df)
 
     def _batch_run_multi_processes(
         self,
         cfg: DictConfig,
         repeats,
         number_process: Optional[int] = 1,
         display_progress: bool = True,
@@ -257,22 +270,28 @@
                 futures = [
                     executor.submit(self.run, cfg, repeat_id, self.outpath)
                     for repeat_id in range(1, repeats + 1)
                 ]
                 # 使用as_completed等待任务完成
                 for i, future in enumerate(as_completed(futures)):
                     # 每完成一个任务，更新进度条和运行计数
-                    result = future.result()
+                    result, model_df = future.result()
                     pbar.update()
-                    self._update_result(reports=result, repeat_id=i + 1)
+                    self._update_result(
+                        reports=result, model_df=model_df, repeat_id=i + 1
+                    )
 
     def _batch_run_repeats(self, cfg, repeats, display_progress) -> None:
         for repeat in tqdm(range(repeats), disable=not display_progress):
-            result = self.run(cfg, repeat_id=repeat + 1, outpath=self.outpath)
-            self._update_result(reports=result, repeat_id=repeat + 1)
+            result, model_df = self.run(
+                cfg, repeat_id=repeat + 1, outpath=self.outpath
+            )
+            self._update_result(
+                reports=result, model_df=model_df, repeat_id=repeat + 1
+            )
 
     def _parse_path(self, relative_path: str) -> Path:
         """Parse the path of the configuration file.
         Convert the relpath of current work space to the relpath of this script.
         """
         # 目标绝对路径
         abs_config_file_path = (Path(os.getcwd()) / relative_path).resolve()
@@ -372,29 +391,30 @@
             self._job_id += 1
         # finally, clean up the overrides now.
         self.overrides = {}
 
     @classmethod
     def summary(cls, save: bool = False, **kwargs) -> None:
         """Ending the experiment."""
-        df = pd.DataFrame(cls.results)
+        df = pd.DataFrame(cls.final_vars)
         if save:
             df.to_csv(cls.folder / "summary.csv", index=False, **kwargs)
         return df
 
     @classmethod
     def clean(cls, new_exp: bool = False) -> None:
         """Clean the results.
 
         Parameters:
             new_exp:
                 Whether to create a new experiment.
                 If True, it will delete all the current settings.
         """
-        cls.results = []
+        cls.final_vars = []
+        cls.model_vars = []
         if new_exp:
             cls._instance = None
             cls.folder = Path(os.getcwd())
             cls.hydra_config = DictConfig({})
             cls.name = None
 
     @classmethod
@@ -412,7 +432,14 @@
                 If the model class `model_cls` is not a valid `ABSESpy` model.
 
         Returns:
             An experiment.
         """
         cls.clean(new_exp=True)
         return cls(model_cls=model_cls)
+
+    @classmethod
+    def get_model_vars_dataframe(cls) -> pd.DataFrame:
+        """Aggregation of model vars dataframe."""
+        if cls.model_vars:
+            return pd.concat(cls.model_vars, axis=0)
+        raise ValueError("No model vars found.")
```

### Comparing `abses-0.6.2/abses/human.py` & `abses-0.6.3/abses/human.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/links.py` & `abses-0.6.3/abses/links.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/main.py` & `abses-0.6.3/abses/main.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/move.py` & `abses-0.6.3/abses/move.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/nature.py` & `abses-0.6.3/abses/nature.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/patch.py` & `abses-0.6.3/abses/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
                 E.g., class Module -> module.
             cell_cls:
                 Class type of `PatchCell` to create.
 
         """
         to_create = cast(PatchModule, self._check_cls(module_cls=module_cls))
         with rasterio.open(raster_file, "r") as dataset:
-            values = dataset.read(band)
+            values = dataset.read(band).astype(float)
             nodata_mask = values == dataset.nodata
             set_null_values(values, nodata_mask)
             height, width = values.shape
             total_bounds = [
                 dataset.bounds.left,
                 dataset.bounds.bottom,
                 dataset.bounds.right,
```

### Comparing `abses-0.6.2/abses/random.py` & `abses-0.6.3/abses/random.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/selection.py` & `abses-0.6.3/abses/selection.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/sequences.py` & `abses-0.6.3/abses/sequences.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/time.py` & `abses-0.6.3/abses/time.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/tools/func.py` & `abses-0.6.3/abses/tools/func.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/tools/regex.py` & `abses-0.6.3/abses/tools/regex.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/viz/viz_actors.py` & `abses-0.6.3/abses/viz/viz_actors.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/viz/viz_model.py` & `abses-0.6.3/abses/viz/viz_model.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/abses/viz/viz_nature.py` & `abses-0.6.3/abses/viz/viz_nature.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/data/.DS_Store` & `abses-0.6.3/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/data/YR_cities.zip` & `abses-0.6.3/data/YR_cities.zip`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/data/farmland.tif` & `abses-0.6.3/data/farmland.tif`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/data/irr_lands.csv` & `abses-0.6.3/data/irr_lands.csv`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/data/precipitation.nc` & `abses-0.6.3/data/precipitation.nc`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/icons/fa-regular-400.otf` & `abses-0.6.3/icons/fa-regular-400.otf`

 * *Files identical despite different names*

### Comparing `abses-0.6.2/pyproject.toml` & `abses-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "abses"
-version = "0.6.2"
+version = "0.6.3"
 description = "ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour."
 authors = ["Shuang Song <songshgeo@gmail.com>"]
 license = "Apache 2.0 License"
 readme = "README.md"
 include = [
   "icons/fa-regular-400.otf",
   "abses/conf/**/*.yaml",
```

### Comparing `abses-0.6.2/PKG-INFO` & `abses-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abses
-Version: 0.6.2
+Version: 0.6.3
 Summary: ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour.
 License: Apache 2.0 License
 Author: Shuang Song
 Author-email: songshgeo@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: abses Version: 0.6.2 Summary: ABSESpy makes it
+Metadata-Version: 2.1 Name: abses Version: 0.6.3 Summary: ABSESpy makes it
 easier to build artificial Social-ecological systems with real GeoSpatial
 datasets and fully incorporate human behaviour. License: Apache 2.0 License
 Author: Shuang Song Author-email: songshgeo@gmail.com Requires-Python:
 >=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: fiona (>1.8) Requires-
```

