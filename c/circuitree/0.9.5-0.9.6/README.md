# Comparing `tmp/circuitree-0.9.5.tar.gz` & `tmp/circuitree-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitree-0.9.5.tar", max compression
+gzip compressed data, was "circuitree-0.9.6.tar", max compression
```

## Comparing `circuitree-0.9.5.tar` & `circuitree-0.9.6.tar`

### file list

```diff
@@ -1,16 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-08-08 23:12:20.534641 circuitree-0.9.5/LICENSE
--rw-r--r--   0        0        0     1011 2023-08-08 23:12:20.534641 circuitree-0.9.5/README.md
--rwxr-xr-x   0        0        0      140 2023-10-20 18:12:44.635922 circuitree-0.9.5/circuitree/__init__.py
--rwxr-xr-x   0        0        0    40538 2024-02-29 21:33:16.348041 circuitree-0.9.5/circuitree/circuitree.py
--rw-r--r--   0        0        0     1621 2023-10-23 22:25:37.646685 circuitree-0.9.5/circuitree/grammar.py
--rw-r--r--   0        0        0     1230 2023-08-08 23:12:20.534641 circuitree-0.9.5/circuitree/metrics.py
--rwxr-xr-x   0        0        0    31838 2023-11-16 22:43:56.035553 circuitree-0.9.5/circuitree/models.py
--rw-r--r--   0        0        0     3991 2023-08-29 19:51:25.141731 circuitree-0.9.5/circuitree/modularity.py
--rw-r--r--   0        0        0     6541 2023-11-14 01:41:12.991399 circuitree-0.9.5/circuitree/parallel.py
--rw-r--r--   0        0        0     8471 2023-11-14 01:39:47.741427 circuitree-0.9.5/circuitree/parallel.py.backup
--rw-r--r--   0        0        0      267 2023-08-08 23:12:20.534641 circuitree-0.9.5/circuitree/regret.py
--rw-r--r--   0        0        0      758 2023-10-20 16:36:26.268282 circuitree-0.9.5/circuitree/utils.py
--rw-r--r--   0        0        0    10716 2023-11-06 23:52:29.694926 circuitree-0.9.5/circuitree/viz.py
--rw-r--r--   0        0        0      761 2024-02-29 21:44:15.487263 circuitree-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 circuitree-0.9.5/setup.py
--rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 circuitree-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 23:12:20.534641 circuitree-0.9.6/LICENSE
+-rw-r--r--   0        0        0     1011 2023-08-08 23:12:20.534641 circuitree-0.9.6/README.md
+-rwxr-xr-x   0        0        0      118 2024-04-02 19:18:57.943202 circuitree-0.9.6/circuitree/__init__.py
+-rwxr-xr-x   0        0        0    40638 2024-04-23 00:25:27.756613 circuitree-0.9.6/circuitree/circuitree.py
+-rw-r--r--   0        0        0     1621 2023-10-23 22:25:37.646685 circuitree-0.9.6/circuitree/grammar.py
+-rwxr-xr-x   0        0        0    32344 2024-04-17 22:29:27.655740 circuitree-0.9.6/circuitree/models.py
+-rw-r--r--   0        0        0     3991 2023-08-29 19:51:25.141731 circuitree-0.9.6/circuitree/modularity.py
+-rw-r--r--   0        0        0     6541 2023-11-14 01:41:12.991399 circuitree-0.9.6/circuitree/parallel.py
+-rw-r--r--   0        0        0      758 2023-10-20 16:36:26.268282 circuitree-0.9.6/circuitree/utils.py
+-rw-r--r--   0        0        0    17981 2024-04-23 20:23:59.829251 circuitree-0.9.6/circuitree/viz.py
+-rw-r--r--   0        0        0     1285 2024-04-23 20:27:19.769198 circuitree-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 circuitree-0.9.6/setup.py
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 circuitree-0.9.6/PKG-INFO
```

### Comparing `circuitree-0.9.5/LICENSE` & `circuitree-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.5/README.md` & `circuitree-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.5/circuitree/circuitree.py` & `circuitree-0.9.6/circuitree/circuitree.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 from pathlib import Path
 from typing import Callable, Hashable, Literal, Optional, Iterable, Any
 import numpy as np
 import networkx as nx
 import pandas as pd
 from scipy import stats
