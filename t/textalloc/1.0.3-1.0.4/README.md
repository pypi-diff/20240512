# Comparing `tmp/textalloc-1.0.3.tar.gz` & `tmp/textalloc-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textalloc-1.0.3.tar", last modified: Tue Apr 30 21:56:29 2024, max compression
+gzip compressed data, was "textalloc-1.0.4.tar", last modified: Sun May 12 08:08:09 2024, max compression
```

## Comparing `textalloc-1.0.3.tar` & `textalloc-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:56:29.716476 textalloc-1.0.3/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-1.0.3/LICENSE
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9265 2024-04-30 21:56:29.716476 textalloc-1.0.3/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8601 2024-04-30 21:55:11.000000 textalloc-1.0.3/README.md
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-04-30 21:54:34.000000 textalloc-1.0.3/pyproject.toml
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-04-30 21:56:29.730302 textalloc-1.0.3/setup.cfg
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:56:29.372959 textalloc-1.0.3/src/
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:56:29.531246 textalloc-1.0.3/src/textalloc/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    14506 2024-04-30 21:52:25.000000 textalloc-1.0.3/src/textalloc/__init__.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-1.0.3/src/textalloc/candidates.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9795 2024-04-30 21:54:41.000000 textalloc-1.0.3/src/textalloc/non_overlapping_boxes.py
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-1.0.3/src/textalloc/overlap_functions.py
-drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-04-30 21:56:29.705279 textalloc-1.0.3/src/textalloc.egg-info/
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9265 2024-04-30 21:56:29.000000 textalloc-1.0.3/src/textalloc.egg-info/PKG-INFO
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-04-30 21:56:29.000000 textalloc-1.0.3/src/textalloc.egg-info/SOURCES.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-04-30 21:56:29.000000 textalloc-1.0.3/src/textalloc.egg-info/dependency_links.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-04-30 21:56:29.000000 textalloc-1.0.3/src/textalloc.egg-info/requires.txt
--rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-04-30 21:56:29.000000 textalloc-1.0.3/src/textalloc.egg-info/top_level.txt
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-05-12 08:08:09.530091 textalloc-1.0.4/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     1077 2023-02-14 19:18:58.000000 textalloc-1.0.4/LICENSE
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9396 2024-05-12 08:08:09.519413 textalloc-1.0.4/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     8732 2024-05-12 08:05:42.000000 textalloc-1.0.4/README.md
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      741 2024-05-12 08:07:12.000000 textalloc-1.0.4/pyproject.toml
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       38 2024-05-12 08:08:09.532571 textalloc-1.0.4/setup.cfg
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-05-12 08:08:09.005796 textalloc-1.0.4/src/
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-05-12 08:08:09.272987 textalloc-1.0.4/src/textalloc/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    15442 2024-05-12 08:05:42.000000 textalloc-1.0.4/src/textalloc/__init__.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     6539 2024-02-20 19:23:50.000000 textalloc-1.0.4/src/textalloc/candidates.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9795 2024-04-30 21:54:41.000000 textalloc-1.0.4/src/textalloc/non_overlapping_boxes.py
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)    10042 2024-02-20 19:25:04.000000 textalloc-1.0.4/src/textalloc/overlap_functions.py
+drwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        0 2024-05-12 08:08:09.504643 textalloc-1.0.4/src/textalloc.egg-info/
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)     9396 2024-05-12 08:08:08.000000 textalloc-1.0.4/src/textalloc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)      344 2024-05-12 08:08:08.000000 textalloc-1.0.4/src/textalloc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)        1 2024-05-12 08:08:08.000000 textalloc-1.0.4/src/textalloc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       49 2024-05-12 08:08:08.000000 textalloc-1.0.4/src/textalloc.egg-info/requires.txt
+-rwxrwxrwx   0 ckjellson  (1000) ckjellson  (1000)       10 2024-05-12 08:08:08.000000 textalloc-1.0.4/src/textalloc.egg-info/top_level.txt
```

### Comparing `textalloc-1.0.3/LICENSE` & `textalloc-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `textalloc-1.0.3/PKG-INFO` & `textalloc-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -124,14 +124,17 @@
     If set to True, avoids overlap for drawn lines to text labels.
 plot_kwargs: (dict), default None
     kwargs for the plt.plot of the lines if draw_lines is True.
 **kwargs: ()
     kwargs for the plt.text() call.
     If transform is used, it only needs to be provided here, i.e. not also in plot_kwargs.
 ```
