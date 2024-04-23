# Comparing `tmp/circuitree-0.9.6.tar.gz` & `tmp/circuitree-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitree-0.9.6.tar", max compression
+gzip compressed data, was "circuitree-0.9.7.tar", max compression
```

## Comparing `circuitree-0.9.6.tar` & `circuitree-0.9.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-08-08 23:12:20.534641 circuitree-0.9.6/LICENSE
--rw-r--r--   0        0        0     1011 2023-08-08 23:12:20.534641 circuitree-0.9.6/README.md
--rwxr-xr-x   0        0        0      118 2024-04-02 19:18:57.943202 circuitree-0.9.6/circuitree/__init__.py
--rwxr-xr-x   0        0        0    40638 2024-04-23 00:25:27.756613 circuitree-0.9.6/circuitree/circuitree.py
--rw-r--r--   0        0        0     1621 2023-10-23 22:25:37.646685 circuitree-0.9.6/circuitree/grammar.py
--rwxr-xr-x   0        0        0    32344 2024-04-17 22:29:27.655740 circuitree-0.9.6/circuitree/models.py
--rw-r--r--   0        0        0     3991 2023-08-29 19:51:25.141731 circuitree-0.9.6/circuitree/modularity.py
--rw-r--r--   0        0        0     6541 2023-11-14 01:41:12.991399 circuitree-0.9.6/circuitree/parallel.py
--rw-r--r--   0        0        0      758 2023-10-20 16:36:26.268282 circuitree-0.9.6/circuitree/utils.py
--rw-r--r--   0        0        0    17981 2024-04-23 20:23:59.829251 circuitree-0.9.6/circuitree/viz.py
--rw-r--r--   0        0        0     1285 2024-04-23 20:27:19.769198 circuitree-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 circuitree-0.9.6/setup.py
--rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 circuitree-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 23:12:20.534641 circuitree-0.9.7/LICENSE
+-rw-r--r--   0        0        0     1011 2023-08-08 23:12:20.534641 circuitree-0.9.7/README.md
+-rwxr-xr-x   0        0        0      118 2024-04-02 19:18:57.943202 circuitree-0.9.7/circuitree/__init__.py
+-rwxr-xr-x   0        0        0    40647 2024-04-23 20:58:47.368706 circuitree-0.9.7/circuitree/circuitree.py
+-rw-r--r--   0        0        0     1621 2023-10-23 22:25:37.646685 circuitree-0.9.7/circuitree/grammar.py
+-rwxr-xr-x   0        0        0    32344 2024-04-17 22:29:27.655740 circuitree-0.9.7/circuitree/models.py
+-rw-r--r--   0        0        0     3991 2023-08-29 19:51:25.141731 circuitree-0.9.7/circuitree/modularity.py
+-rw-r--r--   0        0        0     6541 2023-11-14 01:41:12.991399 circuitree-0.9.7/circuitree/parallel.py
+-rw-r--r--   0        0        0      758 2023-10-20 16:36:26.268282 circuitree-0.9.7/circuitree/utils.py
+-rw-r--r--   0        0        0    18102 2024-04-23 20:34:18.519091 circuitree-0.9.7/circuitree/viz.py
+-rw-r--r--   0        0        0     1285 2024-04-23 20:57:42.588724 circuitree-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 circuitree-0.9.7/setup.py
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 circuitree-0.9.7/PKG-INFO
```

### Comparing `circuitree-0.9.6/LICENSE` & `circuitree-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.6/README.md` & `circuitree-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.6/circuitree/circuitree.py` & `circuitree-0.9.7/circuitree/circuitree.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,15 +575,15 @@
     ) -> list[Hashable]:
         """Sample a random successful state by first creating a new graph that contains
         all possible paths from the root to a successful terminal state. Then, sample
         paths by random traversal from the root."""
 
         # Check if is_success() is implemented
         try:
-            _ = self.is_success(self.terminal_states[0])
+            _ = self.is_success(next(self.terminal_states))
         except NotImplementedError:
             raise NotImplementedError(
                 "The CircuiTree subclass must implement the is_success() method to "
                 "use this function."
             )
 
         ## Create a graph with all possible paths to success
@@ -636,15 +636,15 @@
     ) -> list[Hashable]:
         """Sample a random successful state with rejection sampling. Starts from the
         root state, selects random actions until termination, and accepts the sample if
         it is successful."""
 
         # Check if is_success() is implemented
         try:
-            _ = self.is_success(self.terminal_states[0])
+            _ = self.is_success(next(self.terminal_states))
         except NotImplementedError:
             raise NotImplementedError(
                 "The CircuiTree subclass must implement the is_success() method to "
                 "use this function."
             )
 
         # Use rejection sampling to sample paths with the given pattern
@@ -944,15 +944,15 @@
     ) -> nx.DiGraph:
         if isinstance(successes, Iterable):
             successful_children = set(successes)
         elif successes is True:
 
             # Check if is_success() is implemented
             try:
-                _ = self.is_success(self.terminal_states[0])
+                _ = self.is_success(next(self.terminal_states))
             except NotImplementedError:
                 raise NotImplementedError(
                     "If successes=True, the CircuiTree subclass must implement "
                     "the is_success() method."
                 )
 
             # Keep only the successful nodes
