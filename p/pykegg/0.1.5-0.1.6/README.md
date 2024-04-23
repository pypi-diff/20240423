# Comparing `tmp/pykegg-0.1.5.tar.gz` & `tmp/pykegg-0.1.6.tar.gz`

## Comparing `pykegg-0.1.5.tar` & `pykegg-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rwxr-xr-x   0        0        0      874 2020-02-02 00:00:00.000000 pykegg-0.1.5/recipe/meta.yaml
--rwxr-xr-x   0        0        0    10670 2020-02-02 00:00:00.000000 pykegg-0.1.5/src/pykegg/KGML_graph.py
--rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 pykegg-0.1.5/src/pykegg/__init__.py
--rwxr-xr-x   0        0        0    37925 2020-02-02 00:00:00.000000 pykegg-0.1.5/src/pykegg/utils.py
--rwxr-xr-x   0        0        0     2679 2020-02-02 00:00:00.000000 pykegg-0.1.5/.gitignore
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pykegg-0.1.5/LICENSE
--rwxr-xr-x   0        0        0     1635 2020-02-02 00:00:00.000000 pykegg-0.1.5/README.md
--rwxr-xr-x   0        0        0      862 2020-02-02 00:00:00.000000 pykegg-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 pykegg-0.1.5/PKG-INFO
+-rwxr-xr-x   0        0        0      782 2020-02-02 00:00:00.000000 pykegg-0.1.6/recipe/meta.yaml
+-rwxr-xr-x   0        0        0    10670 2020-02-02 00:00:00.000000 pykegg-0.1.6/src/pykegg/KGML_graph.py
+-rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 pykegg-0.1.6/src/pykegg/__init__.py
+-rwxr-xr-x   0        0        0    33735 2020-02-02 00:00:00.000000 pykegg-0.1.6/src/pykegg/utils.py
+-rwxr-xr-x   0        0        0     2679 2020-02-02 00:00:00.000000 pykegg-0.1.6/.gitignore
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pykegg-0.1.6/LICENSE
+-rwxr-xr-x   0        0        0     1635 2020-02-02 00:00:00.000000 pykegg-0.1.6/README.md
+-rwxr-xr-x   0        0        0      845 2020-02-02 00:00:00.000000 pykegg-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 pykegg-0.1.6/PKG-INFO
```

### Comparing `pykegg-0.1.5/recipe/meta.yaml` & `pykegg-0.1.6/recipe/meta.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 {% set name = "pykegg" %}
-{% set version = "0.1.5" %}
+{% set version = "0.1.6" %}
 
 package:
   name: {{ name|lower }}
   version: {{ version }}
 
 source:
   url: https://pypi.io/packages/source/{{ name[0] }}/{{ name }}/pykegg-{{ version }}.tar.gz
-  sha256: bfbb96bef2dc60fa2a5bb235b79716370efddf2a62533128e68f5476f3e7ba62
 
 build:
   noarch: python
   script: {{ PYTHON }} -m pip install . -vv --no-deps --no-build-isolation
   number: 0
 
 requirements:
@@ -20,15 +19,14 @@
     - hatchling
     - pip
   run:
     - python >=3.7
     - python-igraph
     - pandas
     - biopython
-    - plotnine
     - requests
     - opencv
 
 test:
   imports:
     - pykegg
   commands:
```

### Comparing `pykegg-0.1.5/src/pykegg/KGML_graph.py` & `pykegg-0.1.6/src/pykegg/KGML_graph.py`

 * *Files identical despite different names*

### Comparing `pykegg-0.1.5/src/pykegg/utils.py` & `pykegg-0.1.6/src/pykegg/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,14 @@
 
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import pandas as pd
 
 from PIL import Image
-from plotnine import (
-    ggplot,
-    geom_point,
-    aes,
-    geom_segment,
-    theme_void,
-    geom_rect,
-    geom_text,
-)
 
 import pykegg
 
 
 def overlay_opencv_image(
     node_df,
     path=None,
@@ -206,144 +197,14 @@
         ],
         axis=1,
     )
     seg_df.columns = ["x", "y", "xend", "yend"]
     seg_df = pd.concat([seg_df, edge_df], axis=1)
     return seg_df
 
