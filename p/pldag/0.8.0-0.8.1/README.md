# Comparing `tmp/pldag-0.8.0.tar.gz` & `tmp/pldag-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.8.0.tar", max compression
+gzip compressed data, was "pldag-0.8.1.tar", max compression
```

## Comparing `pldag-0.8.0.tar` & `pldag-0.8.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.0/LICENSE
--rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.0/README.md
--rw-r--r--   0        0        0    35723 2024-05-08 08:21:12.707126 pldag-0.8.0/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.0/pldag/solver/__init__.py
--rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.0/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-05-08 08:25:34.786486 pldag-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2833 2024-05-07 07:16:43.962166 pldag-0.8.1/README.md
+-rw-r--r--   0        0        0    36409 2024-05-12 18:13:16.288613 pldag-0.8.1/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:47:23.684023 pldag-0.8.1/pldag/solver/__init__.py
+-rw-r--r--   0        0        0     1021 2024-04-25 07:47:35.469193 pldag-0.8.1/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-05-12 18:29:15.546030 pldag-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 pldag-0.8.1/PKG-INFO
```

### Comparing `pldag-0.8.0/LICENSE` & `pldag-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.8.0/README.md` & `pldag-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.8.0/pldag/__init__.py` & `pldag-0.8.1/pldag/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,17 @@
         Each node in the graph encapsulates information about how its incoming nodes or leafs are logically related. For instance, a node might represent an AND operation, meaning that if it evaluates to true, all its incoming nodes or leafs must also evaluate to true.
         
         In summary, this data structure combines elements of a DAG with a logic network, utilizing prime numbers to encode relationships and facilitate operations within the graph.
     """
 
     def __init__(self):
         # Adjacency matrix. Each entry is a boolean (0/1) indicating if there is a dependency
-        self._amat = np.zeros((0, 0),   dtype=np.uint8)
+        self._amat = np.zeros((0, 0),   dtype=np.int64)
+        # Weight matrix. Each entry is a weight on the dependency
+        self._wmat = np.zeros((0, 0),   dtype=np.int64)
         # Boolean vector indicating if negated
         self._nvec = np.zeros((0, ),    dtype=bool)
         # Complex vector representing bounds of complex number data type
         self._dvec = np.zeros((0, ),    dtype=complex)
         # Bias vector
         self._bvec = np.zeros((0, ),    dtype=complex)
         # Boolean vector indicating if the node is a composition
@@ -142,22 +144,28 @@
     
     def _row(self, id: str) -> int:
         """
             Returns the row index of the given ID.
         """
         return self.composites.tolist().index(id)
     
-    def _set_gelineq(self, children: list, bias: int, negate: bool = False, alias: Optional[str] = None) -> str:
+    def set_gelineq(self, children: list, bias: int, negate: bool = False, alias: Optional[str] = None, weights: Optional[List[int]] = None) -> str:
         """
             Add a composite constraint of at least `value`.
         """
         _id = self._composite_id(children, bias, negate)
         if not _id in self._imap:
             self._amat = np.pad(self._amat, ((0, 1), (0, 1)), mode='constant')
-            self._amat[-1, [self._col(child) for child in children]] = 1
+            if weights:
+                if not len(weights) == len(children):
+                    raise ValueError("Weights must be the same length as children.")
+                self._amat[-1, [self._col(child) for child in children]] = weights
+            else:
+                self._amat[-1, [self._col(child) for child in children]] = 1
+
             self._dvec = np.append(self._dvec, complex(0, 1))
             self._bvec = np.append(self._bvec, complex(*repeat(bias * (1-negate) + (bias + 1) * negate * -1, 2)))
             self._nvec = np.append(self._nvec, negate)
             self._cvec = np.append(self._cvec, True)
             self._imap[_id] = self._amat.shape[1] - 1
 
         if alias:
@@ -181,15 +189,15 @@
         #    For instance, [1 1](A) = [0 1](x) + [0 1](y) + [0 1](z) - [3 3] >= 0 has an inner bound of [0 1]+[0 1]+[0 1]-[3 3] = [-3 0] and should result in x=1, y=1 and z=1, since A=1 is fixed
         #    Or, [1 1](A) = [-1 0](x) + [-1 0](y) + [-1 0](z) >= 0 has an inner bound of [-1 0]+[-1 0]+[-1 0] = [-3 0] and should result in x=0, y=0, z=0, since A=1 is fixed
 
         # 2. When the inner lower bound is -1 AND the outer bound is false.
         #    Then we can assume each variable's bound in the composite to be their constant lower bound. I.e. set their variables upper bound to their lower bound.
         #    For instance, [0 0](A) = [0 1](x) + [0 1](y) + [0 1](z) - [1 1] >= 0 has an inner bound of [0 1]+[0 1]+[0 1]-[1 1] = [-1 2] and should result in x≈0, y≈0 and z≈0, since A=0 is fixed
         #    Or, [0 0] = [-1 0](x) + [-1 0](y) + [-1 0](z) + 2 >= 0 has an inner bound of [-1 0]+[-1 0]+[-1 0]+[2 2] = [-1 2] and should result in x≈0, y≈0 and z≈0, since A=0 is fixed
-        _A = np.vstack((np.zeros((A.shape[1]-A.shape[0], A.shape[1]), dtype=np.uint8), A))
+        _A = np.vstack((np.zeros((A.shape[1]-A.shape[0], A.shape[1]), dtype=np.int64), A))
         _B = np.append(np.zeros(A.shape[1]-A.shape[0], dtype=complex), B)
         _F = np.append(np.zeros(A.shape[1]-A.shape[0], dtype=bool), F)
         _fixed = fixed | (D.real == D.imag)
         M = (_A == 1) & ~_fixed
         for i in filter(
             lambda i: C[i] and M[i].any(), 
             reversed(
@@ -449,15 +457,16 @@
             str
                 The ID of the primitive variable.
         """
         if id in self._imap:
             # Update value if already in map
             self._dvec[self._col(id)] = bound
         else:
