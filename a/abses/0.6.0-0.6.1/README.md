# Comparing `tmp/abses-0.6.0.tar.gz` & `tmp/abses-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abses-0.6.0.tar", max compression
+gzip compressed data, was "abses-0.6.1.tar", max compression
```

## Comparing `abses-0.6.0.tar` & `abses-0.6.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
--rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.0/LICENSE
-drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.0/LICENSES/
--rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.0/README.md
--rw-r--r--   0        0        0     1076 2024-05-11 09:28:11.067993 abses-0.6.0/abses/__init__.py
--rw-r--r--   0        0        0     2651 2024-05-11 09:28:11.068165 abses-0.6.0/abses/_bases/bases.py
--rw-r--r--   0        0        0     3124 2024-05-11 09:28:11.068264 abses-0.6.0/abses/_bases/components.py
--rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.0/abses/_bases/dynamic.py
--rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.0/abses/_bases/errors.py
--rw-r--r--   0        0        0      347 2024-05-11 09:28:11.068990 abses-0.6.0/abses/_bases/logging.py
--rw-r--r--   0        0        0     6280 2024-05-11 09:28:11.069510 abses-0.6.0/abses/_bases/modules.py
--rw-r--r--   0        0        0     3075 2024-05-11 09:28:11.069838 abses-0.6.0/abses/_bases/objects.py
--rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.0/abses/_bases/states.py
--rw-r--r--   0        0        0     9572 2024-05-11 09:28:11.070216 abses-0.6.0/abses/actor.py
--rw-r--r--   0        0        0     4979 2024-05-11 09:28:11.070565 abses-0.6.0/abses/cells.py
--rw-r--r--   0        0        0      297 2024-05-11 09:28:11.070733 abses-0.6.0/abses/conf/default.yaml
--rw-r--r--   0        0        0    17526 2024-05-11 09:28:11.070970 abses-0.6.0/abses/container.py
--rw-r--r--   0        0        0      969 2024-05-11 09:28:11.071255 abses-0.6.0/abses/data.py
--rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.0/abses/decision.py
--rw-r--r--   0        0        0    14654 2024-05-11 09:28:11.071603 abses-0.6.0/abses/experiment.py
--rw-r--r--   0        0        0     3930 2024-05-11 09:28:11.071776 abses-0.6.0/abses/human.py
--rw-r--r--   0        0        0    19386 2024-05-11 09:28:11.072342 abses-0.6.0/abses/links.py
--rw-r--r--   0        0        0    13666 2024-05-11 09:28:11.072495 abses-0.6.0/abses/main.py
--rw-r--r--   0        0        0     8375 2024-05-11 09:28:11.072683 abses-0.6.0/abses/move.py
--rw-r--r--   0        0        0    12421 2024-05-11 09:28:11.073005 abses-0.6.0/abses/nature.py
--rw-r--r--   0        0        0    28654 2024-05-11 09:28:11.073487 abses-0.6.0/abses/patch.py
--rw-r--r--   0        0        0     6802 2024-05-11 09:28:11.073646 abses-0.6.0/abses/random.py
--rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.0/abses/selection.py
--rw-r--r--   0        0        0    11768 2024-05-11 09:28:11.073845 abses-0.6.0/abses/sequences.py
--rw-r--r--   0        0        0    14598 2024-05-11 09:28:11.073992 abses-0.6.0/abses/time.py
--rw-r--r--   0        0        0     4494 2024-05-11 09:28:11.074135 abses-0.6.0/abses/tools/func.py
--rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.0/abses/tools/regex.py
--rw-r--r--   0        0        0      918 2024-05-11 09:28:11.074248 abses-0.6.0/abses/viz/viz_actors.py
--rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.0/abses/viz/viz_model.py
--rw-r--r--   0        0        0     4620 2024-05-11 09:28:11.074600 abses-0.6.0/abses/viz/viz_nature.py
--rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.0/data/.DS_Store
--rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.0/data/YR_cities.zip
--rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.0/data/farmland.tif
--rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.0/data/irr_lands.csv
--rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.0/data/precipitation.nc
--rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.0/icons/fa-regular-400.otf
--rw-r--r--   0        0        0     2714 2024-05-11 09:28:11.086826 abses-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     7334 1970-01-01 00:00:00.000000 abses-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.1/LICENSE
+drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.1/LICENSES/
+-rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.1/README.md
+-rw-r--r--   0        0        0     1076 2024-05-12 01:53:37.423919 abses-0.6.1/abses/__init__.py
+-rw-r--r--   0        0        0     2651 2024-05-11 09:28:11.068165 abses-0.6.1/abses/_bases/bases.py
+-rw-r--r--   0        0        0     3124 2024-05-11 09:28:11.068264 abses-0.6.1/abses/_bases/components.py
+-rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.1/abses/_bases/dynamic.py
+-rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.1/abses/_bases/errors.py
+-rw-r--r--   0        0        0      347 2024-05-11 09:28:11.068990 abses-0.6.1/abses/_bases/logging.py
+-rw-r--r--   0        0        0     6280 2024-05-11 09:28:11.069510 abses-0.6.1/abses/_bases/modules.py
+-rw-r--r--   0        0        0     3075 2024-05-11 09:28:11.069838 abses-0.6.1/abses/_bases/objects.py
+-rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.1/abses/_bases/states.py
+-rw-r--r--   0        0        0     9572 2024-05-11 09:28:11.070216 abses-0.6.1/abses/actor.py
+-rw-r--r--   0        0        0     4979 2024-05-11 09:28:11.070565 abses-0.6.1/abses/cells.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.1/abses/conf/__init__.py
+-rw-r--r--   0        0        0      297 2024-05-11 14:21:43.684047 abses-0.6.1/abses/conf/default.yaml
+-rw-r--r--   0        0        0    17526 2024-05-11 09:28:11.070970 abses-0.6.1/abses/container.py
+-rw-r--r--   0        0        0      969 2024-05-11 09:28:11.071255 abses-0.6.1/abses/data.py
+-rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.1/abses/decision.py
+-rw-r--r--   0        0        0    14654 2024-05-11 09:28:11.071603 abses-0.6.1/abses/experiment.py
+-rw-r--r--   0        0        0     3930 2024-05-11 09:28:11.071776 abses-0.6.1/abses/human.py
+-rw-r--r--   0        0        0    19386 2024-05-11 09:28:11.072342 abses-0.6.1/abses/links.py
+-rw-r--r--   0        0        0    13666 2024-05-11 09:28:11.072495 abses-0.6.1/abses/main.py
+-rw-r--r--   0        0        0     8375 2024-05-11 09:28:11.072683 abses-0.6.1/abses/move.py
+-rw-r--r--   0        0        0    12561 2024-05-11 14:49:37.222743 abses-0.6.1/abses/nature.py
+-rw-r--r--   0        0        0    28816 2024-05-12 01:34:57.898417 abses-0.6.1/abses/patch.py
+-rw-r--r--   0        0        0     6802 2024-05-11 09:28:11.073646 abses-0.6.1/abses/random.py
+-rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.1/abses/selection.py
+-rw-r--r--   0        0        0    11768 2024-05-11 09:28:11.073845 abses-0.6.1/abses/sequences.py
+-rw-r--r--   0        0        0    14598 2024-05-11 09:28:11.073992 abses-0.6.1/abses/time.py
+-rw-r--r--   0        0        0     5391 2024-05-12 01:34:57.375663 abses-0.6.1/abses/tools/func.py
+-rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.1/abses/tools/regex.py
+-rw-r--r--   0        0        0      918 2024-05-11 09:28:11.074248 abses-0.6.1/abses/viz/viz_actors.py
+-rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.1/abses/viz/viz_model.py
+-rw-r--r--   0        0        0     4620 2024-05-11 09:28:11.074600 abses-0.6.1/abses/viz/viz_nature.py
+-rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.1/data/.DS_Store
+-rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.1/data/YR_cities.zip
+-rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.1/data/farmland.tif
+-rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.1/data/irr_lands.csv
+-rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.1/data/precipitation.nc
+-rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.1/icons/fa-regular-400.otf
+-rw-r--r--   0        0        0     2778 2024-05-12 01:53:37.423782 abses-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     7334 1970-01-01 00:00:00.000000 abses-0.6.1/PKG-INFO
```

### Comparing `abses-0.6.0/LICENSE` & `abses-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/README.md` & `abses-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/__init__.py` & `abses-0.6.1/abses/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "PatchCell",
     "perception",
     "alive_required",
     "time_condition",
     "Experiment",
     "load_data",
 ]
