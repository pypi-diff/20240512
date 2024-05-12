# Comparing `tmp/networkx_viewer-0.3.0.tar.gz` & `tmp/networkx_viewer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\networkx_viewer-0.3.0.tar", last modified: Sat Aug 29 23:24:14 2020, max compression
+gzip compressed data, was "networkx_viewer-0.3.1.tar", last modified: Sun May 12 18:58:15 2024, max compression
```

## Comparing `networkx_viewer-0.3.0.tar` & `networkx_viewer-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2020-08-29 23:24:14.000000 networkx_viewer-0.3.0/
--rw-rw-rw-   0        0        0     1809 2020-08-29 23:24:14.000000 networkx_viewer-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     9006 2020-08-29 23:10:43.000000 networkx_viewer-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2020-08-29 23:24:14.000000 networkx_viewer-0.3.0/networkx_viewer/
--rw-rw-rw-   0        0        0      292 2020-08-29 23:10:43.000000 networkx_viewer-0.3.0/networkx_viewer/__init__.py
--rw-rw-rw-   0        0        0     4546 2020-08-29 20:17:44.000000 networkx_viewer-0.3.0/networkx_viewer/autocomplete_entry.py
--rw-rw-rw-   0        0        0    46559 2020-08-29 23:10:43.000000 networkx_viewer-0.3.0/networkx_viewer/graph_canvas.py
--rw-rw-rw-   0        0        0    19621 2020-08-29 23:10:43.000000 networkx_viewer-0.3.0/networkx_viewer/tests.py
--rw-rw-rw-   0        0        0    10774 2020-08-29 20:17:44.000000 networkx_viewer-0.3.0/networkx_viewer/tokens.py
--rw-rw-rw-   0        0        0    17591 2020-08-29 23:10:43.000000 networkx_viewer-0.3.0/networkx_viewer/viewer.py
-drwxrwxrwx   0        0        0        0 2020-08-29 23:24:14.000000 networkx_viewer-0.3.0/networkx_viewer.egg-info/
--rw-rw-rw-   0        0        0     1809 2020-08-29 23:24:13.000000 networkx_viewer-0.3.0/networkx_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2020-08-29 23:24:13.000000 networkx_viewer-0.3.0/networkx_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-08-29 23:24:13.000000 networkx_viewer-0.3.0/networkx_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-08-29 23:13:46.000000 networkx_viewer-0.3.0/networkx_viewer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2020-08-29 23:24:13.000000 networkx_viewer-0.3.0/networkx_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2020-08-29 23:24:13.000000 networkx_viewer-0.3.0/networkx_viewer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-08-29 23:24:14.000000 networkx_viewer-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2553 2020-08-29 23:10:43.000000 networkx_viewer-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:58:15.934460 networkx_viewer-0.3.1/
+-rw-rw-rw-   0        0        0    35147 2014-07-05 12:18:16.000000 networkx_viewer-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1643 2024-05-12 18:58:15.934460 networkx_viewer-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9000 2024-05-12 18:30:51.000000 networkx_viewer-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 18:58:15.914455 networkx_viewer-0.3.1/networkx_viewer/
+-rw-rw-rw-   0        0        0      292 2024-05-12 18:57:25.000000 networkx_viewer-0.3.1/networkx_viewer/__init__.py
+-rw-rw-rw-   0        0        0     4546 2014-12-12 02:23:31.000000 networkx_viewer-0.3.1/networkx_viewer/autocomplete_entry.py
+-rw-rw-rw-   0        0        0    46580 2024-05-12 18:39:59.000000 networkx_viewer-0.3.1/networkx_viewer/graph_canvas.py
+-rw-rw-rw-   0        0        0    19627 2024-05-12 18:45:35.000000 networkx_viewer-0.3.1/networkx_viewer/tests.py
+-rw-rw-rw-   0        0        0    10774 2015-08-02 14:04:17.000000 networkx_viewer-0.3.1/networkx_viewer/tokens.py
+-rw-rw-rw-   0        0        0    17591 2024-05-12 18:30:51.000000 networkx_viewer-0.3.1/networkx_viewer/viewer.py
+drwxrwxrwx   0        0        0        0 2024-05-12 18:58:15.933461 networkx_viewer-0.3.1/networkx_viewer.egg-info/
+-rw-rw-rw-   0        0        0     1643 2024-05-12 18:58:15.000000 networkx_viewer-0.3.1/networkx_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-05-12 18:58:15.000000 networkx_viewer-0.3.1/networkx_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 18:58:15.000000 networkx_viewer-0.3.1/networkx_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-12 18:58:15.000000 networkx_viewer-0.3.1/networkx_viewer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-05-12 18:58:15.000000 networkx_viewer-0.3.1/networkx_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-12 18:58:15.000000 networkx_viewer-0.3.1/networkx_viewer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 18:58:15.934460 networkx_viewer-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2659 2024-05-12 18:30:51.000000 networkx_viewer-0.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `networkx_viewer-0.3.0/PKG-INFO` & `networkx_viewer-0.3.1/networkx_viewer.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 1.2
-Name: networkx_viewer
-Version: 0.3.0
+Metadata-Version: 2.1
+Name: networkx-viewer
+Version: 0.3.1
 Summary: Interactive viewer for networkx graphs.
 Home-page: http://github.com/jsexauer/networkx_viewer
 Author: Jason Sexauer
 Author-email: genericcarbonlifeform@gmail.com
 License: LICENSE.txt
-Description: 
-        NetworkX Viewer provides a basic interactive GUI to view
-        `networkx <https://networkx.github.io/>`_ graphs.  In addition to standard
-        plotting and layout features as found natively in networkx, the GUI allows
-        you to:
-        
-          - Drag nodes around to tune the default layout
-          - Show and hide nodes
-          - Filter nodes
-          - Pan and zoom
-          - Display nodes only within a certain number of hops ("levels") of
-            a "home node"
-          - Display and highlight the shortest path between two nodes.  Nodes
-            around the path can also be displayed within a settable number of
-            levels
-          - Intelligently find and display nodes near displayed nodes using
-            "Grow" and "Grow Until" functions
-          - Use attributes stored in the graph's node and edge dictionaries to
-            customize the appearance of the node and edge tokens in the GUI
-          - Mark nodes and edges for reference
-          - Support for both `nx.Graph` and `nx.MultiGraph`
-        
-        See https://github.com/jsexauer/networkx_viewer for more details
-        
 Keywords: networkx,topology,graph theory
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >3.5
+License-File: LICENSE.txt
+
+
+NetworkX Viewer provides a basic interactive GUI to view
+`networkx <https://networkx.github.io/>`_ graphs.  In addition to standard
+plotting and layout features as found natively in networkx, the GUI allows
+you to:
+
+  - Drag nodes around to tune the default layout
+  - Show and hide nodes
+  - Filter nodes
+  - Pan and zoom
+  - Display nodes only within a certain number of hops ("levels") of
+    a "home node"
+  - Display and highlight the shortest path between two nodes.  Nodes
+    around the path can also be displayed within a settable number of
+    levels
+  - Intelligently find and display nodes near displayed nodes using
+    "Grow" and "Grow Until" functions
+  - Use attributes stored in the graph's node and edge dictionaries to
+    customize the appearance of the node and edge tokens in the GUI
+  - Mark nodes and edges for reference
+  - Support for both `nx.Graph` and `nx.MultiGraph`
+
+See https://github.com/jsexauer/networkx_viewer for more details
+
+
```

### Comparing `networkx_viewer-0.3.0/README.md` & `networkx_viewer-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 app = ExampleApp(G)
 app.mainloop()
 
 ```
 
 Development Status
 ==================
-As of August 2020, networkx_viewer is under considered feature complete.  No
+As of August 2020, networkx_viewer is considered feature complete.  No
   additional development is expected. Bugs or feature
 requests should be submitted to the
 [github issue tracker](https://github.com/jsexauer/networkx_viewer/issues).
 
 Many thanks to [Faith Eser](https://github.com/afeser) for doing the majority of the 
 development work to make this library work with networkx version 2.2+.
```