-
-def plot_kegg_pathway_plotnine(
-    graph,
-    node_x_nudge=20,
-    node_y_nudge=10,
-    split_graphics_name=True,
-    subtype_num=0,
-    label_size=2,
-    show_label="gene",
-    edge_color="subtype",
-    text_label="graphics_name",
-):
-    """Plot KEGG pathway using plotnine.
-
-    Parameters:
-    -----------
-    graph: KGML_graph class
-        graph object obtained by `KGML_graph()`.
-    node_x_nudge: int
-        nudge the x position of nodes.
-    node_y_nudge: int
-        nudge the y position of nodes.
-    split_graphics_name: bool
-        if True, split the graphics_name by comma and use the first one.
-    subtype_num: int
-        the number of subtypes to be used for the edge label.
-    label_size: int
-        the size of the label.
-    show_label: str
-        the type of label to be shown, e.g. "gene", "compound".
-    edge_color: str
-        the column in `edge_df` specifying edge color.
-    text_label: str
-        the column in `node_df` specifying node label.
-    """
-    node_df = graph.get_nodes(node_x_nudge=node_x_nudge, node_y_nudge=node_y_nudge)
-    edge_df = graph.get_edges()
-    if split_graphics_name:
-        node_df["graphics_name"] = node_df.graphics_name.apply(
-            lambda x: x.split(",")[0]
-        )
-
-    ## Collapse subtypes
-    edge_df_col = []
-    for i in edge_df.index:
-        tmp = edge_df.iloc[i, :]
-        for subtype in tmp.subtypes:
-            edge_df_col.append(
-                [tmp.entry1, tmp.entry2, tmp.type, subtype, tmp.reaction]
-            )
-    edge_df = pd.DataFrame(edge_df_col)
-    edge_df.columns = ["entry1", "entry2", "type", "subtypes", "reaction"]
-    seg_df = pd.concat(
-        [
-            node_df.reset_index()
-            .set_index("id")
-            .loc[edge_df.entry1]
-            .reset_index()
-            .loc[:, ["x", "y"]],
-            node_df.reset_index()
-            .set_index("id")
-            .loc[edge_df.entry2]
-            .reset_index()
-            .loc[:, ["x", "y"]],
-        ],
-        axis=1,
-    )
-    seg_df.columns = ["x", "y", "xend", "yend"]
-    seg_df = pd.concat([seg_df, edge_df], axis=1)
-
-    ## [TODO] implement multiple edges like `geom_edge_parallel` in ggraph
-    ## Currently edges are overlapped.
-    seg_df["subtype"] = seg_df.subtypes.apply(
-        lambda x: x[subtype_num] if x is not None else x
-    )
-
-    plot = (
-        ggplot()
-        + geom_segment(
-            aes(x="x", y="y", xend="xend", yend="yend", color=edge_color), data=seg_df
-        )
-        + geom_rect(
-            aes(xmin="xmin", ymin="ymin", xmax="xmax", ymax="ymax"),
-            data=node_df[node_df.original_type == "gene"],
-            fill="white",
-            color="grey",
-        )
-        + geom_rect(
-            aes(xmin="xmin", ymin="ymin", xmax="xmax", ymax="ymax"),
-            data=node_df[node_df.original_type == "compound"],
-            fill="white",
-            color="grey",
-        )
-        + geom_text(
-            aes(x="x", y="y", label=text_label, filter="original_type!='group'"),
-            data=node_df[node_df.original_type == show_label],
-            size=label_size,
-        )
-        + theme_void()
-    )
-    return plot
-
-
-def plot_kegg_global_map_plotnine(graph, hide_map=True):
-    """Plot KEGG global map using plotnine.
-
-    Parameters:
-    -----------
-    graph: KGML_graph class
-        graph object of global map like ko01100, obtained by `KGML_graph()`.
-    hide_map: bool
-        if True, hide the map nodes.
-    """
-    node_df = graph.get_nodes()
-    coords = graph.get_coords()
-    if hide_map:
-        node_df = node_df[node_df.original_type != "map"]
-    plt = (
-        ggplot()
-        + geom_segment(
-            aes(x="x", y="y", xend="xend", yend="yend"),
-            color=coords["fgcolor"].tolist(),
-            data=coords,
-        )
-        + geom_point(aes(x="x", y="y"), color=node_df["fgcolor"].tolist(), data=node_df)
-        + theme_void()
-    )
-    return plt
-
-
 def hex2rgb(hex_str):
     """Convert hex string to rgb tuple.
 
     Parameters:
     -----------
     hex_str: str
         hex string, e.g. "#ffffff".
```

### Comparing `pykegg-0.1.5/.gitignore` & `pykegg-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pykegg-0.1.5/README.md` & `pykegg-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pykegg-0.1.5/pyproject.toml` & `pykegg-0.1.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 authors = [
   { name="Noriaki Sato", email="nori@hgc.jp" },
 ]
 dependencies = [
     "igraph",
     "pandas",
     "biopython",
-    "plotnine",
     "requests",
     "opencv-python"
 ]
 description = "Visualizing and analyzing KEGG information in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pykegg-0.1.5/PKG-INFO` & `pykegg-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pykegg
-Version: 0.1.5
+Version: 0.1.6
 Summary: Visualizing and analyzing KEGG information in Python
 Project-URL: Homepage, https://github.com/noriakis/pykegg
 Project-URL: Bug Tracker, https://github.com/noriakis/pykegg/issues
 Author-email: Noriaki Sato <nori@hgc.jp>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: biopython
 Requires-Dist: igraph
 Requires-Dist: opencv-python
 Requires-Dist: pandas
-Requires-Dist: plotnine
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # pykegg
 Analyze and visualize KEGG information using network approach.
 
 Using `biopython`, `igraph` and [`plotnine`](https://github.com/has2k1/plotnine), parse the KGML into `igraph` and easily plot the relevant information contained in KEGG Pathway in Python environment.
```

