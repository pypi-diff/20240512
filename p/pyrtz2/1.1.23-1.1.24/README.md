# Comparing `tmp/pyrtz2-1.1.23.tar.gz` & `tmp/pyrtz2-1.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtz2-1.1.23.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyrtz2-1.1.24.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyrtz2-1.1.23.tar` & `pyrtz2-1.1.24.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.23/.gitattributes
--rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.1.23/.gitignore
--rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.23/LICENSE
--rw-r--r--   0        0        0      771 2024-04-19 14:18:48.509303 pyrtz2-1.1.23/README.md
--rw-r--r--   0        0        0   108501 2024-04-12 19:08:16.330771 pyrtz2-1.1.23/example/con050.PNG
--rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.1.23/example/con050/jasYcon050cell37m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.1.23/example/con050/jasYcon050cell37m0001.tif
--rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.1.23/example/con050/jasYcon050cell38m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.1.23/example/con050/jasYcon050cell38m0001.tif
--rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.1.23/example/con050/jasYcon050cell39m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.1.23/example/con050/jasYcon050cell39m0001.tif
--rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.1.23/example/con050/jasYcon050cell40m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.1.23/example/con050/jasYcon050cell40m0001.tif
--rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.1.23/example/con050/jasYcon050cell42m0000.ibw
--rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.1.23/example/con050/jasYcon050cell42m0001.tif
--rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.23/example/con050_cp_annotations.json
--rw-r--r--   0        0        0   216499 2024-04-09 18:08:42.337499 pyrtz2-1.1.23/example/con050_curves.pdf
--rw-r--r--   0        0        0     1245 2024-04-09 18:08:23.807163 pyrtz2-1.1.23/example/con050_fits.csv
--rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.23/example/con050_vd_annotations.json
--rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.1.23/example/test.py
--rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.23/pyproject.toml
--rw-r--r--   0        0        0       62 2024-05-09 16:25:39.043590 pyrtz2-1.1.23/pyrtz2/__init__.py
--rw-r--r--   0        0        0     1874 2024-04-04 20:43:57.261121 pyrtz2-1.1.23/pyrtz2/afm.py
--rw-r--r--   0        0        0      335 2024-04-05 13:06:49.354563 pyrtz2-1.1.23/pyrtz2/app.py
--rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.23/pyrtz2/assets/style.css
--rw-r--r--   0        0        0     5108 2024-05-09 16:24:06.292616 pyrtz2-1.1.23/pyrtz2/asylum.py
--rw-r--r--   0        0        0    17635 2024-05-09 16:12:23.316799 pyrtz2-1.1.23/pyrtz2/curves.py
--rw-r--r--   0        0        0     4451 2024-04-09 18:06:56.894949 pyrtz2-1.1.23/pyrtz2/fit.py
--rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.23/pyrtz2/src/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.23/pyrtz2/src/components/__init__.py
--rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.23/pyrtz2/src/components/annotator.py
--rw-r--r--   0        0        0     5060 2024-04-05 12:35:50.358816 pyrtz2-1.1.23/pyrtz2/src/components/contact_controls.py
--rw-r--r--   0        0        0     4115 2024-04-06 15:49:10.536249 pyrtz2-1.1.23/pyrtz2/src/components/curve_dropdown.py
--rw-r--r--   0        0        0     2826 2024-04-06 15:45:15.625467 pyrtz2-1.1.23/pyrtz2/src/components/fig.py
--rw-r--r--   0        0        0     2874 2024-04-06 15:44:47.448540 pyrtz2-1.1.23/pyrtz2/src/components/fig_frame.py
--rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.23/pyrtz2/src/components/fitter.py
--rw-r--r--   0        0        0     1186 2024-04-06 15:49:10.935231 pyrtz2-1.1.23/pyrtz2/src/components/ids.py
--rw-r--r--   0        0        0     1718 2024-04-08 16:35:01.806773 pyrtz2-1.1.23/pyrtz2/src/components/image_frame.py
--rw-r--r--   0        0        0     1707 2024-04-06 15:49:56.149071 pyrtz2-1.1.23/pyrtz2/src/components/layout.py
--rw-r--r--   0        0        0     3230 2024-04-06 15:49:27.361168 pyrtz2-1.1.23/pyrtz2/src/components/loader.py
--rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.23/pyrtz2/src/components/toolbox.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.23/pyrtz2/src/data/__init__.py
--rw-r--r--   0        0        0     3275 2024-04-06 15:49:11.334196 pyrtz2-1.1.23/pyrtz2/src/data/downloader.py
--rw-r--r--   0        0        0     1560 2024-04-05 12:35:50.388794 pyrtz2-1.1.23/pyrtz2/src/data/experiment_loader.py
--rw-r--r--   0        0        0     1117 2024-04-05 12:35:50.392818 pyrtz2-1.1.23/pyrtz2/src/data/image_loader.py
--rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.23/pyrtz2/src/data/processor.py
--rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.23/pyrtz2/src/utils/__init__.py
--rw-r--r--   0        0        0     2474 2024-04-05 12:35:50.397796 pyrtz2-1.1.23/pyrtz2/src/utils/utils.py
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 pyrtz2-1.1.23/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-04-02 19:47:59.285340 pyrtz2-1.1.24/.gitattributes
+-rw-r--r--   0        0        0       37 2024-04-05 12:35:50.341792 pyrtz2-1.1.24/.gitignore
+-rw-r--r--   0        0        0    33041 2024-04-02 20:07:11.768711 pyrtz2-1.1.24/LICENSE
+-rw-r--r--   0        0        0      771 2024-04-19 14:18:48.509303 pyrtz2-1.1.24/README.md
+-rw-r--r--   0        0        0   108501 2024-04-12 19:08:16.330771 pyrtz2-1.1.24/example/con050.PNG
+-rw-r--r--   0        0        0   442996 2024-03-22 20:48:12.000000 pyrtz2-1.1.24/example/con050/jasYcon050cell37m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:48:22.000000 pyrtz2-1.1.24/example/con050/jasYcon050cell37m0001.tif
+-rw-r--r--   0        0        0   453575 2024-03-22 20:48:52.000000 pyrtz2-1.1.24/example/con050/jasYcon050cell38m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:00.000000 pyrtz2-1.1.24/example/con050/jasYcon050cell38m0001.tif
+-rw-r--r--   0        0        0   458723 2024-03-22 20:49:32.000000 pyrtz2-1.1.24/example/con050/jasYcon050cell39m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:49:38.000000 pyrtz2-1.1.24/example/con050/jasYcon050cell39m0001.tif
+-rw-r--r--   0        0        0   435180 2024-03-22 20:50:14.000000 pyrtz2-1.1.24/example/con050/jasYcon050cell40m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:50:22.000000 pyrtz2-1.1.24/example/con050/jasYcon050cell40m0001.tif
+-rw-r--r--   0        0        0   457660 2024-03-22 20:54:28.000000 pyrtz2-1.1.24/example/con050/jasYcon050cell42m0000.ibw
+-rw-r--r--   0        0        0   922624 2024-03-22 20:54:36.000000 pyrtz2-1.1.24/example/con050/jasYcon050cell42m0001.tif
+-rw-r--r--   0        0        0      196 2024-03-27 20:17:56.223149 pyrtz2-1.1.24/example/con050_cp_annotations.json
+-rw-r--r--   0        0        0   216499 2024-04-09 18:08:42.337499 pyrtz2-1.1.24/example/con050_curves.pdf
+-rw-r--r--   0        0        0     1245 2024-04-09 18:08:23.807163 pyrtz2-1.1.24/example/con050_fits.csv
+-rw-r--r--   0        0        0      205 2024-03-26 23:15:37.330282 pyrtz2-1.1.24/example/con050_vd_annotations.json
+-rw-r--r--   0        0        0       37 2024-04-05 12:53:39.905466 pyrtz2-1.1.24/example/test.py
+-rw-r--r--   0        0        0      794 2024-04-04 21:36:24.676720 pyrtz2-1.1.24/pyproject.toml
+-rw-r--r--   0        0        0       62 2024-05-12 13:43:28.447751 pyrtz2-1.1.24/pyrtz2/__init__.py
+-rw-r--r--   0        0        0     2806 2024-05-12 13:42:55.055288 pyrtz2-1.1.24/pyrtz2/afm.py
+-rw-r--r--   0        0        0      335 2024-04-05 13:06:49.354563 pyrtz2-1.1.24/pyrtz2/app.py
+-rw-r--r--   0        0        0     1320 2024-03-29 18:30:21.132859 pyrtz2-1.1.24/pyrtz2/assets/style.css
+-rw-r--r--   0        0        0     5108 2024-05-09 16:24:06.292616 pyrtz2-1.1.24/pyrtz2/asylum.py
+-rw-r--r--   0        0        0    17635 2024-05-09 16:12:23.316799 pyrtz2-1.1.24/pyrtz2/curves.py
+-rw-r--r--   0        0        0     4451 2024-05-12 13:36:33.665861 pyrtz2-1.1.24/pyrtz2/fit.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:57:24.101285 pyrtz2-1.1.24/pyrtz2/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.24/pyrtz2/src/components/__init__.py
+-rw-r--r--   0        0        0     1982 2024-04-04 23:28:38.697339 pyrtz2-1.1.24/pyrtz2/src/components/annotator.py
+-rw-r--r--   0        0        0     5060 2024-04-05 12:35:50.358816 pyrtz2-1.1.24/pyrtz2/src/components/contact_controls.py
+-rw-r--r--   0        0        0     4115 2024-04-06 15:49:10.536249 pyrtz2-1.1.24/pyrtz2/src/components/curve_dropdown.py
+-rw-r--r--   0        0        0     2826 2024-04-06 15:45:15.625467 pyrtz2-1.1.24/pyrtz2/src/components/fig.py
+-rw-r--r--   0        0        0     2874 2024-04-06 15:44:47.448540 pyrtz2-1.1.24/pyrtz2/src/components/fig_frame.py
+-rw-r--r--   0        0        0     2393 2024-04-04 18:36:08.361121 pyrtz2-1.1.24/pyrtz2/src/components/fitter.py
+-rw-r--r--   0        0        0     1186 2024-04-06 15:49:10.935231 pyrtz2-1.1.24/pyrtz2/src/components/ids.py
+-rw-r--r--   0        0        0     1718 2024-05-11 14:17:25.543113 pyrtz2-1.1.24/pyrtz2/src/components/image_frame.py
+-rw-r--r--   0        0        0     1707 2024-04-06 15:49:56.149071 pyrtz2-1.1.24/pyrtz2/src/components/layout.py
+-rw-r--r--   0        0        0     3230 2024-04-06 15:49:27.361168 pyrtz2-1.1.24/pyrtz2/src/components/loader.py
+-rw-r--r--   0        0        0     1052 2024-04-04 18:50:12.478289 pyrtz2-1.1.24/pyrtz2/src/components/toolbox.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.24/pyrtz2/src/data/__init__.py
+-rw-r--r--   0        0        0     3275 2024-04-06 15:49:11.334196 pyrtz2-1.1.24/pyrtz2/src/data/downloader.py
+-rw-r--r--   0        0        0     1560 2024-04-05 12:35:50.388794 pyrtz2-1.1.24/pyrtz2/src/data/experiment_loader.py
+-rw-r--r--   0        0        0     1117 2024-04-05 12:35:50.392818 pyrtz2-1.1.24/pyrtz2/src/data/image_loader.py
+-rw-r--r--   0        0        0     1218 2024-04-04 21:40:13.246607 pyrtz2-1.1.24/pyrtz2/src/data/processor.py
+-rw-r--r--   0        0        0        0 2024-03-22 19:36:41.923791 pyrtz2-1.1.24/pyrtz2/src/utils/__init__.py
+-rw-r--r--   0        0        0     2474 2024-04-05 12:35:50.397796 pyrtz2-1.1.24/pyrtz2/src/utils/utils.py
+-rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 pyrtz2-1.1.24/PKG-INFO
```

### Comparing `pyrtz2-1.1.23/LICENSE` & `pyrtz2-1.1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/README.md` & `pyrtz2-1.1.24/README.md`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050.PNG` & `pyrtz2-1.1.24/example/con050.PNG`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050/jasYcon050cell37m0000.ibw` & `pyrtz2-1.1.24/example/con050/jasYcon050cell37m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050/jasYcon050cell37m0001.tif` & `pyrtz2-1.1.24/example/con050/jasYcon050cell37m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050/jasYcon050cell38m0000.ibw` & `pyrtz2-1.1.24/example/con050/jasYcon050cell38m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050/jasYcon050cell38m0001.tif` & `pyrtz2-1.1.24/example/con050/jasYcon050cell38m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050/jasYcon050cell39m0000.ibw` & `pyrtz2-1.1.24/example/con050/jasYcon050cell39m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050/jasYcon050cell39m0001.tif` & `pyrtz2-1.1.24/example/con050/jasYcon050cell39m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050/jasYcon050cell40m0000.ibw` & `pyrtz2-1.1.24/example/con050/jasYcon050cell40m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050/jasYcon050cell40m0001.tif` & `pyrtz2-1.1.24/example/con050/jasYcon050cell40m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050/jasYcon050cell42m0000.ibw` & `pyrtz2-1.1.24/example/con050/jasYcon050cell42m0000.ibw`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050/jasYcon050cell42m0001.tif` & `pyrtz2-1.1.24/example/con050/jasYcon050cell42m0001.tif`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050_curves.pdf` & `pyrtz2-1.1.24/example/con050_curves.pdf`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/example/con050_fits.csv` & `pyrtz2-1.1.24/example/con050_fits.csv`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyproject.toml` & `pyrtz2-1.1.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/afm.py` & `pyrtz2-1.1.24/pyrtz2/afm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import copy
+import numpy as np
 import os
 from . import asylum
 
 
 class AFM():
     def __init__(
         self,
@@ -53,7 +54,29 @@
         return keys
 
     def drop_curves_by_num(self, drop_idx: list[int], label: int = 1, fill: int = 2) -> None:
         for idx in drop_idx:
             keys = self.get_key_by_num(idx, label=label, fill=fill)
             for key in keys:
                 self.experiment.remove_curve(key)
+
+    def compile(self, export_path: str) -> None:
+        self.experiment.set_cp_by_annotations()
+        self.experiment.set_vd_by_annotations()
+        self.experiment.remove_unannotated()
+        for idx, curve in enumerate(self.experiment):
+            curve.adjust_to_contact()
+            approach = curve.get_indent()
+            ind = approach['ind'].to_numpy()
+            dwell = curve.get_dwell()
+            t_dwell = dwell['t'].to_numpy()
+            directory = os.path.join(export_path, self.exp_name)
+            if not os.path.exists(directory):
+                os.makedirs(directory, exist_ok=True)
+            file_name = 'key' + str(idx) + '.npz'
+            np.savez(
+                os.path.join(directory, file_name),
+                approach=approach,
+                I=ind[-1],
+                dwell=dwell,
+                L=t_dwell[-1] - t_dwell[0],
+            )
```

### Comparing `pyrtz2-1.1.23/pyrtz2/assets/style.css` & `pyrtz2-1.1.24/pyrtz2/assets/style.css`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/asylum.py` & `pyrtz2-1.1.24/pyrtz2/asylum.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/curves.py` & `pyrtz2-1.1.24/pyrtz2/curves.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/fit.py` & `pyrtz2-1.1.24/pyrtz2/fit.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/annotator.py` & `pyrtz2-1.1.24/pyrtz2/src/components/annotator.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/contact_controls.py` & `pyrtz2-1.1.24/pyrtz2/src/components/contact_controls.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/curve_dropdown.py` & `pyrtz2-1.1.24/pyrtz2/src/components/curve_dropdown.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/fig.py` & `pyrtz2-1.1.24/pyrtz2/src/components/fig.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/fig_frame.py` & `pyrtz2-1.1.24/pyrtz2/src/components/fig_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/fitter.py` & `pyrtz2-1.1.24/pyrtz2/src/components/fitter.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/ids.py` & `pyrtz2-1.1.24/pyrtz2/src/components/ids.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/image_frame.py` & `pyrtz2-1.1.24/pyrtz2/src/components/image_frame.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/layout.py` & `pyrtz2-1.1.24/pyrtz2/src/components/layout.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/loader.py` & `pyrtz2-1.1.24/pyrtz2/src/components/loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/components/toolbox.py` & `pyrtz2-1.1.24/pyrtz2/src/components/toolbox.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/data/downloader.py` & `pyrtz2-1.1.24/pyrtz2/src/data/downloader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/data/experiment_loader.py` & `pyrtz2-1.1.24/pyrtz2/src/data/experiment_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/data/image_loader.py` & `pyrtz2-1.1.24/pyrtz2/src/data/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/data/processor.py` & `pyrtz2-1.1.24/pyrtz2/src/data/processor.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/pyrtz2/src/utils/utils.py` & `pyrtz2-1.1.24/pyrtz2/src/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyrtz2-1.1.23/PKG-INFO` & `pyrtz2-1.1.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtz2
-Version: 1.1.23
+Version: 1.1.24
 Summary: Force spectroscopy in Python
 Author-email: "Hoseyn A. Amiri" <aamirihoseyn@gmail.com>
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: dash
 Requires-Dist: dash-bootstrap-components
```

