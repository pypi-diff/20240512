# Comparing `tmp/subdivision_hole_filler-1.0.1.tar.gz` & `tmp/subdivision_hole_filler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subdivision_hole_filler-1.0.1.tar", last modified: Wed May  8 07:49:48 2024, max compression
+gzip compressed data, was "subdivision_hole_filler-1.0.2.tar", last modified: Sun May 12 11:37:28 2024, max compression
```

## Comparing `subdivision_hole_filler-1.0.1.tar` & `subdivision_hole_filler-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:49:48.542389 subdivision_hole_filler-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:49:48.538389 subdivision_hole_filler-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:49:48.542389 subdivision_hole_filler-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)   200849 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-08 07:49:48.542389 subdivision_hole_filler-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   106308 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/iso.png
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 07:49:48.542389 subdivision_hole_filler-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    52038 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/side.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:49:48.538389 subdivision_hole_filler-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:49:48.542389 subdivision_hole_filler-1.0.1/src/subdivision_hole_filler/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/src/subdivision_hole_filler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 07:49:48.000000 subdivision_hole_filler-1.0.1/src/subdivision_hole_filler/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/src/subdivision_hole_filler/hole_filler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:49:48.542389 subdivision_hole_filler-1.0.1/src/subdivision_hole_filler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-08 07:49:48.000000 subdivision_hole_filler-1.0.1/src/subdivision_hole_filler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-08 07:49:48.000000 subdivision_hole_filler-1.0.1/src/subdivision_hole_filler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 07:49:48.000000 subdivision_hole_filler-1.0.1/src/subdivision_hole_filler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 07:49:48.000000 subdivision_hole_filler-1.0.1/src/subdivision_hole_filler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-08 07:49:48.000000 subdivision_hole_filler-1.0.1/src/subdivision_hole_filler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 07:49:48.542389 subdivision_hole_filler-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-08 07:49:43.000000 subdivision_hole_filler-1.0.1/tests/test_6sided_hole.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.427783 subdivision_hole_filler-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.419783 subdivision_hole_filler-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.423783 subdivision_hole_filler-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   200849 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-12 11:37:28.427783 subdivision_hole_filler-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   106308 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/iso.png
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 11:37:28.427783 subdivision_hole_filler-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    52038 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/side.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.419783 subdivision_hole_filler-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.423783 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler/hole_filler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.423783 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-12 11:37:28.000000 subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 11:37:28.423783 subdivision_hole_filler-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-12 11:37:23.000000 subdivision_hole_filler-1.0.2/tests/test_6sided_hole.py
```

### Comparing `subdivision_hole_filler-1.0.1/.github/workflows/python-package.yml` & `subdivision_hole_filler-1.0.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.1/.github/workflows/python-publish.yml` & `subdivision_hole_filler-1.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.1/.gitignore` & `subdivision_hole_filler-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.1/LICENSE` & `subdivision_hole_filler-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.1/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf` & `subdivision_hole_filler-1.0.2/Levin_2000_Filling N-sided Holes Using Combined Subdivision Schemes.pdf`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.1/PKG-INFO` & `subdivision_hole_filler-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,19 @@
-Metadata-Version: 2.1
-Name: subdivision-hole-filler
-Version: 1.0.1
-Summary: A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison.
-Author-email: HUANG Lihao <huang-lihao@outlook.com>
-Project-URL: Homepage, https://github.com/huang-lihao/subdivision-hole-filler
-Project-URL: Bug Tracker, https://github.com/huang-lihao/subdivision-hole-filler/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-
 # Filler for N-sided holes
 [![GitHub release (with filter)](https://img.shields.io/github/v/release/huang-lihao/subdivision-hole-filler?logo=github)
 ](https://github.com/huang-lihao/subdivision-hole-filler)
 [![Upload Python Package](https://github.com/huang-lihao/subdivision-hole-filler/actions/workflows/python-publish.yml/badge.svg)](https://github.com/huang-lihao/subdivision-hole-filler/actions/workflows/python-publish.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/subdivision-hole-filler?logo=pypi)](https://pypi.org/project/subdivision-hole-filler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/subdivision-hole-filler?logo=PyPI)](https://pypi.org/project/subdivision-hole-filler/)
 [![GitHub License](https://img.shields.io/github/license/huang-lihao/subdivision-hole-filler)](https://github.com/huang-lihao/subdivision-hole-filler/blob/main/LICENSE)
 
 
 A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison.
 
-See [Levin, Adi. “Filling N-sided Holes Using Combined Subdivision Schemes.” (2000).](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=925ab5e9375ae3b3d64fb9870e5d08d7d50141d4)
+See [Levin, Adi. “Filling N-sided Holes Using Combined Subdivision Schemes.” (2000).](https://github.com/huang-lihao/subdivision-hole-filler/blob/main/Levin_2000_Filling%20N-sided%20Holes%20Using%20Combined%20Subdivision%20Schemes.pdf)
 
 
 Install
 ----------------------
 Use PyPI to install [subdivision-hole-filler](https://pypi.org/project/subdivision-hole-filler/):
 ```sh
 pip install subdivision-hole-filler
