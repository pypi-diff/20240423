# Comparing `tmp/scgraph-2.0.0.tar.gz` & `tmp/scgraph-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgraph-2.0.0.tar", last modified: Fri Apr 19 19:10:45 2024, max compression
+gzip compressed data, was "scgraph-2.1.0.tar", last modified: Tue Apr 23 15:41:31 2024, max compression
```

## Comparing `scgraph-2.0.0.tar` & `scgraph-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-19 19:10:45.098317 scgraph-2.0.0/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-2.0.0/LICENSE
--rw-r--r--   0 conmak    (1000) conmak    (1000)     9178 2024-04-19 19:10:45.098317 scgraph-2.0.0/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     8556 2024-04-19 19:07:52.000000 scgraph-2.0.0/README.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      857 2024-04-19 18:27:15.000000 scgraph-2.0.0/pyproject.toml
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-19 19:10:45.090317 scgraph-2.0.0/scgraph/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-04-19 19:03:42.000000 scgraph-2.0.0/scgraph/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    38367 2024-04-19 19:09:29.000000 scgraph-2.0.0/scgraph/core.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-19 19:10:45.094317 scgraph-2.0.0/scgraph/geographs/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-09-15 15:24:50.000000 scgraph-2.0.0/scgraph/geographs/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   733914 2024-04-19 18:27:15.000000 scgraph-2.0.0/scgraph/geographs/marnet.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   557967 2024-04-19 18:27:15.000000 scgraph-2.0.0/scgraph/geographs/north_america_rail.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   583015 2024-04-19 18:27:15.000000 scgraph-2.0.0/scgraph/geographs/oak_ridge_maritime.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   867927 2024-04-19 18:27:15.000000 scgraph-2.0.0/scgraph/geographs/us_freeway.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4256 2024-04-19 18:27:15.000000 scgraph-2.0.0/scgraph/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-19 19:10:45.098317 scgraph-2.0.0/scgraph.egg-info/
--rw-r--r--   0 conmak    (1000) conmak    (1000)     9178 2024-04-19 19:10:45.000000 scgraph-2.0.0/scgraph.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      389 2024-04-19 19:10:45.000000 scgraph-2.0.0/scgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-04-19 19:10:45.000000 scgraph-2.0.0/scgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2024-04-19 19:10:45.000000 scgraph-2.0.0/scgraph.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      138 2024-04-19 19:10:45.098317 scgraph-2.0.0/setup.cfg
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-23 15:41:31.493446 scgraph-2.1.0/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-2.1.0/LICENSE
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     9354 2024-04-23 15:41:31.493446 scgraph-2.1.0/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     8732 2024-04-23 15:39:41.000000 scgraph-2.1.0/README.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      857 2024-04-23 15:41:16.000000 scgraph-2.1.0/pyproject.toml
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-23 15:41:31.489446 scgraph-2.1.0/scgraph/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    40505 2024-04-23 15:00:52.000000 scgraph-2.1.0/scgraph/core.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-23 15:41:31.493446 scgraph-2.1.0/scgraph/geographs/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-09-15 15:24:50.000000 scgraph-2.1.0/scgraph/geographs/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   733914 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/geographs/marnet.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   557967 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/geographs/north_america_rail.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   583015 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/geographs/oak_ridge_maritime.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   867927 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/geographs/us_freeway.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4426 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-23 15:41:31.493446 scgraph-2.1.0/scgraph.egg-info/
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     9354 2024-04-23 15:41:31.000000 scgraph-2.1.0/scgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      389 2024-04-23 15:41:31.000000 scgraph-2.1.0/scgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-04-23 15:41:31.000000 scgraph-2.1.0/scgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2024-04-23 15:41:31.000000 scgraph-2.1.0/scgraph.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      138 2024-04-23 15:41:31.493446 scgraph-2.1.0/setup.cfg
```

### Comparing `scgraph-2.0.0/LICENSE` & `scgraph-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scgraph-2.0.0/PKG-INFO` & `scgraph-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 2.0.0
+Version: 2.1.0
 Summary: Determine an approximate route between two points on earth.
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/scgraph
 Project-URL: Bug Tracker, https://github.com/connor-makowski/scgraph/issues
 Project-URL: Documentation, https://connor-makowski.github.io/scgraph/core.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -97,14 +97,16 @@
         - `output_units` options:
             - `km` (kilometers - default)
             - `m` (meters)
             - `mi` (miles)
             - `ft` (feet)
 - `coordinate_path`: A list of lists [`latitude`,`longitude`] that make up the shortest path
 