+
+The allocate call returns a tuple containing the resulting positions used to plot the text labels and the connecting label lines
+
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
 1. Generate a large number of candidate boxes near the original point with size that matches the fontsize.
 2. Find the candidates that do not overlap any points, lines, plot boundaries, or already allocated boxes.
```

### Comparing `textalloc-1.0.3/README.md` & `textalloc-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,17 @@
     If set to True, avoids overlap for drawn lines to text labels.
 plot_kwargs: (dict), default None
     kwargs for the plt.plot of the lines if draw_lines is True.
 **kwargs: ()
     kwargs for the plt.text() call.
     If transform is used, it only needs to be provided here, i.e. not also in plot_kwargs.
 ```
+
+The allocate call returns a tuple containing the resulting positions used to plot the text labels and the connecting label lines
+
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
 1. Generate a large number of candidate boxes near the original point with size that matches the fontsize.
 2. Find the candidates that do not overlap any points, lines, plot boundaries, or already allocated boxes.
```

### Comparing `textalloc-1.0.3/pyproject.toml` & `textalloc-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textalloc"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="Christoffer Kjellson", email="c.kjellson@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Efficient Text Allocation in matplotlib using NumPy Broadcasting"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `textalloc-1.0.3/src/textalloc/__init__.py` & `textalloc-1.0.4/src/textalloc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from matplotlib.path import get_path_collection_extents
 from textalloc.non_overlapping_boxes import (
     get_non_overlapping_boxes,
     find_nearest_point_on_box,
 )
 import numpy as np
 import time
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 import warnings
 
 try:
     from tqdm import tqdm
 except ImportError:
 
     def tqdm(iterator, *args, **kwargs):
@@ -40,15 +40,17 @@
     linewidth: float = 1,
     textcolor: Union[str, List[str]] = "k",
     seed: int = 0,
     direction: str = None,
     avoid_label_lines_overlap: bool = False,
     plot_kwargs: Dict[str, Any] = None,
     **kwargs,
-):
+) -> Tuple[List[Optional[Tuple[float, float]]],
+           List[Optional[Tuple[Tuple[float, float],
+                               Tuple[float, float]]]]]:
     """Main function of allocating text-boxes in matplotlib plot
 
     Args:
         ax (_type_): matplotlib axes used for plotting.
         x (Union[np.ndarray, List[float]]): x-coordinates of texts 1d array/list.
         y (Union[np.ndarray, List[float]]): y-coordinates of texts 1d array/list.
         text_list (List[str]): list of texts.
@@ -71,14 +73,18 @@
         linewidth (float, optional): width of line. Defaults to 1.
         textcolor (Union[str, List[str]], optional): color code of the text. Defaults to "k".
         seed (int, optional): seeds order of text allocations. Defaults to 0.
         direction (str, optional): set preferred location of the boxes (south, north, east, west, northeast, northwest, southeast, southwest). Defaults to None.
         avoid_label_lines_overlap (bool, optional): If True, avoids overlap with lines drawn between text labels and locations. Defaults to False.
         plot_kwargs (dict, optional): kwargs for the plt.plot of the lines if draw_lines is True.
         **kwargs (): kwargs for the plt.text() call.
+
+    Returns:
+        result_text_xy (List[Optional[Tuple[float, float]]]): List of resulting (x,y) positions for text labels used in the plt.text call.
+        result_line (List[Union[Optional[Tuple[float, float], Tuple[float, float]]]]): List of resulting (x,y) pairs used in the plt.plot call for drawing lines.
     """
     t0 = time.time()
     fig = ax.get_figure()
     if kwargs.get("transform", None) is None:
         fig.draw_without_rendering()
     else:
         if plot_kwargs is None:
@@ -220,63 +226,78 @@
     if verbose:
         print("Plotting")
     if len(non_overlapping_boxes) == 0:
         if direction is not None:
             print(f"No non overlapping boxes found in direction {direction}")
         else:
             print("No non overlapping boxes found")
