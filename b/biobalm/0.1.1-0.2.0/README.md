# Comparing `tmp/biobalm-0.1.1.tar.gz` & `tmp/biobalm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biobalm-0.1.1.tar", last modified: Thu Apr 11 16:06:15 2024, max compression
+gzip compressed data, was "biobalm-0.2.0.tar", last modified: Tue Apr 23 16:46:01 2024, max compression
```

## Comparing `biobalm-0.1.1.tar` & `biobalm-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:06:15.880384 biobalm-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-11 16:06:07.000000 biobalm-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-11 16:06:15.880384 biobalm-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-11 16:06:07.000000 biobalm-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:06:15.880384 biobalm-0.1.1/biobalm/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:06:15.880384 biobalm-0.1.1/biobalm/_sd_algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/compute_attractor_seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_attractor_seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_bfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_dfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_minimal_spaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_source_SCCs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/_sd_algorithms/expand_to_target.py
--rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/control.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/interaction_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17167 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/motif_avoidant.py
--rw-r--r--   0 runner    (1001) docker     (127)    16211 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/petri_net_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/space_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37095 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/succession_diagram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/symbolic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19392 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/trappist_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-11 16:06:07.000000 biobalm-0.1.1/biobalm/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 16:06:15.880384 biobalm-0.1.1/biobalm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-11 16:06:15.000000 biobalm-0.1.1/biobalm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-11 16:06:15.000000 biobalm-0.1.1/biobalm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 16:06:15.000000 biobalm-0.1.1/biobalm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-11 16:06:15.000000 biobalm-0.1.1/biobalm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 16:06:15.000000 biobalm-0.1.1/biobalm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-11 16:06:07.000000 biobalm-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-11 16:06:15.880384 biobalm-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:46:01.754237 biobalm-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-23 16:45:41.000000 biobalm-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-23 16:46:01.754237 biobalm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-23 16:45:41.000000 biobalm-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:46:01.754237 biobalm-0.2.0/biobalm/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5393 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_pint_reachability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:46:01.754237 biobalm-0.2.0/biobalm/_sd_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_sd_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_sd_algorithms/expand_attractor_seeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_sd_algorithms/expand_bfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_sd_algorithms/expand_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_sd_algorithms/expand_minimal_spaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10033 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_sd_algorithms/expand_source_SCCs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_sd_algorithms/expand_to_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:46:01.754237 biobalm-0.2.0/biobalm/_sd_attractors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_sd_attractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31772 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_sd_attractors/attractor_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/_sd_attractors/attractor_symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20234 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/interaction_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16336 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/petri_net_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/space_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55367 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/succession_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/symbolic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19392 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/trappist_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-23 16:45:41.000000 biobalm-0.2.0/biobalm/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:46:01.754237 biobalm-0.2.0/biobalm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-23 16:46:01.000000 biobalm-0.2.0/biobalm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-23 16:46:01.000000 biobalm-0.2.0/biobalm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:46:01.000000 biobalm-0.2.0/biobalm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 16:46:01.000000 biobalm-0.2.0/biobalm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 16:46:01.000000 biobalm-0.2.0/biobalm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-23 16:45:41.000000 biobalm-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 16:46:01.754237 biobalm-0.2.0/setup.cfg
```

### Comparing `biobalm-0.1.1/LICENSE` & `biobalm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/PKG-INFO` & `biobalm-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: biobalm
-Version: 0.1.1
+Version: 0.2.0
 Summary: Boolean Attractor Landscape Mapper
 Author-email: Jordan Rozum <jrozum@binghamton.edu>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: biodivine_aeon==1.0.0a4
+Requires-Dist: biodivine_aeon==1.0.0a6
 Requires-Dist: clingo>=5.6.2
 Requires-Dist: networkx>=2.8.8