-__version__ = "v0.6.0"
+__version__ = "v0.6.1"
 
 from .actor import Actor, alive_required, perception
 from .container import ActorsList
 from .data import load_data
 from .decision import Decision
 from .experiment import Experiment
 from .human import BaseHuman
```

### Comparing `abses-0.6.0/abses/_bases/bases.py` & `abses-0.6.1/abses/_bases/bases.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/_bases/components.py` & `abses-0.6.1/abses/_bases/components.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/_bases/dynamic.py` & `abses-0.6.1/abses/_bases/dynamic.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/_bases/modules.py` & `abses-0.6.1/abses/_bases/modules.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/_bases/objects.py` & `abses-0.6.1/abses/_bases/objects.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/_bases/states.py` & `abses-0.6.1/abses/_bases/states.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/actor.py` & `abses-0.6.1/abses/actor.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/cells.py` & `abses-0.6.1/abses/cells.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/container.py` & `abses-0.6.1/abses/container.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/data.py` & `abses-0.6.1/abses/data.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/decision.py` & `abses-0.6.1/abses/decision.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/experiment.py` & `abses-0.6.1/abses/experiment.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/human.py` & `abses-0.6.1/abses/human.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/links.py` & `abses-0.6.1/abses/links.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/main.py` & `abses-0.6.1/abses/main.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/move.py` & `abses-0.6.1/abses/move.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/nature.py` & `abses-0.6.1/abses/nature.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,48 +43,57 @@
 from abses.viz.viz_nature import _VizNature
 
 if TYPE_CHECKING:
     from abses.main import MainModel
 
 
 class _PatchModuleProtocol(Protocol):
