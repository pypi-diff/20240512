# Comparing `tmp/matsubplots-1.1.1.tar.gz` & `tmp/matsubplots-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matsubplots-1.1.1.tar", last modified: Fri May  3 21:14:24 2024, max compression
+gzip compressed data, was "matsubplots-1.2.0.tar", last modified: Sun May 12 01:12:05 2024, max compression
```

## Comparing `matsubplots-1.1.1.tar` & `matsubplots-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 21:14:24.155451 matsubplots-1.1.1/
--rw-rw-rw-   0        0        0     1089 2024-05-03 21:13:27.000000 matsubplots-1.1.1/LICENSE.md
--rw-rw-rw-   0        0        0     1274 2024-05-03 21:14:24.154410 matsubplots-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      786 2024-05-03 21:13:27.000000 matsubplots-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 21:14:24.111680 matsubplots-1.1.1/matsubplots/
--rw-rw-rw-   0        0        0      166 2024-05-03 21:13:27.000000 matsubplots-1.1.1/matsubplots/__init__.py
--rw-rw-rw-   0        0        0     5268 2024-05-03 21:13:27.000000 matsubplots-1.1.1/matsubplots/matsubplots.py
--rw-rw-rw-   0        0        0       23 2024-05-03 21:13:27.000000 matsubplots-1.1.1/matsubplots/version.py
--rw-rw-rw-   0        0        0     8575 2024-05-03 21:13:27.000000 matsubplots-1.1.1/matsubplots/viewers.py
-drwxrwxrwx   0        0        0        0 2024-05-03 21:14:24.151433 matsubplots-1.1.1/matsubplots.egg-info/
--rw-rw-rw-   0        0        0     1274 2024-05-03 21:14:23.000000 matsubplots-1.1.1/matsubplots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-05-03 21:14:24.000000 matsubplots-1.1.1/matsubplots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 21:14:23.000000 matsubplots-1.1.1/matsubplots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-03 21:14:23.000000 matsubplots-1.1.1/matsubplots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-03 21:14:23.000000 matsubplots-1.1.1/matsubplots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      312 2024-05-03 21:14:24.158450 matsubplots-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-05-03 21:13:27.000000 matsubplots-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 01:12:05.730215 matsubplots-1.2.0/
+-rw-rw-rw-   0        0        0     1089 2024-05-12 01:10:31.000000 matsubplots-1.2.0/LICENSE.md
+-rw-rw-rw-   0        0        0     1274 2024-05-12 01:12:05.728212 matsubplots-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      786 2024-05-12 01:10:31.000000 matsubplots-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 01:12:05.682201 matsubplots-1.2.0/matsubplots/
+-rw-rw-rw-   0        0        0      166 2024-05-12 01:10:31.000000 matsubplots-1.2.0/matsubplots/__init__.py
+-rw-rw-rw-   0        0        0     5268 2024-05-12 01:10:31.000000 matsubplots-1.2.0/matsubplots/matsubplots.py
+-rw-rw-rw-   0        0        0       23 2024-05-12 01:10:31.000000 matsubplots-1.2.0/matsubplots/version.py
+-rw-rw-rw-   0        0        0     9005 2024-05-12 01:10:31.000000 matsubplots-1.2.0/matsubplots/viewers.py
+drwxrwxrwx   0        0        0        0 2024-05-12 01:12:05.725186 matsubplots-1.2.0/matsubplots.egg-info/
+-rw-rw-rw-   0        0        0     1274 2024-05-12 01:12:05.000000 matsubplots-1.2.0/matsubplots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-12 01:12:05.000000 matsubplots-1.2.0/matsubplots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 01:12:05.000000 matsubplots-1.2.0/matsubplots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-12 01:12:05.000000 matsubplots-1.2.0/matsubplots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-12 01:12:05.000000 matsubplots-1.2.0/matsubplots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      312 2024-05-12 01:12:05.733899 matsubplots-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-12 01:10:31.000000 matsubplots-1.2.0/setup.py
```

### Comparing `matsubplots-1.1.1/LICENSE.md` & `matsubplots-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matsubplots-1.1.1/PKG-INFO` & `matsubplots-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matsubplots
-Version: 1.1.1
+Version: 1.2.0
 Summary: Better subplots for matplotlib.
 Home-page: https://auneri.github.io/matsubplots
 Author: Ali Uneri
 License: MIT
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `matsubplots-1.1.1/README.md` & `matsubplots-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `matsubplots-1.1.1/matsubplots/matsubplots.py` & `matsubplots-1.2.0/matsubplots/matsubplots.py`

 * *Files identical despite different names*

### Comparing `matsubplots-1.1.1/matsubplots/viewers.py` & `matsubplots-1.2.0/matsubplots/viewers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,85 @@
 import numpy as np
 from matplotlib.backend_bases import MouseButton
 
 
