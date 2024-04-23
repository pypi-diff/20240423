# Comparing `tmp/pldag-0.7.0.tar.gz` & `tmp/pldag-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.7.0.tar", max compression
+gzip compressed data, was "pldag-0.7.1.tar", max compression
```

## Comparing `pldag-0.7.0.tar` & `pldag-0.7.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.0/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.0/README.md
--rw-r--r--   0        0        0    31133 2024-04-23 09:33:19.711046 pldag-0.7.0/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 11:08:54.241329 pldag-0.7.0/pldag/solver/__init__.py
--rw-r--r--   0        0        0      973 2024-04-22 15:04:47.780408 pldag-0.7.0/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-04-23 09:34:32.006494 pldag-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.1/README.md
+-rw-r--r--   0        0        0    31509 2024-04-23 14:55:03.002193 pldag-0.7.1/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:08:54.241329 pldag-0.7.1/pldag/solver/__init__.py
+-rw-r--r--   0        0        0      973 2024-04-22 15:04:47.780408 pldag-0.7.1/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-04-23 13:54:51.080665 pldag-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.1/PKG-INFO
```

### Comparing `pldag-0.7.0/LICENSE` & `pldag-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.7.0/README.md` & `pldag-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.7.0/pldag/__init__.py` & `pldag-0.7.1/pldag/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,14 +181,16 @@
         # 2. When the inner lower bound is -1 AND the outer bound is false.
         #    Then we can assume each variable's bound in the composite to be their constant lower bound. I.e. set their variables upper bound to their lower bound.
         #    For instance, [0 0](A) = [0 1](x) + [0 1](y) + [0 1](z) - [1 1] >= 0 has an inner bound of [0 1]+[0 1]+[0 1]-[1 1] = [-1 2] and should result in x≈0, y≈0 and z≈0, since A=0 is fixed
         #    Or, [0 0] = [-1 0](x) + [-1 0](y) + [-1 0](z) + 2 >= 0 has an inner bound of [-1 0]+[-1 0]+[-1 0]+[2 2] = [-1 2] and should result in x≈0, y≈0 and z≈0, since A=0 is fixed
         
         _A = np.vstack((np.zeros((A.shape[1]-A.shape[0], A.shape[1]), dtype=np.uint8), A))
         _B = np.append(np.zeros(A.shape[1]-A.shape[0], dtype=complex), B)
+        _F = np.append(np.zeros(A.shape[1]-A.shape[0], dtype=bool), F)
+        _fixed = fixed | (D.real == D.imag)
         for i in filter(
             lambda i: C[i], 
             reversed(
                 list(
                     TopologicalSorter(
                         dict(
                             map(
@@ -196,22 +198,30 @@
                                 groupby(np.argwhere(_A).tolist(), key=lambda x: x[0])
                             )
                         )
                     ).static_order()
                 )
             )
         ):