+import warnings
 
 from .modularity import tree_modularity, tree_modularity_estimate
 from .grammar import CircuitGrammar
 
 __all__ = ["CircuiTree"]
 
 
@@ -40,15 +41,16 @@
     def __init__(
         self,
         grammar: CircuitGrammar,
         root: str,
         exploration_constant: Optional[float] = None,
         seed: int = 2023,
         graph: Optional[nx.DiGraph] = None,
-        tree_shape: Literal["tree", "dag"] = "dag",
+        tree_shape: Optional[Literal["tree", "dag"]] = None,
+        compute_symmetries: bool = True,
         **kwargs,
     ):
         self.rg = np.random.default_rng(seed)
         self.seed = self.rg.bit_generator._seed_seq.entropy
 
         self.root = root
         if graph is None:
@@ -58,17 +60,22 @@
             self.graph = graph
             if self.root not in self.graph:
                 raise ValueError(
                     f"Supplied graph does not contain the root node: {root}"
                 )
         self.graph.root = self.root
 
-        if tree_shape not in ("tree", "dag"):
-            raise ValueError("Argument `tree_shape` must be `tree` or `dag`.")
-        self.tree_shape = tree_shape
+        self.compute_symmetries = compute_symmetries
+        if tree_shape is not None:
+            if tree_shape not in ("tree", "dag"):
+                raise ValueError("Argument `tree_shape` must be `tree` or `dag`.")
+            warnings.warn(
+                "The `tree_shape` argument is deprecated and will be removed in a "
+                "future version. Please use `compute_symmetries` instead."
+            )
 
         self.grammar = grammar
 
         if exploration_constant is None:
             self.exploration_constant = np.sqrt(2)
         else:
             self.exploration_constant = exploration_constant
@@ -89,24 +96,24 @@
 
     @property
     def terminal_states(self):
         return (node for node in self.graph.nodes if self.grammar.is_terminal(node))
 
     def _do_action(self, state: Hashable, action: Hashable):
         new_state = self.grammar.do_action(state, action)
-        if self.tree_shape == "dag":
+        if self.compute_symmetries:
             new_state = self.grammar.get_unique_state(new_state)
         return new_state
 
     def _undo_action(self, state: Hashable, action: Hashable) -> Hashable:
         """Undo one action from the given state."""
         if state == self.root:
             return None
         new_state = self.grammar.undo_action(state, action)
-        if self.tree_shape == "dag":
+        if self.compute_symmetries:
             new_state = self.grammar.get_unique_state(new_state)
         return new_state
 
     @staticmethod
     def _get_random_terminal_descendant(
         grammar: CircuitGrammar, start: Hashable, rg: np.random.Generator
     ) -> Hashable:
@@ -233,20 +240,14 @@
         # Between backprop of visit and reward, we incur virtual loss
         self.backpropagate_visit(selection_path)
         reward = self.get_reward(sim_node, **kwargs)
         self.backpropagate_reward(selection_path, reward)
 
         return selection_path, reward, sim_node
 
-    def accumulate_visits_and_rewards(self, graph: Optional[nx.DiGraph] = None):
-        _accumulated = self.graph if graph is None else graph
-        accumulate_visits_and_rewards(_accumulated)
-        if graph is None:
-            return _accumulated
-
     def grow_tree(
         self, root=None, n_visits: int = 0, print_updates=False, print_every=1000
     ):
         if root is None:
             root = self.root
             if print_updates:
                 print(f"Adding root: {root}")
@@ -316,15 +317,14 @@
             iterator = islice(cycle(iterator), n_steps)
 
         if progress:
             from tqdm import tqdm
 
             iterator = tqdm(iterator, desc="BFS search")
 
-        cb_results = []
         if callback is not None:
             callback(self, None, None)
 
         for i, node in enumerate(iterator):
             self.graph.nodes[node]["visits"] += 1
             reward = self.get_reward(node, **run_kwargs)
             self.graph.nodes[node]["reward"] += reward