+    @property
     def cells(self) -> ActorsList[PatchCell]:
         """The cells stored in this layer."""
 
+    @property
     def mask(self) -> np.ndarray:
         """Where is not accessible."""
 
+    @property
     def cell_properties(self) -> set[str]:
         """The accessible attributes of cells stored in this layer.
         All `PatchCell` methods decorated by `raster_attribute` should be appeared here.
         """
 
+    @property
     def xda(self) -> xr.DataArray:
         """Get the xarray raster layer with spatial coordinates."""
 
+    @property
     def plot(self) -> _VizNature:
         """Plotting"""
 
+    @property
     def attributes(self) -> set[str]:
         """All accessible attributes from this layer."""
 
     @property
     def shape2d(self) -> Coordinate:
         """Raster shape in 2D (height, width).
         This is useful when working with 2d `numpy.array`.
         """
 
+    @property
     def shape3d(self) -> Coordinate:
         """Raster shape in 3D (1, heigh, width).
         This is useful when working with `rasterio` band.
         """
 
+    @property
     def array_cells(self) -> np.ndarray:
         """Array type of the `PatchCell` stored in this module."""
 
+    @property
     def coords(self) -> Coordinate:
         """Coordinate system of the raster data.
         This is useful when working with `xarray.DataArray`.
         """
 
     def to_crs(self, crs, inplace=False) -> Optional[PatchModule]:
         """Converting the raster data to a another CRS."""
@@ -127,14 +136,15 @@
         """
 
     def out_of_bounds(self, pos: Coordinate) -> bool:
         """Check if a pos is out of the bounds.
         This is a protocol method.
         """
 
+    @property
     def random(self) -> ListRandom:
         """Randomly"""
 
     def select(
         self,
         where: Optional[CellFilter] = None,
     ) -> ActorsList[PatchCell]:
```

### Comparing `abses-0.6.0/abses/patch.py` & `abses-0.6.1/abses/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from shapely import Geometry
 
 from abses._bases.errors import ABSESpyError
 from abses._bases.modules import Module, _ModuleFactory
 from abses.cells import PatchCell
 from abses.random import ListRandom
 from abses.sequences import ActorsList
-from abses.tools.func import get_buffer
+from abses.tools.func import get_buffer, set_null_values
 from abses.viz.viz_nature import _VizNature
 
 if TYPE_CHECKING:
     from abses.main import MainModel
 
 CRS = "epsg:4326"
 CellFilter: TypeAlias = Optional[str | np.ndarray | xr.DataArray | Geometry]
@@ -173,15 +173,15 @@
         model: MainModel[Any, Any],
         cell_cls: type[PatchCell] = PatchCell,
         module_cls: Optional[Type[PatchModule]] = None,
         name: str | None = None,
         attr_name: str | None = None,
         apply_raster: bool = False,
         band: int = 1,
-        nodata: Any = np.nan,
+        apply_nodata: bool = True,
         **kwargs: Any,
     ) -> PatchModule:
         """Create a raster layer module from a file.
 
         Parameters:
             raster_file:
                 File path of a geo-tiff dataset.
