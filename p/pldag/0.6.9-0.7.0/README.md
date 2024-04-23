# Comparing `tmp/pldag-0.6.9.tar.gz` & `tmp/pldag-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pldag-0.6.9.tar", max compression
+gzip compressed data, was "pldag-0.7.0.tar", max compression
```

## Comparing `pldag-0.6.9.tar` & `pldag-0.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.6.9/LICENSE
--rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.6.9/README.md
--rw-r--r--   0        0        0    31135 2024-04-22 15:00:50.811385 pldag-0.6.9/pldag/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 11:08:54.241329 pldag-0.6.9/pldag/solver/__init__.py
--rw-r--r--   0        0        0      973 2024-04-22 15:04:47.780408 pldag-0.6.9/pldag/solver/glpk_solver.py
--rw-r--r--   0        0        0      399 2024-04-22 15:04:56.568103 pldag-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-02-17 13:06:46.819923 pldag-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-22 11:08:59.388067 pldag-0.7.0/README.md
+-rw-r--r--   0        0        0    31133 2024-04-23 09:33:19.711046 pldag-0.7.0/pldag/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 11:08:54.241329 pldag-0.7.0/pldag/solver/__init__.py
+-rw-r--r--   0        0        0      973 2024-04-22 15:04:47.780408 pldag-0.7.0/pldag/solver/glpk_solver.py
+-rw-r--r--   0        0        0      399 2024-04-23 09:34:32.006494 pldag-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3303 1970-01-01 00:00:00.000000 pldag-0.7.0/PKG-INFO
```

### Comparing `pldag-0.6.9/LICENSE` & `pldag-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pldag-0.6.9/README.md` & `pldag-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pldag-0.6.9/pldag/__init__.py` & `pldag-0.7.0/pldag/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         """
         return self._imap[id]
     
     def _row(self, id: str) -> int:
         """
             Returns the row index of the given ID.
         """
-        return self._col(id) - (~self._cvec).sum()
+        return self.composites.tolist().index(id)
     
     def _set_gelineq(self, children: list, bias: int, negate: bool = False, alias: Optional[str] = None) -> str:
         """
             Add a composite constraint of at least `value`.
         """
         _id = self._composite_id(children, bias, negate)
         if not _id in self._imap:
@@ -247,15 +247,15 @@
         
         raise Exception(f"Maximum iterations ({max_iterations}) reached without convergence.")
     
     def id_from_alias(self, alias: str) -> Optional[str]:
         """Get the ID of the given alias"""
         return self._amap.get(alias, None)
     
-    def alias_to_ids(self, id: str) -> List[str]:
+    def id_to_alias(self, id: str) -> List[str]:
         """Get the aliases of the given ID"""
         return list(
             map(
                 lambda x: x[0],
                 filter(
                     lambda x: x[1] == id,
                     self._amap.items(),
```

### Comparing `pldag-0.6.9/pldag/solver/glpk_solver.py` & `pldag-0.7.0/pldag/solver/glpk_solver.py`

 * *Files identical despite different names*

### Comparing `pldag-0.6.9/PKG-INFO` & `pldag-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pldag
-Version: 0.6.9
+Version: 0.7.0
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