-Requires-Dist: pypint>=1.6.2
+Provides-Extra: pint
+Requires-Dist: pypint==1.6.2; extra == "pint"
 
 [![PyPI](https://img.shields.io/pypi/v/biobalm?style=flat-square)](https://pypi.org/project/biobalm/) 
 [![Api Docs](https://img.shields.io/badge/docs-api-yellowgreen?style=flat-square)](https://jcrozum.github.io/biobalm/)
 [![Continuous integration](https://img.shields.io/github/actions/workflow/status/jcrozum/biobalm/test.yml?branch=main&style=flat-square)](https://github.com/jcrozum/biobalm/actions?query=workflow%3Atest)
 [![Coverage](https://img.shields.io/codecov/c/github/jcrozum/biobalm?style=flat-square)](https://codecov.io/gh/jcrozum/biobalm) 
 [![GitHub issues](https://img.shields.io/github/issues/jcrozum/biobalm?style=flat-square)](https://github.com/jcrozum/biobalm/issues) 
 [![License](https://img.shields.io/pypi/l/biobalm?style=flat-square)](https://github.com/jcrozum/biobalm/blob/main/LICENSE)
```

### Comparing `biobalm-0.1.1/README.md` & `biobalm-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm/_sd_algorithms/__init__.py` & `biobalm-0.2.0/biobalm/_sd_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm/_sd_algorithms/expand_attractor_seeds.py` & `biobalm-0.2.0/biobalm/_sd_algorithms/expand_attractor_seeds.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from biobalm.succession_diagram import SuccessionDiagram
 
-import biobalm
-import biobalm.succession_diagram
-from biobalm.motif_avoidant import make_retained_set
+from biobalm.types import BooleanSpace
 from biobalm.space_utils import intersect
 from biobalm.trappist_core import compute_fixed_point_reduced_STG
+from biobalm._sd_attractors.attractor_candidates import make_heuristic_retained_set
+from biodivine_aeon import AsynchronousGraph
 
 
 def expand_attractor_seeds(sd: SuccessionDiagram, size_limit: int | None = None):
     """
     See `SuccessionDiagram.expand_attractor_seeds` for documentation.
     """
 
     # First, expand the succession diagram such that all minimal trap spaces are
     # found. This reduces the amount of work performed in this algorithm,
     # because for every attractor in a minimal trap space, we already have the
     # closest trap space, now we just need to do the same for (potential)
     # motif-avoidant attractors.
     sd.expand_minimal_spaces(size_limit)
 
-    if biobalm.succession_diagram.DEBUG:
+    if sd.config["debug"]:
         print(
             "Minimal trap space expansion finished. Proceeding to attractor expansion."
         )
 
     root = sd.root()
     seen = set([root])
     stack: list[tuple[int, list[int] | None]] = [(root, None)]
@@ -65,49 +65,61 @@
                 # The next node to explore is expanded (by some previous procedure)
                 # but not "seen" in this search yet. We need to visit this node
                 # regardless of other conditions
                 break
             # Now, we need to asses if the next successor has some candidate states which
             # are not covered by the already expanded children.
 
-            successor_space = sd.node_data(successors[-1])["space"]
-            retained_set = make_retained_set(
-                sd.symbolic, sd.node_nfvs(node), successor_space
-            )
+            s = successors[-1]
+
+            successor_space = sd.node_data(s)["space"]
+            successor_bn = sd.node_percolated_network(s, compute=True)
+            successor_nfvs = sd.node_percolated_nfvs(s, compute=True)
+            successor_pn = sd.node_percolated_petri_net(s, compute=True)
+            successor_graph = AsynchronousGraph(successor_bn)
 
             avoid_or_none = [
                 intersect(successor_space, child) for child in expanded_motifs
             ]
             avoid = [x for x in avoid_or_none if x is not None]
+            avoid_restricted: list[BooleanSpace] = []
+            for x in avoid:
+                y: BooleanSpace = {
+                    var: val for (var, val) in x.items() if var not in successor_space
+                }
+                avoid_restricted.append(y)
+
+            retained_set = make_heuristic_retained_set(
+                successor_graph, successor_nfvs, avoid
+            )
 
             successor_seeds = compute_fixed_point_reduced_STG(
-                sd.petri_net,
+                successor_pn,
                 retained_set,
-                ensure_subspace=successor_space,
-                avoid_subspaces=avoid,
+                avoid_subspaces=avoid_restricted,
                 solution_limit=1,
             )
 
             if len(successor_seeds) == 0:
                 # At this point, we know that this successor is not expanded and
                 # there are either no candidate states in it, or all candidate
                 # states are already covered by some other expanded successor.
                 successors.pop()
                 continue
 
-            if biobalm.succession_diagram.DEBUG:
+            if sd.config["debug"]:
                 print(
                     f"[{node}] Found successor with new attractor candidate seeds. Expand node {successors[-1]}."
                 )
 
             break
 
         if len(successors) == 0:
             # Everything is done for this `node` and we can continue to the next one.
-            if biobalm.succession_diagram.DEBUG:
+            if sd.config["debug"]:
                 print(f"[{node}] Finished node attractor expansion.")
             continue
 
         s = successors.pop()
         seen.add(s)
         # Push the node back with the remaining successors.
         stack.append((node, successors))
```

### Comparing `biobalm-0.1.1/biobalm/_sd_algorithms/expand_bfs.py` & `biobalm-0.2.0/biobalm/_sd_algorithms/expand_bfs.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm/_sd_algorithms/expand_dfs.py` & `biobalm-0.2.0/biobalm/_sd_algorithms/expand_dfs.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm/_sd_algorithms/expand_minimal_spaces.py` & `biobalm-0.2.0/biobalm/_sd_algorithms/expand_minimal_spaces.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm/_sd_algorithms/expand_source_SCCs.py` & `biobalm-0.2.0/biobalm/_sd_algorithms/expand_source_SCCs.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,17 @@
 
             sub_space = source_comb
             sub_space.update(perc_space)
 
             next_level.append(sd._ensure_node(root, sub_space))  # type: ignore
 
         sd.node_data(root)["expanded"] = True
-        sd.node_data(root)["attractors"] = []  # no need to look for attractors here
+        sd.node_data(root)[
+            "attractor_seeds"
+        ] = []  # no need to look for attractors here
         current_level = next_level
         next_level = []
 
     while len(current_level) > 0:
         if DEBUG:
             print(f"{current_level=}")
 
@@ -128,15 +130,17 @@
     # Finally, expand the sd in a usual way.
     # TODO: motif avoidance that is already calculated in the source SCCs should be used here somehow.
     if DEBUG:
         print(f"{final_level=}")
     for node_id in final_level:
         # These assertions should be unnecessary, but just to be sure.
         assert not sd.node_data(node_id)["expanded"]  # expand nodes from here
-        assert sd.node_data(node_id)["attractors"] is None  # check attractors from here
+        assert (
+            sd.node_data(node_id)["attractor_seeds"] is None
+        )  # check attractors from here
 
         # restore this once we allow all expansion algorithms to expand from a node
         # expander(sd, node_id)
         sd.expand_bfs(node_id)
 
     return True
```

### Comparing `biobalm-0.1.1/biobalm/_sd_algorithms/expand_to_target.py` & `biobalm-0.2.0/biobalm/_sd_algorithms/expand_to_target.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm/control.py` & `biobalm-0.2.0/biobalm/control.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm/drivers.py` & `biobalm-0.2.0/biobalm/drivers.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm/interaction_graph_utils.py` & `biobalm-0.2.0/biobalm/interaction_graph_utils.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm/motif_avoidant.py` & `biobalm-0.2.0/biobalm/petri_net_translation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,430 +1,452 @@
 """
-A module which provides utility methods for detecting motif-avoidant attractors
-within a terminal restriction space.
+Utilities for translating Boolean networks into Petri nets.
+
+Implements the translation from a `BooleanNetwork` object into a Petri net that
+can be processed by Trappist (for finding trap spaces). The Petri net is
+represented as a `networkx.DiGraph`, with nodes having either a `kind=place` or
+a `kind=transition` attribute.
+
+The variable names in the network have to be "sanitized" before translation. In
+particular, this means they can't use any special characters beyond "_". In the
+resulting Petri net, we then use a "b0_*" and "b1_*" prefix to distinguish the
+"zero" and "one" places created for each variable. This is also important for
+`clingo`, as we have to guarantee that in our logic program, symbols start with
+a lowercase letter.
 """
 
 from __future__ import annotations
 
-import random
-from functools import reduce
 from typing import TYPE_CHECKING
 
-from networkx import DiGraph  # type: ignore
-from pypint import Goal, InMemoryModel  # type:ignore
+if TYPE_CHECKING:
+    from typing import Generator
+
+    from biodivine_aeon import Bdd, BooleanNetwork
+
+    from biobalm.types import BooleanSpace
 
-from biobalm.petri_net_translation import place_to_variable
-from biobalm.space_utils import dnf_function_is_true, remove_state_from_dnf
-from biobalm.symbolic_utils import (
-    function_eval,
-    function_is_true,
-    state_list_to_bdd,
-    state_to_bdd,
+import copy
+import re
+from typing import cast
+
+from biodivine_aeon import (
+    BddPartialValuation,
+    BddVariableSet,
+    BoolType,
+    SymbolicContext,
 )
-from biobalm.types import BooleanSpace
+from networkx import DiGraph  # type: ignore
 
-if TYPE_CHECKING:
-    from biodivine_aeon import AsynchronousGraph, Bdd
+# Enables statistics logging.
+DEBUG = False
+"""Enables debug logging to stdout."""
 
 
-def make_retained_set(
-    graph: AsynchronousGraph,
-    nfvs: list[str],
-    space: BooleanSpace,
-    child_spaces: list[BooleanSpace] | None = None,
-) -> BooleanSpace:
-    """
-    Calculate the retained set for a given `space`.
-
-    The retained set is technically a space-like object that describes the
-    variables which have to be fixed in order for the network to lose all
-    complex attractors. However, note that this really means changing the update
-    functions. This is not a trap space that only contains fixed-points,
-    but a description of how the network must be modified to eliminate
-    all complex attractors in the given `space`.
-
-    The construction guarantees that any complex attractor of the old
-    network will manifest as at least one fixed-point in the new network. But this
-    network modification is not implemented here. This method only generates
-    the necessary list of variables and values.
-
-    Finally, note that the method uses a heuristic to select values
-    that should lead to the least amount of fixed-points in
-    the modified network.
+def sanitize_network_names(network: BooleanNetwork, check_only: bool = False):
+    """
+    Rename variables in a network so that they can be safely used in Trappist.
+
+    Verifies that all network variable names contain only alphanumeric
+    characters and underscores. If this is not the case, attempts to rename the
+    variables to make them compliant. Returns a *copy* of the original network
+    that only uses sanitized names.
+
+    Note that AEON should already prune away most of the special characters when
+    parsing models, but it still allows names like `Gene_{Subscript}` (i.e.
+    curly brackets) which we have to sanitize here.
+
+    If `check_only=True` is specified, no renaming takes place and the function
+    fails with a `RuntimeError` instead.
 
     Parameters
     ----------
-    graph : AsynchronousGraph
-        The symbolic update functions stored as an `AsynchronousGraph` object
-        from the `biodivine_aeon` library.
-    nfvs : list[str]
-        The list of variables in the NFVS that is valid for a network
-        restricted to the given `space`.
-    space : BooleanSpace
-        A :class:`BooleanSpace<biobalm.types.BooleanSpace>` object describing the
-        current trap space.
-    child_spaces : list[BooleanSpace] | None, optional
-        A list of :class:`BooleanSpace<biobalm.types.BooleanSpace>` objects
-        describing the child spaces of the current node. Only attractors that
-        are not in the child spaces are considered. If no child spaces are
-        provided, then all attractors are considered.
+    network : BooleanNetwork
+        The network to sanitize.
+    check_only : bool
+        If `True`, no renaming takes place and the function fails with a
+        `RuntimeError` if the network contains invalid variable names.
 
     Returns
     -------
-    BooleanSpace
-        A :class:`BooleanSpace<biobalm.types.BooleanSpace>` object describing the
-        retained set.
-    """
-
-    if child_spaces is None:
-        child_spaces = []
-
-    # Initially, the retained set only contains the fixed values from the
-    # current node space (this elimiantes unnecessary Petri net transitions for
-    # values which we already proved are constant).
-    #
-    # In the following code, we then extend the retained set based on the
-    # model's NFVS and the current child spaces.
-    retained_set = space.copy()
-
-    # First, if there are any child spaces present, we extend the retained set
-    # with the values from the one that has the least amount of fixed variables
-    # shared with the NFVS.
-    if len(child_spaces) > 0:
-        # Find the child space that has the fewest nodes in common with the NFVS:
-        least_common_child_space = child_spaces[0]
-        least_common_nodes = len(set(least_common_child_space) & set(nfvs))
-        for child_space in child_spaces:
-            common_nodes = len(set(child_space) & set(nfvs))
-            if common_nodes < least_common_nodes:
-                least_common_nodes = common_nodes
-                least_common_child_space = child_space
-
-        for x in least_common_child_space:
-            if (x not in retained_set) and (x in nfvs):
-                retained_set[x] = least_common_child_space[x]
-
-    # Then, set the remaining NFVS variables based on the majority output value
-    # in the update function of the relevant variable.
-    for x in nfvs:
-        if x in retained_set:
-            continue
-
-        fn_bdd = graph.mk_update_function(x)
-
-        # If most of the function is positive, we set the value
-        # to `1`, otherwise set it to `0`.
-        if fn_bdd.cardinality() > fn_bdd.l_not().cardinality():
-            retained_set[x] = 1
-        else:
-            retained_set[x] = 0
+    BooleanNetwork
+        A copy of the original network with sanitized variable names.
+    """
+    network = copy.copy(network)
+    for var in network.variables():
+        name = network.get_variable_name(var)
+        if not re.match("^[a-zA-Z0-9_]+$", name):
+            if check_only:
+                raise RuntimeError(f"Found unsanitized variable: `{name}`.")
+            # Replace all invalid characters with an underscore
+            new_name = re.sub("[^a-zA-Z0-9_]", "_", name)
+            while True:
+                try:
+                    network.set_variable_name(var, new_name)
+                    break
+                except Exception:
+                    # Name clash happened. Try to resolve this by adding an extra underscore to
+                    # the variable name. In theory, this can repeat until a unique name is found.
+                    new_name = "_" + new_name
 
-    return retained_set
+    return network
 
 
-def detect_motif_avoidant_attractors(
-    graph: AsynchronousGraph,
-    petri_net: DiGraph,
-    candidates: list[BooleanSpace],
-    terminal_restriction_space: Bdd,
-    max_iterations: int,
-    is_in_an_mts: bool = False,
-) -> list[BooleanSpace]:
-    """
-    Determine which seed states from the `candidates` list map to true
-    motif-avoidant attractors.
-
-    Assumes that all attractors in the `terminal_restriction_space` are
-    covered by at least one state in `candidates`. Eliminates all states
-    from `candidates` that are provably not in an attractor, or that correspond
-    to an attractor that is already covered by some other candidate.
-
-    The method consists of two steps: initial pruning, and exact reachability
-    analysis. As such, the result is always complete. However, some of the
-    parameters can be used to adjust the initial pruning step.
-
-    If `is_in_an_mts` is set, the method assumes the `candidates` are members
-    of a minimal trap space. In such case, a different simulation algorithm
-    is used for initial pruning. Furthermore, `max_iterations` can be used to
-    to limit the time spent on the initial pruning step.
+def variable_to_place(variable: str, positive: bool) -> str:
+    """
+    Generate a Petri net place name from a network variable name.
 
     Parameters
     ----------
-    graph : AsynchronousGraph
-        The symbolic update functions stored as an `AsynchronousGraph` object
-        from the `biodivine_aeon` library.
-    petri_net : DiGraph
-        The Petri net representation of the update functions.
-    candidates : list[BooleanSpace]
-        A list of :class:`BooleanSpace<biobalm.types.BooleanSpace>` objects
-        describing the candidate seed states.
-    terminal_restriction_space : Bdd
-        A symbolic set of states which contains all motif avoidant attractors
-        in question (i.e. if a candidate state can leave this set, the candidate
-        cannot be an attractor).
-    max_iterations : int
-        Specifies how much time should be spent on the simpler preprocessing methods.
-    is_in_an_mts : bool, optional
-        By default `False`. If `True`, then we assume that the candidates lie
-        within a minimal trap space, enabling certain optimizations. If
-        incorrectly set to `True`, the result is undefined.
+    variable : str
+        The name of the network variable.
+    positive : bool
+        `True` if the place corresponding to the variable should be positive,
+        `False` if it shoudl be negative.
 
     Returns
     -------
-    list[BooleanSpace]
-        A list of :class:`BooleanSpace<biobalm.types.BooleanSpace>` objects
-        describing the motif-avoidant attractors among the input candidate set.
-    """
-    if len(candidates) == 0:
-        return []
-
-    if len(candidates) == 1 and is_in_an_mts:
-        return candidates
-
-    candidates = _preprocess_candidates(
-        graph,
-        candidates,
-        terminal_restriction_space,
-        max_iterations,
-        is_in_an_mts=is_in_an_mts,
-    )
-
-    if len(candidates) == 0:
-        return []
-
-    if len(candidates) == 1 and is_in_an_mts:
-        return candidates
-
-    return _filter_candidates(petri_net, candidates, terminal_restriction_space)
-
-
-def _preprocess_candidates(
-    graph: AsynchronousGraph,
-    candidates: list[BooleanSpace],
-    terminal_restriction_space: Bdd,
-    max_iterations: int,
-    is_in_an_mts: bool = False,
-    simulation_seed: int = 0,
-) -> list[BooleanSpace]:
-    """
-    A fast but incomplete method for eliminating spurious attractor candidates.
-
-    The idea is to build the symbolic encoding of the given `network`, and then
-    randomly simulate transitions for individual states, trying to reach a state
-    outside of the `terminal_restriction_space`.
-
-    TODO (2): We could probably make this algorithm slighlty less random by doing
-    a limited version of symbolic reachability. I.e. instead of simulating just one
-    state transition in each step, compute the whole successor BDD and then test
-    against that. Once the BDD becomes too large after several steps, we can just
-    pick a single state from it and start again. Sam: I'll add a version of this
-    later, once we can actually benchmark how it performs :)
-    """
-    # A random generator initialized with a fixed seed. Ensures simulation
-    # is randomized but deterministic.
-    generator = random.Random(simulation_seed)
-
-    variables = graph.network_variable_names()
-    update_functions = {var: graph.mk_update_function(var) for var in variables}
-
-    # Use stochastic simulation to prune the set of candidate states.
-    # We use different simulation approach depending on whether this space
-    # is a minimal trap or not. In previous work, this was shown to work
-    # well, but in the future we need to better document the resoning
-    # behind these two algorithms.
-    if not is_in_an_mts:
-        # Copy is sufficient because we won't be modifying the states within the set.
-        candidates_dnf = candidates.copy()
-        filtered_candidates: list[BooleanSpace] = []
-        for state in candidates:
-            # Remove the state from the candidates. If we can prove that is
-            # is not an attractor, we will put it back.
-            candidates_dnf = remove_state_from_dnf(candidates_dnf, state)
-
-            simulation = state.copy()  # A copy of the state that we can overwrite.
-            is_valid_candidate = True
-            for _ in range(max_iterations):
-                # Advance all variables by one step in random order.
-                generator.shuffle(variables)
-                for var in variables:
-                    step = function_eval(update_functions[var], simulation)
-                    assert step is not None
-                    simulation[var] = step
-
-                if dnf_function_is_true(candidates_dnf, simulation):
-                    # The state can reach some other state in the candidate
-                    # set. This does not mean it cannot be an attractor, but
-                    # it means it is sufficient to keep considering
-                    # the remaining candidates.
-                    is_valid_candidate = False
-                    break
+    str
+        The name of the corresponding Petri net place.
+    """
+    if positive:
+        return f"b1_{variable}"
+    else:
+        return f"b0_{variable}"
 
-                if not function_is_true(terminal_restriction_space, simulation):
-                    # The state can reach some other state outside of the
-                    # terminal restriction space, which means it cannot be
-                    # a motif avoidant attractor in this subspace.
-                    is_valid_candidate = False
-                    break
 
-            if is_valid_candidate:
-                # If we cannot rule out the candidate, we have to put it back
-                # into the candidate set.
-                candidates_dnf.append(state)
-                filtered_candidates.append(state)
+def place_to_variable(place: str) -> tuple[str, bool]:
+    """
+    Extract the variable name and state from a Petri net place name.
 
-        return filtered_candidates
+    Parameters
+    ----------
+    place : str
+        The name of the Petri net place.
+
+    Returns
+    -------
+    tuple[str, bool]
+        The name of the variable, and whether the variable is positive or negative.
+    """
+    if place.startswith("b1_"):
+        return (place[3:], True)
+    elif place.startswith("b0_"):
+        return (place[3:], False)
     else:
-        filtered_candidates = []
-        for _ in range(max_iterations):
-            generator.shuffle(variables)
-            candidates_dnf = candidates.copy()
-            filtered_candidates = []
+        raise Exception(f"Invalid place name: `{place}`.")
 
-            for state in candidates:
-                candidates_dnf = remove_state_from_dnf(candidates_dnf, state)
 
-                simulation = state.copy()
-                for var in variables:
-                    step = function_eval(update_functions[var], simulation)
-                    assert step is not None
-                    simulation[var] = step
+def extract_variable_names(encoded_network: DiGraph) -> list[str]:
+    """
+    Extract the variable names from a Petri net encoded Boolean network.
 
-                if not dnf_function_is_true(candidates_dnf, simulation):
-                    candidates_dnf.append(simulation)
-                    filtered_candidates.append(simulation)
+    The variables are  sorted lexicographically, since the original BN ordering
+    is not preserved by the Petri net. However, BNs order variables
+    lexicographically by default, so unless the Petri net was created from a
+    custom BN (i.e. not from a normal model file), the ordering should be the
+    same.
 
-            if len(filtered_candidates) <= 1:
-                break
+    Parameters
+    ----------
+    encoded_network : DiGraph
+        The Petri net encoded Boolean network.
 
-            candidates = filtered_candidates
+    Returns
+    -------
+    list[str]
+        The list of variable names.
+    """
+    variables: list[str] = []
+    for node in encoded_network.nodes():  # type: ignore
+        node = str(node)  # type: ignore
+        if node.startswith("b0_"):
+            variables.append(place_to_variable(node)[0])
 
-        return filtered_candidates
+    return sorted(variables)
 
 
-def _filter_candidates(
-    petri_net: DiGraph,
-    candidates: list[BooleanSpace],
-    terminal_restriction_space: Bdd,
-) -> list[BooleanSpace]:
+def extract_source_variables(encoded_network: DiGraph) -> list[str]:
     """
-    Filter candidate states using reachability procedure in Pint.
+    List variable names that represent source nodes of the encoded network.
+
+    Source nodes are those nodes with an identity update function.
+
+    Parameters
+    ----------
+    encoded_network : DiGraph
+        The Petri net encoded Boolean network.
+
+    Returns
+    -------
+    list[str]
+        The list of source variable names.
     """
+    variables = extract_variable_names(encoded_network)
+    source_set = set(variables)
+    for _, change_var in encoded_network.nodes(data="change"):  # type: ignore
+        if change_var in source_set:
+            source_set.remove(change_var)  # type: ignore[reportUnknownArgumentType] # noqa
+    source_nodes: list[str] = sorted(source_set)
+    return source_nodes
 
-    ctx = terminal_restriction_space.__ctx__()
-    candidates_bdd = state_list_to_bdd(ctx, candidates)
-    avoid_states = candidates_bdd.l_and_not(terminal_restriction_space)
-    filtered_candidates: list[BooleanSpace] = []
 
-    for state in candidates:
-        state_bdd = state_to_bdd(ctx, state)
+def restrict_petrinet_to_subspace(
+    petri_net: DiGraph,
+    sub_space: BooleanSpace,
+) -> DiGraph:
+    """
+    Create a copy of a Petri net restricted to a sub-space.
 
-        # Remove state from the symbolic set. If we can prove that it
-        # is not an attractor, we will put it back.
-        avoid_states = avoid_states.l_and_not(state_bdd)
+    Creates a copy of the given Petri net, but with the variables given in
+    `sub_space` fixed to their respective values.
 
-        if not _Pint_reachability(petri_net, state, avoid_states):
-            avoid_states = avoid_states.l_or(state_bdd)
-            filtered_candidates.append(state)
+    Note that this completely eliminates the constant variables from the Petri
+    net, but it does not perform any further constant propagation or
+    percolation. Variables that are fixed in the `sub_space` but do not exist in
+    the Petri net are ignored.
 
-    return filtered_candidates
+    The `sub_space` can contain variables that do not appear
+    in the `petri_net`. Such variables are simply ignored.
 
+    Parameters
+    ----------
+    petri_net : DiGraph
+        The Petri net to restrict.
+    sub_space : BooleanSpace
+        The sub-space to restrict the Petri net to.
 
-def _Pint_reachability(
-    petri_net: DiGraph,
-    initial_state: BooleanSpace,
-    target_states: Bdd,
-) -> bool:
+    Returns
+    -------
+    DiGraph
+        The restricted Petri net.
     """
-    Use Pint to check if a given `initial_state` can possibly reach some state
-    in the `target_states` BDD.
+    result = copy.deepcopy(petri_net)
+    for var, value in sub_space.items():
+        # The idea is that we want to *remove* the place that corresponds to the fixed
+        # value (it's effect on transitions is assumed to be fulfilled). Then, we remove
+        # all transitions that depend on the inverse of the fixed value, as these can
+        # never be satisfied. Then, we also remove inverse place.
+        fixed_place = variable_to_place(var, bool(value))
+        inverse_place = variable_to_place(var, not bool(value))
 
-    TODO: Here, if the result of static analysis is inconclusive, Pint falls back to `mole`
-    model checker. However, in the future, we might also explore other methods, such as
-    petri net reduction or symbolic reachability.
-    """
-    if target_states.is_false():
-        return False  # Cannot reach a stat in an empty set.
+        if fixed_place not in result.nodes or inverse_place not in result.nodes:
+            # These nodes were already removed.
+            continue
 
-    # Build a Pint model through an automata network and copy
-    # over the initial condition.
-    pint_model = InMemoryModel(_petri_net_as_automata_network(petri_net))
-    for var, level in initial_state.items():
-        pint_model.initial_state[var] = level
+        # First, remove all transitions that modify the fixed variable.
+        # These are removed regardless of the actual value.
 
-    goal = _Pint_build_symbolic_goal(target_states)
+        to_delete: set[str] = set()
 
-    return pint_model.reachability(goal=goal, fallback="mole")  # type: ignore
+        # Transitions that put marker into one of the place values, but do not take it.
+        for tr in result.predecessors(fixed_place):  # type: ignore
+            if not result.has_edge(fixed_place, tr):  # type: ignore
+                to_delete.add(cast(str, tr))
+        for tr in result.predecessors(inverse_place):  # type: ignore
+            if not result.has_edge(inverse_place, tr):  # type: ignore
+                to_delete.add(cast(str, tr))
 
+        # Transitions that depend on the value of the inverse place
+        for tr in result.successors(inverse_place):  # type: ignore
+            to_delete.add(cast(str, tr))
 
-def _Pint_build_symbolic_goal(states: Bdd) -> Goal:
-    """
-    A helper method which (very explicitly) converts a set of states
-    represented through a BDD into a Pint `Goal`.
+        for tr in to_delete:
+            result.remove_node(tr)  # type: ignore
+
+        result.remove_node(fixed_place)  # type: ignore
+        result.remove_node(inverse_place)  # type: ignore
+    return result
+
+
+def network_to_petrinet(
+    network: BooleanNetwork, symbolic_context: SymbolicContext | None = None
+) -> DiGraph:
     """
-    assert not states.is_false()
+    Convert a Boolean network to a Petri net.
 
-    goals: list[Goal] = []
-    for clause in states.clause_iterator():
-        named_clause = {
-            states.__ctx__().get_variable_name(var): int(value)
-            for var, value in clause.items()
-        }
-        goal_atoms = [f"{var}={level}" for var, level in named_clause.items()]
-        goals.append(Goal(",".join(goal_atoms)))
+    Converts a `biodivine_aeon.BooleanNetwork` to a `DiGraph` representing a Petri net encoding
+    of the original network. For details about the encoding, see module
+    description.
 
-    return reduce(lambda a, b: a | b, goals)
+    Note that the given network needs to have "sanitized" names, otherwise the
+    method will fail (see `sanitize_network_names` in this module).
 
+    The operation uses translation through `biodivine_aeon.Bdd` to generate a
+    disjunctive normal form of the network's update functions. This is
+    facilitated by `biodivine_aeon.SymbolicContext`. If a suitable context already
+    exists, it can be provided as the second argument. Otherwise it will be
+    created.
 
-def _petri_net_as_automata_network(petri_net: DiGraph) -> str:
-    """
-    Takes a Petri net which was created by implicant encoding from a Boolean network,
-    and builds an automata network file (`.an`) compatible with the Pint tool.
+    Parameters
+    ----------
+    network : BooleanNetwork
+        The network to convert.
+    symbolic_context : SymbolicContext | None
+        The context used for the symbolic conversion, as an
+        `biodivine_aeon.SymbolicContext` object. This is a mapping from the
+        network nodes to BDD variables that preserves variable ordering in BDDs.
+        If not given, a new one will be created from the network.
 
-    TODO: This is one of those things that would probably be better served by having
-    an "explicit" `PetriNetEncoding` class.
+    Returns
+    -------
+    DiGraph
+        The Petri net encoding of the given network.
     """
-    automata_network = ""
+    # Assert that all network names are already sanitized.
+    sanitize_network_names(network, check_only=True)
 
-    # Go through all PN places and save them as model variables.
-    variable_set: set[str] = set()
-    for place, kind in petri_net.nodes(data="kind"):  # type: ignore
-        if kind != "place":
+    assert (
+        network.explicit_parameter_count() == 0
+    ), f"Parametrized networks are not supported. Found parameters: {network.explicit_parameter_names()}."
+
+    # Implicit parameters with no regulators are allowed, since they just reprtesent free inputs
+    # and are explicitly handled by the succession diagram.
+    non_input_implicit = [
+        v for v in network.implicit_parameters() if len(network.predecessors(v)) > 0
+    ]
+    if len(non_input_implicit) > 0:
+        names = [network.get_variable_name(x) for x in non_input_implicit]
+        raise AssertionError(
+            f"Parametrized networks are not supported. Found implicit parameters: {names}."
+        )
+
+    if symbolic_context is None:
+        symbolic_context = SymbolicContext(network)
+
+    pn = DiGraph()
+
+    # Create a positive and a negative place for each variable.
+    places: dict[str, tuple[str, str]] = {}
+    for name in network.variable_names():
+        p_name = variable_to_place(name, positive=True)
+        n_name = variable_to_place(name, positive=False)
+        pn.add_node(p_name, kind="place")  # type: ignore[reportUnknownMemberType]
+        pn.add_node(n_name, kind="place")  # type: ignore[reportUnknownMemberType]
+        places[name] = (n_name, p_name)
+
+    # Create PN transitions for implicants of every BN transition.
+    for var in network.variables():
+        var_name = network.get_variable_name(var)
+        update_function = network.get_update_function(var)
+        if update_function is None:
+            # This variable is a constant input with a free update function.
+            assert len(network.predecessors(var)) == 0
             continue
-        variable_set.add(place_to_variable(place)[0])  # type: ignore[reportUnknownArgumentType] # noqa
-    variables = sorted(variable_set)
 
-    # Declare all variables with 0/1 domains.
-    for var in variables:
-        automata_network += f'"{var}" [0, 1]\n'
+        function_bdd = symbolic_context.mk_update_function(update_function)
+        var_bdd = symbolic_context.mk_network_variable(var)
 
-    for transition, kind in petri_net.nodes(data="kind"):  # type: ignore
-        if kind != "transition":
-            continue
+        p_bdd = function_bdd.l_and(var_bdd.l_not())
+        n_bdd = function_bdd.l_not().l_and(var_bdd)
 
-        predecessors = set(petri_net.predecessors(transition))  # type: ignore
-        successors = set(petri_net.successors(transition))  # type: ignore
+        if DEBUG:
+            print(f"Start translation for `{var_name}`: {len(p_bdd)} | {len(n_bdd)}")
 
-        # The value under modification is the only
-        # value that is different between successors and predecessors.
-        source_place = next(iter(predecessors - successors))  # type: ignore[reportUnknownVariableType,reportUnknownArgumentType] # noqa
-        target_place = next(iter(successors - predecessors))  # type: ignore[reportUnknownVariableType,reportUnknownArgumentType] # noqa
-
-        (s_var, s_level) = place_to_variable(source_place)  # type: ignore[reportUnknownArgumentType] # noqa
-        (t_var, t_level) = place_to_variable(target_place)  # type: ignore[reportUnknownArgumentType] # noqa
-        assert s_var == t_var
-
-        # The remaining places represent the necessary conditions.
-        # Here, we transform them into a text format.
-        conditions = sorted(predecessors.intersection(successors))  # type: ignore[reportUnknownVariableType,reportUnknownArgumentType] # noqa
-        conditions = [place_to_variable(p) for p in conditions]  # type: ignore[reportUnknownVariableType,reportUnknownArgumentType] # noqa
-        conditions = [f'"{var}"={int(level)}' for var, level in conditions]
-
-        # A pint rule consists of a variable name, value transition,
-        # and a list of necessary conditions for the transition (if any).
-        if len(conditions) == 0:
-            rule = f'"{s_var}" {int(s_level)} -> {int(t_level)}\n'
+        # Add 0->1 edges.
+        _create_transitions(
+            pn, symbolic_context.bdd_variable_set(), places, var_name, p_bdd, go_up=True
+        )
+        # Add 1-> 0 edges.
+        _create_transitions(
+            pn,
+            symbolic_context.bdd_variable_set(),
+            places,
+            var_name,
+            n_bdd,
+            go_up=False,
+        )
+
+    return pn
+
+
+def optimized_recursive_dnf_generator(
+    bdd: Bdd,
+) -> Generator[BddPartialValuation, None, None]:
+    """
+    Yields a generator of `BddPartialValuation` objects, similar to
+    `Bdd.clause_iterator` in AEON, but uses a recursive optimization strategy
+    to return a smaller result than the default method `Bdd` clause sequence.
+    Note that this is still not the "optimal" DNF, but is often close enough.
+
+    This is technically slower for BDDs that already have a small clause count,
+    but can be much better in the long-term when the clause count is high.
+    """
+
+    # Some performance notes:
+    #  - We could cache the best restriced BDDs, but usually this does not help much.
+    #  - We could try optimizing based on clause count instead of BDD size, but this will
+    #    need a new method in `lib-bdd` to compute clause count efficiently. (Now
+    #    we can only do it by walking the iterator.)
+    #  - The initial BDD size/ordering still do matter: starting with a smaller but equivalent
+    #    BDD can help achieve smaller DNF size.
+
+    if bdd.is_false():
+        return
+    if bdd.is_true():
+        yield BddPartialValuation(bdd.__ctx__(), cast(dict[str, BoolType], {}))
+        return
+
+    support = sorted(bdd.support_set())
+    best_var = support[0]
+    best_size = 10 * len(bdd)
+    for var in support:
+        t = bdd.r_restrict({var: True})
+        f = bdd.r_restrict({var: False})
+        t_size = len(t)
+        f_size = len(f)
+        if t_size + f_size < best_size:
+            best_size = t_size + f_size
+            best_var = var
+
+    for t_val in optimized_recursive_dnf_generator(bdd.r_restrict({best_var: True})):
+        t_val[best_var] = True
+        yield t_val
+
+    for f_val in optimized_recursive_dnf_generator(bdd.r_restrict({best_var: False})):
+        f_val[best_var] = False
+        yield f_val
+
+
+def _create_transitions(
+    pn: DiGraph,
+    ctx: BddVariableSet,
+    places: dict[str, tuple[str, str]],
+    var_name: str,
+    implicant_bdd: Bdd,
+    go_up: bool,
+):
+    """
+    Just a helper method that creates PN transitions from BDDs representing
+    positive/negative BN transitions.
+    """
+    dir_str = "up" if go_up else "down"
+    total = 0
+    for t_id, implicant in enumerate(optimized_recursive_dnf_generator(implicant_bdd)):
+        total += 1
+        t_name = f"tr_{var_name}_{dir_str}_{t_id + 1}"
+        pn.add_node(  # type: ignore[reportUnknownMemberType]
+            t_name,
+            kind="transition",  # type: ignore[reportUnknownMemberType]
+            change=var_name,
+            direction=dir_str,
+        )
+        # The transition moves a token either from "zero place" to the
+        # "one place", or vice versa.
+        if go_up:
+            pn.add_edge(places[var_name][0], t_name)  # type: ignore[reportUnknownMemberType] # noqa
+            pn.add_edge(t_name, places[var_name][1])  # type: ignore[reportUnknownMemberType] # noqa
         else:
-            rule = f"\"{s_var}\" {int(s_level)} -> {int(t_level)} when {' and '.join(conditions)}\n"
-
-        automata_network += rule
-
-    return automata_network
+            pn.add_edge(places[var_name][1], t_name)  # type: ignore[reportUnknownMemberType] # noqa
+            pn.add_edge(t_name, places[var_name][0])  # type: ignore[reportUnknownMemberType] # noqa
+        for variable, value in implicant.items():
+            variable_str = ctx.get_variable_name(
+                variable
+            )  # Convert from BDD variable to name.
+            if variable_str == var_name:
+                continue
+            # For the remaining variables, we simply check if the required
+            # token is present in the corresponding place.
+            pn.add_edge(places[variable_str][value], t_name)  # type: ignore[reportUnknownMemberType] # noqa
+            pn.add_edge(t_name, places[variable_str][value])  # type: ignore[reportUnknownMemberType] # noqa
+    if DEBUG:
+        print(f"  >> Generated {total} total PN transitions.")
```

### Comparing `biobalm-0.1.1/biobalm/space_utils.py` & `biobalm-0.2.0/biobalm/space_utils.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm/symbolic_utils.py` & `biobalm-0.2.0/biobalm/symbolic_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """
 Utility operations for creating and manipulating symbolic functions.
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Literal, cast
 
 if TYPE_CHECKING:
-    from typing import Literal
-
     from biodivine_aeon import Bdd, SymbolicContext
 
-from biodivine_aeon import BddVariableSet
+from biodivine_aeon import BddVariableSet, BddValuation
 
 from biobalm.types import BooleanSpace
 
 
 def state_to_bdd(
     bdd_context: SymbolicContext | BddVariableSet, state: BooleanSpace
 ) -> Bdd:
@@ -124,7 +122,33 @@
 
     Returns
     -------
     bool
         `True` if the function evaluates to `1` in the given state.
     """
     return function_eval(f, state) == 1
+
+
+def valuation_to_state(ctx: SymbolicContext, valuation: BddValuation) -> BooleanSpace:
+    """
+    Extract network state from a `BddValuation` into a `BooleanSpace`.
+
+    Parameters
+    ----------
+    f : SymbolicContext
+        A context which maps between network variables and their symbolic counterparts.
+    state : BddValuation
+        A valuation of the network's symbolic encoding.
+
+    Returns
+    -------
+    BooleanSpace
+        A `BooleanSpace` encoding the state data from the given valuation.
+    """
+
+    result: BooleanSpace = {}
+    for var, val in valuation.items():
+        n_var = ctx.find_network_variable(var)
+        if n_var is not None:
+            result[ctx.get_network_variable_name(n_var)] = cast(Literal[0, 1], int(val))
+
+    return result
```

### Comparing `biobalm-0.1.1/biobalm/trappist_core.py` & `biobalm-0.2.0/biobalm/trappist_core.py`

 * *Files identical despite different names*

### Comparing `biobalm-0.1.1/biobalm.egg-info/PKG-INFO` & `biobalm-0.2.0/biobalm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: biobalm
-Version: 0.1.1
+Version: 0.2.0
 Summary: Boolean Attractor Landscape Mapper
 Author-email: Jordan Rozum <jrozum@binghamton.edu>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: biodivine_aeon==1.0.0a4
+Requires-Dist: biodivine_aeon==1.0.0a6
 Requires-Dist: clingo>=5.6.2
 Requires-Dist: networkx>=2.8.8
-Requires-Dist: pypint>=1.6.2
+Provides-Extra: pint
+Requires-Dist: pypint==1.6.2; extra == "pint"
 
 [![PyPI](https://img.shields.io/pypi/v/biobalm?style=flat-square)](https://pypi.org/project/biobalm/) 
 [![Api Docs](https://img.shields.io/badge/docs-api-yellowgreen?style=flat-square)](https://jcrozum.github.io/biobalm/)
 [![Continuous integration](https://img.shields.io/github/actions/workflow/status/jcrozum/biobalm/test.yml?branch=main&style=flat-square)](https://github.com/jcrozum/biobalm/actions?query=workflow%3Atest)
 [![Coverage](https://img.shields.io/codecov/c/github/jcrozum/biobalm?style=flat-square)](https://codecov.io/gh/jcrozum/biobalm) 
 [![GitHub issues](https://img.shields.io/github/issues/jcrozum/biobalm?style=flat-square)](https://github.com/jcrozum/biobalm/issues) 
 [![License](https://img.shields.io/pypi/l/biobalm?style=flat-square)](https://github.com/jcrozum/biobalm/blob/main/LICENSE)
```

### Comparing `biobalm-0.1.1/pyproject.toml` & `biobalm-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 name = "biobalm"
 authors = [{ name = "Jordan Rozum", email = "jrozum@binghamton.edu" }]
 description = "Boolean Attractor Landscape Mapper"
 readme = "README.md"
 license = { file = "LISENSE" }
 requires-python = ">=3.11"
 dependencies = [
-    'biodivine_aeon ==1.0.0a4',
+    'biodivine_aeon ==1.0.0a6',
     'clingo >=5.6.2',
-    'networkx>=2.8.8',
-    'pypint>=1.6.2',
+    'networkx >=2.8.8',    
 ]
-version = "0.1.1"
+version = "0.2.0"
 
+# Pint can be used for static analysis, but is not mandatory.
+[project.optional-dependencies]
+pint = [
+    "pypint==1.6.2"
+]
 
 [tool.setuptools]
-packages = ['biobalm', 'biobalm._sd_algorithms']
-
+packages = ['biobalm', 'biobalm._sd_algorithms', 'biobalm._sd_attractors']
 
 [tool.pyright]
 include = ["biobalm", "tests"]
 stubPath = "stubs"
 reportMissingImports = true
 reportMissingTypeStubs = true
 reportUntypedFunctionDecorator = true
```

