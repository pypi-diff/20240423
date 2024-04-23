# Comparing `tmp/chess2vec-0.3.1b1.tar.gz` & `tmp/chess2vec-0.3.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.1b1.tar", max compression
+gzip compressed data, was "chess2vec-0.3.1b2.tar", max compression
```

## Comparing `chess2vec-0.3.1b1.tar` & `chess2vec-0.3.1b2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.1b1/README.md
--rw-r--r--   0        0        0     1748 2024-04-23 20:32:51.427651 chess2vec-0.3.1b1/chess2vec/__init__.py
--rw-r--r--   0        0        0      293 2024-04-20 10:13:12.779868 chess2vec-0.3.1b1/chess2vec/pgn.py
--rw-r--r--   0        0        0      180 2024-04-23 20:20:36.818268 chess2vec-0.3.1b1/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.1b1/chess2vec/utils/vector.py
--rw-r--r--   0        0        0     1246 2024-04-23 20:21:14.401429 chess2vec-0.3.1b1/chess2vec/vectorizers.py
--rw-r--r--   0        0        0      403 2024-04-23 20:37:54.533552 chess2vec-0.3.1b1/pyproject.toml
--rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 chess2vec-0.3.1b1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.1b2/README.md
+-rw-r--r--   0        0        0     1836 2024-04-23 21:13:10.520791 chess2vec-0.3.1b2/chess2vec/__init__.py
+-rw-r--r--   0        0        0      287 2024-04-23 21:18:28.472128 chess2vec-0.3.1b2/chess2vec/pgn.py
+-rw-r--r--   0        0        0      202 2024-04-23 21:17:26.179422 chess2vec-0.3.1b2/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.1b2/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0     1308 2024-04-23 21:17:02.920716 chess2vec-0.3.1b2/chess2vec/vectorizers.py
+-rw-r--r--   0        0        0      403 2024-04-23 21:18:46.133096 chess2vec-0.3.1b2/pyproject.toml
+-rw-r--r--   0        0        0      650 1970-01-01 00:00:00.000000 chess2vec-0.3.1b2/PKG-INFO
```

### Comparing `chess2vec-0.3.1b1/chess2vec/__init__.py` & `chess2vec-0.3.1b2/chess2vec/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,39 +20,45 @@
 
     def add(self, board: chess.Board) -> None:
         self.data.append([v(board) for v in self.vectorizers] + [self.game_id])
         self.game_id += 1
 
     def load_pgn(
         self, pgn: TextIO, num_of_games: int = None, status: bool = False
-    ) -> None:
+    ) -> bool:
         if num_of_games is None:
             num_of_games = float("inf")
 
         if status:
             bar = tqdm(total=num_of_games)
 
-        n, game = 0, chess.pgn.read_game(pgn)
+        n = 0
 
-        while game and n < num_of_games:
+        while n < num_of_games:
+            game = chess.pgn.read_game(pgn)
+            
+            if not game:
+                return False
+            
             board = game.board()
             self.add(board)
 
             for move in game.mainline_moves():
                 board.push(move)
                 self.add(board)
 
             if status:
                 bar.update(1)
-
-            game = chess.pgn.read_game(pgn)
+                
             n += 1
 
         if status:
             bar.close()
+            
+        return True
 
     def get_position(self, idx):
         return self.data[idx]
 
     def get_vector(self, idx):
         return list(zip(*self.data))[idx]
```

### Comparing `chess2vec-0.3.1b1/chess2vec/utils/vector.py` & `chess2vec-0.3.1b2/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.1b1/chess2vec/vectorizers.py` & `chess2vec-0.3.1b2/chess2vec/vectorizers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import abc
 
 import chess
 
 from chess2vec import utils
 
+import numpy as np
+
 
 def full_classname(obj):
     return ".".join((obj.__class__.__module__, obj.__class__.__qualname__))
 
 
 class BaseVectorizer(abc.ABC):
     @abc.abstractmethod
     def __call__(self, board: chess.Board): ...
 
     def __repr__(self) -> str:
         return f"{full_classname(self)}(size={self.size}, dtype={self.dtype})"
 
 
 class ActionVectorizer(BaseVectorizer):
-    @utils.convert_return(list)
+    @utils.convert_return(np.array, dtype=np.uint16)
     def __call__(self, board: chess.Board):
         for move in board.legal_moves:
             pt = board.piece_type_at(move.from_square)
 
             if not board.turn:
                 move.from_square ^= 0x38
                 move.to_square ^= 0x38
 
             yield 64 * (64 * (pt - 1) + move.from_square) + move.to_square
 
 
 class PieceVectorizer(BaseVectorizer):
-    @utils.convert_return(list)
+    @utils.convert_return(np.array, dtype=np.uint16)
     def __call__(self, board: chess.Board):
         for sq in chess.scan_reversed(board.occupied):
             piece = board.piece_at(sq)
 
             if not board.turn:
                 sq ^= 0x38
```

### Comparing `chess2vec-0.3.1b1/PKG-INFO` & `chess2vec-0.3.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.1b1
+Version: 0.3.1b2
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

