# Comparing `tmp/game_prediction2-0.1.8.tar.gz` & `tmp/game_prediction2-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game_prediction2-0.1.8.tar", last modified: Thu Apr 18 13:07:49 2024, max compression
+gzip compressed data, was "game_prediction2-0.1.9.tar", last modified: Mon Apr 22 09:46:52 2024, max compression
```

## Comparing `game_prediction2-0.1.8.tar` & `game_prediction2-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-04-18 13:07:46.000000 game_prediction2-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.955339 game_prediction2-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-16 07:38:55.000000 game_prediction2-0.1.8/src/game_prediction2/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/beam/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      184 2024-04-16 07:36:22.000000 game_prediction2-0.1.8/src/game_prediction2/beam/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1933 2024-04-16 07:38:02.000000 game_prediction2-0.1.8/src/game_prediction2/beam/decoding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1125 2024-04-16 07:37:30.000000 game_prediction2-0.1.8/src/game_prediction2/beam/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2068 2024-04-16 11:55:55.000000 game_prediction2-0.1.8/src/game_prediction2/beam/searching.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1686 2024-04-16 07:24:24.000000 game_prediction2-0.1.8/src/game_prediction2/beam/succs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-04-16 07:35:57.000000 game_prediction2-0.1.8/src/game_prediction2/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/util/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-03-16 09:09:26.000000 game_prediction2-0.1.8/src/game_prediction2/util/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/util/aggregate/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-03-15 19:06:22.000000 game_prediction2-0.1.8/src/game_prediction2/util/aggregate/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-03-15 19:06:22.000000 game_prediction2-0.1.8/src/game_prediction2/util/aggregate/aggregate.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/util/logprobs/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      133 2024-04-16 07:19:37.000000 game_prediction2-0.1.8/src/game_prediction2/util/logprobs/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3341 2024-04-16 09:16:03.000000 game_prediction2-0.1.8/src/game_prediction2/util/logprobs/logprobs.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2/util/predict/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      100 2024-04-16 07:25:13.000000 game_prediction2-0.1.8/src/game_prediction2/util/predict/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1468 2024-04-16 07:27:05.000000 game_prediction2-0.1.8/src/game_prediction2/util/predict/predict.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-18 13:07:49.965339 game_prediction2-0.1.8/src/game_prediction2.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-18 13:07:49.000000 game_prediction2-0.1.8/src/game_prediction2.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-18 13:07:49.000000 game_prediction2-0.1.8/src/game_prediction2.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-18 13:07:49.000000 game_prediction2-0.1.8/src/game_prediction2.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       73 2024-04-18 13:07:49.000000 game_prediction2-0.1.8/src/game_prediction2.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       17 2024-04-18 13:07:49.000000 game_prediction2-0.1.8/src/game_prediction2.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      606 2024-04-22 09:46:47.000000 game_prediction2-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.045434 game_prediction2-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.055434 game_prediction2-0.1.9/src/game_prediction2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       63 2024-04-16 07:38:55.000000 game_prediction2-0.1.9/src/game_prediction2/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.055434 game_prediction2-0.1.9/src/game_prediction2/beam/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      184 2024-04-16 07:36:22.000000 game_prediction2-0.1.9/src/game_prediction2/beam/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1855 2024-04-22 05:12:47.000000 game_prediction2-0.1.9/src/game_prediction2/beam/decoding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1125 2024-04-22 05:14:20.000000 game_prediction2-0.1.9/src/game_prediction2/beam/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2076 2024-04-22 05:14:05.000000 game_prediction2-0.1.9/src/game_prediction2/beam/searching.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1686 2024-04-16 07:24:24.000000 game_prediction2-0.1.9/src/game_prediction2/beam/succs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      976 2024-04-16 07:35:57.000000 game_prediction2-0.1.9/src/game_prediction2/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.055434 game_prediction2-0.1.9/src/game_prediction2/util/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-03-16 09:09:26.000000 game_prediction2-0.1.9/src/game_prediction2/util/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/src/game_prediction2/util/aggregate/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       57 2024-03-15 19:06:22.000000 game_prediction2-0.1.9/src/game_prediction2/util/aggregate/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      737 2024-03-15 19:06:22.000000 game_prediction2-0.1.9/src/game_prediction2/util/aggregate/aggregate.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/src/game_prediction2/util/logprobs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      133 2024-04-16 07:19:37.000000 game_prediction2-0.1.9/src/game_prediction2/util/logprobs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3341 2024-04-16 09:16:03.000000 game_prediction2-0.1.9/src/game_prediction2/util/logprobs/logprobs.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/src/game_prediction2/util/predict/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      100 2024-04-16 07:25:13.000000 game_prediction2-0.1.9/src/game_prediction2/util/predict/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1450 2024-04-22 05:14:36.000000 game_prediction2-0.1.9/src/game_prediction2/util/predict/predict.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:46:52.065434 game_prediction2-0.1.9/src/game_prediction2.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      433 2024-04-22 09:46:52.000000 game_prediction2-0.1.9/src/game_prediction2.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-22 09:46:52.000000 game_prediction2-0.1.9/src/game_prediction2.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 09:46:52.000000 game_prediction2-0.1.9/src/game_prediction2.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       73 2024-04-22 09:46:52.000000 game_prediction2-0.1.9/src/game_prediction2.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       17 2024-04-22 09:46:52.000000 game_prediction2-0.1.9/src/game_prediction2.egg-info/top_level.txt
```

### Comparing `game_prediction2-0.1.8/pyproject.toml` & `game_prediction2-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "game-prediction2"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Game prediction, simplified. No edits, no GCP. Everything's just `AsyncIterables` in and out."
 dependencies = [
     "haskellian",
     "lcz",
```

### Comparing `game_prediction2-0.1.8/src/game_prediction2/beam/decoding.py` & `game_prediction2-0.1.9/src/game_prediction2/beam/decoding.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from typing import AsyncIterable
 import numpy as np
 import ramda as R
-from haskellian.core import pipe
-import haskellian.iterables as hk
-import haskellian.asyn.iter as AI
+from haskellian import iter as I, Iter, Pipe, asyn_iter as AI
 from .succs import Node, Child
 
 @R.curry
 def reconstruct(node: Node, max_depth: int | None = None, with_probs: bool = True) -> list[tuple[str, float]] | list[str]:
   """Reconstruct backwards from `node` (keeping log-probs as they are)
   - `max_depth`: limit of backward steps
   """
@@ -19,29 +17,28 @@
       else:
         return curr
     case _:
       return []
     
 def exp(preds_logps: list[tuple[str, float]]) -> list[tuple[str, float]]:
   """Exponentiate log-probabilities"""
-  preds, logps = hk.unzip(preds_logps)
+  preds, logps = I.unzip(preds_logps)
   exps = np.exp(logps)
   return list(zip(preds, exps))
 
 def convergence(beam: list[Node], max_depth: int | None = None) -> int:
   """Convergence point: ply back to which all lines of the `beam` agree on the best move
   - `max_depth`: limit of backward steps (from the current beam's ply)
   """
-  return pipe(
-    map(reconstruct(max_depth=max_depth, with_probs=False), beam), # line of every beam
-    hk.transpose, # moves at every ply
-    hk.map(set), # aka uniq
-    hk.take_while(lambda uniq_preds: len(uniq_preds) == 1),
-    list, len
-)
+  return Iter(beam) \
+    .map(reconstruct(max_depth=max_depth, with_probs=False)) \
+    .i(I.transpose) \
+    .map(set) \
+    .take_while(lambda uniq_preds: len(uniq_preds) == 1) \
+    .f(list).f(len).value
   
 async def decode(beams: AsyncIterable[list[Node]]) -> AsyncIterable[list[tuple[str, float]]]:
   last_converged = 0
   beam = None
   async for ply, beam in AI.enumerate(beams):
     converged = convergence(beam, max_depth=ply-last_converged)
     if converged > 0:
```

### Comparing `game_prediction2-0.1.8/src/game_prediction2/beam/main.py` & `game_prediction2-0.1.9/src/game_prediction2/beam/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import AsyncIterable, Unpack
-import haskellian.asyn.iter as AI
+import haskellian.asyn_iter as AI
 from .succs import Logprob
 from .searching import search, SearchParams
 from .decoding import decode
 
 @AI.lift
 def predict(logprobs: AsyncIterable[Logprob], **params: Unpack[SearchParams]):
   """Beam decoding across the forest of moves stemming from `start_fens`
```

### Comparing `game_prediction2-0.1.8/src/game_prediction2/beam/searching.py` & `game_prediction2-0.1.9/src/game_prediction2/beam/searching.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Protocol, Iterable, AsyncIterable, Unpack, NotRequired
-import haskellian.iterables as hk
-import haskellian.asyn.iter as AI
+from haskellian import iter as I, asyn_iter as AI
+from itertools import starmap
 import chess
 import lcz
 from ..util import logprobs as logps
 from .succs import AggregateLogps, SuccParams, Logprob, successors, Node
 
 class UCIPrior(Protocol):
   """Evaluates a batch of `fens` into `UCI -> Probability` mappings"""
@@ -34,15 +34,15 @@
   beam_width = p.get('beam_width', lambda _: 4)
   fen = p.get('fen') or chess.STARTING_FEN
 
   beam: Beam = [Node(fen)]
   priors = uci_prior([fen])
   async for i, lp in AI.enumerate(logprobs):
     inputs = zip(beam, priors)
-    nested_succs = hk.starmap(lambda node, prior: successors(node, prior, lp, agg_logp))(inputs)
-    succs = list(hk.flatten(nested_succs))
+    nested_succs = starmap(lambda node, prior: successors(node, prior, lp, agg_logp), inputs)
+    succs = list(I.flatten(nested_succs))
     if succs == []:
       return
     else:
       beam = sorted(succs, key=lambda x: x.sum_logp, reverse=True)[:beam_width(i)]
       priors = uci_prior(n.fen for n in beam)
       yield beam
```

### Comparing `game_prediction2-0.1.8/src/game_prediction2/beam/succs.py` & `game_prediction2-0.1.9/src/game_prediction2/beam/succs.py`

 * *Files identical despite different names*

### Comparing `game_prediction2-0.1.8/src/game_prediction2/main.py` & `game_prediction2-0.1.9/src/game_prediction2/main.py`

 * *Files identical despite different names*

### Comparing `game_prediction2-0.1.8/src/game_prediction2/util/aggregate/aggregate.py` & `game_prediction2-0.1.9/src/game_prediction2/util/aggregate/aggregate.py`

 * *Files identical despite different names*

### Comparing `game_prediction2-0.1.8/src/game_prediction2/util/logprobs/logprobs.py` & `game_prediction2-0.1.9/src/game_prediction2/util/logprobs/logprobs.py`

 * *Files identical despite different names*

### Comparing `game_prediction2-0.1.8/src/game_prediction2/util/predict/predict.py` & `game_prediction2-0.1.9/src/game_prediction2/util/predict/predict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Protocol, Awaitable, AsyncIterable, TypedDict, NotRequired, Unpack
-import haskellian.asyn.promises as P
-import haskellian.asyn.iter as AI
+from haskellian import promise as P, asyn_iter as AI
 from ..logprobs import logprob, Annotations
 from ...beam.succs import Logprob
 
 class PredictFn(Protocol):
   """Batched predictions of plies `[from_ply, to_ply)` for all (1 or 2) players
   - Must return an array of shape `BATCH x PLAYERS x TOP_PREDS` of `(pred, logprob)` tuples
   """
```

### Comparing `game_prediction2-0.1.8/src/game_prediction2.egg-info/SOURCES.txt` & `game_prediction2-0.1.9/src/game_prediction2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