### Comparing `networkx_viewer-0.3.0/networkx_viewer/autocomplete_entry.py` & `networkx_viewer-0.3.1/networkx_viewer/autocomplete_entry.py`

 * *Files identical despite different names*

### Comparing `networkx_viewer-0.3.0/networkx_viewer/graph_canvas.py` & `networkx_viewer-0.3.1/networkx_viewer/graph_canvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1102,15 +1102,15 @@
             dom_size = 1.0
 
         if len(G)==0:
             return {}
         if len(G)==1:
             return {G.nodes()[0]:(1,)*dim}
 
-        A=nx.to_numpy_matrix(G)
+        A=nx.adjacency_matrix(G).todense()
         nnodes,_ = A.shape
         # I've found you want to occupy about a two-thirds of the window size
         if fixed is not None:
             k=(min(self.winfo_width(), self.winfo_height())*.66)/np.sqrt(nnodes)
         else:
             k = None
 
@@ -1159,18 +1159,18 @@
             raise nx.NetworkXError(
                 "fruchterman_reingold() takes an adjacency matrix as input")
 
         A=np.asarray(A) # make sure we have an array instead of a matrix
 
         if pos is None:
             # random initial positions
-            pos=np.asarray(np.random.random((nnodes,dim)),dtype=A.dtype)
+            pos=np.asarray(np.random.random((nnodes,dim)),dtype='float64')
         else:
             # make sure positions are of same type as matrix
