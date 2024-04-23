# Comparing `tmp/chess2vec-0.3.1.tar.gz` & `tmp/chess2vec-0.3.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.1.tar", max compression
+gzip compressed data, was "chess2vec-0.3.1b1.tar", max compression
```

## Comparing `chess2vec-0.3.1.tar` & `chess2vec-0.3.1b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.1/README.md
--rw-r--r--   0        0        0     1884 2024-04-23 20:20:37.648701 chess2vec-0.3.1/chess2vec/__init__.py
--rw-r--r--   0        0        0      293 2024-04-20 10:13:12.779868 chess2vec-0.3.1/chess2vec/pgn.py
--rw-r--r--   0        0        0      180 2024-04-23 20:20:36.818268 chess2vec-0.3.1/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.1/chess2vec/utils/vector.py
--rw-r--r--   0        0        0     1246 2024-04-23 20:21:14.401429 chess2vec-0.3.1/chess2vec/vectorizers.py
--rw-r--r--   0        0        0      401 2024-04-23 20:21:51.053297 chess2vec-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 chess2vec-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.1b1/README.md
+-rw-r--r--   0        0        0     1748 2024-04-23 20:32:51.427651 chess2vec-0.3.1b1/chess2vec/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-20 10:13:12.779868 chess2vec-0.3.1b1/chess2vec/pgn.py
+-rw-r--r--   0        0        0      180 2024-04-23 20:20:36.818268 chess2vec-0.3.1b1/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.1b1/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0     1246 2024-04-23 20:21:14.401429 chess2vec-0.3.1b1/chess2vec/vectorizers.py
+-rw-r--r--   0        0        0      403 2024-04-23 20:37:54.533552 chess2vec-0.3.1b1/pyproject.toml
+-rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 chess2vec-0.3.1b1/PKG-INFO
```

### Comparing `chess2vec-0.3.1/chess2vec/__init__.py` & `chess2vec-0.3.1b1/chess2vec/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,36 +5,26 @@
 import compress_pickle
 from tqdm import tqdm
 
 from chess2vec import vectorizers as _vec
 
 
 class PositionLoader:
-    def __init__(
-        self, vectorizers: Iterable[_vec.BaseVectorizer], mark: bool = False
-    ) -> None:
+    def __init__(self, vectorizers: Iterable[_vec.BaseVectorizer]) -> None:
         self.vectorizers = vectorizers
         self.data = []
-
-        if mark:
-            self.mark = mark
-            self.id = 0
+        self.game_id = 0
 
     @property
     def size(self) -> int:
         return len(self.data)
 
     def add(self, board: chess.Board) -> None:
-        pos = [v(board) for v in self.vectorizers]
-
-        if self.mark:
-            pos.append(self.id)
-            self.id += 1
-
-        self.data.append(pos)
+        self.data.append([v(board) for v in self.vectorizers] + [self.game_id])
+        self.game_id += 1
 
     def load_pgn(
         self, pgn: TextIO, num_of_games: int = None, status: bool = False
     ) -> None:
         if num_of_games is None:
             num_of_games = float("inf")
```

### Comparing `chess2vec-0.3.1/chess2vec/utils/vector.py` & `chess2vec-0.3.1b1/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.1/chess2vec/vectorizers.py` & `chess2vec-0.3.1b1/chess2vec/vectorizers.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.1/PKG-INFO` & `chess2vec-0.3.1b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.1
+Version: 0.3.1b1
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