-            self._amat = np.hstack((self._amat, np.zeros((self._amat.shape[0], 1), dtype=np.uint8)))
+            self._amat = np.hstack((self._amat, np.zeros((self._amat.shape[0], 1), dtype=np.int64)))
+            self._wmat = np.hstack((self._wmat, np.zeros((self._wmat.shape[0], 1), dtype=np.int64)))
             self._dvec = np.append(self._dvec, bound)
             self._cvec = np.append(self._cvec, False)
             self._imap[id] = self._amat.shape[1] - 1
 
         return id
 
     def set_primitives(self, ids: List[str], bound: complex = complex(0,1)) -> List[str]:
@@ -487,15 +496,15 @@
             List[str]
                 The IDs of the primitive variables.
         """
         for id in ids:
             self.set_primitive(id, bound)
         return ids
     
-    def set_atleast(self, references: List[str], value: int, alias: Optional[str] = None) -> str:
+    def set_atleast(self, references: List[str], value: int, alias: Optional[str] = None, weights: Optional[List[int]] = None) -> str:
         """
             Add a composite constraint of at least `value`.
 
             Parameters
             ----------
             references : List[str]
                 The references to composite constraints or primitive variables.
@@ -512,17 +521,17 @@
             1+1j
 
             Returns
             -------
             str
                 The ID of the composite constraint.
         """
-        return self._set_gelineq(references, -1 * value, False, alias)
+        return self.set_gelineq(references, -1 * value, False, alias, weights)
     
-    def set_atmost(self, references: List[str], value: int, alias: Optional[str] = None) -> str:
+    def set_atmost(self, references: List[str], value: int, alias: Optional[str] = None, weights: Optional[List[int]] = None) -> str:
         """
             Add a composite constraint of at most `value`.
 
             Parameters
             ----------
             references : List[str]
                 The references to composite constraints or primitive variables.
@@ -539,15 +548,15 @@
             1+1j
 
             Returns
             -------
             str
                 The ID of the composite constraint.
         """
-        return self._set_gelineq(references, -1 * (value + 1), True, alias)
+        return self.set_gelineq(references, -1 * (value + 1), True, alias, weights)
     
     def set_or(self, references: List[str], alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of an OR operation.
 
             Parameters
             ----------
@@ -767,31 +776,31 @@
         mn = ad.real
         mx = ad.imag
 
         # Extract `d` vector from bias
         d = -1 * self._bvec.real
 
         # Adjacent points
-        adj_points = np.argwhere(self._amat == 1)
+        adj_points = np.argwhere(self._amat != 0)
 
         # If no adjacent points, return empty matrix
         if adj_points.size == 0:
             return np.zeros((0, self._amat.shape[1]), dtype=np.int64), np.zeros(0, dtype=np.int64)
 
         # A -> X row indices
         A_X_ri = adj_points.T[0]
         A_X = np.arange(self._amat.shape[0])
         # X -> A row indices
         X_A = A_X + A_X.max() + 1
         X_A_ri = adj_points.T[0] + A_X.max() + 1
 
         # Fill the matrix with adjacency points
-        A[A_X_ri, adj_points.T[1]] = -1
+        A[A_X_ri, adj_points.T[1]] = -self._amat[A_X_ri, adj_points.T[1]]
         if double_binding:
-            A[X_A_ri, adj_points.T[1]] = -1
+            A[X_A_ri, adj_points.T[1]] = -self._amat[A_X_ri, adj_points.T[1]]
 
         # Assign 1 instead of -1 to the at least A -> X, and at most constraints for X -> A.
         A[A_X[~self._nvec], :] *= -1
         if double_binding:
             A[X_A[self._nvec], :] *= -1
 
         # Composite index in matrix
```

### Comparing `pldag-0.8.0/pldag/solver/glpk_solver.py` & `pldag-0.8.1/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.8.0/PKG-INFO` & `pldag-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.8.0
+Version: 0.8.1
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