-            pos=pos.astype(A.dtype)
+            pos=pos.astype('float64')
 
         # optimal distance between nodes
         if k is None:
             k=np.sqrt(1.0/nnodes)
         # the initial "temperature"  is about .1 of domain area (=1x1)
         # this is the largest step allowed in the dynamics.
         # Modified to actually detect for domain area
@@ -1197,14 +1197,15 @@
             # update positions
             length=np.sqrt((displacement**2).sum(axis=1))
             length=np.where(length<0.01,0.1,length)
             delta_pos=np.transpose(np.transpose(displacement)*t/length)
             if fixed is not None:
                 # don't change positions of fixed nodes
                 delta_pos[fixed]=0.0
+
             pos+=delta_pos
             # cool temperature
             t-=dt
             ###pos=_rescale_layout(pos)
         return pos
 
 class NodeFiltered(Exception):
@@ -1213,12 +1214,12 @@
 def flatten(l):
     try:
         bs = basestring
     except NameError:
         # Py3k
         bs = str
     for el in l:
-        if isinstance(el, collections.Iterable) and not isinstance(el, bs):
+        if isinstance(el, collections.abc.Iterable) and not isinstance(el, bs):
             for sub in flatten(el):
                 yield sub
         else:
             yield el
```

### Comparing `networkx_viewer-0.3.0/networkx_viewer/tests.py` & `networkx_viewer-0.3.1/networkx_viewer/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,15 +452,15 @@
     def test_node_passthrough(self):
         node = self.a._find_disp_node('a')
         token = self.a.dispG.nodes[node]['token']
         cfg = token.itemconfig(token.marker)
 
         self.assertEqual(cfg['fill'][-1], 'white')
         chk = (cfg['dash'][-1] == ('2','2')) or (cfg['dash'][-1] == ('2 2'))
-        self.assert_(chk)
+        self.assertTrue(chk)
 
     def test_node_label_passthrough(self):
         node = self.a._find_disp_node(2)
         token = self.a.dispG.nodes[node]['token']
         cfg = token.itemconfig(token.label)
 
         self.assertEqual(cfg['fill'][-1], 'blue')
@@ -473,15 +473,15 @@
 
         # Test edge a-c
         token = self.a.dispG.get_edge_data(a, c, 0)['token']
         token_id = token.id
         cfg = self.a.itemconfig(token_id)
 
         chk = (cfg['dash'][-1] == ('2','2')) or (cfg['dash'][-1] == ('2 2'))