-            r = _A[i].dot(D) + _B[i]
-            m = (_A[i] == 1) & ~fixed
-            # If the inner upper bound is 0 and the outer bound is true
-            if r.imag == 0 and D[i].real == 1:
-                D[m] = D[m].imag + D[m].imag * 1j
-
-            elif r.real == -1 and D[i].imag == 0:
-                D[m] = D[m].real + D[m].real * 1j
+            r = _A[i].dot(D)
+            rf = (-1j * np.conj(r) * _F[i] + (1-_F[i]) * r) + _B[i]
+            m = (_A[i] == 1) & ~_fixed
+            re = D[m].real
+            im = D[m].imag
+            if rf.imag == 0 and D[i].real == 1:
+                if _F[i]:
+                    D[m] = re + re * 1j
+                else:
+                    D[m] = im + im * 1j
+
+            elif rf.real == -1 and D[i].imag == 0:
+                if _F[i]:
+                    D[m] = im + im * 1j
+                else:
+                    D[m] = re + re * 1j
 
         return D
     
     @staticmethod
     def _prop_algo_downstream(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray, F: np.ndarray, fixed: np.ndarray, max_iterations: int = 100):
 
         """
@@ -243,14 +253,57 @@
             new_D = fixed * D + ~fixed * prop(previous_D)
             if (new_D == previous_D).all():
                 return new_D
             previous_D = new_D
         
         raise Exception(f"Maximum iterations ({max_iterations}) reached without convergence.")
     
+    @staticmethod
+    def _prop_algo_bistream(A: np.ndarray, B: np.ndarray, C: np.ndarray, D: np.ndarray, F: np.ndarray, fixed: np.ndarray, max_iterations: int = 100):
+        """
+            Propagates the graph downstream and upstream, and returns the propagated bounds.
+        """
+        return PLDAG._prop_upstream_algo(A, B, C, PLDAG._prop_algo_downstream(A, B, C, D, F, fixed), F, fixed, max_iterations)
+    
+    def _propagate(self, method: str, query: dict, freeze: bool = True) -> dict:
+        """
+            Propagates the graph downstream and returns the propagated bounds.
+        """
+        A: np.ndarray = self._amat
+        B: np.ndarray = self._bvec
+        C: np.ndarray = self._cvec
+        D: np.ndarray = self._dvec.copy()
+        F: np.ndarray = self._nvec
+
+        # Filter query based on existing variables
+        query = {k: v for k, v in query.items() if k in self._imap}
+
+        # Query translation into primes
+        qprimes = np.zeros(D.shape[0], dtype=bool)
+        qprimes[[self._imap[q] for q in query]] = True and freeze
+
+        # Replace the observed bounds
+        D[[self._imap[q] for q in query]] = np.array(list(query.values()))
+
+        if method == "downstream":
+            res = self._prop_algo_downstream(A, B, C, D, F, qprimes)
+        elif method == "upstream":
+            res = self._prop_upstream_algo(A, B, C, D, F, qprimes)
+        elif method == "bistream":
+            res = self._prop_algo_bistream(A, B, C, D, F, qprimes)
+        else:
+            raise ValueError(f"Method '{method}' not found.")
+        
+        return dict(
+            zip(
+                self._imap.keys(),
+                res,
+            )
+        )
+    
     def id_from_alias(self, alias: str) -> Optional[str]:
         """Get the ID of the given alias"""
         return self._amap.get(alias, None)
     
     def id_to_alias(self, id: str) -> List[str]:
         """Get the aliases of the given ID"""
         return list(
@@ -282,15 +335,15 @@
             )
         )
     
     def negated(self, id: str) -> bool:
         """Get the negated state of the given id"""
         return bool(self._nvec[self._row(id)])
 
-    def propagate_downstream(self):
+    def propagate_downstream(self, query: dict = {}, freeze: bool = True) -> dict:
         """
             Propagates the graph downstream, towards the root node(s), and returns the propagated bounds.
 
             Examples
             --------
             >>> model = PLDAG()
             >>> model.set_primitives("xy")
@@ -304,96 +357,43 @@
             >>> model.get(a)
             1+1j
 
             Returns
             -------
             None
         """
-        A: np.ndarray = self._amat
-        B: np.ndarray = self._bvec
-        C: np.ndarray = self._cvec
-        D: np.ndarray = self._dvec
-        F: np.ndarray = self._nvec
-
-        self._dvec = self._prop_algo_downstream(A, B, C, D, F, np.zeros(D.shape[0], dtype=bool))
+        return self._propagate("downstream", query, freeze)
     
-    def propagate_upstream(self):
+    def propagate_upstream(self, query: dict = {}, freeze: bool = True) -> dict:
         """
             Propagates the graph upstream, from the root node(s), and returns the propagated bounds.
 
             Examples
             --------
             >>> model = PLDAG()
             >>> model.set_primitives("xy")
             >>> a = model.set_atleast("xy", 1)