@@ -66,31 +50,33 @@
 
     bd = Boundary()
     bd.coord = coord # A function of parametric coord `u` in [0.0, 2.0], which defines the coordinate of a point on the boundary 
     bd.deriv = deriv # A function of parametric coord `u` in [0.0, 2.0], which defines the cross boundary derivative of a point on the boundary, poining to the inside
     boundaries[d*2] = bd
 
 for d in range(3):
-    bd = Boundary()
     def coord(u: float, d=d):
         phi = (1.0 - u / 2.0) * np.pi / 2.0
         x = R + r - R * np.cos(phi)
         y = R + r - R * np.sin(phi)
         z = 0
         c = np.zeros(3)
         c[d] = z
         c[(d + 1) % 3] = x
         c[(d + 2) % 3] = y
         return c
-    bd.coord = coord
+    
     def deriv(u: float, d=d):
         vec = np.zeros(3)
         vec[d] = 1
         return np.array(vec)
-    bd.deriv = deriv
+
+    bd = Boundary()
+    bd.coord = coord # A function of parametric coord `u` in [0.0, 2.0], which defines the coordinate of a point on the boundary 
+    bd.deriv = deriv # A function of parametric coord `u` in [0.0, 2.0], which defines the cross boundary derivative of a point on the boundary, poining to the inside
     boundaries[(d + 1) % 3 * 2 + 1] = bd
 
 filler = NsidedHoleFiller(boundaries)
 
 center_point = np.array([r, r, r])
 filler.gen_initial_mesh(center_point)