```

### Comparing `circuitree-0.9.6/circuitree/grammar.py` & `circuitree-0.9.7/circuitree/grammar.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.6/circuitree/models.py` & `circuitree-0.9.7/circuitree/models.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.6/circuitree/modularity.py` & `circuitree-0.9.7/circuitree/modularity.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.6/circuitree/parallel.py` & `circuitree-0.9.7/circuitree/parallel.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.6/circuitree/utils.py` & `circuitree-0.9.7/circuitree/utils.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.6/circuitree/viz.py` & `circuitree-0.9.7/circuitree/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,26 +115,28 @@
     plot_layers_as_blocks: bool = True,
     block_height: float = 0.1,
     block_clr: str = "gray",
     marker_clr: str = "k",
     marker_size: float = 10,
     n_to_highlight: Optional[float] = None,
     highlight_clr: str = "tab:orange",
+    fig: Optional[plt.Figure] = None,
+    ax: Optional[plt.Axes] = None,
 ) -> None:
 
     G = tree.to_complexity_graph()
 
     if depth_of_node is None or pos is None:
         print("Computing layout...")
         depth_of_node, pos = complexity_layout(tree)
 
     xvals, yvals = zip(*pos.values())
     xvals = np.array(xvals)
     yvals = np.array(yvals)
-    
+
     # Get the limits for the number of visits - only show edges with visits in this range
     if vlim[0] is None:
         vmin = min(v for *e, v in G.edges(data="visits"))
     else:
         vmin = vlim[0]
     if vlim[1] is None:
         vmax = max(v for *e, v in G.edges(data="visits"))
@@ -175,15 +177,18 @@
         weights.append(normalize(v))
     weights = np.array(weights)
 
     # # Black edges with alpha proportional to the weight
     # edge_colors = np.zeros((len(weights), 4))
     # edge_colors[:, 3] = alpha * weights
 
-    fig, ax = plt.subplots(figsize=figsize)
+    if fig is None:
+        fig = plt.figure(figsize=figsize)
+    if ax is None:
+        ax = fig.add_subplot(1, 1, 1)
 
     # set edge positions
     if plot_layers_as_blocks:
         ybias = 0.5 * block_height
     else:
         ybias = 0.0
     edge_pos = []
@@ -201,15 +206,15 @@
         linewidths=lw,
         antialiaseds=(1,),
         linestyle="-",
         alpha=alpha,
     )
     edges.set_zorder(0)  # edges go behind nodes
     ax.add_collection(edges)
-    
+
     # edges = nx.draw_networkx_edges(
     #     G,
     #     G_pos,
     #     ax=ax,
     #     edge_color=edge_colors,
     #     width=0.5,
     #     arrows=False,
@@ -231,25 +236,25 @@
                 height=block_height,
                 color=block_clr,
                 zorder=1,
             )
             rects.append(rect)
         layer_blocks = mpl_coll.PatchCollection(rects, match_original=True)
         ax.add_collection(layer_blocks)
-    
+
     else:
         # Draw each node as a circle
         for n, (x, y) in pos.items():
             ax.scatter(x, y, color=marker_clr, s=marker_size, zorder=1)
-    
+
     # for xmin_d, xmax_d, yval_d in zip(depth_xmins, depth_xmaxs, depth_yvals):
     #     plt.hlines(yval_d, xmin_d, xmax_d, color="gray", zorder=4, lw=1.0)
 
     if n_to_highlight is not None:
-        
+
         # Get locations of the top "N" oscillators
         highlight_states = sorted(
             tree.terminal_states, key=lambda n: -tree.graph.nodes[n]["visits"]
         )[:n_to_highlight]
         top_states_pos = []
         for state in highlight_states:
             nonterm = state.lstrip("*")
@@ -263,19 +268,20 @@
                 *top_states_pos.T,
                 color=highlight_clr,
                 s=15,
                 zorder=5,
                 edgecolors="k",
                 lw=0.3,
             )
-    
+
     ax.set_axis_off()
 
     return fig, ax
 
+
 ## Plot a diagram of an N-component network (see models.SimpleNetworkTree)
 
 
 def plot_network(
     names: Iterable[str],
     activations: np.ndarray[np.int_],
     inhibitions: np.ndarray[np.int_],
```

### Comparing `circuitree-0.9.6/pyproject.toml` & `circuitree-0.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circuitree"
-version = "0.9.6"
+version = "0.9.7"
 description = "Genetic circuit design using Monte Carlo tree search"
 authors = ["pranav-bhamidipati <pbhamidi@usc.edu>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `circuitree-0.9.6/setup.py` & `circuitree-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['networkx>=3.1,<4.0', 'numpy>=1.23.0,<2.0.0', 'pandas>=2.0.0,<3.0.0']
 
 extras_require = \
 {':python_version >= "3.10" and python_version < "3.13"': ['scipy>=1.11.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'circuitree',
-    'version': '0.9.6',
+    'version': '0.9.7',
     'description': 'Genetic circuit design using Monte Carlo tree search',
     'long_description': '# CircuiTree\nGenetic circuit design using Monte Carlo tree search\n\n## Installation\n\n### From a package repository\nTo install using `pip`:\n\n```pip install circuitree```\n\n### From the GitHub repository\n\nTo install and use `circuitree` from the GitHub source code, first clone the repo into a directory.\n\n```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```\n\nThen, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). \n\nFrom the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. \n\n## Usage\n\nSee the [quick-start demo](examples/quick_start.ipynb).\n',
     'author': 'pranav-bhamidipati',
     'author_email': 'pbhamidi@usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `circuitree-0.9.6/PKG-INFO` & `circuitree-0.9.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitree
-Version: 0.9.6
+Version: 0.9.7
 Summary: Genetic circuit design using Monte Carlo tree search
 License: GPLv3
 Author: pranav-bhamidipati
 Author-email: pbhamidi@usc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