-        self.assert_(chk)
+        self.assertTrue(chk)
 
         # Test edge out-c
         token = self.a.dispG.get_edge_data(out, c, 0)['token']
         token_id = token.id
         cfg = self.a.itemconfig(token_id)
 
         self.assertEqual(cfg['fill'][-1], 'red')
```

### Comparing `networkx_viewer-0.3.0/networkx_viewer/tokens.py` & `networkx_viewer-0.3.1/networkx_viewer/tokens.py`

 * *Files identical despite different names*

### Comparing `networkx_viewer-0.3.0/networkx_viewer/viewer.py` & `networkx_viewer-0.3.1/networkx_viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `networkx_viewer-0.3.0/networkx_viewer.egg-info/PKG-INFO` & `networkx_viewer-0.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-Metadata-Version: 1.2
-Name: networkx-viewer
-Version: 0.3.0
+Metadata-Version: 2.1
+Name: networkx_viewer
+Version: 0.3.1
 Summary: Interactive viewer for networkx graphs.
 Home-page: http://github.com/jsexauer/networkx_viewer
 Author: Jason Sexauer
 Author-email: genericcarbonlifeform@gmail.com
 License: LICENSE.txt
-Description: 
-        NetworkX Viewer provides a basic interactive GUI to view
-        `networkx <https://networkx.github.io/>`_ graphs.  In addition to standard
-        plotting and layout features as found natively in networkx, the GUI allows
-        you to:
-        
-          - Drag nodes around to tune the default layout
-          - Show and hide nodes
-          - Filter nodes
-          - Pan and zoom
-          - Display nodes only within a certain number of hops ("levels") of
-            a "home node"
-          - Display and highlight the shortest path between two nodes.  Nodes
-            around the path can also be displayed within a settable number of
-            levels
-          - Intelligently find and display nodes near displayed nodes using
-            "Grow" and "Grow Until" functions
-          - Use attributes stored in the graph's node and edge dictionaries to
-            customize the appearance of the node and edge tokens in the GUI
-          - Mark nodes and edges for reference
-          - Support for both `nx.Graph` and `nx.MultiGraph`
-        
-        See https://github.com/jsexauer/networkx_viewer for more details
-        
 Keywords: networkx,topology,graph theory
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >3.5
+License-File: LICENSE.txt
+
+
+NetworkX Viewer provides a basic interactive GUI to view
+`networkx <https://networkx.github.io/>`_ graphs.  In addition to standard
+plotting and layout features as found natively in networkx, the GUI allows
+you to:
+
+  - Drag nodes around to tune the default layout
+  - Show and hide nodes
+  - Filter nodes
+  - Pan and zoom
+  - Display nodes only within a certain number of hops ("levels") of
+    a "home node"
+  - Display and highlight the shortest path between two nodes.  Nodes
+    around the path can also be displayed within a settable number of
+    levels
+  - Intelligently find and display nodes near displayed nodes using
+    "Grow" and "Grow Until" functions
+  - Use attributes stored in the graph's node and edge dictionaries to
+    customize the appearance of the node and edge tokens in the GUI
+  - Mark nodes and edges for reference
+  - Support for both `nx.Graph` and `nx.MultiGraph`
+
+See https://github.com/jsexauer/networkx_viewer for more details
+
+
```

### Comparing `networkx_viewer-0.3.0/setup.py` & `networkx_viewer-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from setuptools import setup, find_packages
 import sys, os
 
 # python setup.py check
 # python.exe setup.py --long-description | rst2html.py > dummy.html
 
+# To upload to pypi
+#  python setup.py sdist bdist_wheel
+#  python -m twine upload dist/*
+
+# LEGACY:
 # To upload to PyPI test server
 #   http://peterdowns.com/posts/first-time-with-pypi.html
 # python setup.py register -r pypitest
 # python setup.py sdist upload -r pypitest
 # Test repo is at: https://testpypi.python.org/pypi
 
 # To distribute on PyPI:
```