@@ -335,24 +335,25 @@
     def search_mcts(
         self,
         n_steps: int,
         callback_every: int = 1,
         callback: Optional[Callable] = None,
         progress_bar: bool = False,
         run_kwargs: Optional[dict] = None,
+        callback_before_start: bool = True,
     ) -> None:
         if progress_bar:
             from tqdm import trange
 
             iterator = trange(n_steps, desc="MCTS search")
         else:
             iterator = range(n_steps)
 
         run_kwargs = {} if run_kwargs is None else run_kwargs
-        if callback is not None:
+        if callback is not None and callback_before_start:
             callback(self, -1, [None], None, None)
 
         for i in iterator:
             selection_path, reward, sim_node = self.traverse(**run_kwargs)
             if callback is not None and i % callback_every == 0:
                 _ = callback(self, i, selection_path, sim_node, reward)
 
@@ -572,14 +573,23 @@
         nprocs: int = 1,
         chunksize: int = 100,
     ) -> list[Hashable]:
         """Sample a random successful state by first creating a new graph that contains
         all possible paths from the root to a successful terminal state. Then, sample
         paths by random traversal from the root."""
 
+        # Check if is_success() is implemented
+        try:
+            _ = self.is_success(self.terminal_states[0])
+        except NotImplementedError:
+            raise NotImplementedError(
+                "The CircuiTree subclass must implement the is_success() method to "
+                "use this function."
+            )
+
         ## Create a graph with all possible paths to success
         successful_terminals = set(
             s for s in self.terminal_states if self.is_success(s)
         )
 
         # Generate the graph with all possible paths to success
         all_paths_to_success = self.grow_tree_from_leaves(successful_terminals)
@@ -624,14 +634,23 @@
         nprocs: int = 1,
         chunksize: int = 100,
     ) -> list[Hashable]:
         """Sample a random successful state with rejection sampling. Starts from the
         root state, selects random actions until termination, and accepts the sample if
         it is successful."""
 
+        # Check if is_success() is implemented
+        try:
+            _ = self.is_success(self.terminal_states[0])
+        except NotImplementedError:
+            raise NotImplementedError(
+                "The CircuiTree subclass must implement the is_success() method to "
+                "use this function."
+            )
+
         # Use rejection sampling to sample paths with the given pattern
         successful_terminals = set(
             s for s in self.terminal_states if self.is_success(s)
         )
         if progress:
             from tqdm import tqdm
 
@@ -922,14 +941,24 @@
 
     def to_complexity_graph(
         self, successes: bool | Iterable[Hashable] = True
     ) -> nx.DiGraph:
         if isinstance(successes, Iterable):
             successful_children = set(successes)
         elif successes is True:
+
+            # Check if is_success() is implemented
+            try:
+                _ = self.is_success(self.terminal_states[0])
+            except NotImplementedError:
+                raise NotImplementedError(
+                    "If successes=True, the CircuiTree subclass must implement "
+                    "the is_success() method."
+                )
+
             # Keep only the successful nodes
             successful_children = set(
                 c for c in self.terminal_states if self.is_success(c)
             )
         elif successes is False:
             # keep all terminal nodes
             successful_children = set(self.terminal_states)
@@ -948,24 +977,14 @@
         ).copy()
 
         for (parent, child), d in child_attrs.items():
             complexity_graph.nodes[parent]["terminal_state"] = d | {"name": child}
 
         return complexity_graph
 
-    @property
-    def modularity(self) -> float:
-        return tree_modularity(
-            self.graph, self.root, self.grammar.is_terminal, self.is_success
-        )
-
-    @property
-    def modularity_estimate(self) -> float:
-        return tree_modularity_estimate(self.graph, self.root)
-
 
 def compute_odds_ratio_and_ci(
     table: np.ndarray, confidence_level: float
 ) -> tuple[float, tuple[float, float]]:
     """Compute the odds ratio and confidence interval for a 2x2 contingency table."""
     # Compute the odds ratio
     (a, b), (c, d) = table