-def orthoview(axs, image, spacing=(1,1,1), xyz=None, ijk=None, slab_thickness=None, slab_func=np.mean, reposition=True, backend=None, **kwargs):
-    axs = np.asarray(axs)
-    image = np.asarray(image)
-    spacing = np.asarray(spacing)
-    if not (axs.size == image.ndim == spacing.size == 3):
-        raise ValueError('Expected a 3D image, 3 axes, and 3 values for spacing')
-    if ijk is not None and xyz is not None:
-        raise ValueError('Cannot specify ijk and xyz at the same time')
-    bounds = []
-    cbounds = []
-    for i, ax in enumerate(axs.ravel()):
-        if xyz is not None:
-            j = round(xyz[::-1][i] / spacing[::-1][i] + (image.shape[i] - 1) / 2)
-        elif ijk is not None:
-            j = ijk[i]
-        else:
+def orthoview(*args, backend=None, **kwargs):
+    if backend is None:
+        return OrthoView(*args, **kwargs)
+    elif backend.lower() == 'interactive':
+        return OrthoViewInteractive(*args, **kwargs)
+    elif backend.lower() == 'static':
+        return OrthoViewStatic(*args, **kwargs)
+
+
+class OrthoView:
+
+    alignments = (0, 0), (0, 1), (1, 1)
+    colors = '#ff0000', '#00ff00', '#ffff00'
+    indices = (1, 2), (0, 2), (0, 1)
+
+    def __init__(self, axs, image, spacing=(1,1,1), slab_thickness=None, slab_func=np.mean, reposition=True, **kwargs):
+        axs = np.asarray(axs)
+        image = np.asarray(image)
+        spacing = np.asarray(spacing)
+        if not (axs.size == image.ndim == spacing.size == 3):
+            raise ValueError('Expected a 3D image, 3 axes, and 3 values for spacing')
+        bounds = []
+        for i, ax in enumerate(axs.ravel()):
             j = image.shape[i] // 2