```

### Comparing `subdivision_hole_filler-1.0.1/README.md` & `subdivision_hole_filler-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,35 @@
+Metadata-Version: 2.1
+Name: subdivision-hole-filler
+Version: 1.0.2
+Summary: A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison.
+Author-email: HUANG Lihao <huang-lihao@outlook.com>
+Project-URL: Homepage, https://github.com/huang-lihao/subdivision-hole-filler
+Project-URL: Bug Tracker, https://github.com/huang-lihao/subdivision-hole-filler/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+
 # Filler for N-sided holes
 [![GitHub release (with filter)](https://img.shields.io/github/v/release/huang-lihao/subdivision-hole-filler?logo=github)
 ](https://github.com/huang-lihao/subdivision-hole-filler)
 [![Upload Python Package](https://github.com/huang-lihao/subdivision-hole-filler/actions/workflows/python-publish.yml/badge.svg)](https://github.com/huang-lihao/subdivision-hole-filler/actions/workflows/python-publish.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/subdivision-hole-filler?logo=pypi)](https://pypi.org/project/subdivision-hole-filler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/subdivision-hole-filler?logo=PyPI)](https://pypi.org/project/subdivision-hole-filler/)
 [![GitHub License](https://img.shields.io/github/license/huang-lihao/subdivision-hole-filler)](https://github.com/huang-lihao/subdivision-hole-filler/blob/main/LICENSE)
 
 
 A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison.
 
-See [Levin, Adi. “Filling N-sided Holes Using Combined Subdivision Schemes.” (2000).](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=925ab5e9375ae3b3d64fb9870e5d08d7d50141d4)
+See [Levin, Adi. “Filling N-sided Holes Using Combined Subdivision Schemes.” (2000).](https://github.com/huang-lihao/subdivision-hole-filler/blob/main/Levin_2000_Filling%20N-sided%20Holes%20Using%20Combined%20Subdivision%20Schemes.pdf)
 
 
 Install
 ----------------------
 Use PyPI to install [subdivision-hole-filler](https://pypi.org/project/subdivision-hole-filler/):
 ```sh
 pip install subdivision-hole-filler
@@ -50,31 +66,33 @@
 
     bd = Boundary()
     bd.coord = coord # A function of parametric coord `u` in [0.0, 2.0], which defines the coordinate of a point on the boundary 
     bd.deriv = deriv # A function of parametric coord `u` in [0.0, 2.0], which defines the cross boundary derivative of a point on the boundary, poining to the inside
     boundaries[d*2] = bd
 
 for d in range(3):
-    bd = Boundary()
     def coord(u: float, d=d):
         phi = (1.0 - u / 2.0) * np.pi / 2.0
         x = R + r - R * np.cos(phi)
         y = R + r - R * np.sin(phi)
         z = 0
         c = np.zeros(3)
         c[d] = z
         c[(d + 1) % 3] = x
         c[(d + 2) % 3] = y
         return c
-    bd.coord = coord
+    
     def deriv(u: float, d=d):
         vec = np.zeros(3)
         vec[d] = 1
         return np.array(vec)
-    bd.deriv = deriv
+
+    bd = Boundary()
+    bd.coord = coord # A function of parametric coord `u` in [0.0, 2.0], which defines the coordinate of a point on the boundary 
+    bd.deriv = deriv # A function of parametric coord `u` in [0.0, 2.0], which defines the cross boundary derivative of a point on the boundary, poining to the inside
     boundaries[(d + 1) % 3 * 2 + 1] = bd
 
 filler = NsidedHoleFiller(boundaries)
 
 center_point = np.array([r, r, r])
 filler.gen_initial_mesh(center_point)
```

### Comparing `subdivision_hole_filler-1.0.1/iso.png` & `subdivision_hole_filler-1.0.2/iso.png`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.1/pyproject.toml` & `subdivision_hole_filler-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.1/side.png` & `subdivision_hole_filler-1.0.2/side.png`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.1/src/subdivision_hole_filler/hole_filler.py` & `subdivision_hole_filler-1.0.2/src/subdivision_hole_filler/hole_filler.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,66 +21,80 @@
 class Point:
     def __init__(self, x, y, z, boundary_u_tuples: list[tuple[Boundary, float]] = []):
         self.coord = np.array([x, y, z])
         self.boundary_u_tuples = boundary_u_tuples
         assert len(boundary_u_tuples) in [0, 1, 2]
         self.neighbours: list[Point] = []
         self.faces: list[Face] = []
+        self.id = -1
+
+        self.parametric_coord_in_sub_face: dict[int, np.ndarray] = {}
 
 
 class Face:
-    def __init__(self, points: list[Point]) -> None:
+    def __init__(self, points: list[Point], sub_face: int) -> None:
         assert len(points) == 4
         self.points = points
         for i in range(4):
             points[i].faces.append(self)
             for d in [-1, +1]:
                 j = (i + d) % 4
                 if points[i] not in points[i].neighbours:
                     points[i].neighbours.append(points[j])
+        self.sub_face = sub_face
+        
     
     def center_point(self) -> Point:
-        return Point(*np.mean([p.coord for p in self.points], axis=0))
+        point = Point(*np.mean([p.coord for p in self.points], axis=0))
+        point.parametric_coord_in_sub_face[self.sub_face] = 0.25 * (
+            self.points[0].parametric_coord_in_sub_face[self.sub_face] +
+            self.points[1].parametric_coord_in_sub_face[self.sub_face] +
+            self.points[2].parametric_coord_in_sub_face[self.sub_face] +
+            self.points[3].parametric_coord_in_sub_face[self.sub_face]
+        )
+        return point
 
 
 def get_edge_tuple(point1: Point, point2: Point, points: list[Point]) -> tuple[Point, Point]:
     idxi = points.index(point1)
     idxj = points.index(point2)
     idx1, idx2 = sorted([idxi, idxj])
     return (points[idx1], points[idx2])
 
 
 class NsidedHoleFiller:
     def __init__(self, boundaries: list[Boundary]) -> None:
         self.boundaries = boundaries
         self.points: list[Point] = []
         self.faces: list[Face] = []
+        self.iteration = 0
     
     def plot_faces(self, output_path: str = None):
         faces = self.faces
         fig, ax = plt.subplots(subplot_kw={"projection": "3d"})
         fig.set_size_inches(5, 5)
         for face in faces:
             coord = [pt.coord for pt in face.points]
             coord = np.array([[coord[0], coord[1]], [coord[3], coord[2]]])
             X = coord[:, :, 0]
             Y = coord[:, :, 1]
             Z = coord[:, :, 2]
-            ax.plot_surface(X,Y,Z)
+            ax.plot_surface(X,Y,Z,color="none", edgecolor="black")
+        ax.scatter([self.center_point[0]], [self.center_point[1]], [self.center_point[2]])
         plt.axis('equal')
         ax.set_proj_type('ortho')
         ax.view_init(elev=np.arctan(np.sqrt(0.5))/np.pi*180, azim=45)
         ax.view_init(elev=0, azim=0)
         if output_path is not None:
             plt.tight_layout()
             plt.savefig(output_path)
         else:
             plt.show()
 
-    def gen_initial_mesh(self, center_point: np.ndarray) -> None:
+    def gen_initial_mesh(self, center_point_coord: np.ndarray) -> None:
         r"""
         Generate the initial mesh as in Levin 1999 paper.
 
         .. code-block:: python
 
                       *------+------*
                      /       |       \
@@ -102,16 +116,16 @@
                            \   /
                             \ /
                              *
 
         Args:
             boundaries (list[Boundary]):
                 Boundaries having exact coordinates and tangential direction
-            center_point (np.ndarray):
-                The center point to generate the initial mesh
+            center_point_coord (np.ndarray):
+                The center point coordinates to generate the initial mesh
         """
         boundaries = self.boundaries
         num = len(boundaries)
 
         # check adjacent boundaries are linked together
         for i in range(num):
             j = (i + 1) % num
@@ -122,34 +136,44 @@
         points: list[Point] = []
         faces: list[Face] = []
         for i, boundary in enumerate(boundaries):
             l = (i - 1) % num
             left_boundary = boundaries[l]
             points.append(Point(*boundary.coord(0.0), [(left_boundary, 2.0), (boundary, 0.0)]))
             points.append(Point(*boundary.coord(1.0), [(boundary, 1.0)]))
-        points.append(Point(*center_point))
+        points.append(Point(*center_point_coord))
         center_point = points[-1]
+        self.center_point = center_point
 
         for i in range(num):
-            faces.append(Face([
+            vertices = [
                 points[2 * i],
                 points[(2 * i + 1) % (2* num)],
                 center_point,
                 points[(2 * i -1) % (2 * num)]
-            ]))
+            ]
+            vertices[0].parametric_coord_in_sub_face[i] = np.array([0.0, 0.0])
+            vertices[1].parametric_coord_in_sub_face[i] = np.array([1.0, 0.0])
+            vertices[2].parametric_coord_in_sub_face[i] = np.array([1.0, 1.0])
+            vertices[3].parametric_coord_in_sub_face[i] = np.array([0.0, 1.0])
+            faces.append(Face(
+                points=vertices,
+                sub_face=i
+            ))
         self.points = points
         self.faces = faces
     
     def clear_points(self, points: list[Point] = None):
         if points is None: points = self.points
         for point in points:
             point.neighbours = []
             point.faces = []
 
     def cmc_subdiv_for_1step(self, iteration: int) -> None:
+        assert iteration == self.iteration
         step = 2**(-iteration)
         points = self.points
         faces = self.faces
         new_faces: list[Face] = []
         new_points: list[Point] = []
         new_points.extend(points)
         for point in points:
@@ -220,45 +244,70 @@
             face_centers = [face_points[face].coord for face in edge_faces[edge]]
             ends = [edge[0].coord, edge[1].coord]
             coord = np.mean(face_centers + ends, axis=0)
             edge_point = Point(
                 *coord,
                 boundary_u_tuples=boundary_u_tuples,
             )
+            for face in edge_faces[edge]:
+                edge_point.parametric_coord_in_sub_face[face.sub_face] = 0.5 * (
+                    edge[0].parametric_coord_in_sub_face[face.sub_face] + edge[1].parametric_coord_in_sub_face[face.sub_face]
+                )
             edge_points[edge] = edge_point
             new_points.append(edge_points[edge])
         
         # Move each original point to the new vertex point
         for point in points:
             F = np.mean(
                 [face_points[face].coord for face in point.faces],
                 axis=0
             )
             R = np.mean(
                 [1/2*(point.coord + q.coord) for q in point.neighbours],
                 axis=0
             )
-            n = 4
+            n = max(len(point.neighbours), 4)
             point.coord = (F + 2*R + (n - 3) * point.coord) / n
                 
 
         # Form faces in the new mesh
         self.clear_points(points)
         for face in faces:
             for i in range(4):
                 mid = []
                 for d in [-1, +1]:
                     j = (i + d) % 4
                     edge = get_edge_tuple(face.points[i], face.points[j], points)
                     mid.append(edge_points[edge])
                 new_faces.append(Face(
-                    [face.points[i], mid[0], face_points[face], mid[1]]
+                    points = [face.points[i], mid[0], face_points[face], mid[1]],
+                    sub_face = face.sub_face
                 ))
         
         # sample boundary points
         for point in new_points:
             if len(point.boundary_u_tuples) > 0:
                 boundary, u = point.boundary_u_tuples[-1]
                 point.coord = boundary.coord(u)
 
         self.faces = new_faces
         self.points = new_points
+        self.iteration += 1
+    
+    def gen_bspline_surfaces(self) -> list[list[np.ndarray]]:
+        bspline_surfaces = []
+        num = len(self.boundaries)
+        for n in range(num):
+            points_in_sub_face = []
+            for point in self.points:
+                if n not in point.parametric_coord_in_sub_face: continue
+                points_in_sub_face.append(point)
+                        
+            points_in_sub_face = sorted(
+                points_in_sub_face,
+                key=lambda p: (
+                    p.parametric_coord_in_sub_face[n][0],
+                    p.parametric_coord_in_sub_face[n][1]
+                )
+            )
+            bspline_surfaces.append(points_in_sub_face)
+        return bspline_surfaces
```

### Comparing `subdivision_hole_filler-1.0.1/src/subdivision_hole_filler.egg-info/PKG-INFO` & `subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subdivision-hole-filler
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison.
 Author-email: HUANG Lihao <huang-lihao@outlook.com>
 Project-URL: Homepage, https://github.com/huang-lihao/subdivision-hole-filler
 Project-URL: Bug Tracker, https://github.com/huang-lihao/subdivision-hole-filler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/subdivision-hole-filler?logo=pypi)](https://pypi.org/project/subdivision-hole-filler/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/subdivision-hole-filler?logo=PyPI)](https://pypi.org/project/subdivision-hole-filler/)
 [![GitHub License](https://img.shields.io/github/license/huang-lihao/subdivision-hole-filler)](https://github.com/huang-lihao/subdivision-hole-filler/blob/main/LICENSE)
 
 
 A python package to fill N-sided holes using combined subdivision schemes, based on Catmull-Clark subdivison.
 
-See [Levin, Adi. “Filling N-sided Holes Using Combined Subdivision Schemes.” (2000).](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=925ab5e9375ae3b3d64fb9870e5d08d7d50141d4)
+See [Levin, Adi. “Filling N-sided Holes Using Combined Subdivision Schemes.” (2000).](https://github.com/huang-lihao/subdivision-hole-filler/blob/main/Levin_2000_Filling%20N-sided%20Holes%20Using%20Combined%20Subdivision%20Schemes.pdf)
 
 
 Install
 ----------------------
 Use PyPI to install [subdivision-hole-filler](https://pypi.org/project/subdivision-hole-filler/):
 ```sh
 pip install subdivision-hole-filler
@@ -66,31 +66,33 @@
 
     bd = Boundary()
     bd.coord = coord # A function of parametric coord `u` in [0.0, 2.0], which defines the coordinate of a point on the boundary 
     bd.deriv = deriv # A function of parametric coord `u` in [0.0, 2.0], which defines the cross boundary derivative of a point on the boundary, poining to the inside
     boundaries[d*2] = bd
 
 for d in range(3):
-    bd = Boundary()
     def coord(u: float, d=d):
         phi = (1.0 - u / 2.0) * np.pi / 2.0
         x = R + r - R * np.cos(phi)
         y = R + r - R * np.sin(phi)
         z = 0
         c = np.zeros(3)
         c[d] = z
         c[(d + 1) % 3] = x
         c[(d + 2) % 3] = y
         return c
-    bd.coord = coord
+    
     def deriv(u: float, d=d):
         vec = np.zeros(3)
         vec[d] = 1
         return np.array(vec)
-    bd.deriv = deriv
+
+    bd = Boundary()
+    bd.coord = coord # A function of parametric coord `u` in [0.0, 2.0], which defines the coordinate of a point on the boundary 
+    bd.deriv = deriv # A function of parametric coord `u` in [0.0, 2.0], which defines the cross boundary derivative of a point on the boundary, poining to the inside
     boundaries[(d + 1) % 3 * 2 + 1] = bd
 
 filler = NsidedHoleFiller(boundaries)
 
 center_point = np.array([r, r, r])
 filler.gen_initial_mesh(center_point)
```

### Comparing `subdivision_hole_filler-1.0.1/src/subdivision_hole_filler.egg-info/SOURCES.txt` & `subdivision_hole_filler-1.0.2/src/subdivision_hole_filler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subdivision_hole_filler-1.0.1/tests/test_6sided_hole.py` & `subdivision_hole_filler-1.0.2/tests/test_6sided_hole.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,42 +26,44 @@
 
             def deriv(u: float, d=d):
                 vec = np.zeros(3)
                 vec[d] = -1
                 return np.array(vec)
 
             bd = Boundary()
-            bd.coord = coord
-            bd.deriv = deriv
+            bd.coord = coord # A function of parametric coord `u` in [0.0, 2.0], which defines the coordinate of a point on the boundary 
+            bd.deriv = deriv # A function of parametric coord `u` in [0.0, 2.0], which defines the cross boundary derivative of a point on the boundary, poining to the inside
             boundaries[d*2] = bd
 
         for d in range(3):
-            bd = Boundary()
             def coord(u: float, d=d):
                 phi = (1.0 - u / 2.0) * np.pi / 2.0
                 x = R + r - R * np.cos(phi)
                 y = R + r - R * np.sin(phi)
                 z = 0
                 c = np.zeros(3)
                 c[d] = z
                 c[(d + 1) % 3] = x
                 c[(d + 2) % 3] = y
                 return c
-            bd.coord = coord
+            
             def deriv(u: float, d=d):
                 vec = np.zeros(3)
                 vec[d] = 1
                 return np.array(vec)
-            bd.deriv = deriv
+
+            bd = Boundary()
+            bd.coord = coord # A function of parametric coord `u` in [0.0, 2.0], which defines the coordinate of a point on the boundary 
+            bd.deriv = deriv # A function of parametric coord `u` in [0.0, 2.0], which defines the cross boundary derivative of a point on the boundary, poining to the inside
             boundaries[(d + 1) % 3 * 2 + 1] = bd
 
         filler = NsidedHoleFiller(boundaries)
 
         center_point = np.array([r, r, r])
         filler.gen_initial_mesh(center_point)
 
         for iteration in range(3):
             filler.cmc_subdiv_for_1step(iteration=iteration)
-        filler.plot_faces("out.png")
+
 
 if __name__ == "__main__":
     pytest.main(["-s", "-k", "Test6SidedHole"])
```