@@ -1069,26 +1088,7 @@
     else:
         res = stats.chi2_contingency(table, correction=correction)
         table_df["test"] = "chi2"
         table_df["statistic"] = res.statistic
         table_df["pvalue"] = res.pvalue
 
     return table_df
-
-
-def accumulate_visits_and_rewards(
-    graph: nx.DiGraph, visits_attr: str = "visits", reward_attr: str = "reward"
-):
-    """Accumulate results on nodes post-hoc"""
-    for n in graph.nodes:
-        total_visits = sum([v for _, _, v in graph.in_edges(n, data=visits_attr)])
-        total_reward = sum([r for _, _, r in graph.in_edges(n, data=reward_attr)])
-        graph.nodes[n]["visits"] = total_visits
-        graph.nodes[n]["reward"] = total_reward
-
-    for n in graph.nodes:
-        graph.nodes[n][visits_attr] = 0
-        graph.nodes[n][reward_attr] = 0
-
-    for parent, child, data in graph.edges(data=True):
-        graph.nodes[parent][visits_attr] += data[visits_attr]
-        graph.nodes[parent][reward_attr] += data[reward_attr]
```

### Comparing `circuitree-0.9.5/circuitree/grammar.py` & `circuitree-0.9.6/circuitree/grammar.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.5/circuitree/models.py` & `circuitree-0.9.6/circuitree/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     def __init__(
         self,
         components: Iterable[Iterable[str]],
         interactions: Iterable[str],
         max_interactions: Optional[int] = None,
         root: Optional[str] = None,
         cache_maxsize: int | None = 128,
+        fixed_components: Optional[list[str]] = None,
     ):
         super().__init__()
 
         if len(set(c[0] for c in components)) < len(components):
             raise ValueError("First character of each component must be unique")
         if len(set(c[0] for c in interactions)) < len(interactions):
             raise ValueError("First character of each interaction must be unique")
@@ -46,14 +47,19 @@
         self.interaction_map = {ixn[0]: ixn for ixn in self.interactions}
 
         if max_interactions is None:
             self.max_interactions = len(self.components) ** 2  # all possible edges
         else:
             self.max_interactions = max_interactions
 
+        self.fixed_components = fixed_components or []
+        self.recolorable_components = [
+            c for c in self.components if c not in self.fixed_components
+        ]
+
         # Allow user to specify a cache size for the get_interaction_recolorings method.
         # This method is called frequently during search, and evaluation can become a
         # bottleneck for large spaces. Caching the results of this method can
         # significantly speed up search, but cache size is limited by system memory.
         self._cache_maxsize = cache_maxsize
         self.get_interaction_recolorings: Callable[[str], list[str]] = lru_cache(
             maxsize=self._cache_maxsize
@@ -70,23 +76,23 @@
                 "get_interaction_recolorings",
             ]
         )
 
     def __getstate__(self):
         result = copy(self.__dict__)
 
-        # This is a hack to get around the fact that lru_cache objects are not
-        # serializable. We can't just delete the attribute because it is needed for
-        # the grammar to function properly. Instead, we set it to None here and then
-        # re-initialize it in the __setstate__ method.
+        # We need to remove the lru_cache object because it is not serializable. We
+        # will re-initialize it in the __setstate__ method.
         result["get_interaction_recolorings"] = NotImplemented
         return result
 
     def __setstate__(self, state):
         self.__dict__ = state