-        thickness = 1 if slab_thickness is None else round(slab_thickness / spacing[i])
-        j0 = np.maximum(j - thickness // 2, 0)
-        j1 = j - (-thickness // 2)
-        slice_ = slab_func(np.rollaxis(image, i)[j0:j1], axis=0)
-        aspect = np.divide(*spacing[::-1][np.arange(spacing.size) != i])
-        bounds.append([])
-        bounds[-1].append(ax.get_position().bounds)
-        im = ax.imshow(slice_, aspect=aspect, **kwargs)
-        bounds[-1].append(ax.get_position().bounds)
-        if hasattr(ax, 'cax'):
-            ax.get_figure().colorbar(im, cax=ax.cax)
-            cbounds.append(ax.cax.get_position().bounds)
-    if reposition:
+            thickness = 1 if slab_thickness is None else round(slab_thickness / spacing[i])
+            j0 = np.maximum(j - thickness // 2, 0)
+            j1 = j - (-thickness // 2)
+            slice_ = slab_func(np.rollaxis(image, i)[j0:j1], axis=0)
+            aspect = np.divide(*spacing[::-1][np.arange(spacing.size) != i])
+            bounds.append([])
+            bounds[-1].append(ax.get_position().bounds)
+            im = ax.imshow(slice_, aspect=aspect, **kwargs)
+            bounds[-1].append(ax.get_position().bounds)
+            if hasattr(ax, 'cax'):
+                ax.get_figure().colorbar(im, cax=ax.cax)
+        crosshairs = [[
+            axs[i].axhline(image.shape[x]//2, lw=1, c=self.colors[x], visible=False),
+            axs[i].axvline(image.shape[y]//2, lw=1, c=self.colors[y], visible=False)]
+            for i, (x,y) in enumerate(self.indices)]
+        self.axs = axs
+        self.image = image
+        self.spacing = spacing
+        self._crosshairs = crosshairs
+        if reposition:
+            self._reposition(axs, bounds)
+
+    def crosshairs(self, toggle=None):
+        if toggle is None:
+            toggle = not self._crosshairs[0][0].get_visible()
+        default_color = self.axs[0].get_xaxis().get_label().get_color()
+        for i, crosshairs in enumerate(self._crosshairs):
+            for line in crosshairs:
+                line.set_visible(toggle)
+            for spine in self.axs[i].spines.values():
+                spine.set_edgecolor(self.colors[i] if toggle else default_color)
+
+    def ijk(self, i, j, k, crosshairs=None):
+        for index, value in enumerate((i, j, k)):
+            self._scroll(index, value)
+        if crosshairs is not None:
+            self.crosshairs(crosshairs)
+
+    def xyz(self, x, y, z, crosshairs=None):
+        xyz = x, y, z
+        ijk = [round(xyz[::-1][i] / self.spacing[::-1][i] + (self.image.shape[i] - 1) / 2) for i in range(3)]
+        self.ijk(*ijk, crosshairs=crosshairs)
+
+    def _scroll(self, index, value):
+        self.axs[index].images[0].set_data(np.rollaxis(self.image, index)[value])
+        for i, alignment in zip(self.indices[index], self.alignments[index]):
+            getattr(self._crosshairs[i][alignment], 'set_ydata' if alignment == 0 else 'set_xdata')([value, value])
+
+    @staticmethod
+    def _reposition(axs, bounds):
         _, _, w00, _ = bounds[0][0]
         l01, b01, w01, h01 = bounds[0][1]
         l0, b0, w0, h0 = l01, b01, w01, h01
         _, _, w10, _ = bounds[1][0]
         l11, b11, w11, h11 = bounds[1][1]
         l1, b1, w1, h1 = l11, b11, w11, h11
         _, _, w20, _ = bounds[2][0]
@@ -60,54 +104,19 @@
         w2 *= h1 / h2
         h2 = h1
         b2 = b1
         lshift += (w20 - w21) / 2
         axs[2].set_position((l2 - lshift, b2, w2, h2))
         lshift += (w20 - w21) / 2
         lshift += w21 - w2
-        if cbounds:
-            cl, cb, cw, ch = cbounds[2]
+        if hasattr(axs[-1], 'cax'):
+            cl, cb, cw, ch = axs[-1].cax.get_position().bounds
             ch2 = max(h0, h1, h2)
             cb2 = cb + (ch - ch2) / 2
-            ax.cax.set_position((cl - lshift, cb2, cw, ch2))
-    if backend is None:
-        pass
-    elif backend.lower() == 'interactive':
-        return OrthoViewInteractive(axs, image)
-    elif backend.lower() == 'static':
-        return OrthoViewStatic(axs, image)
-    else:
-        raise NotImplementedError(backend)
-
-
-class OrthoView:
-
-    alignments = (0, 0), (0, 1), (1, 1)
-    colors = '#ff0000', '#00ff00', '#ffff00'
-    indices = (1, 2), (0, 2), (0, 1)
-
-    def __init__(self, axs, image):
-        self.axs = axs
-        self.image = image
-        self.crosshairs = [[
-            axs[i].axhline(image.shape[x]//2, lw=1, c=self.colors[x]),
-            axs[i].axvline(image.shape[y]//2, lw=1, c=self.colors[y])]
-            for i, (x,y) in enumerate(self.indices)]
-        for x in self.crosshairs:
-            for y in x:
-                y.set_visible(False)
-
-    def scroll(self, i, j, k):
-        for index, value in enumerate((i, j, k)):
-            self.scrolli(index, value)
-
-    def scrolli(self, index, value):
-        self.axs[index].images[0].set_data(np.rollaxis(self.image, index)[value])
-        for i, alignment in zip(self.indices[index], self.alignments[index]):
-            getattr(self.crosshairs[i][alignment], 'set_ydata' if alignment == 0 else 'set_xdata')([value, value])
+            axs[-1].cax.set_position((cl - lshift, cb2, cw, ch2))
 
 
 class OrthoViewInteractive(OrthoView):
 
     def __init__(self, axs, *args, **kwargs):
         super().__init__(axs, *args, **kwargs)
         self.pressed = [None, None]
@@ -124,31 +133,29 @@
 
     def _ipython_display_(self):
         self.axs[0].get_figure().show()
 
     def on_press(self, event):
         if event.inaxes in self.axs:
             if event.dblclick:
-                for x in self.crosshairs:
-                    for y in x:
-                        y.set_visible(not y.get_visible())
+                self.crosshairs()
             elif event.button == MouseButton.LEFT:
                 self.pressed[0] = event
             elif event.button == MouseButton.RIGHT:
                 self.pressed[1] = event
         self.on_motion(event)
 
     def on_release(self, _):
         self.pressed[:] = None, None
 
     def on_motion(self, event):
         for i, ax in enumerate(self.axs):
             if self.pressed[0] is not None and event.inaxes is ax:
                 for j, index in enumerate(self.indices[i]):
-                    self.scrolli(index, round(getattr(event, 'ydata' if j == 0 else 'xdata')))
+                    self._scroll(index, round(getattr(event, 'ydata' if j == 0 else 'xdata')))
             elif self.pressed[1] is not None and event.inaxes is ax:
                 vmin, vmax = self.axs[0].images[0].get_clim()
                 win = vmax - vmin
                 lvl = vmin + (win / 2)
                 win += 0.1 * (event.x - self.pressed[1].x) / self.axs[0].images[0].get_size()[0]
                 lvl += 0.1 * (event.y - self.pressed[1].y) / self.axs[0].images[0].get_size()[1]
                 vmin = lvl - (win / 2)
@@ -166,30 +173,28 @@
             import ipywidgets
             from IPython.display import display
         except ModuleNotFoundError as exception:
             raise RuntimeError('ipywidgets is required to provide interactivity with static matplotlib backends') from exception
         super().__init__(axs, image, *args, **kwargs)
         self.wslices = [ipywidgets.IntSlider(description=x, value=image.shape[i]//2, min=0, max=image.shape[i]-1) for i, x in enumerate('ijk')]
         self.wclim = ipywidgets.FloatRangeSlider(description='clim', value=axs[0].images[0].get_clim(), min=np.min(image), max=np.max(image))
-        self.wcrosshairs = ipywidgets.Checkbox(description='crosshairs', value=self.crosshairs[0][0].get_visible())
+        self.wcrosshairs = ipywidgets.Checkbox(description='crosshairs', value=self._crosshairs[0][0].get_visible())
         self.woutput = ipywidgets.Output()
         with self.woutput:
             display(axs[0].get_figure())
 
         @self.woutput.capture(clear_output=True, wait=True)
         def update(change):
             if change['owner'] is self.wclim:
                 for ax in axs:
                     ax.images[0].set_clim(change['new'])
             elif change['owner'] is self.wcrosshairs:
-                for x in self.crosshairs:
-                    for y in x:
-                        y.set_visible(change['new'])
+                self.crosshairs(change['new'])
             elif change['owner'] in self.wslices:
-                self.scrolli(self.wslices.index(change['owner']), change['new'])
+                self._scroll(self.wslices.index(change['owner']), change['new'])
             display(axs[0].get_figure())
 
         for widget in self.wslices + [self.wclim, self.wcrosshairs]:
             widget.observe(update, names='value')
 
     def _ipython_display_(self):
         from IPython.display import display
```

### Comparing `matsubplots-1.1.1/matsubplots.egg-info/PKG-INFO` & `matsubplots-1.2.0/matsubplots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matsubplots
-Version: 1.1.1
+Version: 1.2.0
 Summary: Better subplots for matplotlib.
 Home-page: https://auneri.github.io/matsubplots
 Author: Ali Uneri
 License: MIT
 Classifier: Framework :: Matplotlib
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `matsubplots-1.1.1/setup.py` & `matsubplots-1.2.0/setup.py`

 * *Files identical despite different names*