@@ -197,15 +197,15 @@
                 Class type of `PatchCell` to create.
 
         """
         to_create = cast(PatchModule, self._check_cls(module_cls=module_cls))
         with rasterio.open(raster_file, "r") as dataset:
             values = dataset.read(band)
             nodata_mask = values == dataset.nodata
-            values[nodata_mask] = nodata
+            set_null_values(values, nodata_mask)
             height, width = values.shape
             total_bounds = [
                 dataset.bounds.left,
                 dataset.bounds.bottom,
                 dataset.bounds.right,
                 dataset.bounds.top,
             ]
@@ -214,15 +214,16 @@
             name=name,
             width=width,
             height=height,
             crs=dataset.crs,
             total_bounds=total_bounds,
             cell_cls=cell_cls,
         )
-        obj.mask = np.squeeze(~nodata_mask)
+        if apply_nodata:
+            obj.mask = np.squeeze(~nodata_mask)
         # obj._transform = dataset.transform
         if apply_raster:
             obj.apply_raster(values, attr_name=attr_name, **kwargs)
         return obj
 
 
 class PatchModule(Module, RasterBase):
@@ -610,21 +611,24 @@
         return np.ndenumerate(self.array_cells)
 
     def _add_attribute(
         self,
         data: np.ndarray,
         attr_name: Optional[str] = None,
         flipud: bool = False,
+        apply_mask: bool = False,
     ) -> None:
         data = np.squeeze(data)
         if data.shape != self.shape2d:
             raise ValueError(
                 f"Data shape does not match raster shape. "
                 f"Expected {self.shape2d}, received {data.shape}."
             )
+        if apply_mask:
+            set_null_values(data, ~self.mask)
         if attr_name is None:
             attr_name = f"attribute_{len(self.attributes)}"
         self._attributes.add(attr_name)
         if flipud:
             data = np.flipud(data)
         np.vectorize(setattr)(self.array_cells, attr_name, data)
```

### Comparing `abses-0.6.0/abses/random.py` & `abses-0.6.1/abses/random.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/selection.py` & `abses-0.6.1/abses/selection.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/sequences.py` & `abses-0.6.1/abses/sequences.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/time.py` & `abses-0.6.1/abses/time.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/tools/func.py` & `abses-0.6.1/abses/tools/func.py`

 * *Files 18% similar despite different names*

```diff
@@ -148,7 +148,37 @@
             else:
                 return func(*args, **kwargs)
 
         return wrapper
 
     # 检查是否有参数传递给装饰器，若没有则返回装饰器本身
     return decorator(decorated_func) if decorated_func else decorator
+
+
+def set_null_values(arr: np.ndarray, mask: np.ndarray):
+    """
+    Set null values in an array based on a boolean mask and the array's data type.
+
+    Parameters:
+        arr:
+            The input array that can contain float or strings.
+        mask:
+            A boolean array where True indicates that a null value should be set.
+
+    Returns:
+        The modified array with null values set.
+    """
+    if arr.shape != mask.shape:
+        raise ValueError(f"Mismatching shape {mask.shape} and {arr.shape}.")
+    # Check if the dtype is float or integer
+    if arr.dtype.kind in {"f", "i"}:
+        null_value = np.nan
+    # Unicode string
+    elif arr.dtype.kind == "U":
+        null_value = ""
+    # # Byte string
+    elif arr.dtype.kind == "S":
+        null_value = b""
+    else:
+        raise ValueError(f"Unsupported data type {arr.dtype}")
+    arr[mask] = null_value
+    return arr
```

### Comparing `abses-0.6.0/abses/tools/regex.py` & `abses-0.6.1/abses/tools/regex.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/viz/viz_actors.py` & `abses-0.6.1/abses/viz/viz_actors.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/viz/viz_model.py` & `abses-0.6.1/abses/viz/viz_model.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/abses/viz/viz_nature.py` & `abses-0.6.1/abses/viz/viz_nature.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/data/.DS_Store` & `abses-0.6.1/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/data/YR_cities.zip` & `abses-0.6.1/data/YR_cities.zip`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/data/farmland.tif` & `abses-0.6.1/data/farmland.tif`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/data/irr_lands.csv` & `abses-0.6.1/data/irr_lands.csv`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/data/precipitation.nc` & `abses-0.6.1/data/precipitation.nc`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/icons/fa-regular-400.otf` & `abses-0.6.1/icons/fa-regular-400.otf`

 * *Files identical despite different names*

### Comparing `abses-0.6.0/pyproject.toml` & `abses-0.6.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -27,33 +27,35 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "abses"
-version = "0.6.0"
+version = "0.6.1"
 description = "ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour."
 authors = ["Shuang Song <songshgeo@gmail.com>"]
 license = "Apache 2.0 License"
 readme = "README.md"
 include = [
   "icons/fa-regular-400.otf",
   "abses/conf/**/*.yaml",
-  "data/*"
+  "abses/conf/*.py",
+  "data/*",
+  "hydra_plugins.abses_searchpath_plugin"
 ]
 
 [tool.poetry.plugins."hydra.searchpath"]
 abses = "hydra_plugins.abses_searchpath_plugin:ABSESpySearchPathPlugin"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 netcdf4 = ">=1.6"
 hydra-core = "~1.3"
-mesa-geo = "^0.6.0"
+mesa-geo = "^0.6.1"
 xarray = "~2023"
 fiona = ">1.8"
 loguru = "~0.7"
 rioxarray = "~0.13"
 pendulum = "~2"
 geopandas = "~0"
 typing-extensions = "^4.10.0"
```

### Comparing `abses-0.6.0/PKG-INFO` & `abses-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abses
-Version: 0.6.0
+Version: 0.6.1
 Summary: ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour.
 License: Apache 2.0 License
 Author: Shuang Song
 Author-email: songshgeo@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fiona (>1.8)
 Requires-Dist: fontawesome (>=5.10.1.post1,<6.0.0)
 Requires-Dist: geopandas (>=0,<1)
 Requires-Dist: hydra-core (>=1.3,<1.4)
 Requires-Dist: loguru (>=0.7,<0.8)
-Requires-Dist: mesa-geo (>=0.6.0,<0.7.0)
+Requires-Dist: mesa-geo (>=0.6.1,<0.7.0)
 Requires-Dist: netcdf4 (>=1.6)
 Requires-Dist: pendulum (>=2,<3)
 Requires-Dist: rioxarray (>=0.13,<0.14)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Requires-Dist: xarray (>=2023,<2024)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: abses Version: 0.6.0 Summary: ABSESpy makes it
+Metadata-Version: 2.1 Name: abses Version: 0.6.1 Summary: ABSESpy makes it
 easier to build artificial Social-ecological systems with real GeoSpatial
 datasets and fully incorporate human behaviour. License: Apache 2.0 License
 Author: Shuang Song Author-email: songshgeo@gmail.com Requires-Python:
 >=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: fiona (>1.8) Requires-
 Dist: fontawesome (>=5.10.1.post1,<6.0.0) Requires-Dist: geopandas (>=0,<1)
 Requires-Dist: hydra-core (>=1.3,<1.4) Requires-Dist: loguru (>=0.7,<0.8)
-Requires-Dist: mesa-geo (>=0.6.0,<0.7.0) Requires-Dist: netcdf4 (>=1.6)
+Requires-Dist: mesa-geo (>=0.6.1,<0.7.0) Requires-Dist: netcdf4 (>=1.6)
 Requires-Dist: pendulum (>=2,<3) Requires-Dist: rioxarray (>=0.13,<0.14)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0) Requires-Dist: typing-extensions
 (>=4.10.0,<5.0.0) Requires-Dist: xarray (>=2023,<2024) Description-Content-
 Type: text/markdown # ABSESpy: Agent-Based Modeling Framework for Social-
 Ecological Systems ![ABSES_banner](https://songshgeo-picgo-1302043007.cos.ap-
 beijing.myqcloud.com/uPic/CleanShot%202023-10-19%20at%2019.08.12@2x.png)
   _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]_[_R_e_p_o
```

