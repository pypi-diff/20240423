# Comparing `tmp/game_prediction2-0.1.9.tar.gz` & `tmp/game_prediction2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game_prediction2-0.1.9.tar", last modified: Mon Apr 22 09:46:52 2024, max compression
+gzip compressed data, was "game_prediction2-0.2.0.tar", last modified: Tue Apr 23 08:54:34 2024, max compression
```

## Comparing `game_prediction2-0.1.9.tar` & `game_prediction2-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-04-22 09:46:47.000000 game_prediction2-0.1.9/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.045434 game_prediction2-0.1.9/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.055434 game_prediction2-0.1.9/src/game_prediction2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-16 07:38:55.000000 game_prediction2-0.1.9/src/game_prediction2/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.055434 game_prediction2-0.1.9/src/game_prediction2/beam/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      184 2024-04-16 07:36:22.000000 game_prediction2-0.1.9/src/game_prediction2/beam/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1855 2024-04-22 05:12:47.000000 game_prediction2-0.1.9/src/game_prediction2/beam/decoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1125 2024-04-22 05:14:20.000000 game_prediction2-0.1.9/src/game_prediction2/beam/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2076 2024-04-22 05:14:05.000000 game_prediction2-0.1.9/src/game_prediction2/beam/searching.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1686 2024-04-16 07:24:24.000000 game_prediction2-0.1.9/src/game_prediction2/beam/succs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-04-16 07:35:57.000000 game_prediction2-0.1.9/src/game_prediction2/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.055434 game_prediction2-0.1.9/src/game_prediction2/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-03-16 09:09:26.000000 game_prediction2-0.1.9/src/game_prediction2/util/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/src/game_prediction2/util/aggregate/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-03-15 19:06:22.000000 game_prediction2-0.1.9/src/game_prediction2/util/aggregate/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-03-15 19:06:22.000000 game_prediction2-0.1.9/src/game_prediction2/util/aggregate/aggregate.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/src/game_prediction2/util/logprobs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      133 2024-04-16 07:19:37.000000 game_prediction2-0.1.9/src/game_prediction2/util/logprobs/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3341 2024-04-16 09:16:03.000000 game_prediction2-0.1.9/src/game_prediction2/util/logprobs/logprobs.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/src/game_prediction2/util/predict/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      100 2024-04-16 07:25:13.000000 game_prediction2-0.1.9/src/game_prediction2/util/predict/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1450 2024-04-22 05:14:36.000000 game_prediction2-0.1.9/src/game_prediction2/util/predict/predict.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/src/game_prediction2.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-22 09:46:52.000000 game_prediction2-0.1.9/src/game_prediction2.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-22 09:46:52.000000 game_prediction2-0.1.9/src/game_prediction2.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 09:46:52.000000 game_prediction2-0.1.9/src/game_prediction2.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       73 2024-04-22 09:46:52.000000 game_prediction2-0.1.9/src/game_prediction2.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       17 2024-04-22 09:46:52.000000 game_prediction2-0.1.9/src/game_prediction2.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:54:34.022890 game_prediction2-0.2.0/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-23 08:54:34.022890 game_prediction2-0.2.0/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      625 2024-04-23 08:54:30.000000 game_prediction2-0.2.0/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-23 08:54:34.022890 game_prediction2-0.2.0/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:54:34.022890 game_prediction2-0.2.0/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:54:34.022890 game_prediction2-0.2.0/src/game_prediction2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-22 10:45:01.000000 game_prediction2-0.2.0/src/game_prediction2/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      410 2024-04-23 08:54:00.000000 game_prediction2-0.2.0/src/game_prediction2/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:54:34.022890 game_prediction2-0.2.0/src/game_prediction2/beam/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-23 06:23:40.000000 game_prediction2-0.2.0/src/game_prediction2/beam/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      615 2024-04-23 08:05:09.000000 game_prediction2-0.2.0/src/game_prediction2/beam/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2520 2024-04-23 07:34:05.000000 game_prediction2-0.2.0/src/game_prediction2/beam/decoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2167 2024-04-23 06:33:52.000000 game_prediction2-0.2.0/src/game_prediction2/beam/predict.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3142 2024-04-23 08:07:12.000000 game_prediction2-0.2.0/src/game_prediction2/beam/searching.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1698 2024-04-23 08:48:43.000000 game_prediction2-0.2.0/src/game_prediction2/beam/succs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2687 2024-04-23 08:48:31.000000 game_prediction2-0.2.0/src/game_prediction2/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1574 2024-04-23 08:53:38.000000 game_prediction2-0.2.0/src/game_prediction2/manual.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:54:34.022890 game_prediction2-0.2.0/src/game_prediction2/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-23 05:17:55.000000 game_prediction2-0.2.0/src/game_prediction2/util/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      280 2024-04-23 06:39:04.000000 game_prediction2-0.2.0/src/game_prediction2/util/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-23 05:16:05.000000 game_prediction2-0.2.0/src/game_prediction2/util/aggregate.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3230 2024-04-23 08:47:01.000000 game_prediction2-0.2.0/src/game_prediction2/util/logprobs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1435 2024-04-23 06:38:53.000000 game_prediction2-0.2.0/src/game_prediction2/util/predict.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:54:34.022890 game_prediction2-0.2.0/src/game_prediction2.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      460 2024-04-23 08:54:34.000000 game_prediction2-0.2.0/src/game_prediction2.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      777 2024-04-23 08:54:34.000000 game_prediction2-0.2.0/src/game_prediction2.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-23 08:54:34.000000 game_prediction2-0.2.0/src/game_prediction2.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-04-23 08:54:34.000000 game_prediction2-0.2.0/src/game_prediction2.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       17 2024-04-23 08:54:34.000000 game_prediction2-0.2.0/src/game_prediction2.egg-info/top_level.txt
```

### Comparing `game_prediction2-0.1.9/pyproject.toml` & `game_prediction2-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "game-prediction2"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
     {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Game prediction, simplified. No edits, no GCP. Everything's just `AsyncIterables` in and out."
 dependencies = [
     "haskellian",
     "lcz",
     "chess-notation",
     "ramda",
     "chess",
     "numpy",
     "editdistance",
-    "chess-utils"
+    "chess-utils",
+    "lazy-loader"
 ]
 requires-python = ">=3.10"
 # readme = {file="README.md", content-type="text/markdown"}
 
 # [project.urls]
 # repo = "<GIT_REPO_URL>"
```

### Comparing `game_prediction2-0.1.9/src/game_prediction2/beam/main.py` & `game_prediction2-0.2.0/src/game_prediction2/beam/predict.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,33 @@
-from typing import AsyncIterable, Unpack
-import haskellian.asyn_iter as AI
+from typing import AsyncIterable, Iterable, Unpack
+from haskellian import asyn_iter as AI, iter as I
 from .succs import Logprob
-from .searching import search, SearchParams
-from .decoding import decode
+from .searching import search_sync, search_async, SearchParams
+from .decoding import decode_async, decode_sync
 
 @AI.lift
-def predict(logprobs: AsyncIterable[Logprob], **params: Unpack[SearchParams]):
+def predict_async(logprobs: AsyncIterable[Logprob], **params: Unpack[SearchParams]):
   """Beam decoding across the forest of moves stemming from `start_fens`
   - Yields predictions as the beams converge (i.e. agree on a single move) or the search stops (because no legal moves have high enough probability)
     - Thus, a bigger `beam_width` can increase accuracy but also prediction time by more than a constant factor
     
   Params:
   - `logprobs[ply](san, piece)`: (OCR) log-probability of `san` (which captures `piece`) at `ply`
   - `uci_prior(fens)`: batched prior distribution of legal moves (defaults to using `MaiaChess` with `Leela Chess Zero`)
   - `agg_logp(logp, logq)`: aggregation function of the OCR and prior log-probabilities. Defaults to a weighted geometric average giving the OCR probabilities 10x the importance. I.e. `(p^10 * q)^(1/11)` (but in log-space, ofc)
   """
-  beams = search(logprobs, **params)
-  return decode(beams)
+  beams = search_async(logprobs, **params)
+  return decode_async(beams)
+
+@I.lift
+def predict_sync(logprobs: Iterable[Logprob], **params: Unpack[SearchParams]):
+  """Beam decoding across the forest of moves stemming from `start_fens`
+  - Yields predictions as the beams converge (i.e. agree on a single move) or the search stops (because no legal moves have high enough probability)
+    - Thus, a bigger `beam_width` can increase accuracy but also prediction time by more than a constant factor
+    
+  Params:
+  - `logprobs[ply](san, piece)`: (OCR) log-probability of `san` (which captures `piece`) at `ply`
+  - `uci_prior(fens)`: batched prior distribution of legal moves (defaults to using `MaiaChess` with `Leela Chess Zero`)
+  - `agg_logp(logp, logq)`: aggregation function of the OCR and prior log-probabilities. Defaults to a weighted geometric average giving the OCR probabilities 10x the importance. I.e. `(p^10 * q)^(1/11)` (but in log-space, ofc)
+  """
+  beams = search_sync(logprobs, **params)
+  return decode_sync(beams)
```

### Comparing `game_prediction2-0.1.9/src/game_prediction2/beam/succs.py` & `game_prediction2-0.2.0/src/game_prediction2/beam/succs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Protocol, Iterable, TypedDict, NotRequired
 from dataclasses import dataclass
 import numpy as np
 import chess
-from chess_utils import CapturablePiece, parse, unchecked_san, captured_piece, fen_after
+from chess_utils import CapturablePiece, unchecked_san, captured_piece, fen_after
 
 class Logprob(Protocol):
-  def __call__(self, san: str, captured_piece: CapturablePiece | None) -> float:
+  def __call__(self, san: str, captured_piece: CapturablePiece | None, /) -> float:
     ...
     
 class AggregateLogps(Protocol):
-  def __call__(self, logp_ocr: float, logp_prior: float) -> float:
+  def __call__(self, logp_ocr: float, logp_prior: float, /) -> float:
     ...
     
 @dataclass
 class Node:
   fen: str
   sum_logp: float
   
@@ -34,23 +34,23 @@
     self.sum_logp = sum_logp or logp + parent.sum_logp
     self.logp = logp
     self.san = san
     self.parent = parent
     
 class SuccParams(TypedDict):
   logp_min: NotRequired[float]
-  ocr_logp_min: NotRequired[float]
+  logp_ocr_min: NotRequired[float]
 
 def successors(
-  node: Node, uci_priors: dict[str, float], lp: Logprob, agg_lp: AggregateLogps,
+  node: Node, uci_priors: dict[str, float], lp: Logprob, agg_lp: AggregateLogps, *,
   logp_min: float = np.log(0.02), logp_ocr_min: float = np.log(0.02),
 ) -> Iterable[Child]:
   board = chess.Board(node.fen)
   for uci, p_prior in uci_priors.items():
-    move = parse.uci(uci)
+    move = chess.Move.from_uci(uci)
     san = unchecked_san(board, move)
     logp_prior = np.log(p_prior)
     captured = captured_piece(board, move) if 'x' in san else None
     logp_ocr = lp(san, captured)
     if logp_ocr < logp_ocr_min:
       continue
     logp = agg_lp(logp_ocr, logp_prior)
```

### Comparing `game_prediction2-0.1.9/src/game_prediction2/util/aggregate/aggregate.py` & `game_prediction2-0.2.0/src/game_prediction2/util/aggregate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from collections import Counter
-import numpy as np
 
-def agg_max(preds: list[tuple[str, float]], k: int = None) -> list[tuple[str, float]]:
+def agg_max(preds: list[tuple[str, float]], k: int | None = None) -> list[tuple[str, float]]:
     """Aggregates by maxing probabilities of equal predictions"""
     acc = Counter()
     for move, prob in preds:
         cur = acc[move]
-        acc[move] = max(prob, float("-inf") if cur == 0 else cur) # Counter defaults to 0, but logprob's identity is log(0) = -inf
-    return acc.most_common(k)
+        # Counter defaults to 0, but logprob's identity is log(0) = -inf vvvvv
+        acc[move] = max(prob, float("-inf") if cur == 0 else cur) # type: ignore
+    return acc.most_common(k) # type: ignore
 
-def agg_union(preds: list[tuple[str, float]], k: int = None) -> list[tuple[str, float]]:
+def agg_union(preds: list[tuple[str, float]], k: int | None = None) -> list[tuple[str, float]]:
     """Aggregates by summing probabilities of equal predictions"""
+    import numpy as np
     acc = Counter()
     for move, prob in preds:
         acc[move] += np.exp(prob)
     return [(m, np.log(p)) for m, p in acc.most_common(k)]
```

### Comparing `game_prediction2-0.1.9/src/game_prediction2/util/logprobs/logprobs.py` & `game_prediction2-0.2.0/src/game_prediction2/util/logprobs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from editdistance import distance as edit_dist
 from itertools import zip_longest
 import numpy as np
 from pydantic import BaseModel
-from chess_notation.represent import representations, MotionStyles
-from chess_notation.styles import PawnCapture, PieceCapture
-from chess_notation.language import Language
-from chess_utils import CapturablePiece
-from ...beam import Logprob
+from chess_notation import representations, Language, MotionStyles, PawnCapture, PieceCapture, CapturedPiece
+from ..beam import Logprob
 
 def pseudo_logp(word: str, top_preds: list[tuple[str, float]]) -> float:
   """Approximates the log probability of `word` given a subset of the best outputs `top_preds` of a model.
   - `top_preds :: [(Pred, Logprob)]`: the top-k predictions of a model with probability distribution `P`
     - So, each `(pred, logp) in top_preds` holds `logp = log P(pred)`
   - If `word` is in `top_preds`, the real log-probability is returned
   - Otherwise, an approximation factor `alpha(p)` is computed as `1 - NED(word, p)` for every `p in preds`
@@ -39,31 +36,30 @@
     if self.piece_capture: styles.piece_captures = [self.piece_capture]
     return styles
   
   def langs(self) -> list[Language] | None:
     if self.lang is not None:
       return [self.lang]
     
-def max_pseudo_logp(san: str, captured_piece: CapturablePiece | None, top_preds: list[tuple[str, float]], ann: Annotations) -> float:
+def max_pseudo_logp(san: str, captured_piece: CapturedPiece | None, top_preds: list[tuple[str, float]], ann: Annotations) -> float:
   """Max `pseudo_logp` across all possible representations of `san`"""
   reprs = representations(san, motions=ann.motions(), captured_piece=captured_piece, languages=ann.langs() or ['CA', 'EN'])
   return max(pseudo_logp(r, top_preds) for r in reprs)
 
-def players_max_pseudo_logp(san: str, captured_piece: CapturablePiece | None, players_preds: list[list[tuple[str, float]]], annotations: list[Annotations] | None = None) -> float:
+def players_max_pseudo_logp(san: str, captured_piece: CapturedPiece | None, players_preds: list[list[tuple[str, float]]], annotations: list[Annotations] | None = None) -> float:
   """Max `max_pseudo_logp` across players"""
   annotations = annotations or [Annotations() for _ in players_preds]
   return max(
     max_pseudo_logp(san, captured_piece, preds, ann or Annotations())
     for preds, ann in zip_longest(players_preds, annotations)
       if preds is not None
   )
 
-
 def logprob(players_preds: list[list[tuple[str, float]]], annotations: list[Annotations] | None = None) -> Logprob:
   """Curried version of `players_max_pseudo_logp`"""
-  def _logprob(san: str, captured_piece: CapturablePiece | None):
+  def _logprob(san: str, captured_piece: CapturedPiece | None):
     return players_max_pseudo_logp(san, captured_piece, players_preds, annotations)
   return _logprob
   
 def weighted_geo_mean(logp: float, logq: float, a: float, b: float):
   """Weighted geometrical mean (`[p^a * q^b]^(1/(a+b))`) but in log-space"""
   return (a*logp + b*logq) / (a+b)
```

### Comparing `game_prediction2-0.1.9/src/game_prediction2/util/predict/predict.py` & `game_prediction2-0.2.0/src/game_prediction2/util/predict.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from typing import Protocol, Awaitable, AsyncIterable, TypedDict, NotRequired, Unpack
-from haskellian import promise as P, asyn_iter as AI
-from ..logprobs import logprob, Annotations
-from ...beam.succs import Logprob
+from haskellian import promise as P, asyn_iter as AI, iter as I
+from .logprobs import logprob, Annotations
+from ..beam.succs import Logprob
 
 class PredictFn(Protocol):
   """Batched predictions of plies `[from_ply, to_ply)` for all (1 or 2) players
   - Must return an array of shape `BATCH x PLAYERS x TOP_PREDS` of `(pred, logprob)` tuples
   """
   def __call__(self, from_ply: int, to_ply: int) -> Awaitable[list[list[list[tuple[str, float]]]]]:
     ...
 
 class BatchedParams(TypedDict):
-  max_moves: int
   start_ply: NotRequired[int]
   batch_size: NotRequired[int]
 
 class PrefetchedParams(BatchedParams):
   prefetch: NotRequired[int]
 
 @AI.lift
-async def batched_logprobs(predict: PredictFn, annotations: list[Annotations] | None = None, *, max_moves: int, start_ply: int = 0, batch_size: int = 8) -> AsyncIterable[list[Logprob]]:
-  for i in range(start_ply, max_moves, batch_size):
+async def batched_logprobs(predict: PredictFn, annotations: list[Annotations] | None = None, *, start_ply: int = 0, batch_size: int = 8) -> AsyncIterable[list[Logprob]]:
+  for i in I.range(start_ply, step=batch_size):
     preds = await P.wait(predict(i, i+batch_size))
+    if preds == []:
+      return
     yield [logprob(ps, annotations) for ps in preds]
 
-@AI.lift
 def prefetched_logprobs(predict: PredictFn, annotations: list[Annotations] | None = None, *, prefetch: int = 2, **p: Unpack[BatchedParams]) -> AsyncIterable[Logprob]:
   """Async iterable of `Logprob`s by calling `predict`. Prefetches and batches requests"""
-  prefetched = batched_logprobs(predict, annotations, **p) \
-    .prefetch(prefetch)
-  return AI.flatten(prefetched)
+  return batched_logprobs(predict, annotations, **p) \
+    .prefetch(prefetch) \
+    .f(AI.flatten).value
```