-            >>> model.propagate_upstream()
-            >>> model.get(a)
+            >>> model.propagate_upstream().get(a)
             1j
             
             >>> model.set_primitive("x", 1+1j)
-            >>> model.propagate_upstream()
-            >>> model.get(a)
+            >>> model.propagate_upstream().get(a)
             1+1j
 
             Returns
             -------
             None
         """
-        A: np.ndarray = self._amat
-        B: np.ndarray = self._bvec
-        C: np.ndarray = self._cvec
-        D: np.ndarray = self._dvec
-        F: np.ndarray = self._nvec
-
-        self._dvec = self._prop_upstream_algo(A, B, C, D, F, np.zeros(D.shape[0], dtype=bool))
-    
-    def test(self, query: Dict[str, complex], freeze: bool = True) -> Dict[str, complex]:
+        return self._propagate("upstream", query, freeze)
 
+    def propagate_bistream(self, query: Dict[str, complex], freeze: bool = True) -> dict:
         """
-            Propagates the graph downstream and returns the result.
-
-            Parameters
-            ----------
-            query : Dict[str, complex]
-                The query to test.
-
-            freeze : bool = True
-                If the bounds given in query should be changeable
-                during propagation.
-
-            Examples
-            --------
-            >>> model = PLDAG()
-            >>> model.set_primitives("xy")
-            >>> a = model.set_atleast("xy", 1)
-            >>> model.test({"x": 1j, "y": 1+1j}).get(a)
-            1+1j
-
-            Returns
-            -------
-            Dict[str, complex]
-                The result of the query.
+            Propagates the graph downstream and upstream, and returns the propagated bounds.
         """
-        A: np.ndarray = self._amat
-        B: np.ndarray = self._bvec
-        C: np.ndarray = self._cvec
-        D: np.ndarray = self._dvec.copy()
-        F: np.ndarray = self._nvec
-
-        # Filter query based on existing variables
-        query = {k: v for k, v in query.items() if k in self._imap}
-
-        # Query translation into primes
-        qprimes = np.zeros(D.shape[0], dtype=bool)
-        qprimes[[self._imap[q] for q in query]] = True and freeze
-
-        # Replace the observed bounds
-        D[[self._imap[q] for q in query]] = np.array(list(query.values()))
-
-        return dict(zip(self._imap.keys(), self._prop_algo_downstream(A, B, C, D, F, qprimes)))
+        return self.propagate_bistream(query, freeze)
     
     def set_primitive(self, id: str, bound: complex = complex(0,1)) -> str:
         """
             Add a primitive variable.
 
             Parameters
             ----------
@@ -859,15 +859,15 @@
 
         col_idxs = np.array(sorted(list(map(col_vars.index, matching_variables))))
         row_idxs = np.array(sorted(list(map(row_vars.index, filter(lambda v: v in self._row_vars, matching_variables)))))
         return self._from_indices(row_idxs, col_idxs)
     
     def solve(self, objectives: List[Dict[str, int]], fix: Dict[str, int], solver: Solver) -> List[Dict[str, int]]:
         """
-            Solve the polyhedron with the given objectives.
+            Solves the model with the given objectives.
 
             Parameters
             ----------
             objectives : List[Dict[str, int]]
                 The objectives to solve for.
 
             fix : Dict[str, int]
@@ -877,15 +877,14 @@
                 The solver to use.
 
             Examples
             --------
             >>> model = PLDAG()
             >>> model.set_primitives("xyz")
             >>> a = model.set_atleast("xyz", 1)
-            >>> A,b,vs = model.to_polyhedron()
             >>> model.solve([{"x": 0, "y": 1, "z": 0}], Solver.GLPK)
             [{'x': 0, 'y': 1, 'z': 0}]
 
             Returns
             -------
             List[Dict[str, int]]
                 The solutions for the objectives.
```

### Comparing `pldag-0.7.0/pldag/solver/glpk_solver.py` & `pldag-0.7.1/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.7.0/PKG-INFO` & `pldag-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