+
+        # Re-initialize the lru_cache object
         self.get_interaction_recolorings = lru_cache(maxsize=self._cache_maxsize)(
             self._get_interaction_recolorings
         )
 
     @cached_property
     def edge_options(self):
         return [
@@ -221,18 +227,21 @@
 
     @staticmethod
     def is_terminal(genotype: str) -> bool:
         return genotype.startswith("*")
 
     @cached_property
     def _recolor(self):
-        return [dict(zip(self.components, p)) for p in permutations(self.components)]
+        return [
+            dict(zip(self.recolorable_components, p))
+            for p in permutations(self.recolorable_components)
+        ]
 
     @staticmethod
-    def _recolor_string(mapping, string):
+    def _recolor_string(mapping: dict[str, str], string: str):
         return "".join([mapping.get(c, c) for c in string])
 
     def _get_interaction_recolorings(self, interactions: str) -> list[str]:
         interaction_recolorings = []
         for mapping in self._recolor:
             recolored_interactions = sorted(
                 [self._recolor_string(mapping, ixn) for ixn in interactions.split("_")]
@@ -338,31 +347,35 @@
         components: Iterable[Iterable[str]] = None,
         interactions: Iterable[str] = None,
         max_interactions: Optional[int] = None,
         root: Optional[str] = None,
         exploration_constant: float | None = None,
         seed: int = 2023,
         graph: nx.DiGraph | None = None,
-        tree_shape: Literal["tree", "dag"] = "dag",
+        tree_shape: Optional[Literal["tree", "dag"]] = None,
+        compute_symmetries: bool = True,
+        fixed_components: Optional[list[str]] = None,
         **kwargs,
     ):
         if grammar is None:
             grammar = SimpleNetworkGrammar(
                 components=components,
                 interactions=interactions,
                 max_interactions=max_interactions,
                 root=root,
+                fixed_components=fixed_components,
             )
         super().__init__(
             grammar=grammar,
             root=root,
             exploration_constant=exploration_constant,
             seed=seed,
             graph=graph,
             tree_shape=tree_shape,
+            compute_symmetries=compute_symmetries,
             **kwargs,
         )
 
 
 class DimersGrammar(CircuitGrammar):
     """A grammar class for circuits consisting of dimerizing molecules."""
 
@@ -775,15 +788,16 @@
         interactions: Iterable[str],
         max_interactions: Optional[int] = None,
         max_interactions_per_promoter: int = 2,
         root: Optional[str] = None,
         exploration_constant: float | None = None,
         seed: int = 2023,
         graph: nx.DiGraph | None = None,
-        tree_shape: Literal["tree", "dag"] = "dag",
+        tree_shape: Optional[Literal["tree", "dag"]] = None,
+        compute_symmetries: bool = True,
         **kwargs,
     ):
         grammar = DimersGrammar(
             components=components,
             regulators=regulators,
             interactions=interactions,
             max_interactions=max_interactions,
@@ -793,9 +807,10 @@
         super().__init__(
             grammar=grammar,
             root=root,
             exploration_constant=exploration_constant,
             seed=seed,
             graph=graph,
             tree_shape=tree_shape,
+            compute_symmetries=compute_symmetries,
             **kwargs,
         )
```

### Comparing `circuitree-0.9.5/circuitree/modularity.py` & `circuitree-0.9.6/circuitree/modularity.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.5/circuitree/parallel.py` & `circuitree-0.9.6/circuitree/parallel.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.5/circuitree/utils.py` & `circuitree-0.9.6/circuitree/utils.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.5/setup.py` & `circuitree-0.9.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['networkx>=3.1,<4.0', 'numpy>=1.23.0,<2.0.0', 'pandas>=2.0.0,<3.0.0']
 
 extras_require = \
 {':python_version >= "3.10" and python_version < "3.13"': ['scipy>=1.11.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'circuitree',
-    'version': '0.9.5',
+    'version': '0.9.6',
     'description': 'Genetic circuit design using Monte Carlo tree search',
     'long_description': '# CircuiTree\nGenetic circuit design using Monte Carlo tree search\n\n## Installation\n\n### From a package repository\nTo install using `pip`:\n\n```pip install circuitree```\n\n### From the GitHub repository\n\nTo install and use `circuitree` from the GitHub source code, first clone the repo into a directory.\n\n```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```\n\nThen, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). \n\nFrom the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. \n\n## Usage\n\nSee the [quick-start demo](examples/quick_start.ipynb).\n',
     'author': 'pranav-bhamidipati',
     'author_email': 'pbhamidi@usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `circuitree-0.9.5/PKG-INFO` & `circuitree-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitree
-Version: 0.9.5
+Version: 0.9.6
 Summary: Genetic circuit design using Monte Carlo tree search
 License: GPLv3
 Author: pranav-bhamidipati
 Author-email: pbhamidi@usc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