-    if draw_lines:
-        for x_coord, y_coord, w, h, s, ind in non_overlapping_boxes:
-            x_near, y_near = find_nearest_point_on_box(
-                x_coord, y_coord, w, h, x[ind], y[ind]
+
+    result_line: List[Optional[Tuple[Tuple[float, float],
+                                     Tuple[float, float]]]] = [None] * len(text_list)
+
+    for x_coord, y_coord, w, h, s, ind in non_overlapping_boxes:
+        x_near, y_near = find_nearest_point_on_box(
+            x_coord, y_coord, w, h, x[ind], y[ind]
+        )
+        if x_near is not None:
+            x_, y_ = display_to_data(
+                [x_near, x[ind]],
+                [y_near, y[ind]],
+                ax,
+                transform=kwargs.get("transform", None),
             )
-            if x_near is not None:
-                x_, y_ = display_to_data(
-                    [x_near, x[ind]],
-                    [y_near, y[ind]],
-                    ax,
-                    transform=kwargs.get("transform", None),
-                )
+            result_line[ind] = ((x_[0], x_[1]), (y_[0], y_[1]))
+
+    if draw_lines:
+        for line in result_line:
+            if line is not None:
+                x_, y_ = line
                 ax.plot(
                     x_,
                     y_,
                     linewidth=linewidth,
                     c=linecolor[ind],
                     **(plot_kwargs if plot_kwargs is not None else {}),
                 )
+
+    result_text_xy: List[Optional[Tuple[float, float]]] = [None] * len(text_list)
+
     for x_coord, y_coord, w, h, s, ind in non_overlapping_boxes:
         if kwargs.get("ha", None) is not None:
             if kwargs.get("ha") == "center":
                 x_coord += w / 2
             elif kwargs.get("ha") == "right":
                 x_coord += w
         x_coord, y_coord = display_to_data(
             [x_coord], [y_coord], ax, transform=kwargs.get("transform", None)
         )
-        ax.text(
-            x_coord[0], y_coord[0], s, size=textsize[ind], c=textcolor[ind], **kwargs
-        )
+        result_text_xy[ind] = (x_coord[0], y_coord[0])
 
     if draw_all:
         for ind in overlapping_boxes_inds:
             x_coord, y_coord = display_to_data(
                 [x[ind]], [y[ind]], ax, transform=kwargs.get("transform", None)
             )
+            result_text_xy[ind] = (x_coord[0], y_coord[0])
+
+    for ind, xy in enumerate(result_text_xy):
+        if xy is not None:
             ax.text(
-                x_coord[0],
-                y_coord[0],
+                xy[0],
+                xy[1],
                 text_list[ind],
                 size=textsize[ind],
                 c=textcolor[ind],
                 **kwargs,
             )
-
     if verbose:
         print(f"Finished in {time.time()-t0}s")
 
+    return result_text_xy, result_line
+
 
 def allocate_text(
     fig,
     ax,
     x: Union[np.ndarray, List[float]],
     y: Union[np.ndarray, List[float]],
     text_list: List[str],
```

### Comparing `textalloc-1.0.3/src/textalloc/candidates.py` & `textalloc-1.0.4/src/textalloc/candidates.py`

 * *Files identical despite different names*

### Comparing `textalloc-1.0.3/src/textalloc/non_overlapping_boxes.py` & `textalloc-1.0.4/src/textalloc/non_overlapping_boxes.py`

 * *Files identical despite different names*

### Comparing `textalloc-1.0.3/src/textalloc/overlap_functions.py` & `textalloc-1.0.4/src/textalloc/overlap_functions.py`

 * *Files identical despite different names*

### Comparing `textalloc-1.0.3/src/textalloc.egg-info/PKG-INFO` & `textalloc-1.0.4/src/textalloc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textalloc
-Version: 1.0.3
+Version: 1.0.4
 Summary: Efficient Text Allocation in matplotlib using NumPy Broadcasting
 Author-email: Christoffer Kjellson <c.kjellson@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/ckjellson/textalloc
 Project-URL: Bug Tracker, https://github.com/ckjellson/textalloc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -124,14 +124,17 @@
     If set to True, avoids overlap for drawn lines to text labels.
 plot_kwargs: (dict), default None
     kwargs for the plt.plot of the lines if draw_lines is True.
 **kwargs: ()
     kwargs for the plt.text() call.
     If transform is used, it only needs to be provided here, i.e. not also in plot_kwargs.
 ```
+
+The allocate call returns a tuple containing the resulting positions used to plot the text labels and the connecting label lines
+
 # Implementation and speed
 
 The implementation aims to plot as many text-boxes as possible in the free space in the plot. There are three main steps of the algorithm:
 
 For each textbox to be plotted:
 1. Generate a large number of candidate boxes near the original point with size that matches the fontsize.
 2. Find the candidates that do not overlap any points, lines, plot boundaries, or already allocated boxes.
```

