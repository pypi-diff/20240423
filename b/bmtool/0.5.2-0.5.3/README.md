# Comparing `tmp/bmtool-0.5.2.tar.gz` & `tmp/bmtool-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmtool-0.5.2.tar", last modified: Tue Mar  5 19:26:27 2024, max compression
+gzip compressed data, was "bmtool-0.5.3.tar", last modified: Tue Apr 23 18:03:00 2024, max compression
```

## Comparing `bmtool-0.5.2.tar` & `bmtool-0.5.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-03-05 19:26:27.697373 bmtool-0.5.2/
--rw-r--r--   0 gregglickert   (501) staff       (20)     1068 2024-02-06 16:24:55.000000 bmtool-0.5.2/LICENSE
--rw-r--r--   0 gregglickert   (501) staff       (20)    21237 2024-03-05 19:26:27.696692 bmtool-0.5.2/PKG-INFO
--rw-r--r--   0 gregglickert   (501) staff       (20)    20289 2024-03-05 19:23:42.000000 bmtool-0.5.2/README.md
-drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-03-05 19:26:27.683134 bmtool-0.5.2/bmtool/
--rw-r--r--   0 gregglickert   (501) staff       (20)      136 2024-02-13 18:15:29.000000 bmtool-0.5.2/bmtool/__init__.py
--rw-r--r--   0 gregglickert   (501) staff       (20)      650 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/__main__.py
--rw-r--r--   0 gregglickert   (501) staff       (20)    35922 2024-03-05 19:15:01.000000 bmtool-0.5.2/bmtool/bmplot.py
--rw-r--r--   0 gregglickert   (501) staff       (20)    59610 2024-02-16 20:14:51.000000 bmtool-0.5.2/bmtool/connectors.py
-drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-03-05 19:26:27.689529 bmtool-0.5.2/bmtool/debug/
--rw-r--r--   0 gregglickert   (501) staff       (20)        0 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/debug/__init__.py
--rw-r--r--   0 gregglickert   (501) staff       (20)      583 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/debug/commands.py
--rw-r--r--   0 gregglickert   (501) staff       (20)      207 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/debug/debug.py
--rw-r--r--   0 gregglickert   (501) staff       (20)      657 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/manage.py
--rw-r--r--   0 gregglickert   (501) staff       (20)    12298 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/plot_commands.py
--rw-r--r--   0 gregglickert   (501) staff       (20)    24997 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/singlecell.py
-drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-03-05 19:26:27.692563 bmtool-0.5.2/bmtool/util/
--rw-r--r--   0 gregglickert   (501) staff       (20)        0 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/util/__init__.py
--rw-r--r--   0 gregglickert   (501) staff       (20)    64396 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/util/commands.py
-drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-03-05 19:26:27.694416 bmtool-0.5.2/bmtool/util/neuron/
--rw-r--r--   0 gregglickert   (501) staff       (20)        0 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/util/neuron/__init__.py
--rw-r--r--   0 gregglickert   (501) staff       (20)    87194 2024-02-13 18:15:30.000000 bmtool-0.5.2/bmtool/util/neuron/celltuner.py
--rw-r--r--   0 gregglickert   (501) staff       (20)    53496 2024-03-05 19:15:35.000000 bmtool-0.5.2/bmtool/util/util.py
-drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-03-05 19:26:27.695968 bmtool-0.5.2/bmtool.egg-info/
--rw-r--r--   0 gregglickert   (501) staff       (20)    21237 2024-03-05 19:26:27.000000 bmtool-0.5.2/bmtool.egg-info/PKG-INFO
--rw-r--r--   0 gregglickert   (501) staff       (20)      549 2024-03-05 19:26:27.000000 bmtool-0.5.2/bmtool.egg-info/SOURCES.txt
--rw-r--r--   0 gregglickert   (501) staff       (20)        1 2024-03-05 19:26:27.000000 bmtool-0.5.2/bmtool.egg-info/dependency_links.txt
--rw-r--r--   0 gregglickert   (501) staff       (20)       45 2024-03-05 19:26:27.000000 bmtool-0.5.2/bmtool.egg-info/entry_points.txt
--rw-r--r--   0 gregglickert   (501) staff       (20)       76 2024-03-05 19:26:27.000000 bmtool-0.5.2/bmtool.egg-info/requires.txt
--rw-r--r--   0 gregglickert   (501) staff       (20)        7 2024-03-05 19:26:27.000000 bmtool-0.5.2/bmtool.egg-info/top_level.txt
--rw-r--r--   0 gregglickert   (501) staff       (20)       38 2024-03-05 19:26:27.697591 bmtool-0.5.2/setup.cfg
--rw-r--r--   0 gregglickert   (501) staff       (20)     1301 2024-03-05 19:26:23.000000 bmtool-0.5.2/setup.py
+drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-04-23 18:03:00.723110 bmtool-0.5.3/
+-rw-r--r--   0 gregglickert   (501) staff       (20)     1068 2024-02-06 16:24:55.000000 bmtool-0.5.3/LICENSE
+-rw-r--r--   0 gregglickert   (501) staff       (20)    24084 2024-04-23 18:03:00.722371 bmtool-0.5.3/PKG-INFO
+-rw-r--r--   0 gregglickert   (501) staff       (20)    23060 2024-04-23 17:59:54.000000 bmtool-0.5.3/README.md
+drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-04-23 18:03:00.711199 bmtool-0.5.3/bmtool/
+-rw-r--r--   0 gregglickert   (501) staff       (20)      136 2024-02-13 18:15:29.000000 bmtool-0.5.3/bmtool/__init__.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)      650 2024-02-13 18:15:30.000000 bmtool-0.5.3/bmtool/__main__.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)    39680 2024-04-23 17:30:51.000000 bmtool-0.5.3/bmtool/bmplot.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)    66376 2024-04-18 15:49:10.000000 bmtool-0.5.3/bmtool/connectors.py
+drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-04-23 18:03:00.716333 bmtool-0.5.3/bmtool/debug/
+-rw-r--r--   0 gregglickert   (501) staff       (20)        0 2024-02-13 18:15:30.000000 bmtool-0.5.3/bmtool/debug/__init__.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)      583 2024-02-13 18:15:30.000000 bmtool-0.5.3/bmtool/debug/commands.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)      207 2024-02-13 18:15:30.000000 bmtool-0.5.3/bmtool/debug/debug.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)     5752 2024-04-23 17:28:14.000000 bmtool-0.5.3/bmtool/graphs.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)      657 2024-02-13 18:15:30.000000 bmtool-0.5.3/bmtool/manage.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)    12298 2024-02-13 18:15:30.000000 bmtool-0.5.3/bmtool/plot_commands.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)    24965 2024-03-15 14:38:55.000000 bmtool-0.5.3/bmtool/singlecell.py
+drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-04-23 18:03:00.718708 bmtool-0.5.3/bmtool/util/
+-rw-r--r--   0 gregglickert   (501) staff       (20)        0 2024-02-13 18:15:30.000000 bmtool-0.5.3/bmtool/util/__init__.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)    64396 2024-02-13 18:15:30.000000 bmtool-0.5.3/bmtool/util/commands.py
+drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-04-23 18:03:00.720347 bmtool-0.5.3/bmtool/util/neuron/
+-rw-r--r--   0 gregglickert   (501) staff       (20)        0 2024-02-13 18:15:30.000000 bmtool-0.5.3/bmtool/util/neuron/__init__.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)    87194 2024-02-13 18:15:30.000000 bmtool-0.5.3/bmtool/util/neuron/celltuner.py
+-rw-r--r--   0 gregglickert   (501) staff       (20)    56060 2024-04-23 17:04:53.000000 bmtool-0.5.3/bmtool/util/util.py
+drwxr-xr-x   0 gregglickert   (501) staff       (20)        0 2024-04-23 18:03:00.721634 bmtool-0.5.3/bmtool.egg-info/
+-rw-r--r--   0 gregglickert   (501) staff       (20)    24084 2024-04-23 18:03:00.000000 bmtool-0.5.3/bmtool.egg-info/PKG-INFO
+-rw-r--r--   0 gregglickert   (501) staff       (20)      566 2024-04-23 18:03:00.000000 bmtool-0.5.3/bmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 gregglickert   (501) staff       (20)        1 2024-04-23 18:03:00.000000 bmtool-0.5.3/bmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 gregglickert   (501) staff       (20)       45 2024-04-23 18:03:00.000000 bmtool-0.5.3/bmtool.egg-info/entry_points.txt
+-rw-r--r--   0 gregglickert   (501) staff       (20)       83 2024-04-23 18:03:00.000000 bmtool-0.5.3/bmtool.egg-info/requires.txt
+-rw-r--r--   0 gregglickert   (501) staff       (20)        7 2024-04-23 18:03:00.000000 bmtool-0.5.3/bmtool.egg-info/top_level.txt
+-rw-r--r--   0 gregglickert   (501) staff       (20)       38 2024-04-23 18:03:00.723241 bmtool-0.5.3/setup.cfg
+-rw-r--r--   0 gregglickert   (501) staff       (20)     1373 2024-04-23 18:01:45.000000 bmtool-0.5.3/setup.py
```

### Comparing `bmtool-0.5.2/LICENSE` & `bmtool-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bmtool-0.5.2/PKG-INFO` & `bmtool-0.5.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,19 @@
-Metadata-Version: 2.1
-Name: bmtool
-Version: 0.5.2
-Summary: BMTool
-Home-page: https://github.com/cyneuro/bmtool
-Download-URL: 
-Author: Tyler Banks
-Author-email: tbanks@mail.missouri.edu
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: bmtk
-Requires-Dist: click
-Requires-Dist: clint
-Requires-Dist: h5py
-Requires-Dist: matplotlib
-Requires-Dist: networkx
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: questionary
-Requires-Dist: pynmodlt
-
 # bmtool
 A collection of modules to make developing [Neuron](https://www.neuron.yale.edu/neuron/) and [BMTK](https://alleninstitute.github.io/bmtk/) models easier.
 
 [![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/cyneuro/bmtool/blob/master/LICENSE) 
 
 ## Table of Contents
 - [Getting Started](#Getting-Started)
 - [CLI](#CLI)
 - [Single Cell](#Single-Cell-Module)
 - [Connectors](#Connectors-Module)
 - [Bmplot](#bmplot-Module)
+- [Graphs](#graphs-module)
 
 ## Getting Started
 
 **Installation**
 ```bash
 pip install bmtool
 ```
@@ -387,14 +357,15 @@
 ```
 
 ## Bmplot Module
 - [Total connections](#Total-connection-plot)
 - [Percent connections](#Percent-connection-plot)
 - [Convergence connnections](#convergence-plot)
 - [Divergence connections](#divergence-plot)
+- [Gap Junction connections](#gap-junction-plot)
 - [connection histogram](#connection-histogram)
 - [probability connection](#probability-of-connection-plot)
 - [3D location](#3d-position-plot)
 - [3D rotation](#cell-rotations)
 - [Plot Connection Diagram](#plot-connection-diagram)
 
 ### Total connection plot
@@ -448,14 +419,25 @@
 bmplot.divergence_connection_matrix(config='config.json',sources='LA',targets='LA',tids='pop_name',sids='pop_name',no_prepend_pop=True,include_gap=False,method='mean+std')
 ```
 
 
     
 ![png](readme_figures/output_25_0.png)
     
+### Gap Junction plot
+#### While gap junctions can be include in the above plots, you can use this function to only view gap junctions.Type can be either 'convergence' or 'percent' connections to generate different plots
+
+
+```python
+bmplot.gap_junction_matrix(config='config.json',sources='LA',targets='LA',sids='pop_name',tids='pop_name',no_prepend_pop=True,type='percent')
+```
+
+
+    
+![png](output_gap.png)
 
 
 ### Connection histogram 
 #### Generates a histogram of the distribution of connections a population of cells give to individual cells of another population 
 
 
 ```python
@@ -772,9 +754,131 @@
 </table>
 
 
 
 
 
     'LA'
+## Graphs Module
+- [Generate graph](#generate-graph)
+- [Plot Graph](#plot-graph)
+- [Connectioon table](#generate-graph-connection-table)
+
+### Generate Graph
+
+
+```python
+from bmtool import graphs
+import networkx as nx
+
+Graph = graphs.generate_graph(config='config.json',source='LA',target='LA')
+print("Number of nodes:", Graph.number_of_nodes())
+print("Number of edges:", Graph.number_of_edges())
+print("Node labels:", set(nx.get_node_attributes(Graph, 'label').values()))
+```
+
+    Number of nodes: 2000
+    Number of edges: 84235
+    Node labels: {'SOM', 'PNc', 'PNa', 'PV'}
+
+
+### Plot Graph
+#### Generates an interactive plot showing nodes, edges and # of connections
+
+
+```python
+graphs.plot_graph(Graph)
+```
+
+
+
+### Generate graph connection table
+#### Generates a CSV of all cells and the number of connections each individual cell receives
+
+
+```python
+import pandas as pd
+graphs.export_node_connections_to_csv(Graph, 'node_connections.csv')
+df = pd.read_csv('node_connections.csv')
+df.head()
+```
+
+
+
+
+<div>
+<style scoped>
+    .dataframe tbody tr th:only-of-type {
+        vertical-align: middle;
+    }
+
+    .dataframe tbody tr th {
+        vertical-align: top;
+    }
+
+    .dataframe thead th {
+        text-align: right;
+    }
+</style>
+<table border="1" class="dataframe">
+  <thead>
+    <tr style="text-align: right;">
+      <th></th>
+      <th>Unnamed: 0</th>
+      <th>Node Label</th>
+      <th>PNc Connections</th>
+      <th>PV Connections</th>
+      <th>SOM Connections</th>
+      <th>PNa Connections</th>
+    </tr>
+  </thead>
+  <tbody>
+    <tr>
+      <th>0</th>
+      <td>0</td>
+      <td>PNa</td>
+      <td>15</td>
+      <td>11</td>
+      <td>9</td>
+      <td>6</td>
+    </tr>
+    <tr>
+      <th>1</th>
+      <td>1</td>
+      <td>PNa</td>
+      <td>24</td>
+      <td>25</td>
+      <td>6</td>
+      <td>21</td>
+    </tr>
+    <tr>
+      <th>2</th>
+      <td>2</td>
+      <td>PNa</td>
+      <td>27</td>
+      <td>28</td>
+      <td>12</td>
+      <td>25</td>
+    </tr>
+    <tr>
+      <th>3</th>
+      <td>3</td>
+      <td>PNa</td>
+      <td>19</td>
+      <td>27</td>
+      <td>15</td>
+      <td>35</td>
+    </tr>
+    <tr>
+      <th>4</th>
+      <td>4</td>
+      <td>PNa</td>
+      <td>25</td>
+      <td>11</td>
+      <td>8</td>
+      <td>16</td>
+    </tr>
+  </tbody>
+</table>
+</div>
```

### Comparing `bmtool-0.5.2/README.md` & `bmtool-0.5.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,51 @@
+Metadata-Version: 2.1
+Name: bmtool
+Version: 0.5.3
+Summary: BMTool
+Home-page: https://github.com/cyneuro/bmtool
+Download-URL: 
+Author: Neural Engineering Laboratory at the University of Missouri
+Author-email: gregglickert@mail.missouri.edu
+License: MIT
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: bmtk
+Requires-Dist: click
+Requires-Dist: clint
+Requires-Dist: h5py
+Requires-Dist: matplotlib
+Requires-Dist: networkx
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: questionary
+Requires-Dist: pynmodlt
+Requires-Dist: plotly
+
 # bmtool
 A collection of modules to make developing [Neuron](https://www.neuron.yale.edu/neuron/) and [BMTK](https://alleninstitute.github.io/bmtk/) models easier.
 
 [![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/cyneuro/bmtool/blob/master/LICENSE) 
 
 ## Table of Contents
 - [Getting Started](#Getting-Started)
 - [CLI](#CLI)
 - [Single Cell](#Single-Cell-Module)
 - [Connectors](#Connectors-Module)
 - [Bmplot](#bmplot-Module)
+- [Graphs](#graphs-module)
 
 ## Getting Started
 
 **Installation**
 ```bash
 pip install bmtool
 ```
@@ -356,14 +389,15 @@
 ```
 
 ## Bmplot Module
 - [Total connections](#Total-connection-plot)
 - [Percent connections](#Percent-connection-plot)
 - [Convergence connnections](#convergence-plot)
 - [Divergence connections](#divergence-plot)
+- [Gap Junction connections](#gap-junction-plot)
 - [connection histogram](#connection-histogram)
 - [probability connection](#probability-of-connection-plot)
 - [3D location](#3d-position-plot)
 - [3D rotation](#cell-rotations)
 - [Plot Connection Diagram](#plot-connection-diagram)
 
 ### Total connection plot
@@ -417,14 +451,25 @@
 bmplot.divergence_connection_matrix(config='config.json',sources='LA',targets='LA',tids='pop_name',sids='pop_name',no_prepend_pop=True,include_gap=False,method='mean+std')
 ```
 
 
     
 ![png](readme_figures/output_25_0.png)
     
+### Gap Junction plot
+#### While gap junctions can be include in the above plots, you can use this function to only view gap junctions.Type can be either 'convergence' or 'percent' connections to generate different plots
+
+
+```python
+bmplot.gap_junction_matrix(config='config.json',sources='LA',targets='LA',sids='pop_name',tids='pop_name',no_prepend_pop=True,type='percent')
+```
+
+
+    
+![png](output_gap.png)
 
 
 ### Connection histogram 
 #### Generates a histogram of the distribution of connections a population of cells give to individual cells of another population 
 
 
 ```python
@@ -741,9 +786,131 @@
 </table>
 
 
 
 
 
     'LA'
+## Graphs Module
+- [Generate graph](#generate-graph)
+- [Plot Graph](#plot-graph)
+- [Connectioon table](#generate-graph-connection-table)
+
+### Generate Graph
+
+
+```python
+from bmtool import graphs
+import networkx as nx
+
+Graph = graphs.generate_graph(config='config.json',source='LA',target='LA')
+print("Number of nodes:", Graph.number_of_nodes())
+print("Number of edges:", Graph.number_of_edges())
+print("Node labels:", set(nx.get_node_attributes(Graph, 'label').values()))
+```
+
+    Number of nodes: 2000
+    Number of edges: 84235
+    Node labels: {'SOM', 'PNc', 'PNa', 'PV'}
+
+
+### Plot Graph
+#### Generates an interactive plot showing nodes, edges and # of connections
+
+
+```python
+graphs.plot_graph(Graph)
+```
+
+
+
+### Generate graph connection table
+#### Generates a CSV of all cells and the number of connections each individual cell receives
+
+
+```python
+import pandas as pd
+graphs.export_node_connections_to_csv(Graph, 'node_connections.csv')
+df = pd.read_csv('node_connections.csv')
+df.head()
+```
+
+
+
+
+<div>
+<style scoped>
+    .dataframe tbody tr th:only-of-type {
+        vertical-align: middle;
+    }
+
+    .dataframe tbody tr th {
+        vertical-align: top;
+    }
+
+    .dataframe thead th {
+        text-align: right;
+    }
+</style>
+<table border="1" class="dataframe">
+  <thead>
+    <tr style="text-align: right;">
+      <th></th>
+      <th>Unnamed: 0</th>
+      <th>Node Label</th>
+      <th>PNc Connections</th>
+      <th>PV Connections</th>
+      <th>SOM Connections</th>
+      <th>PNa Connections</th>
+    </tr>
+  </thead>
+  <tbody>
+    <tr>
+      <th>0</th>
+      <td>0</td>
+      <td>PNa</td>
+      <td>15</td>
+      <td>11</td>
+      <td>9</td>
+      <td>6</td>
+    </tr>
+    <tr>
+      <th>1</th>
+      <td>1</td>
+      <td>PNa</td>
+      <td>24</td>
+      <td>25</td>
+      <td>6</td>
+      <td>21</td>
+    </tr>
+    <tr>
+      <th>2</th>
+      <td>2</td>
+      <td>PNa</td>
+      <td>27</td>
+      <td>28</td>
+      <td>12</td>
+      <td>25</td>
+    </tr>
+    <tr>
+      <th>3</th>
+      <td>3</td>
+      <td>PNa</td>
+      <td>19</td>
+      <td>27</td>
+      <td>15</td>
+      <td>35</td>
+    </tr>
+    <tr>
+      <th>4</th>
+      <td>4</td>
+      <td>PNa</td>
+      <td>25</td>
+      <td>11</td>
+      <td>8</td>
+      <td>16</td>
+    </tr>
+  </tbody>
+</table>
+</div>
```

### Comparing `bmtool-0.5.2/bmtool/__main__.py` & `bmtool-0.5.3/bmtool/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.5.2/bmtool/bmplot.py` & `bmtool-0.5.3/bmtool/bmplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Want to be able to take multiple plot names in and plot them all at the same time, to save time
 https://stackoverflow.com/questions/458209/is-there-a-way-to-detach-matplotlib-plots-so-that-the-computation-can-continue
 """
 from .util import util
-
 import argparse,os,sys
 
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 import matplotlib.cm as cmx
 import matplotlib.colors as colors
@@ -263,14 +262,90 @@
         if convergence:
             title = title + "Synaptic Convergence"
         else:
             title = title + "Synaptic Divergence"
     plot_connection_info(syn_info,data,source_labels,target_labels,title, save_file=save_file)
     return
 
+def gap_junction_matrix(config=None,title=None,sources=None, targets=None, sids=None,tids=None, no_prepend_pop=False,save_file=None,type='convergence'):
+    """
+    Generates connection plot displaying gap junction data.
+    config: A BMTK simulation config 
+    sources: network name(s) to plot
+    targets: network name(s) to plot
+    sids: source node identifier 
+    tids: target node identifier
+    no_prepend_pop: dictates if population name is displayed before sid or tid when displaying graph
+    save_file: If plot should be saved
+    type:'convergence' or 'percent' connections
+    """
+    if not config:
+        raise Exception("config not defined")
+    if not sources or not targets:
+        raise Exception("Sources or targets not defined")
+    if type !='convergence' and type!='percent':
+        raise Exception("type must be 'convergence' or 'percent'")
+    sources = sources.split(",")
+    targets = targets.split(",")
+    if sids:
+        sids = sids.split(",")
+    else:
+        sids = []
+    if tids:
+        tids = tids.split(",")
+    else:
+        tids = []
+    syn_info, data, source_labels, target_labels = util.gap_junction_connections(config=config,nodes=None,edges=None,sources=sources,targets=targets,sids=sids,tids=tids,prepend_pop=not no_prepend_pop,type=type)
+    
+    
+    def filter_rows(syn_info, data, source_labels, target_labels):
+        new_syn_info = syn_info
+        new_data = data
+        new_source_labels = source_labels
+        new_target_labels = target_labels
+        for row in new_data:
+            row_index = -1
+            try:
+                if((np.isnan(row).all())): #checks if all of a row is nan
+                    row_index = np.where(np.isnan(new_data)==np.isnan(row))[0][0]  
+            except:
+                row_index = -1
+            finally:          
+                if(all(x==0 for x in row)): #checks if all of a row is zeroes
+                    row_index = np.where(new_data==row)[0][0] 
+                if row_index!=-1:   #deletes corresponding row accordingly in all relevant variables.
+                    new_syn_info = np.delete(new_syn_info,row_index,0) 
+                    new_data = np.delete(new_data,row_index,0)
+                    new_source_labels = np.delete(new_source_labels,row_index)
+        return new_syn_info, new_data,new_source_labels,new_target_labels
+
+    def filter_rows_and_columns(syn_info,data,source_labels,target_labels):
+        syn_info, data, source_labels, target_labels = filter_rows(syn_info, data, source_labels, target_labels)
+        transposed_syn_info = np.transpose(syn_info) #transpose everything and put it in to make sure columns get filtered
+        transposed_data = np.transpose(data)
+        transposed_source_labels = target_labels
+        transposed_target_labels = source_labels
+        syn_info, data, source_labels, target_labels = filter_rows(transposed_syn_info, transposed_data, transposed_source_labels, transposed_target_labels)
+        filtered_syn_info = np.transpose(syn_info) #transpose everything back to original order after filtering.
+        filtered_data = np.transpose(data)
+        filtered_source_labels = target_labels
+        filtered_target_labels = source_labels
+        return filtered_syn_info,filtered_data,filtered_source_labels,filtered_target_labels
+    
+    syn_info, data, source_labels, target_labels = filter_rows_and_columns(syn_info, data, source_labels, target_labels)
+
+    if title == None or title=="":
+        title = 'Gap Junction'
+        if type == 'convergence':
+            title+=' Syn Convergence'
+        elif type == 'percent':
+            title+=' Percent Connectivity'
+    plot_connection_info(syn_info,data,source_labels,target_labels,title, save_file=save_file)
+    return
+    
 def connection_histogram(config=None,nodes=None,edges=None,sources=[],targets=[],sids=[],tids=[],prepend_pop=True,synaptic_info='0',
                       source_cell = None,target_cell = None,include_gap=True):
     """
     Generates histogram of number of connections individual cells in a population receieve from another population
     config: A BMTK simulation config 
     sources: network name(s) to plot
     targets: network name(s) to plot
```

### Comparing `bmtool-0.5.2/bmtool/connectors.py` & `bmtool-0.5.3/bmtool/connectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from abc import ABC, abstractmethod
 import numpy as np
 from scipy.special import erf
 from scipy.optimize import minimize_scalar
 from functools import partial
 import time
+import types
 
 rng = np.random.default_rng()
 
 ##############################################################################
 ############################## CONNECT CELLS #################################
 
 # Utility Functions
+def num_prop(ratio, N):
+    """Calculate numbers of total N in proportion to ratio"""
+    ratio = np.asarray(ratio)
+    p = np.cumsum(np.insert(ratio.ravel(), 0, 0))  # cumulative proportion
+    return np.diff(np.round(N / p[-1] * p).astype(int)).reshape(ratio.shape)
+
+
 def decision(prob, size=None):
     """
     Make single random decision based on input probability.
     prob: scalar input
     Return bool array if size specified, otherwise scalar
     """
     return rng.random(size) < prob
@@ -72,38 +80,41 @@
 class DistantDependentProbability(ProbabilityFunction):
     """Base class for distance dependent probability"""
 
     def __init__(self, min_dist=0., max_dist=np.inf):
         assert(min_dist >= 0 and min_dist < max_dist)
         self.min_dist, self.max_dist = min_dist, max_dist
 
-    def __call__(self, dist):
+    def __call__(self, dist, *arg, **kwargs):
         """Return probability for single distance input"""
         if dist >= self.min_dist and dist <= self.max_dist:
-            return self.probability(dist).item()
+            return self.probability(dist)
         else:
             return 0.
 
     def decisions(self, dist):
         """Return bool array of decisions given distance array"""
         dist = np.asarray(dist)
         dec = np.zeros(dist.shape, dtype=bool)
         mask = (dist >= self.min_dist) & (dist <= self.max_dist)
-        dec[mask] = decisions(self.probability(dist[mask]))
+        dist = dist[mask]
+        prob = np.empty(dist.shape)
+        prob[:] = self.probability(dist)
+        dec[mask] = decisions(prob)
         return dec
 
 
 class UniformInRange(DistantDependentProbability):
     """Constant probability within a distance range"""
 
     def __init__(self, p=0., min_dist=0., max_dist=np.inf):
         super().__init__(min_dist=min_dist, max_dist=max_dist)
         self.p = np.array(p)
         assert(self.p.size == 1)
-        assert(self.p >= 0. and self.p <= 1.)
+        assert(p >= 0. and p <= 1.)
 
     def probability(self, dist):
         return self.p
 
 
 NORM_COEF = (2 * np.pi) ** (-.5)  # coefficient of standard normal PDF
 
@@ -123,15 +134,15 @@
         min_dist, max_dist: Distance range for any possible connection,
             the support of the Gaussian function.
         pmax: The maximum value of the Gaussian function at its mean parameter.
         ptotal: Overall probability within distance range. If specified, ignore
             input pmax, and calculate pmax. See calc_pmax_from_ptotal() method.
         ptotal_dist_range: Distance range for calculating pmax when ptotal is
         specified. If not specified, set to range (min_dist, max_dist).
-        dist_type: spherical or cylindrical for distance metric.
+        dist_type: 'spherical' or 'cylindrical' for distance metric.
             Used when ptotal is specified.
 
     Returns:
         A callable object. When called with a single distance input,
         returns the probability value.
 
     TODO: Accept convergence and cell density information for calculating pmax.
@@ -211,14 +222,59 @@
                 warn += " ptotal may not be reached."
             print(warn)
             self.probability = lambda dist: np.fmin(probability(dist), 1.)
         else:
             self.probability = probability
 
 
+class NormalizedReciprocalRate(ProbabilityFunction):
+    """Reciprocal connection probability given normalized reciprocal rate.
+    Normalized reciprocal rate is defined as the ratio between the reciprocal
+    connection probability and the connection probability for a randomly
+    connected network where the two unidirectional connections between any pair
+    of neurons are independent. NRR = pr / (p0 * p1)
+    
+    Parameters:
+        NRR: a constant or distance dependent function for normalized reciprocal
+            rate. When being a function, it should be accept vectorized input.
+    Returns:
+        A callable object that returns the probability value.
+    """
+
+    def __init__(self, NRR=1.):
+        self.NRR = NRR if callable(NRR) else lambda *x: NRR
+
+    def probability(self, dist, p0, p1):
+        """Allow numpy array input and return probability in numpy array"""
+        return p0 * p1 * self.NRR(dist)
+
+    def __call__(self, dist, p0, p1, *arg, **kwargs):
+        """Return probability for single distance input"""
+        return self.probability(dist, p0, p1)
+
+    def decisions(self, dist, p0, p1, cond=None):
+        """Return bool array of decisions
+        dist: distance (scalar or array). Will be ignored if NRR is constant.
+        p0, p1: forward and backward probability (scalar or array)
+        cond: A tuple (direction, array of outcomes) representing the condition.
+            Conditional probability will be returned if specified. The condition
+            event is determined by connection direction (0 for forward, or 1 for
+            backward) and outcomes (bool array of whether connection exists).
+        """
+        dist, p0, p1 = map(np.asarray, (dist, p0, p1))
+        pr = np.empty(dist.shape)
+        pr[:] = self.probability(dist, p0, p1)
+        pr = np.clip(pr, a_min=np.fmax(p0 + p1 - 1., 0.), a_max=np.fmin(p0, p1))
+        if cond is not None:
+            mask = np.asarray(cond[1])
+            pr[mask] /= p1 if cond[0] else p0
+            pr[~mask] = 0.
+        return decisions(pr)
+
+
 # Connector Classes
 class AbstractConnector(ABC):
     """Abstract base class for connectors"""
     @abstractmethod
     def setup_nodes(self, source=None, target=None):
         """After network nodes are added to the BMTK network. Pass in the
         Nodepool objects of source and target nodes using this method.
@@ -228,38 +284,38 @@
     @abstractmethod
     def edge_params(self, **kwargs):
         """Create the arguments for BMTK add_edges() method including the
         `connection_rule` method."""
         return NotImplemented
 
     @staticmethod
-    def is_same_pop(source, target, quick=True):
-        """Whether two NodePool objects direct to the same population"""
-        if quick:
-            # Quick check (compare filter conditions)
-            same = (source.network_name == target.network_name and
-                    source._NodePool__properties ==
-                    target._NodePool__properties)
-        else:
-            # Strict check (compare all nodes)
-            same = (source.network_name == target.network_name and
-                    len(source) == len(target) and
-                    all([s.node_id == t.node_id
-                         for s, t in zip(source, target)]))
-        return same
-
-    @staticmethod
     def constant_function(val):
         """Convert a constant to a constant function"""
         def constant(*arg):
             return val
         return constant
 
 
-# Helper class
+# Helper functions
+def is_same_pop(source, target, quick=False):
+    """Check whether two NodePool objects direct to the same population"""
+    if quick:
+        # Quick check (compare filter conditions)
+        same = (source.network_name == target.network_name and
+                source._NodePool__properties ==
+                target._NodePool__properties)
+    else:
+        # Strict check (compare all nodes)
+        same = (source.network_name == target.network_name and
+                len(source) == len(target) and
+                all([s.node_id == t.node_id
+                     for s, t in zip(source, target)]))
+    return same
+
+
 class Timer(object):
     def __init__(self, unit='sec'):
         if unit == 'ms':
             self.scale = 1e3
         elif unit == 'us':
             self.scale = 1e6
         elif unit == 'min':
@@ -299,15 +355,15 @@
         print('rho changed from %.3f to %.3f; pr changed from %.3f to %.3f'
               % (rho0, rho, pr0, pr))
     return pr
 
 
 class ReciprocalConnector(AbstractConnector):
     """
-    Object for building connections in bmtk network model with reciprocal
+    Object for buiilding connections in bmtk network model with reciprocal
     probability within a single population (or between two populations).
 
     Algorithm:
         Create random connection for every pair of cells independently,
         following a bivariate Bernoulli distribution. Each variable is 0 or 1,
         whether a connection exists in a forward or backward direction. There
         are four possible outcomes for each pair, no connection, unidirectional
@@ -384,18 +440,25 @@
             When p0 and p1 does not need inputs arguments, set p0_arg and
             p1_arg to None as so by default. Functions p0 and p1 need to accept
             one unused positional argument as placeholder, e.g., p0(*args), so
             it does not raise an error when p0(None) is called.
         symmetric_p1_arg: Whether p0_arg and p1_arg are identical. If this is
             set to True, argument p1_arg will be ignored. This is forced to be
             True when the population is recurrent.
-        pr, pr_arg: Probability of reciprocal connection and its input argument
-            when it is a function, similar to p0, p0_arg, p1, p1_arg. It can be
-            a function when it has an explicit relation with some node
-            properties such as distance.
+        pr, pr_arg: Probability of reciprocal connection and its first input
+            argument when it is a function, similar to p0, p0_arg, p1, p1_arg.
+            It can be a function when it has an explicit relation with some node
+            properties such as distance. A function pr requires two additional
+            positional arguments p0 and p1 even if they are not used, i.e.,
+            pr(pr_arg, p0, p1), just in case pr is dependent on p0 and p1, e.g.,
+            when normalized reciprocal rate NRR = pr/(p0*p1) is given.
+            When pr_arg is a string, the same value as p1_arg will be used for
+            pr_arg if the string contains '1', e.g., '1', 'p1'. Otherwise, e.g.,
+            '', '0', 'p0', p0_arg will be used for pr_arg. Specifying this can
+            avoid recomputing pr_arg when it's given by p0_arg or p1_arg.
         estimate_rho: Whether estimate rho that result in an overall pr. This
             is forced to be False if pr is a function or if rho is specified.
             To estimate rho, all the pairs with possible connections, meaning
             p0 and p1 are both non-zero for these pairs, are used to estimate
             a value of rho that will result in an expected number of reciprocal
             connections with the given pr. Note that pr is not over all pairs
             of source and target cells but only those has a chance to connect,
@@ -421,14 +484,18 @@
             or random) function whose input arguments are two node objects in
             BMTK like p0_arg, p1_arg. n_syn1 is force to be the same as n_syn0
             when the population is recurrent. Warning: The number must not be
             greater than 255 since it will be converted to uint8 when written
             into the connection matrix to reduce memory consumption.
         autapses: Whether to allow connecting a cell to itself. Default: False.
             This is ignored when the population is not recurrent.
+        quick_pop_check: Whether to use quick method to check if source and
+            target populations are the same. Default: False.
+            Quick method checks only whether filter conditions match.
+            Strict method checks whether all node id's match considering order.
         cache_data: Whether to cache the values of p0, p0_arg, p1, p1_arg
             during estimation of rho. This improves performance when
             estimate_rho is True while not creating a significant overhead in
             the opposite case. However, it requires large memory allocation
             as the population size grows. Set it to False if there is a memory
             issue.
         verbose: Whether show verbose information in console.
@@ -461,58 +528,59 @@
     """
 
     def __init__(self, p0=1., p1=1., symmetric_p1=False,
                  p0_arg=None, p1_arg=None, symmetric_p1_arg=False,
                  pr=0., pr_arg=None, estimate_rho=True, rho=None,
                  dist_range_forward=None, dist_range_backward=None,
                  n_syn0=1, n_syn1=1, autapses=False,
-                 cache_data=True, verbose=True):
+                 quick_pop_check=False, cache_data=True, verbose=True):
         args = locals()
         var_set = ('p0', 'p0_arg', 'p1', 'p1_arg',
                    'pr', 'pr_arg', 'n_syn0', 'n_syn1')
         self.vars = {key: args[key] for key in var_set}
 
         self.symmetric_p1 = symmetric_p1 and symmetric_p1_arg
         self.symmetric_p1_arg = symmetric_p1_arg
 
         self.estimate_rho = estimate_rho and not callable(pr) and rho is None
         self.dist_range_forward = dist_range_forward
         self.dist_range_backward = dist_range_backward
         self.rho = rho
 
         self.autapses = autapses
+        self.quick = quick_pop_check
         self.cache = self.ConnectorCache(cache_data and self.estimate_rho)
         self.verbose = verbose
 
         self.conn_prop = [{}, {}]
         self.stage = 0
         self.iter_count = 0
 
     # *** Two methods executed during bmtk edge creation net.add_edges() ***
     def setup_nodes(self, source=None, target=None):
         """Must run this before building connections"""
         if self.stage:
             # check whether the correct populations
             if (source is None or target is None or
-                    not self.is_same_pop(source, self.target) or
-                    not self.is_same_pop(target, self.source)):
+                    not is_same_pop(source, self.target, quick=self.quick) or
+                    not is_same_pop(target, self.source, quick=self.quick)):
                 raise ValueError("Source or target population not consistent.")
             # Skip adding nodes for the backward stage.
             return
 
         # Update node pools
         self.source = source
         self.target = target
         if self.source is None or len(self.source) == 0:
             raise ValueError("Source nodes do not exists")
         if self.target is None or len(self.target) == 0:
             raise ValueError("Target nodes do not exists")
 
         # Setup nodes
-        self.recurrent = self.is_same_pop(self.source, self.target, quick=True)
+        self.recurrent = is_same_pop(self.source, self.target, quick=self.quick)
         self.source_ids = [s.node_id for s in self.source]
         self.n_source = len(self.source_ids)
         self.source_list = list(self.source)
         if self.recurrent:
             self.target_ids = self.source_ids
             self.n_target = self.n_source
             self.target_list = self.source_list
@@ -547,14 +615,15 @@
     # *** Methods executed during bmtk network.build() ***
     # *** Helper functions ***
     class ConnectorCache(object):
         def __init__(self, enable=True):
             self.enable = enable
             self._output = {}
             self.cache_dict = {}
+            self.set_next_it()
             self.write_mode()
 
         def cache_output(self, func, func_name, cache=True):
             if self.enable and cache:
                 self.cache_dict[func_name] = func
                 self._output[func_name] = []
                 output = self._output[func_name]
@@ -602,17 +671,22 @@
                     # if output not correct, disable and use original function
                     print("\nWarning: Cache did not work properly.\n")
                     for func_name in self.cache_dict:
                         self.fetch_output(func_name, False)
                     self.enable = False
             self.mode = 'read'
 
-        def next_it(self):
+        def set_next_it(self):
             if self.enable:
-                self.iter_count += 1
+                def next_it():
+                    self.iter_count += 1
+            else:
+                def next_it():
+                    pass
+            self.next_it = next_it
 
     def node_2_idx_input(self, var_func, reverse=False):
         """Convert a function that accept nodes as input
         to accept indices as input"""
         if reverse:
             def idx_2_var(j, i):
                 return var_func(self.target_list[j], self.source_list[i])
@@ -699,14 +773,21 @@
 
     def get_conn_prop(self, sid, tid):
         """Get stored value given node ids in a connection"""
         return self.conn_prop[self.stage][sid][tid]
 
     # *** A sequence of major methods executed during build ***
     def setup_variables(self):
+        # If pr_arg is string, use the same value as p0_arg or p1_arg
+        if isinstance(self.vars['pr_arg'], str):
+            pr_arg_func = 'p1_arg' if '1' in self.vars['pr_arg'] else 'p0_arg'
+            self.vars['pr_arg'] = self.vars[pr_arg_func]
+        else:
+            pr_arg_func = None
+
         callable_set = set()
         # Make constant variables constant functions
         for name, var in self.vars.items():
             if callable(var):
                 callable_set.add(name)  # record callable variables
                 setattr(self, name, var)
             else:
@@ -714,14 +795,29 @@
         self.callable_set = callable_set
 
         # Make callable variables except a few, accept index input instead
         for name in callable_set - {'p0', 'p1', 'pr'}:
             var = self.vars[name]
             setattr(self, name, self.node_2_idx_input(var, '1' in name))
 
+        # Set up function for pr_arg if use value from p0_arg or p1_arg
+        if pr_arg_func is None:
+            self._pr_arg = self.pr_arg  # use specified pr_arg
+        else:
+            self._pr_arg_val = 0.  # storing current value from p_arg
+            p_arg = getattr(self, pr_arg_func)
+            def p_arg_4_pr(*args, **kwargs):
+                val = p_arg(*args, **kwargs)
+                self._pr_arg_val = val
+                return val
+            setattr(self, pr_arg_func, p_arg_4_pr)
+            def pr_arg(self, *arg):
+                return self._pr_arg_val
+            self._pr_arg = types.MethodType(pr_arg, self)
+
     def cache_variables(self):
         # Select cacheable attrilbutes
         cache_set = {'p0', 'p0_arg', 'p1', 'p1_arg'}
         if self.symmetric_p1:
             cache_set.remove('p1')
         if self.symmetric_p1_arg:
             cache_set.remove('p1_arg')
@@ -821,15 +917,15 @@
             else:
                 possible_count += [forward, backward, forward and backward]
 
             # Make random decision
             if forward:
                 forward = decision(p0)
             if backward:
-                pr = self.pr(self.pr_arg(i, j))
+                pr = self.pr(self._pr_arg(i, j), p0, p1)
                 backward = decision(self.cond_backward(forward, p0, p1, pr))
 
             # Make connection
             if forward:
                 n_forward = self.n_syn0(i, j)
                 self.add_conn_prop(i, j, p0_arg, 0)
                 self.conn_mat[0, i, j] = n_forward
@@ -845,15 +941,15 @@
             self.cache.next_it()
         self.cache.write_mode()  # clear memory
         self.possible_count = possible_count
 
         if self.verbose:
             self.timer.report('Total time for creating connection matrix')
             if self.wrong_pr:
-                print("\nWarning: Value of 'pr' outside the bounds occurs.\n")
+                print("Warning: Value of 'pr' outside the bounds occurred.\n")
             self.connection_number_info()
 
     def make_connection(self):
         """ Assign number of synapses per iteration.
         Use iterator one_to_all for forward and all_to_one for backward.
         """
         nsyns = self.conn_mat[self.stage, self.iter_count, :]
@@ -945,15 +1041,15 @@
         print("Number of total pairs: %d" % n_pair)
         print("Fraction of connected pairs in all pairs: (%s)\n"
               % arr2str(100 * fraction[1], '%.2f%%'))
 
 
 class UnidirectionConnector(AbstractConnector):
     """
-    Object for building unidirectional connections in bmtk network model with
+    Object for buiilding unidirectional connections in bmtk network model with
     given probability within a single population (or between two populations).
 
     Parameters:
         p, p_arg: Probability of forward connection and its input argument when
             it is a function, similar to p0, p0_arg in ReciprocalConnector. It
             can be a constant or a deterministic function whose value must be
             within range [0, 1]. When p is constant, the connection is
@@ -1077,17 +1173,88 @@
         print("Fraction of connected pairs in possible ones: %.2f%%"
               % (100. * self.n_conn / self.n_poss) if self.n_poss else 0.)
         print("Number of total pairs: %d" % self.n_pair)
         print("Fraction of connected pairs in all pairs: %.2f%%\n"
               % (100. * self.n_conn / self.n_pair))
 
 
-class CorrelatedGapJunction(UnidirectionConnector):
+class GapJunction(UnidirectionConnector):
+    """
+    Object for buiilding gap junction connections in bmtk network model with
+    given probabilities within a single population which is uncorrelated with
+    the recurrent chemical synapses in this population.
+
+    Parameters:
+        p, p_arg: Probability of forward connection and its input argument when
+            it is a function, similar to p0, p0_arg in ReciprocalConnector. It
+            can be a constant or a deterministic function whose value must be
+            within range [0, 1]. When p is constant, the connection is
+            homogenous.
+        verbose: Whether show verbose information in console.
+
+    Returns:
+        An object that works with BMTK to build edges in a network.
+
+    Important attributes:
+        Similar to `UnidirectionConnector`.
+    """
+
+    def __init__(self, p=1., p_arg=None, verbose=True):
+        super().__init__(p=p, p_arg=p_arg, verbose=verbose)
+
+    def setup_nodes(self, source=None, target=None):
+        super().setup_nodes(source=source, target=target)
+        if len(self.source) != len(self.target):
+            raise ValueError("Source and target must be the same for "
+                             "gap junction.")
+        self.n_source = len(self.source)
+
+    def make_connection(self, source, target, *args, **kwargs):
+        """Assign gap junction per iteration using one_to_one iterator"""
+        # Initialize in the first iteration
+        if self.iter_count == 0:
+            self.initialize()
+            if self.verbose:
+                src_str, _ = self.get_nodes_info()
+                print("\nStart building gap junction \n  in " + src_str)
+
+        # Consider each pair only once
+        nsyns = 0
+        i, j = divmod(self.iter_count, self.n_source)
+        if i < j:
+            p_arg = self.p_arg(source, target)
+            p = self.p(p_arg)
+            possible = p > 0
+            self.n_poss += possible
+            if possible and decision(p):
+                nsyns = 1
+                sid, tid = source.node_id, target.node_id
+                self.add_conn_prop(sid, tid, p_arg)
+                self.add_conn_prop(tid, sid, p_arg)
+                self.n_conn += 1
+
+        self.iter_count += 1
+
+        # Detect end of iteration
+        if self.iter_count == self.n_pair:
+            if self.verbose:
+                self.connection_number_info()
+                self.timer.report('Done! \nTime for building connections')
+        return nsyns
+
+    def connection_number_info(self):
+        n_pair = self.n_pair
+        self.n_pair = (n_pair - len(self.source)) // 2
+        super().connection_number_info()
+        self.n_pair = n_pair
+
+
+class CorrelatedGapJunction(GapJunction):
     """
-    Object for building gap junction connections in bmtk network model with
+    Object for buiilding gap junction connections in bmtk network model with
     given probabilities within a single population which could be correlated
     with the recurrent chemical synapses in this population.
 
     Parameters:
         p_non, p_uni, p_rec: Probabilities of gap junction connection for each
             pair of cells given the following three conditions of chemical
             synaptic connections between them, no connection, unidirectional,
@@ -1116,21 +1283,14 @@
         self.vars['p_rec'] = p_rec
         self.connector = connector
         conn_prop = connector.conn_prop
         if isinstance(conn_prop, list):
             conn_prop = conn_prop[0]
         self.ref_conn_prop = conn_prop
 
-    def setup_nodes(self, source=None, target=None):
-        super().setup_nodes(source=source, target=target)
-        if len(self.source) != len(self.target):
-            raise ValueError("Source and target must be the same for "
-                             "gap junction.")
-        self.n_source = len(self.source)
-
     def conn_exist(self, sid, tid):
         trg_dict = self.ref_conn_prop.get(sid)
         if trg_dict is not None and tid in trg_dict:
             return True, trg_dict[tid]
         else:
             return False, None
 
@@ -1149,15 +1309,15 @@
 
     def make_connection(self, source, target, *args, **kwargs):
         """Assign gap junction per iteration using one_to_one iterator"""
         # Initialize in the first iteration
         if self.iter_count == 0:
             self.initialize()
             if self.verbose:
-                src_str, trg_str = self.get_nodes_info()
+                src_str, _ = self.get_nodes_info()
                 print("\nStart building gap junction \n  in " + src_str)
 
         # Consider each pair only once
         nsyns = 0
         i, j = divmod(self.iter_count, self.n_source)
         if i < j:
             sid, tid = source.node_id, target.node_id
@@ -1178,23 +1338,17 @@
         # Detect end of iteration
         if self.iter_count == self.n_pair:
             if self.verbose:
                 self.connection_number_info()
                 self.timer.report('Done! \nTime for building connections')
         return nsyns
 
-    def connection_number_info(self):
-        n_pair = self.n_pair
-        self.n_pair = (n_pair - len(self.source)) // 2
-        super().connection_number_info()
-        self.n_pair = n_pair
-
 
 class OneToOneSequentialConnector(AbstractConnector):
-    """Object for building one to one correspondence connections in bmtk
+    """Object for buiilding one to one correspondence connections in bmtk
     network model with between two populations. One of the population can
     consist of multiple sub-populations. These sub-populations need to be added
     sequentially using setup_nodes() and edge_params() methods followed by BMTK
     add_edges() method. For example, to connect 30 nodes in population A to 30
     nodes in populations B1, B2, B3, each with 10 nodes, set up as follows.
         connector = OneToOneSequentialConnector(**parameters)
         connector.setup_nodes(source=A, target=B1)
@@ -1333,29 +1487,32 @@
 
 SYN_MIN_DELAY = 0.8  # ms
 SYN_VELOCITY = 1000.  # um/ms
 FLUC_STDEV = 0.2  # ms
 DELAY_LOWBOUND = 0.2  # ms must be greater than h.dt
 DELAY_UPBOUND = 2.0  # ms
 
-def syn_dist_delay_feng(source, target,
-                        min_delay=SYN_MIN_DELAY, velocity=SYN_VELOCITY,
-                        fluc_stdev=FLUC_STDEV, connector=None):
+def syn_dist_delay_feng(source, target, min_delay=SYN_MIN_DELAY,
+                        velocity=SYN_VELOCITY, fluc_stdev=FLUC_STDEV,
+                        delay_bound=(DELAY_LOWBOUND, DELAY_UPBOUND),
+                        connector=None):
     """Synpase delay linearly dependent on distance.
     min_delay: minimum delay (ms)
     velocity: synapse conduction velocity (micron/ms)
     fluc_stdev: standard deviation of random Gaussian fluctuation (ms)
+    delay_bound: (lower, upper) bounds of delay (ms)
+    connector: connector object from which to read distance
     """
     if connector is None:
         dist = euclid_dist(target['positions'], source['positions'])
     else:
         dist = connector.get_conn_prop(source.node_id, target.node_id)
     del_fluc = fluc_stdev * rng.normal()
-    delay = dist / SYN_VELOCITY + SYN_MIN_DELAY + del_fluc
-    delay = min(max(delay, DELAY_LOWBOUND), DELAY_UPBOUND)
+    delay = dist / velocity + min_delay + del_fluc
+    delay = min(max(delay, delay_bound[0]), delay_bound[1])
     return delay
 
 
 def syn_section_PN(source, target, p=0.9,
                    sec_id=(1, 2), sec_x=(0.4, 0.6), **kwargs):
     """Synapse location follows a Bernoulli distribution, with probability p
     to obtain the former in sec_id and sec_x"""
@@ -1369,8 +1526,8 @@
     delay = syn_dist_delay_feng(source, target, **kwargs)
     s_id, s_x = syn_section_PN(source, target, p=p, sec_id=sec_id, sec_x=sec_x)
     return delay, s_id, s_x
 
 
 def syn_uniform_delay_section(source, target, low=DELAY_LOWBOUND,
                               high=DELAY_UPBOUND, **kwargs):
-    return rng.uniform(low, high)
+    return rng.uniform(low, high)
```

### Comparing `bmtool-0.5.2/bmtool/debug/commands.py` & `bmtool-0.5.3/bmtool/debug/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.5.2/bmtool/manage.py` & `bmtool-0.5.3/bmtool/manage.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.5.2/bmtool/plot_commands.py` & `bmtool-0.5.3/bmtool/plot_commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.5.2/bmtool/singlecell.py` & `bmtool-0.5.3/bmtool/singlecell.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,16 +213,16 @@
         self.index_v_final = int(self.inj_stop / h.dt)
         self.v_rest = self.v_vec[self.index_v_rest]
         self.v_rest_time = self.t_vec[self.index_v_rest]
         self.cell_v_final = self.v_vec[self.index_v_final]
         self.v_final_time = self.t_vec[self.index_v_final]
 
         t_idx = slice(self.index_v_rest, self.index_v_final + 1)
-        self.v_vec_inj = self.v_vec.as_numpy()[t_idx].copy()
-        self.t_vec_inj = self.t_vec.as_numpy()[t_idx].copy() - self.v_rest_time
+        self.v_vec_inj = np.array(self.v_vec)[t_idx]
+        self.t_vec_inj = np.array(self.t_vec)[t_idx] - self.v_rest_time
 
         self.v_diff = self.cell_v_final - self.v_rest
         self.r_in = self.v_diff / self.inj_amp # MegaOhms
 
         print_calc = self.tau_methods.get(self.method, self.tau_simple)()
 
         print()
@@ -384,16 +384,16 @@
         h.run()
 
         self.zap_vec.resize(self.t_vec.size())
         self.v_rest = self.v_vec[self.index_v_rest]
         self.v_rest_time = self.t_vec[self.index_v_rest]
 
         t_idx = slice(self.index_v_rest, self.index_v_final + 1)
-        self.v_vec_inj = self.v_vec.as_numpy()[t_idx].copy() - self.v_rest
-        self.t_vec_inj = self.t_vec.as_numpy()[t_idx].copy() - self.v_rest_time
+        self.v_vec_inj = np.array(self.v_vec)[t_idx] - self.v_rest
+        self.t_vec_inj = np.array(self.t_vec)[t_idx] - self.v_rest_time
 
         self.cell_v_amp_max = np.abs(self.v_vec_inj).max()
         self.Z = np.fft.rfft(self.v_vec_inj) / np.fft.rfft(self.zap_vec_inj) # MOhms
         self.freq = np.fft.rfftfreq(self.zap_vec_inj.size, d=self.dt * 1e-3) # ms to sec
         self.impedance = np.abs(self.Z)
 
         print()
```

### Comparing `bmtool-0.5.2/bmtool/util/commands.py` & `bmtool-0.5.3/bmtool/util/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.5.2/bmtool/util/neuron/celltuner.py` & `bmtool-0.5.3/bmtool/util/neuron/celltuner.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.5.2/bmtool/util/util.py` & `bmtool-0.5.3/bmtool/util/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -254,26 +254,28 @@
             node_group_id = nodes_grp['node_group_id'][()]
             node_group_index = nodes_grp['node_group_index'][()]
             n_group = node_group_id.max() + 1
             prop_dtype = {}
             for group_id in range(n_group):
                 group = nodes_grp[str(group_id)]
                 idx = node_group_id == group_id
+                group_node = node_id[idx]
+                group_index = node_group_index[idx]
                 for prop in group:
                     if prop == 'positions':
-                        positions = group[prop][node_group_index[idx]]
+                        positions = group[prop][group_index]
                         for i in range(positions.shape[1]):
                             if pos_labels[i] not in nodes_df:
                                 nodes_df[pos_labels[i]] = np.nan
-                            nodes_df.loc[node_id, pos_labels[i]] = positions[:, i]
+                            nodes_df.loc[group_node, pos_labels[i]] = positions[:, i]
                     else:
                         # create new column with NaN if property does not exist
                         if prop not in nodes_df: 
                             nodes_df[prop] = np.nan
-                        nodes_df.loc[idx, prop] = tuple(group[prop][node_group_index[idx]])
+                        nodes_df.loc[group_node, prop] = group[prop][group_index]
                         prop_dtype[prop] = group[prop].dtype
             # convert to original data type if possible
             for prop, dtype in prop_dtype.items():
                 nodes_df[prop] = nodes_df[prop].astype(dtype, errors='ignore')
 
         return population, nodes_df
 
@@ -611,15 +613,17 @@
         if include_gap == False:
             total = total[total['is_gap_junction'] != True]
         total = total.count()
         total = total.source_node_id # may not be the best way to pick
         return total
     return relation_matrix(config,nodes,edges,sources,targets,sids,tids,prepend_pop,relation_func=total_connection_relationship,synaptic_info=synaptic_info)
 
-def percent_connections(config=None,nodes=None,edges=None,sources=[],targets=[],sids=[],tids=[],prepend_pop=True,method=None,include_gap=True):
+
+def percent_connections(config=None,nodes=None,edges=None,sources=[],targets=[],sids=[],tids=[],prepend_pop=True,type='convergence',method=None,include_gap=True):
+
 
     def precent_func(**kwargs): 
         edges = kwargs["edges"]
         source_id_type = kwargs["sid"]
         target_id_type = kwargs["tid"]
         source_id = kwargs["source_id"]
         target_id = kwargs["target_id"]
@@ -640,30 +644,35 @@
         # determine dropped duplicates (keep=False)
         cons_recip_dedup = cons_recip.drop_duplicates(subset=['source_node_id','target_node_id'])
 
         # note counts
         num_bi = (cons_recip.count().source_node_id - cons_recip_dedup.count().source_node_id)
         num_uni = total_cons - num_bi    
 
-        num_sources = s_list.apply(pd.Series.value_counts)[source_id_type].dropna().sort_index().loc[source_id]
-        num_targets = t_list.apply(pd.Series.value_counts)[target_id_type].dropna().sort_index().loc[target_id]
+        #num_sources = s_list.apply(pd.Series.value_counts)[source_id_type].dropna().sort_index().loc[source_id]
+        #num_targets = t_list.apply(pd.Series.value_counts)[target_id_type].dropna().sort_index().loc[target_id]
+
+        num_sources = s_list[source_id_type].value_counts().sort_index().loc[source_id]
+        num_targets = t_list[target_id_type].value_counts().sort_index().loc[target_id]
+
 
         total = round(total_cons / (num_sources*num_targets) * 100,2)
         uni = round(num_uni / (num_sources*num_targets) * 100,2)
         bi = round(num_bi / (num_sources*num_targets) * 100,2)
         if method == 'total':
             return total
         if method == 'uni':
             return uni
         if method == 'bi':
             return bi
 
 
     return relation_matrix(config,nodes,edges,sources,targets,sids,tids,prepend_pop,relation_func=precent_func)
 
+
 def connection_divergence(config=None,nodes=None,edges=None,sources=[],targets=[],sids=[],tids=[],prepend_pop=True,convergence=False,method='mean+std',include_gap=True):
 
     import pandas as pd
 
     def total_connection_relationship(**kwargs):
         edges = kwargs["edges"]
         source_id_type = kwargs["sid"]
@@ -676,49 +685,105 @@
 
         cons = edges[(edges[source_id_type] == source_id) & (edges[target_id_type]==target_id)]
         if include_gap == False:
             cons = cons[cons['is_gap_junction'] != True]
 
         if convergence:
             if method == 'min':
-                count = cons.apply(pd.Series.value_counts).target_node_id.dropna().min()
+                count = cons['target_node_id'].value_counts().min()
                 return round(count,2)
             elif method == 'max':
-                count = cons.apply(pd.Series.value_counts).target_node_id.dropna().max()
+                count = cons['target_node_id'].value_counts().max()
                 return round(count,2)
             elif method == 'std':
-                std = cons.apply(pd.Series.value_counts).target_node_id.dropna().std()
+                std = cons['target_node_id'].value_counts().std()
                 return round(std,2)
             elif method == 'mean': 
                 mean = cons['target_node_id'].value_counts().mean()
                 return round(mean,2)
             elif method == 'mean+std': #default is mean + std
                 mean = cons['target_node_id'].value_counts().mean()
-                std = cons.apply(pd.Series.value_counts).target_node_id.dropna().std()
+                std = cons['target_node_id'].value_counts().std()
+                #std = cons.apply(pd.Series.value_counts).target_node_id.dropna().std() no longer a valid way
                 return (round(mean,2)), (round(std,2))
         else: #divergence
             if method == 'min':
-                count = cons.apply(pd.Series.value_counts).source_node_id.dropna().min()
+                count = cons['source_node_id'].value_counts().min()
                 return round(count,2)
             elif method == 'max':
-                count = cons.apply(pd.Series.value_counts).source_node_id.dropna().max()
+                count = cons['source_node_id'].value_counts().max()
                 return round(count,2)
             elif method == 'std':
-                std = cons.apply(pd.Series.value_counts).source_node_id.dropna().std()
+                std = cons['source_node_id'].value_counts().std()
                 return round(std,2)
             elif method == 'mean': 
                 mean = cons['source_node_id'].value_counts().mean()
                 return round(mean,2)
             elif method == 'mean+std': #default is mean + std
                 mean = cons['source_node_id'].value_counts().mean()
-                std = cons.apply(pd.Series.value_counts).source_node_id.dropna().std()
+                std = cons['source_node_id'].value_counts().std()
                 return (round(mean,2)), (round(std,2))
 
     return relation_matrix(config,nodes,edges,sources,targets,sids,tids,prepend_pop,relation_func=total_connection_relationship)
 
+def gap_junction_connections(config=None,nodes=None,edges=None,sources=[],targets=[],sids=[],tids=[],prepend_pop=True,type='convergence'):
+    import pandas as pd
+
+    
+    def total_connection_relationship(**kwargs): #reduced version of original function; only gets mean+std
+        edges = kwargs["edges"]
+        source_id_type = kwargs["sid"]
+        target_id_type = kwargs["tid"]
+        source_id = kwargs["source_id"]
+        target_id = kwargs["target_id"]
+
+        cons = edges[(edges[source_id_type] == source_id) & (edges[target_id_type]==target_id)] 
+        #print(cons)
+        
+        cons = cons[cons['is_gap_junction'] == True] #only gap_junctions
+        mean = cons['target_node_id'].value_counts().mean()
+        std = cons['target_node_id'].value_counts().std()
+        return (round(mean,2)), (round(std,2))
+    
+    def precent_func(**kwargs): #barely different than original function; only gets gap_junctions.
+        edges = kwargs["edges"]
+        source_id_type = kwargs["sid"]
+        target_id_type = kwargs["tid"]
+        source_id = kwargs["source_id"]
+        target_id = kwargs["target_id"]
+        t_list = kwargs["target_nodes"]
+        s_list = kwargs["source_nodes"]
+
+        cons = edges[(edges[source_id_type] == source_id) & (edges[target_id_type]==target_id)]
+        #add functionality that shows only the one's with gap_junctions
+        cons = cons[cons['is_gap_junction'] == True]
+        total_cons = cons.count().source_node_id
+
+        num_sources = s_list[source_id_type].value_counts().sort_index().loc[source_id]
+        num_targets = t_list[target_id_type].value_counts().sort_index().loc[target_id]
+
+
+        total = round(total_cons / (num_sources*num_targets) * 100,2)
+        return total
+    
+    if type == 'convergence':
+        return relation_matrix(config,nodes,edges,sources,targets,sids,tids,prepend_pop,relation_func=total_connection_relationship)
+    elif type == 'percent':
+        return relation_matrix(config,nodes,edges,sources,targets,sids,tids,prepend_pop,relation_func=precent_func)
+        
+
+def gap_junction_percent_connections(config=None,nodes=None,edges=None,sources=[],targets=[],sids=[],tids=[],prepend_pop=True,method=None):
+    import pandas as pd
+    
+        
+        
+    
+    
+        
+    
 def connection_probabilities(config=None,nodes=None,edges=None,sources=[],
     targets=[],sids=[],tids=[],prepend_pop=True,dist_X=True,dist_Y=True,dist_Z=True,num_bins=10,include_gap=True):
     
     import pandas as pd
     from scipy.spatial import distance
     import matplotlib.pyplot as plt
     pd.options.mode.chained_assignment = None
@@ -749,19 +814,19 @@
         total = total.source_node_id # may not be the best way to pick
         return round(total/count,1)
         """
         
         def eudist(df,use_x=True,use_y=True,use_z=True):
             def _dist(x):
                 if len(x) == 6:
-                    return distance.euclidean((x[0],x[1],x[2]),(x[3],x[4],x[5]))
+                    return distance.euclidean((x.iloc[0], x.iloc[1], x.iloc[2]), (x.iloc[3], x.iloc[4], x.iloc[5]))
                 elif len(x) == 4:
-                    return distance.euclidean((x[0],x[1]),(x[2],x[3]))
+                    return distance.euclidean((x.iloc[0],x.iloc[1]),(x.iloc[2],x.iloc[3]))
                 elif len(x) == 2:
-                    return distance.euclidean((x[0]),(x[1]))
+                    return distance.euclidean((x.iloc[0]),(x.iloc[1]))
                 else:
                     return -1
 
             if use_x and use_y and use_z: #(XYZ)
                 cols = ['source_pos_x','source_pos_y','source_pos_z',
                     'target_pos_x','target_pos_y','target_pos_z']
             elif use_x and use_y and not use_z: #(XY)
@@ -831,14 +896,15 @@
 
         connections = edges[(edges[source_id_type] == source_id) & (edges[target_id_type]==target_id)]
         
         return list(connections[edge_property].unique())
 
     return relation_matrix(config,nodes,edges,sources,targets,sids,tids,prepend_pop,relation_func=synapse_type_relationship,return_type=object)
 
+
 def edge_property_matrix(edge_property, config=None, nodes=None, edges=None, sources=[],targets=[],sids=[],tids=[],prepend_pop=True,report=None,time=-1,time_compare=None):
     
     var_report = None
     if time>=0 and report:
         cfg = load_config(config)
         #report_full, report_file = _get_cell_report(config,report)
         report_file = report # Same difference
@@ -902,18 +968,19 @@
             max_connect[a,b] = i*j
     ret = data/max_connect
     ret = ret*100
     ret = np.around(ret, decimals=1)
 
     return ret, source_labels, target_labels
     
-    
+
 def connection_average_synapses():
     return
 
+
 def connection_divergence_average_old(config=None, nodes=None, edges=None,populations=[],convergence=False):
     """
     For each cell in source count # of connections in target and average
     """
 
     import pandas as pd
```

### Comparing `bmtool-0.5.2/bmtool.egg-info/PKG-INFO` & `bmtool-0.5.3/bmtool.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.5.2
+Version: 0.5.3
 Summary: BMTool
 Home-page: https://github.com/cyneuro/bmtool
 Download-URL: 
-Author: Tyler Banks
-Author-email: tbanks@mail.missouri.edu
+Author: Neural Engineering Laboratory at the University of Missouri
+Author-email: gregglickert@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -24,26 +24,28 @@
 Requires-Dist: h5py
 Requires-Dist: matplotlib
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: questionary
 Requires-Dist: pynmodlt
+Requires-Dist: plotly
 
 # bmtool
 A collection of modules to make developing [Neuron](https://www.neuron.yale.edu/neuron/) and [BMTK](https://alleninstitute.github.io/bmtk/) models easier.
 
 [![license](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://github.com/cyneuro/bmtool/blob/master/LICENSE) 
 
 ## Table of Contents
 - [Getting Started](#Getting-Started)
 - [CLI](#CLI)
 - [Single Cell](#Single-Cell-Module)
 - [Connectors](#Connectors-Module)
 - [Bmplot](#bmplot-Module)
+- [Graphs](#graphs-module)
 
 ## Getting Started
 
 **Installation**
 ```bash
 pip install bmtool
 ```
@@ -387,14 +389,15 @@
 ```
 
 ## Bmplot Module
 - [Total connections](#Total-connection-plot)
 - [Percent connections](#Percent-connection-plot)
 - [Convergence connnections](#convergence-plot)
 - [Divergence connections](#divergence-plot)
+- [Gap Junction connections](#gap-junction-plot)
 - [connection histogram](#connection-histogram)
 - [probability connection](#probability-of-connection-plot)
 - [3D location](#3d-position-plot)
 - [3D rotation](#cell-rotations)
 - [Plot Connection Diagram](#plot-connection-diagram)
 
 ### Total connection plot
@@ -448,14 +451,25 @@
 bmplot.divergence_connection_matrix(config='config.json',sources='LA',targets='LA',tids='pop_name',sids='pop_name',no_prepend_pop=True,include_gap=False,method='mean+std')
 ```
 
 
     
 ![png](readme_figures/output_25_0.png)
     
+### Gap Junction plot
+#### While gap junctions can be include in the above plots, you can use this function to only view gap junctions.Type can be either 'convergence' or 'percent' connections to generate different plots
+
+
+```python
+bmplot.gap_junction_matrix(config='config.json',sources='LA',targets='LA',sids='pop_name',tids='pop_name',no_prepend_pop=True,type='percent')
+```
+
+
+    
+![png](output_gap.png)
 
 
 ### Connection histogram 
 #### Generates a histogram of the distribution of connections a population of cells give to individual cells of another population 
 
 
 ```python
@@ -772,9 +786,131 @@
 </table>
 
 
 
 
 
     'LA'
+## Graphs Module
+- [Generate graph](#generate-graph)
+- [Plot Graph](#plot-graph)
+- [Connectioon table](#generate-graph-connection-table)
+
+### Generate Graph
+
+
+```python
+from bmtool import graphs
+import networkx as nx
+
+Graph = graphs.generate_graph(config='config.json',source='LA',target='LA')
+print("Number of nodes:", Graph.number_of_nodes())
+print("Number of edges:", Graph.number_of_edges())
+print("Node labels:", set(nx.get_node_attributes(Graph, 'label').values()))
+```
+
+    Number of nodes: 2000
+    Number of edges: 84235
+    Node labels: {'SOM', 'PNc', 'PNa', 'PV'}
+
+
+### Plot Graph
+#### Generates an interactive plot showing nodes, edges and # of connections
+
+
+```python
+graphs.plot_graph(Graph)
+```
+
+
+
+### Generate graph connection table
+#### Generates a CSV of all cells and the number of connections each individual cell receives
+
+
+```python
+import pandas as pd
+graphs.export_node_connections_to_csv(Graph, 'node_connections.csv')
+df = pd.read_csv('node_connections.csv')
+df.head()
+```
+
+
+
+
+<div>
+<style scoped>
+    .dataframe tbody tr th:only-of-type {
+        vertical-align: middle;
+    }
+
+    .dataframe tbody tr th {
+        vertical-align: top;
+    }
+
+    .dataframe thead th {
+        text-align: right;
+    }
+</style>
+<table border="1" class="dataframe">
+  <thead>
+    <tr style="text-align: right;">
+      <th></th>
+      <th>Unnamed: 0</th>
+      <th>Node Label</th>
+      <th>PNc Connections</th>
+      <th>PV Connections</th>
+      <th>SOM Connections</th>
+      <th>PNa Connections</th>
+    </tr>
+  </thead>
+  <tbody>
+    <tr>
+      <th>0</th>
+      <td>0</td>
+      <td>PNa</td>
+      <td>15</td>
+      <td>11</td>
+      <td>9</td>
+      <td>6</td>
+    </tr>
+    <tr>
+      <th>1</th>
+      <td>1</td>
+      <td>PNa</td>
+      <td>24</td>
+      <td>25</td>
+      <td>6</td>
+      <td>21</td>
+    </tr>
+    <tr>
+      <th>2</th>
+      <td>2</td>
+      <td>PNa</td>
+      <td>27</td>
+      <td>28</td>
+      <td>12</td>
+      <td>25</td>
+    </tr>
+    <tr>
+      <th>3</th>
+      <td>3</td>
+      <td>PNa</td>
+      <td>19</td>
+      <td>27</td>
+      <td>15</td>
+      <td>35</td>
+    </tr>
+    <tr>
+      <th>4</th>
+      <td>4</td>
+      <td>PNa</td>
+      <td>25</td>
+      <td>11</td>
+      <td>8</td>
+      <td>16</td>
+    </tr>
+  </tbody>
+</table>
+</div>
```

### Comparing `bmtool-0.5.2/bmtool.egg-info/SOURCES.txt` & `bmtool-0.5.3/bmtool.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 bmtool/__init__.py
 bmtool/__main__.py
 bmtool/bmplot.py
 bmtool/connectors.py
+bmtool/graphs.py
 bmtool/manage.py
 bmtool/plot_commands.py
 bmtool/singlecell.py
 bmtool.egg-info/PKG-INFO
 bmtool.egg-info/SOURCES.txt
 bmtool.egg-info/dependency_links.txt
 bmtool.egg-info/entry_points.txt
```

### Comparing `bmtool-0.5.2/setup.py` & `bmtool-0.5.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bmtool",
-    version="0.5.2",
-    author="Tyler Banks",
-    author_email="tbanks@mail.missouri.edu",
+    version="0.5.3",
+    author="Neural Engineering Laboratory at the University of Missouri",
+    author_email="gregglickert@mail.missouri.edu",
     description="BMTool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cyneuro/bmtool",
     download_url='',
     license='MIT',
     install_requires=[
@@ -21,15 +21,16 @@
         'clint',
         'h5py',
         'matplotlib',
         'networkx',
         'numpy',
         'pandas',
         'questionary',
-        'pynmodlt'
+        'pynmodlt',
+        'plotly'
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         "Programming Language :: Python :: 3",
```