+For more examples including viewing the output on a map, see the [example notebook](https://colab.research.google.com/github/connor-makowski/scgraph/blob/main/example.ipynb).
+
 ## Included GeoGraphs
 
 - marnet_geograph:
     - What: A maritime network data set from searoute
     - Use: `from scgraph.geographs.marnet import marnet_geograph`
     - Attribution: [searoute](https://github.com/genthalili/searoute-py)
     - Length Measurement: Kilometers
```

### Comparing `scgraph-2.0.0/README.md` & `scgraph-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,16 @@
         - `output_units` options:
             - `km` (kilometers - default)
             - `m` (meters)
             - `mi` (miles)
             - `ft` (feet)
 - `coordinate_path`: A list of lists [`latitude`,`longitude`] that make up the shortest path
 
+For more examples including viewing the output on a map, see the [example notebook](https://colab.research.google.com/github/connor-makowski/scgraph/blob/main/example.ipynb).
+
 ## Included GeoGraphs
 
 - marnet_geograph:
     - What: A maritime network data set from searoute
     - Use: `from scgraph.geographs.marnet import marnet_geograph`
     - Attribution: [searoute](https://github.com/genthalili/searoute-py)
     - Length Measurement: Kilometers
```

### Comparing `scgraph-2.0.0/pyproject.toml` & `scgraph-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scgraph"
-version = "2.0.0"
+version = "2.1.0"
 description = "Determine an approximate route between two points on earth."
 authors = [
     {name="Connor Makowski", email="conmak@mit.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `scgraph-2.0.0/scgraph/core.py` & `scgraph-2.1.0/scgraph/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -393,43 +393,45 @@
                 (i[0] >= -90 and i[0] <= 90 and i[1] >= -180 and i[1] <= 180)
                 for i in self.nodes
             ]
         ), "Your nodes must be a list of lists where each sub list has a length of 2 with a latitude [-90,90] and longitude [-180,180] value"
 
     def get_shortest_path(
         self,
-        origin_node,
-        destination_node,
+        origin_node: dict[int | float],
+        destination_node: dict[int | float],
         output_units: str = "km",
         algorithm_fn=Graph.dijkstra_makowski,
-        off_graph_circuity: [float, int] = 1,
+        off_graph_circuity: float | int = 1,
         node_addition_type: str = "quadrant",
-        node_addition_circuity: [float, int] = 4,
+        node_addition_circuity: float | int = 4,
         geograph_units: str = "km",
         output_coordinate_path: str = "list_of_lists",
         output_path: bool = False,
+        node_addition_lat_lon_bound: float | int = 5,
+        node_addition_math: str = "euclidean",
         **kwargs,
     ) -> dict:
         """
         Function:
 
         - Identify the shortest path between two nodes in a sparse network graph
 
         - Return a dictionary of various path information including:
             - `id_path`: A list of node ids in the order they are visited
-            - `path`: A list of node dictionaries (lat + long) in the order they are visited
+            - `path`: A list of nodes  (list of lat then long) in the order they are visited
             - `length`: The length of the path
 
          Required Arguments:
 
         - `origin_node`
-            - Type: dict
+            - Type: dict of int | float
             - What: A dictionary with the keys 'latitude' and 'longitude'
         - `destination_node`
-            - Type: dict
+            - Type: dict of int | float
             - What: A dictionary with the keys 'latitude' and 'longitude'
 
         Optional Arguments:
 
         - `output_units`
             - Type: str
             - What: The units in which to return the length of the path
@@ -495,32 +497,53 @@
         - `output_coordinate_path`
             - Type: str
             - What: The format of the output coordinate path
             - Default: 'list_of_lists'
             - Options:
                 - 'list_of_dicts': A list of dictionaries with keys 'latitude' and 'longitude'
                 - 'list_of_lists': A list of lists with the first value being latitude and the second being longitude
+                - 'list_of_lists_long_first': A list of lists with the first value being longitude and the second being latitude
         - `output_path`
             - Type: bool
             - What: Whether to output the path as a list of geograph node ids (for debugging and other advanced uses)
             - Default: False
+        - `node_addition_lat_lon_bound`
+            - Type: float | int
+            - What: Forms a bounding box around the origin and destination nodes as they are added to graph
+                - Only points on the current graph inside of this bounding box are considered when updating the distance matrix for the origin or destination nodes
+            - Default: 5
+            - Note: If no nodes are found within the bounding box, the bounding box is expanded to 180 degrees in all directions (all nodes are considered)
+            - Note: This is only used when adding a new node (the specified origin and destination) to the graph
+        - `node_addition_math`
+            - Type: str
+            - What: The math to use when calculating the distance between nodes when determining the closest node (or closest quadrant node) to add to the graph
+            - Default: 'euclidean'
+            - Options:
+                - 'euclidean': Use the euclidean distance between nodes. This is much faster but is not as accurate (especially near the poles)
+                - 'haversine': Use the haversine distance between nodes. This is slower but is an accurate representation of the surface distance between two points on the earth
+            - Notes:
+                - Only used if `node_addition_type` is set to 'quadrant' or 'closest'
         - `**kwargs`
             - Additional keyword arguments. These are included for forwards and backwards compatibility reasons, but are not currently used.
         """
         original_graph_length = len(self.graph)
         # Add the origin and destination nodes to the graph
         origin_id = self.add_node(
             node=origin_node,
             node_addition_type=node_addition_type,
             circuity=node_addition_circuity,
+            lat_lon_bound=node_addition_lat_lon_bound,
+            node_addition_math=node_addition_math,
         )
         destination_id = self.add_node(
             node=destination_node,
             node_addition_type="all",
             circuity=node_addition_circuity,
+            lat_lon_bound=node_addition_lat_lon_bound,
+            node_addition_math=node_addition_math,
         )
 
         try:
             output = algorithm_fn(
                 graph=self.graph,
                 origin_id=origin_id,
                 destination_id=destination_id,
@@ -537,14 +560,19 @@
                 output_units=output_units,
             )
             if output_coordinate_path == "list_of_dicts":
                 output["coordinate_path"] = [
                     {"latitude": i[0], "longitude": i[1]}
                     for i in output["coordinate_path"]
                 ]
+            elif output_coordinate_path == "list_of_lists_long_first":
+                output["coordinate_path"] = [
+                    [i[1], i[0]] for i in output["coordinate_path"]
+                ]
+                output["long_first"] = True
             if not output_path:
                 del output["path"]
             while len(self.graph) > original_graph_length:
                 self.remove_appended_node()
             return output
         except Exception as e:
             while len(self.graph) > original_graph_length:
@@ -587,15 +615,15 @@
             return round(
                 output["length"]
                 + direct_off_graph_length
                 * (off_graph_circuity - node_addition_circuity),
                 4,
             )
 
-    def get_coordinate_path(self, path: list) -> list:
+    def get_coordinate_path(self, path: list[int]) -> list[dict[int | float]]:
         """
         Function:
 
         - Return a list of node dictionaries (lat + long) in the order they are visited
 
         Required Arguments:
 
@@ -631,19 +659,19 @@
             del self.graph[reverse_connection][node_id]
         self.graph = self.graph[:node_id]
         self.nodes = self.nodes[:node_id]
 
     def get_node_distances(
         self,
         node: list,
-        circuity: [int, float],
+        circuity: int | float,
         node_addition_type: str,
         node_addition_math: str,
-        lat_lon_bound: [int, float],
-    ):
+        lat_lon_bound: int | float,
+    ) -> dict[int | float]:
         """
         Function:
 
         - Get the distances between a node and all other nodes in the graph
         - This is used to determine the closest node to add to the graph when adding a new node
 
         Required Arguments:
@@ -735,19 +763,19 @@
                 haversine(node, self.nodes[node_idx], circuity=circuity), 4
             )
             for node_idx in min_diffs_idx.values()
         }
 
     def add_node(
         self,
-        node: dict[int, float],
-        circuity: [float, int],
+        node: dict[int | float],
+        circuity: int | float,
         node_addition_type: str = "quadrant",
         node_addition_math: str = "euclidean",
-        lat_lon_bound: [int, float] = 5,
+        lat_lon_bound: int | float = 5,
     ) -> int:
         """
         Function:
 
         - Add a node to the network
         - Returns the id of the new node
```

### Comparing `scgraph-2.0.0/scgraph/geographs/marnet.py` & `scgraph-2.1.0/scgraph/geographs/marnet.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.0.0/scgraph/geographs/north_america_rail.py` & `scgraph-2.1.0/scgraph/geographs/north_america_rail.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.0.0/scgraph/geographs/oak_ridge_maritime.py` & `scgraph-2.1.0/scgraph/geographs/oak_ridge_maritime.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.0.0/scgraph/geographs/us_freeway.py` & `scgraph-2.1.0/scgraph/geographs/us_freeway.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.0.0/scgraph/utils.py` & `scgraph-2.1.0/scgraph/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math, json
 
 
 def haversine(
     origin: list[float, int],
     destination: list[float, int],
     units: str = "km",
-    circuity: [float, int] = 1,
+    circuity: int | float = 1,
 ):
     """
     Function:
 
     - Calculate the great circle distance in kilometers between two points on the earth (specified in decimal degrees)
 
     Required Arguments:
@@ -65,15 +65,15 @@
             raise ValueError('Units must be one of "km", "m", "mi", or "ft"')
         return c * radius * circuity
     except:
         print(origin, destination)
         raise Exception()
 
 
-def hard_round(decimal_places, a):
+def hard_round(decimal_places: int, a: int | float):
     """
     Function:
 
     - Round a number to a specified number of decimal places
 
     Required Arguments:
 
@@ -86,15 +86,15 @@
     """
     return int(a * (10**decimal_places) + (0.5 if a > 0 else -0.5)) / (
         10**decimal_places
     )
 
 
 def distance_converter(
-    distance: [int, float], input_units: str, output_units: str
+    distance: int | float, input_units: str, output_units: str
 ):
     """
     Function:
 
     - Convert a distance from one unit to another
 
     Required Arguments:
@@ -111,15 +111,15 @@
     """
     assert input_units in ["mi", "km", "m", "ft"]
     assert output_units in ["mi", "km", "m", "ft"]
     km_table = {"mi": 0.621371, "m": 1000, "ft": 3280.84, "km": 1}
     return (distance / km_table[input_units]) * km_table[output_units]
 
 
-def get_line_path(output, filename=None):
+def get_line_path(output: list | dict, filename=None):
     """
     Function:
 
     - Convert a `get_shortest_path` output into a GeoJSON LineString dictionary object
     - Optionally save the output to a file
 
     Required Arguments:
@@ -133,17 +133,21 @@
     - `filename`:
         - Type: str
         - What: path to save the output to
         - Default: None
         - Note: if `filename` is not None, the output will be saved to the specified path
     """
     if isinstance(output["coordinate_path"], list):
+        if output.get("long_first"):
+            coordinates = output["coordinate_path"]
+        else:
+            coordinates = [[i[1], i[0]] for i in output["coordinate_path"]]
         linestring = {
             "type": "LineString",
-            "coordinates": [[i[1], i[0]] for i in output["coordinate_path"]],
+            "coordinates": coordinates,
         }
     elif isinstance(output["coordinate_path"], dict):
         linestring = {
             "type": "LineString",
             "coordinates": [
                 [i["longitude"], i["latitude"]]
                 for i in output["coordinate_path"]
```

### Comparing `scgraph-2.0.0/scgraph.egg-info/PKG-INFO` & `scgraph-2.1.0/scgraph.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 2.0.0
+Version: 2.1.0
 Summary: Determine an approximate route between two points on earth.
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/scgraph
 Project-URL: Bug Tracker, https://github.com/connor-makowski/scgraph/issues
 Project-URL: Documentation, https://connor-makowski.github.io/scgraph/core.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -97,14 +97,16 @@
         - `output_units` options:
             - `km` (kilometers - default)
             - `m` (meters)
             - `mi` (miles)
             - `ft` (feet)
 - `coordinate_path`: A list of lists [`latitude`,`longitude`] that make up the shortest path
 
+For more examples including viewing the output on a map, see the [example notebook](https://colab.research.google.com/github/connor-makowski/scgraph/blob/main/example.ipynb).
+
 ## Included GeoGraphs
 
 - marnet_geograph:
     - What: A maritime network data set from searoute
     - Use: `from scgraph.geographs.marnet import marnet_geograph`
     - Attribution: [searoute](https://github.com/genthalili/searoute-py)
     - Length Measurement: Kilometers
```

