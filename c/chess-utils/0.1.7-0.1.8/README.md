# Comparing `tmp/chess-utils-0.1.7.tar.gz` & `tmp/chess_utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess-utils-0.1.7.tar", last modified: Thu Apr  4 18:46:08 2024, max compression
+gzip compressed data, was "chess_utils-0.1.8.tar", last modified: Tue Apr 23 08:40:19 2024, max compression
```

## Comparing `chess-utils-0.1.7.tar` & `chess_utils-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,23 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      410 2024-04-04 18:46:08.434860 chess-utils-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      541 2024-04-04 18:45:58.000000 chess-utils-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 18:46:08.434860 chess-utils-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-03-21 05:52:16.000000 chess-utils-0.1.7/src/chess_utils/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/fens/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       42 2024-03-21 05:52:30.000000 chess-utils-0.1.7/src/chess_utils/fens/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      575 2024-03-21 05:50:44.000000 chess-utils-0.1.7/src/chess_utils/fens/fens.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/misc/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/misc/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      723 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/misc/misc.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/parse/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/parse/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      850 2024-03-29 09:29:50.000000 chess-utils-0.1.7/src/chess_utils/parse/parse.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      458 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/parse/test_parsing.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/pgns/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:42:54.000000 chess-utils-0.1.7/src/chess_utils/pgns/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      257 2024-04-04 18:45:41.000000 chess-utils-0.1.7/src/chess_utils/pgns/pgns.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils/random/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/random/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1041 2024-03-21 05:50:11.000000 chess-utils-0.1.7/src/chess_utils/random/random.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      254 2024-04-04 18:45:50.000000 chess-utils-0.1.7/src/chess_utils/test.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 18:46:08.434860 chess-utils-0.1.7/src/chess_utils.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      410 2024-04-04 18:46:08.000000 chess-utils-0.1.7/src/chess_utils.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      617 2024-04-04 18:46:08.000000 chess-utils-0.1.7/src/chess_utils.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 18:46:08.000000 chess-utils-0.1.7/src/chess_utils.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       59 2024-04-04 18:46:08.000000 chess-utils-0.1.7/src/chess_utils.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-04-04 18:46:08.000000 chess-utils-0.1.7/src/chess_utils.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.750948 chess_utils-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      404 2024-04-23 08:40:19.740948 chess_utils-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      529 2024-04-23 08:40:17.000000 chess_utils-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-23 08:40:19.750948 chess_utils-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.740948 chess_utils-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.740948 chess_utils-0.1.8/src/chess_utils/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-23 08:38:49.000000 chess_utils-0.1.8/src/chess_utils/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      157 2024-04-23 08:39:09.000000 chess_utils-0.1.8/src/chess_utils/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      754 2024-04-23 08:37:14.000000 chess_utils-0.1.8/src/chess_utils/boards.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      591 2024-04-23 08:37:05.000000 chess_utils-0.1.8/src/chess_utils/fens.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      226 2024-04-23 08:37:55.000000 chess_utils-0.1.8/src/chess_utils/pgns.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.740948 chess_utils-0.1.8/src/chess_utils/random/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       40 2024-04-23 08:35:13.000000 chess_utils-0.1.8/src/chess_utils/random/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1048 2024-04-23 08:34:52.000000 chess_utils-0.1.8/src/chess_utils/random/random.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.740948 chess_utils-0.1.8/src/chess_utils/test/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      458 2024-03-21 05:50:11.000000 chess_utils-0.1.8/src/chess_utils/test/test_parsing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      254 2024-04-04 18:45:50.000000 chess_utils-0.1.8/src/chess_utils/test.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:40:19.740948 chess_utils-0.1.8/src/chess_utils.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      404 2024-04-23 08:40:19.000000 chess_utils-0.1.8/src/chess_utils.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      468 2024-04-23 08:40:19.000000 chess_utils-0.1.8/src/chess_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-23 08:40:19.000000 chess_utils-0.1.8/src/chess_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-04-23 08:40:19.000000 chess_utils-0.1.8/src/chess_utils.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       12 2024-04-23 08:40:19.000000 chess_utils-0.1.8/src/chess_utils.egg-info/top_level.txt
```

### Comparing `chess-utils-0.1.7/pyproject.toml` & `chess_utils-0.1.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chess-utils"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
-    {name="Marcel Claramunt", email="marcel@moveread.com"}
+  {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Higher level utilities over the `chess` library"
 dependencies = [
-    "chess", "pydantic", "haskellian-either"
+  "chess", "pydantic", "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.optional-dependencies]
 test = [
-    "pytest", "hypothesis"
+  "pytest", "hypothesis"
 ]
 
 # [project.urls]
 # repo = "<GIT_REPO_URL>"
```

### Comparing `chess-utils-0.1.7/src/chess_utils/fens/fens.py` & `chess_utils-0.1.8/src/chess_utils/fens.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,12 +7,12 @@
   castling: str
   passant: str
   plyClock: int
   fullMoves: int
 
 def parse(fen: str) -> FEN:
   position, turn, castling, passant, plyClock, fullMoves = fen.split(' ')
-  return FEN(position=position, turn=turn, castling=castling, passant=passant, plyClock=plyClock, fullMoves=fullMoves)
+  return FEN(position=position, turn=turn, castling=castling, passant=passant, plyClock=plyClock, fullMoves=fullMoves) # type: ignore
 
 def position_idx(fen: str | FEN) -> int:
   fen_obj = parse(fen) if isinstance(fen, str) else fen
-  return 2*(fen_obj.fullMoves-1) + (0 if fen_obj.turn == 'w' else 1)
+  return 2*(fen_obj.fullMoves-1) + (0 if fen_obj.turn == 'w' else 1)
```

### Comparing `chess-utils-0.1.7/src/chess_utils/misc/misc.py` & `chess_utils-0.1.8/src/chess_utils/boards.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import Literal
 import chess
 
 def unchecked_san(board: chess.Board, move: chess.Move) -> str:
   """Like `board.san(move)` but doesn't include check/mate symbols (about 10x faster)"""
   return board._algebraic_without_suffix(move)
-
+  
 def fen_after(move: chess.Move, board: chess.Board) -> str:
     """FEN after `move` made in `board`"""
     board.push(move)
     succ_fen = board.fen()
     board.pop()
     return succ_fen
-  
+
 CapturablePiece = Literal['P', 'N', 'B', 'R', 'Q']
 
 def captured_piece(board: chess.Board, move: chess.Move) -> CapturablePiece | None:
   """The piece captured by `move` on `board` (or `None`)"""
   type = board.piece_type_at(move.to_square)
-  return type and chess.piece_symbol(type).upper()
+  if type is not None:
+    return chess.piece_symbol(type).upper() # type: ignore
```

### Comparing `chess-utils-0.1.7/src/chess_utils/random/random.py` & `chess_utils-0.1.8/src/chess_utils/random/random.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   """A random legal move on the given position"""
   moves = list(board.legal_moves)
   if len(moves) == 0:
     return None
   idx = rng.randint(0, len(moves)-1)
   return moves[idx]
 
-def line(position: chess.Board | str = chess.STARTING_FEN, max_depth: int = None, rng = random.Random()) -> Generator[chess.Move, None, chess.Board]:
+def line(position: chess.Board | str = chess.STARTING_FEN, max_depth: int | None = None, rng = random.Random()) -> Generator[chess.Move, None, chess.Board]:
   """A possibly-infinite line of legal moves, starting at `fen`"""
   board = chess.Board(position) if isinstance(position, str) else position
   mv = move(board)
   while mv is not None and (max_depth is None or board.ply() < max_depth):
     board.push(mv)
     yield mv
     mv = move(board, rng)
```

