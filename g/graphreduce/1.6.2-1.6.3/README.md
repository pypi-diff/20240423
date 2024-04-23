# Comparing `tmp/graphreduce-1.6.2.tar.gz` & `tmp/graphreduce-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphreduce-1.6.2.tar", last modified: Thu Dec 28 03:10:36 2023, max compression
+gzip compressed data, was "graphreduce-1.6.3.tar", last modified: Tue Apr 23 13:08:39 2024, max compression
```

## Comparing `graphreduce-1.6.2.tar` & `graphreduce-1.6.3.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-12-28 03:10:36.951161 graphreduce-1.6.2/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     9230 2023-12-28 03:10:36.950994 graphreduce-1.6.2/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     8254 2023-08-11 02:12:12.000000 graphreduce-1.6.2/README.md
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-12-28 03:10:36.950209 graphreduce-1.6.2/graphreduce/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.6.2/graphreduce/__init__.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     2192 2023-12-28 03:07:30.000000 graphreduce-1.6.2/graphreduce/context.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      520 2023-10-02 18:58:20.000000 graphreduce-1.6.2/graphreduce/enum.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    17603 2023-10-25 13:21:14.000000 graphreduce-1.6.2/graphreduce/graph_reduce.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)    18162 2023-12-28 03:06:06.000000 graphreduce-1.6.2/graphreduce/node.py
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     3225 2023-12-22 04:15:56.000000 graphreduce-1.6.2/graphreduce/storage.py
-drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2023-12-28 03:10:36.950851 graphreduce-1.6.2/graphreduce.egg-info/
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     9230 2023-12-28 03:10:36.000000 graphreduce-1.6.2/graphreduce.egg-info/PKG-INFO
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      364 2023-12-28 03:10:36.000000 graphreduce-1.6.2/graphreduce.egg-info/SOURCES.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-12-28 03:10:36.000000 graphreduce-1.6.2/graphreduce.egg-info/dependency_links.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.6.2/graphreduce.egg-info/not-zip-safe
--rw-r--r--   0 wesmadrigal   (501) staff       (20)      124 2023-12-28 03:10:36.000000 graphreduce-1.6.2/graphreduce.egg-info/requires.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       12 2023-12-28 03:10:36.000000 graphreduce-1.6.2/graphreduce.egg-info/top_level.txt
--rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2023-12-28 03:10:36.951207 graphreduce-1.6.2/setup.cfg
--rw-r--r--   0 wesmadrigal   (501) staff       (20)     1824 2023-12-28 03:07:34.000000 graphreduce-1.6.2/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2024-04-23 13:08:39.121577 graphreduce-1.6.3/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     9230 2024-04-23 13:08:39.121255 graphreduce-1.6.3/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     8254 2023-08-11 02:12:12.000000 graphreduce-1.6.3/README.md
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2024-04-23 13:08:39.120212 graphreduce-1.6.3/graphreduce/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2022-06-22 03:03:07.000000 graphreduce-1.6.3/graphreduce/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     2192 2023-12-28 03:07:30.000000 graphreduce-1.6.3/graphreduce/context.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      520 2023-10-02 18:58:20.000000 graphreduce-1.6.3/graphreduce/enum.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    21951 2024-04-23 13:00:23.000000 graphreduce-1.6.3/graphreduce/graph_reduce.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       80 2024-04-22 13:36:20.000000 graphreduce-1.6.3/graphreduce/metadata.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)    23553 2024-04-23 12:29:07.000000 graphreduce-1.6.3/graphreduce/node.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     3225 2024-04-22 22:17:54.000000 graphreduce-1.6.3/graphreduce/storage.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2024-04-23 13:08:39.120954 graphreduce-1.6.3/graphreduce.egg-info/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     9230 2024-04-23 13:08:39.000000 graphreduce-1.6.3/graphreduce.egg-info/PKG-INFO
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      433 2024-04-23 13:08:39.000000 graphreduce-1.6.3/graphreduce.egg-info/SOURCES.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2024-04-23 13:08:39.000000 graphreduce-1.6.3/graphreduce.egg-info/dependency_links.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        1 2023-06-16 20:09:48.000000 graphreduce-1.6.3/graphreduce.egg-info/not-zip-safe
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)      138 2024-04-23 13:08:39.000000 graphreduce-1.6.3/graphreduce.egg-info/requires.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       18 2024-04-23 13:08:39.000000 graphreduce-1.6.3/graphreduce.egg-info/top_level.txt
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)       38 2024-04-23 13:08:39.121618 graphreduce-1.6.3/setup.cfg
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     1853 2024-04-23 13:08:32.000000 graphreduce-1.6.3/setup.py
+drwxr-xr-x   0 wesmadrigal   (501) staff       (20)        0 2024-04-23 13:08:39.121113 graphreduce-1.6.3/tests/
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)        0 2024-02-27 21:13:06.000000 graphreduce-1.6.3/tests/__init__.py
+-rw-r--r--   0 wesmadrigal   (501) staff       (20)     2260 2024-04-23 13:08:00.000000 graphreduce-1.6.3/tests/test_graph_reduce.py
```

### Comparing `graphreduce-1.6.2/PKG-INFO` & `graphreduce-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.6.2
+Version: 1.6.3
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.6.2/README.md` & `graphreduce-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `graphreduce-1.6.2/graphreduce/context.py` & `graphreduce-1.6.3/graphreduce/context.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.6.2/graphreduce/enum.py` & `graphreduce-1.6.3/graphreduce/enum.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.6.2/graphreduce/graph_reduce.py` & `graphreduce-1.6.3/graphreduce/graph_reduce.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 # third party
 import pandas as pd
 import networkx as nx
 from dask import dataframe as dd
 from structlog import get_logger
 import pyspark
 import pyvis
+import woodwork as ww
 
 # internal
-from graphreduce.node import GraphReduceNode
+from graphreduce.node import GraphReduceNode, DynamicNode
 from graphreduce.enum import ComputeLayerEnum, PeriodUnit
 from graphreduce.storage import StorageClient
 
 logger = get_logger('GraphReduce')
 
 
 
@@ -31,28 +32,34 @@
         name : str = 'graph_reduce',
         parent_node : typing.Optional[GraphReduceNode] = None,
         fmt : str = 'parquet',
         compute_layer : ComputeLayerEnum = None,
         cut_date : datetime.datetime = datetime.datetime.now(),
         compute_period_val : typing.Union[int, float] = 365,
         compute_period_unit : PeriodUnit  = PeriodUnit.day,
-        has_labels : bool = False,
-        label_period_val : typing.Optional[typing.Union[int, float]] = None,
-        label_period_unit : typing.Optional[PeriodUnit] = None,
-        spark_sqlctx : pyspark.sql.SQLContext = None,
-        feature_function : typing.Optional[str] = None,
-        dynamic_propagation : bool = False,
-        type_func_map : typing.Dict[str, typing.List[str]] = {
-            'int64' : ['min', 'max', 'sum'],
-            'str' : ['first'],
-            'object' : ['first'],
+        auto_features: bool = False,
+        auto_feature_hops_back: int = 2,
+        auto_feature_hops_front: int = 1,
+        feature_typefunc_map : typing.Dict[str, typing.List[str]] = {
+            'int64' : ['count'],
+            'str' : ['min', 'max', 'first', 'count'],
+            'object' : ['first', 'count'],
             'float64' : ['min', 'max', 'sum'],
             'bool' : ['first'],
-            'datetime64' : ['first']
+            'datetime64' : ['first', 'min', 'max'],
+            'datetime64[ns]':['first','min','max'],
             },
+        # Label parameters.
+        label_node: typing.Optional[GraphReduceNode] = None,
+        label_operation: typing.Optional[typing.Union[callable, str]] = None,
+        # Field on the node.
+        label_field: typing.Optional[str] = None,
+        label_period_val : typing.Optional[typing.Union[int, float]] = None,
+        label_period_unit : typing.Optional[PeriodUnit] = None,
+        spark_sqlctx : pyspark.sql.SQLContext = None,        
         storage_client: typing.Optional[StorageClient] = None,
         *args,
         **kwargs
     ):
         """
 Constructor for GraphReduce
 
@@ -60,47 +67,57 @@
     name : the name of the graph reduce
     parent_node : parent-most node in the graph, if doing reductions the granularity to which to reduce the data
     fmt : the format of the dataset 
     compute_layer : compute layer to use (e.g., spark)    
     cut_date : the date to cut off history
     compute_period_val : the amount of time to consider during the compute job
     compute_period_unit : the unit for the compute period value (e.g., day)
-    has_labels : whether or not the compute job computes labels, when True `prep_for_labels()` and `compute_labels` will be called
     label_period_val : amount of time to consider when computing labels
     label_period_unit : the unit for the label period value (e.g., day)
     spark_sqlctx : if compute layer is spark this must be passed
-    feature_function : optional custom feature function
-    dynamic_propagation : optional to dynamically propagate children data upward, useful for very large compute graphs
-    type_func_match : optional mapping from type to a list of functions (e.g., {'int' : ['min', 'max', 'sum'], 'str' : ['first']})
+    auto_features: optional to automatically compute features and propagate child features upward; useful for large compute graphs
+    auto_feature_hops_back: optional for automatically computing features
+    auto_feature_hops_front: optional for automatically computing features
+    feature_typefunc_map : optional mapping from type to a list of functions (e.g., {'int' : ['min', 'max', 'sum'], 'str' : ['first']})
         """
         super(GraphReduce, self).__init__(*args, **kwargs)
         
         self.name = name
         self.parent_node = parent_node
         self.cut_date = cut_date
         self.fmt = fmt
+        # Compute period for features.
         self.compute_period_val = compute_period_val
         self.compute_period_unit = compute_period_unit
-        self.has_labels = has_labels
+        self.compute_layer = compute_layer
+
+        # Label parameters.
+        self.label_node = label_node
+        self.label_field = label_field
+        # Options: 'first', 'sum', 'avg', 'median', 'bool'
+        self.label_operation = label_operation
         self.label_period_val = label_period_val
         self.label_period_unit = label_period_unit
-        self.compute_layer = compute_layer
-        self.feature_function = feature_function
-        self.dynamic_propagation = dynamic_propagation
-        self.type_func_map = type_func_map
+
+       
+        # Automatic feature engineering parameters.
+        self.auto_features = auto_features
+        self.auto_feature_hops_back = auto_feature_hops_back
+        self.auto_feature_hops_front = auto_feature_hops_front
+        self.feature_typefunc_map = feature_typefunc_map
         
         # if using Spark
         self._sqlctx = spark_sqlctx
         self._storage_client = storage_client
         
         if self.compute_layer == ComputeLayerEnum.spark and self._sqlctx is None:
             raise Exception(f"Must provide a `spark_sqlctx` kwarg if using {self.compute_layer.value} as compute layer")
         
-        if self.has_labels and (self.label_period_val is None or self.label_period_unit is None):
-            raise Exception(f"If has_labels is True must provide values for `label_period_val` and `label_period_unit`")
+        if self.label_node and (self.label_period_val is None or self.label_period_unit is None):
+            raise Exception(f"If label_node is parameterized must provide values for `label_period_val` and `label_period_unit`")
 
 
     def __repr__(self):
         return f"<GraphReduce: parent_node={self.parent_node.__class__}>"
 
 
     def __str__(self):
@@ -136,19 +153,17 @@
         
     def hydrate_graph_attrs (
         self,
         attrs=[
             'cut_date',
             'compute_period_val',
             'compute_period_unit',
-            'has_labels',
             'label_period_val',
             'label_period_unit',
             'compute_layer',
-            'feature_function',
             'spark_sqlctx',
             '_storage_client',
         ]
     ):
         """
 Hydrate the nodes in the graph with parent 
 attributes in `attrs`
@@ -197,14 +212,75 @@
                     'parent_key' : parent_key,
                     'relation_key' : relation_key,
                     'relation_type' : relation_type,
                     'reduce' : reduce
                 }
             )
 
+    def join_any (
+        self,
+        to_node: GraphReduceNode,
+        from_node: GraphReduceNode,
+        how: str = 'left',
+        to_node_key: str = None,
+        from_node_key: str = None,
+        to_node_df = None,
+        from_node_df = None
+        ):
+        """
+Join the relations.
+        """
+
+        if to_node_key and from_node_key:
+            pass
+        else:
+            meta = self.get_edge_data(to_node, from_node)
+            if meta:
+                meta = meta['keys']
+                to_node_key = meta['parent_key']
+                from_node_key = meta['relation_key']
+
+            elif not meta:
+                meta = self.get_edge_data(from_node, to_node)
+                if meta:
+                    meta = meta['keys']
+                    to_node_key = meta['relation_key']
+                    from_node_key = meta['parent_key']
+                else:
+                    raise Exception(f"no edge metadata for {to_node} and {from_node}")
+
+        if self.compute_layer in [ComputeLayerEnum.pandas, ComputeLayerEnum.dask]:
+            joined = to_node.df.merge(
+                    from_node.df,
+                    left_on=to_node.df[f"{to_node.prefix}_{to_node_key}"],
+                    right_on=from_node.df[f"{from_node.prefix}_{from_node_key}"],
+                    suffixes=('','_dupe'),
+                    how="left"
+                )
+            self._mark_merged(to_node, from_node)
+            if "key_0" in joined.columns:
+                joined = joined[[c for c in joined.columns if c != "key_0"]]
+                return joined
+            else:
+                return joined
+        elif self.compute_layer == ComputeLayerEnum.spark:     
+            if isinstance(to_node.df, pyspark.sql.dataframe.DataFrame) and isinstance(from_node.df, pyspark.sql.dataframe.DataFrame):
+                joined = to_node.df.join(
+                    from_node.df,
+                    on=to_node.df[f"{to_node.prefix}_{to_node_key}"] == from_node.df[f"{relation_node.prefix}_{from_node_key}"],
+                    how="left"
+                ) 
+                self._mark_merged(to_node, from_node)
+                return joined
+            else:
+                raise Exception(f"Cannot use spark on dataframe of type: {type(to_node.df)}")
+                
+        else:
+            logger.error('no valid compute layer')
+
  
     def join (
         self,
         parent_node: GraphReduceNode,
         relation_node: GraphReduceNode,
         relation_df = None
         ):
@@ -213,14 +289,16 @@
         
         Optionally pass the `child_df` directly
         """
         
         meta = self.get_edge_data(parent_node, relation_node)
         
         if not meta:
+            meta = self.get_edge_data(relation_node, parent_node)
+
             raise Exception(f"no edge metadata for {parent_node} and {relation_node}")
             
         if meta.get('keys'):
             meta = meta['keys']
             
         if meta and meta['relation_type'] == 'parent_child':
             parent_pk = meta['parent_key']
@@ -274,26 +352,45 @@
                 raise Exception(f"Cannot use spark on dataframe of type: {type(parent_node.df)}")
                 
         else:
             logger.error('no valid compute layer')
             
         return None
 
-    
-    
+ 
     def depth_first_generator(self):
         """
 Depth-first traversal over the edges
         """
         if not self.parent_node:
             raise Exception("Must have a parent node set to do depth first traversal")
-        for edge in list(reversed(list(nx.dfs_edges(self, source=self.parent_node)))):
+        for edge in list(reversed(list(nx.dfs_edges(self, source=self.parent_node, depth_limit=self.auto_feature_hops_back)))):
             yield edge
 
 
+    def traverse_up (
+            self, 
+            start: typing.Union[GraphReduceNode, DynamicNode]
+            ) -> list:
+        """
+Traverses up the graph for merging parents.
+        """
+        parents = [(start, n,1) for n in self.predecessors(start)]
+        to_traverse = [(n, 1) for n in self.predecessors(start)]
+        while len(to_traverse):
+            cur_node, cur_level = to_traverse[0]
+            del to_traverse[0]
+
+            for node in self.predecessors(cur_node):
+                parents.append((cur_node, node, cur_level+1))
+                to_traverse.append((node, cur_level+1))
+
+        return parents
+
+
     def get_children (
             self,
             node : GraphReduceNode
             ) -> typing.List[GraphReduceNode]:
         """
 Get the children of a given node
         """
@@ -322,18 +419,18 @@
             else:
                 stringG.add_node(n.__class__.__name__)
 
         for edge in self.edges():
             edge_data = self.get_edge_data(edge[0], edge[1])
             edge_data = edge_data['keys']
             edge_title = f"{edge[0].__class__.__name__} key: {edge_data['parent_key']}\n{edge[1].__class__.__name__} key: {edge_data['relation_key']}\nrelation type: {edge_data['relation_type']}\nreduce relation: {edge_data['reduce']}"
-            if n.__class__.__name__ == 'DynamicNodel':
+            if n.__class__.__name__ == 'DynamicNode':
                 stringG.add_edge(
                         edge[0].fpath,
-                        edge[1].path,
+                        edge[1].fpath,
                         title=edge_title
                         )
             else:
                 stringG.add_edge(
                 edge[0].__class__.__name__, 
                 edge[1].__class__.__name__,
                 title=edge_title)
@@ -365,17 +462,16 @@
 Perform all graph transformations
 1) hydrate graph
 2) check for duplicate prefixes
 3) filter data
 4) clip anomalies
 5) annotate data
 6) depth-first edge traversal to: aggregate / reduce features and labels
-6a) optional alternative feature_function mapping
-6b) join back to parent edge
-6c) post-join annotations if any
+6a) join back to parent edge
+6b) post-join annotations if any
 7) repeat step 6 on all edges up the hierarchy
         """
         
         # get data, filter data, clip columns, and annotate
         logger.info("hydrating graph attributes")
         self.hydrate_graph_attrs()
         logger.info("hydrating graph data")
@@ -385,32 +481,41 @@
         self.prefix_uniqueness()
     
         for node in self.nodes():
             logger.info(f"running filters, normalize, and annotations for {node}")
             node.do_annotate()
             node.do_filters()
             node.do_normalize()
+ 
+        if self.auto_features:
+            for to_node, from_node, level in self.traverse_up(start=self.parent_node):
+                if self.auto_feature_hops_front and level <= self.auto_feature_hops_front:
+                    joined_df = self.join_any(
+                            to_node,
+                            from_node
+                    )
+                    to_node.df = joined_df
 
         logger.info(f"depth-first traversal through the graph from source: {self.parent_node}")
         for edge in self.depth_first_generator():
             parent_node = edge[0]
             relation_node = edge[1]
             edge_data = self.get_edge_data(parent_node, relation_node)
             if edge_data.get('keys'):
                 edge_data = edge_data['keys']
 
             if edge_data['reduce']:
                 logger.info(f"reducing relation {relation_node}")
                 join_df = relation_node.do_reduce(edge_data['relation_key'])
                 # only relevant when reducing
-                if self.dynamic_propagation:
-                    logger.info(f"doing dynamic propagation on node {relation_node}")
-                    child_df = relation_node.dynamic_propagation(
+                if self.auto_features:
+                    logger.info(f"performing auto_features on node {relation_node}")
+                    child_df = relation_node.auto_features(
                             reduce_key=edge_data['relation_key'],
-                            type_func_map=self.type_func_map,
+                            type_func_map=self.feature_typefunc_map,
                             compute_layer=self.compute_layer
                         )
                     
                     # NOTE: this is pandas specific and will break
                     # on other compute layers for now 
                     if self.compute_layer in [ComputeLayerEnum.pandas, ComputeLayerEnum.dask]:
                         if isinstance(join_df, pd.DataFrame) or isinstance(join_df, dd.DataFrame):
@@ -427,17 +532,14 @@
                                 child_df,
                                 on=join_df[relation_node.colabbr(edge_data['relation_key'])] == child_df[relation_node.colabbr(edge_data['relation_key'])],
                                 how="left"
                             )
                         else:
                             join_df = child_df
 
-            elif not edge_data['reduce'] and self.feature_function:
-                logger.info(f"not reducing relation {relation_node}")
-                join_df = getattr(relation_node, self.feature_function)()
             else:
                 # in this case we will join the entire relation's dataframe
                 logger.info(f"doing nothing with relation node {relation_node}")
                 join_df = None
                 
             logger.info(f"joining {relation_node} to {parent_node}")
             joined_df = self.join(
@@ -445,17 +547,26 @@
                 relation_node,
                 relation_df=join_df
             )
 
             # Update the parent dataframe.
             parent_node.df = joined_df
             
-            if self.has_labels:
-                #TODO: Handle the required parameterization better.
-                label_df = relation_node.do_labels(edge_data['relation_key'])
+            # Target variables.
+            if self.label_node and self.label_node == relation_node:
+                logger.info(f"Had label node {self.label_node}")
+                if isinstance(relation_node, DynamicNode):
+                    label_df = relation_node.default_label(
+                            op=self.label_operation,
+                            field=self.label_field,
+                            reduce_key=edge_data['relation_key']
+                            )                    
+                elif isinstance(relation_node, GraphReduceNode):
+                    label_df = relation_node.do_labels(edge_data['relation_key'])
+
                 logger.info(f"computed labels for {relation_node}")
                 if label_df.__class__.__name__ != 'NoneType':
                     joined_with_labels = self.join(
                         parent_node,
                         relation_node,
                         relation_df=label_df
                     )
```

### Comparing `graphreduce-1.6.2/graphreduce/node.py` & `graphreduce-1.6.3/graphreduce/node.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,21 +22,19 @@
 
 class GraphReduceNode(metaclass=abc.ABCMeta): 
     fpath : str
     fmt : str
     prefix : str
     date_key : str
     pk : str 
-    feature_function : str
     compute_layer : ComputeLayerEnum
     spark_sqlctx : typing.Optional[pyspark.sql.SQLContext]
     cut_date : datetime.datetime
     compute_period_val : typing.Union[int, float]
     compute_period_unit : PeriodUnit
-    has_labels : bool
     label_period_val : typing.Optional[typing.Union[int, float]]
     label_period_unit : typing.Optional[PeriodUnit] 
     label_field: typing.Optional[str]
     storage_client: typing.Optional[StorageClient]
     batch_features: typing.List
     online_features: typing.List
     on_demand_features: typing.List
@@ -49,19 +47,17 @@
             prefix : str = None,
             date_key : str = None,
             compute_layer : ComputeLayerEnum = None,
             cut_date : datetime.datetime = datetime.datetime.now(),
             compute_period_val : typing.Union[int, float] = 365,
             compute_period_unit : PeriodUnit  = PeriodUnit.day,
             reduce : bool = True,
-            has_labels : bool = False,
             label_period_val : typing.Optional[typing.Union[int, float]] = None,
             label_period_unit : typing.Optional[PeriodUnit] = None,
             label_field : typing.Optional[str] = None,
-            feature_function : typing.Optional[str] = None,
             spark_sqlctx : pyspark.sql.SQLContext = None,
             columns : list = [],
             storage_client: typing.Optional[StorageClient] = None,
             checkpoints: list = [],
             ):
         """
 Constructor
@@ -73,19 +69,17 @@
     prefix : prefix to use for columns
     date_key : column containing the date - if there isn't one leave blank
     compute_layer : compute layer to use (e.g, ComputeLayerEnum.pandas)
     cut_date : date around which to orient the data
     compute_period_val : amount of time to consider
     compute_period_unit : unit of measure for compute period (e.g., PeriodUnit.day)
     reduce : whether or not to reduce the data
-    has_labels : whether or not the node has labels to compute
     label_period_val : optional period of time to compute labels
     label_period_unit : optional unit of measure for label period (e.g., PeriodUnit.day)
     label_field : optional field on which to compute the label
-    feature_function : optional feature function, usually used when reduce is false
     columns : optional list of columns to include
     storage_client: optional storage client
         """
         # For when this is already set on the class definition.
         if not hasattr(self, 'pk'):
             self.pk = pk
         # For when this is already set on the class definition.
@@ -97,28 +91,29 @@
         self.fpath = fpath
         self.fmt = fmt
         self.compute_layer = compute_layer
         self.cut_date = cut_date
         self.compute_period_val = compute_period_val
         self.compute_period_unit = compute_period_unit
         self.reduce = reduce
-        self.has_labels = has_labels
         self.label_period_val = label_period_val
         self.label_period_unit = label_period_unit
         self.label_field = label_field
-        self.feature_function = feature_function
         self.spark_sqlctx = spark_sqlctx
         self.columns = columns
 
         self._storage_client = storage_client
         # List of merged neighbor classes.
         self._merged = []
         # List of checkpoints.
         self._checkpoints = []
 
+        # Logical types of the original columns from `woodwork`.
+        self._logical_types = {}
+
         if not self.date_key:
             logger.warning(f"no `date_key` set for {self}")
 
 
     def __repr__ (
             self
             ):
@@ -132,36 +127,59 @@
             ):
         """
 Instances string
         """
         return f"<GraphReduceNode: fpath={self.fpath} fmt={self.fmt}>"
 
 
+    def reload (
+            self
+            ):
+        """
+Refresh the node.
+        """
+        self._merged = []
+        self._checkpoints = []
+        self.df = None
+        self._logical_types = {}
+
     
     def do_data (
         self
     ) -> typing.Union[
         pd.DataFrame,
         dd.DataFrame,
         pyspark.sql.dataframe.DataFrame
     ]:
         """
 Get some data
         """
         if self.compute_layer.value == 'pandas':
             if not hasattr(self, 'df') or (hasattr(self,'df') and not isinstance(self.df, pd.DataFrame)):
                 self.df = getattr(pd, f"read_{self.fmt}")(self.fpath)
+
+                # Initialize woodwork.
+                self.df.ww.init()
+                self._logical_types = self.df.ww.logical_types
+
+                # Rename columns with prefixes.
                 if len(self.columns):
                     self.df = self.df[[c for c in self.columns]]
                 self.columns = list(self.df.columns)
                 self.df.columns = [f"{self.prefix}_{c}" for c in self.df.columns]
         elif self.compute_layer.value == 'dask':
             if not hasattr(self, 'df') or (hasattr(self, 'df') and not isinstance(self.df, dd.DataFrame
 )):
                 self.df = getattr(dd, f"read_{self.fmt}")(self.fpath)
+
+                # Initialize woodwork.
+                self.df.ww.init()
+                self._logical_types = self.df.ww.logical_types
+
+                # Rename columns with prefixes.
                 if len(self.columns):
                     self.df = self.df[[c for c in self.columns]]
                 self.columns = list(self.df.columns)
                 self.df.columns = [f"{self.prefix}_{c}" for c in self.df.columns]
         elif self.compute_layer.value == 'spark':
             if not hasattr(self, 'df') or (hasattr(self, 'df') and not isinstance(self.df, pyspark.sql.DataFrame)):
                 self.df = getattr(self.spark_sqlctx.read, f"{self.fmt}")(self.fpath)
@@ -223,34 +241,57 @@
         """
 Filter operations that require some
 additional relational data to perform.
         """
         pass
 
 
-    def dynamic_propagation (
+    def auto_features (
             self,
             reduce_key : str,
             type_func_map : dict = {},
             compute_layer : ComputeLayerEnum = ComputeLayerEnum.pandas,
             ):
         """
-If we're doing dynamic propagation
+If we're doing automatic features
 this function will run a series of
-automatic aggregations
+automatic aggregations.  The top-level
+`GraphReduce` object will handle joining
+the results together.
         """
         if compute_layer == ComputeLayerEnum.pandas:
-            return self.pandas_dynamic_propagation(reduce_key=reduce_key, type_func_map=type_func_map)
+            return self.pandas_auto_features(reduce_key=reduce_key, type_func_map=type_func_map)
         elif compute_layer == ComputeLayerEnum.dask:
-            return self.dask_dynamic_propagation(reduce_key=reduce_key, type_func_map=type_func_map)
+            return self.dask_auto_features(reduce_key=reduce_key, type_func_map=type_func_map)
         elif compute_layer == ComputeLayerEnum.spark:
-            return self.spark_dynamic_propagation(reduce_key=reduce_key, type_func_map=type_func_map)
+            return self.spark_auto_features(reduce_key=reduce_key, type_func_map=type_func_map)
 
 
-    def pandas_dynamic_propagation (
+    def auto_labels (
+            self,
+            reduce_key : str,
+            type_func_map : dict = {},
+            compute_layer : ComputeLayerEnum = ComputeLayerEnum.pandas,
+            ):
+        """
+If we're doing automatic features
+this function will run a series of
+automatic aggregations.  The top-level
+`GraphReduce` object will handle joining
+the results together.
+        """
+        if compute_layer == ComputeLayerEnum.pandas:
+            return self.pandas_auto_labels(reduce_key=reduce_key, type_func_map=type_func_map)
+        elif compute_layer == ComputeLayerEnum.dask:
+            return self.dask_auto_labels(reduce_key=reduce_key, type_func_map=type_func_map)
+        elif compute_layer == ComputeLayerEnum.spark:
+            return self.spark_auto_labels(reduce_key=reduce_key, type_func_map=type_func_map)
+
+
+    def pandas_auto_features (
             self,
             reduce_key : str,
             type_func_map : dict = {}
             ) -> pd.DataFrame:
         """
 Pandas implementation of dynamic propagation of features.
 This is basically automated feature engineering but suffixed
@@ -266,15 +307,15 @@
                     col_new = f"{col}_{func}"
                     agg_funcs[col_new] = pd.NamedAgg(column=col, aggfunc=func)
         return self.prep_for_features().groupby(self.colabbr(reduce_key)).agg(
                 **agg_funcs
                 ).reset_index()
 
 
-    def dask_dynamic_propagation (
+    def dask_auto_features (
             self,
             reduce_key : str,
             type_func_map : dict = {},
             ) -> dd.DataFrame:
         """
 Dask implementation of dynamic propagation of features.
 This is basically automated feature engineering but suffixed
@@ -290,15 +331,15 @@
                     col_new = f"{col}_{func}"
                     agg_funcs[col_new] = pd.NamedAgg(column=col, aggfunc=func)
         return self.prep_for_features().groupby(self.colabbr(reduce_key)).agg(
                 **agg_funcs
                 ).reset_index()
 
 
-    def spark_dynamic_propagation (
+    def spark_auto_features (
             self,
             reduce_key : str,
             type_func_map : dict = {},
             ) -> pyspark.sql.DataFrame:
         """
 Spark implementation of dynamic propagation of features.
 This is basically automated feature engineering but suffixed
@@ -316,14 +357,82 @@
                     col_new = f"{col}_{func}"
                     agg_funcs.append(getattr(F, func)(F.col(col)).alias(col_new))
         return self.prep_for_features().groupby(self.colabbr(reduce_key)).agg(
                 *agg_funcs
                 )
 
 
+    def pandas_auto_labels (
+            self,
+            reduce_key : str,
+            type_func_map : dict = {}
+            ) -> pd.DataFrame:
+        """
+Pandas implementation of auto labeling based on
+provided columns.
+        """
+        agg_funcs = {}
+        for col, _type in dict(self.df.dtypes).items():
+            if col.endswith('_label'):
+                _type = str(_type)
+                if type_func_map.get(_type):
+                    for func in type_func_map[_type]:
+                        col_new = f"{col}_{func}_label"
+                        agg_funcs[col_new] = pd.NamedAgg(column=col, aggfunc=func)
+        return self.prep_for_labels().groupby(self.colabbr(reduce_key)).agg(
+                **agg_funcs
+                ).reset_index()
+
+
+    def dask_auto_labels (
+            self,
+            reduce_key : str,
+            type_func_map : dict = {},
+            ) -> dd.DataFrame:
+        """
+Dask implementation of auto labeling based on
+provided columns.
+        """
+        agg_funcs = {}
+        for col, _type in dict(self.df.dtypes).items():
+            if col.endswith('_label'):
+                _type = str(_type)
+                if type_func_map.get(_type):
+                    for func in type_func_map[_type]:
+                        col_new = f"{col}_{func}_label"
+                        agg_funcs[col_new] = pd.NamedAgg(column=col, aggfunc=func)
+        return self.prep_for_labels().groupby(self.colabbr(reduce_key)).agg(
+                **agg_funcs
+                ).reset_index()
+
+
+    def spark_auto_labels (
+            self,
+            reduce_key : str,
+            type_func_map : dict = {},
+            ) -> pyspark.sql.DataFrame:
+        """
+Spark implementation of auto labeling based on
+provided columns.
+        """
+        agg_funcs = []
+        for field in self.df.schema.fields:
+            field_meta = json.loads(field.json())
+            col = field_meta['name']
+            _type = field_meta['type']
+            if col.endswith('_label'):
+                if type_func_map.get(_type):
+                    for func in type_func_map[_type]:
+                        col_new = f"{col}_{func}_label"
+                        agg_funcs.append(getattr(F, func)(F.col(col)).alias(col_new))
+        return self.prep_for_labels().groupby(self.colabbr(reduce_key)).agg(
+                *agg_funcs
+                )
+
+
     @abc.abstractmethod
     def do_reduce (
             self, 
             reduce_key
             ):
         """
 Reduce operation or the node
@@ -469,22 +578,64 @@
                     return self.df.filter(
                     self.df[self.colabbr(self.date_key)] > (datetime.datetime.now() - datetime.timedelta(minutes=self.label_period_minutes()))
                 )
         # no-op
         return self.df
 
 
+
+    def default_label (
+            self,
+            op: typing.Union[str, callable],
+            field: str,
+            reduce_key: typing.Optional[str] = None,
+            ) -> typing.Union[pd.DataFrame, dd.DataFrame, pyspark.sql.dataframe.DataFrame]:
+        """
+Default label operation.
+
+        Arguments
+        ----------
+        op: operation to call for label
+        field: str label field to call operation on
+        reduce: bool whether or not to reduce
+        """
+        if self.colabbr(field) in self.df.columns:
+            if self.compute_layer in [ComputeLayerEnum.pandas, ComputeLayerEnum.dask]:
+                if self.reduce:
+                    if callable(op):
+                        return self.prep_for_labels().groupby(self.colabbr(reduce_key)).agg(**{
+                            self.colabbr(field+'_label') : pd.NamedAgg(column=self.colabbr(field), aggfunc=op)
+                        }).reset_index()
+                    else:
+                        return self.prep_for_labels().groupby(self.colabbr(reduce_key)).agg(**{
+                            self.colabbr(field+'_label') : pd.NamedAgg(column=self.colabbr(field), aggfunc=op)
+                            }).reset_index()
+                else:
+                    label_df = self.prep_for_labels()
+                    if callable(op):
+                        label_df[self.colabbr(field)+'_label'] = label_df[self.colabbr(field)].apply(op)
+                    else:
+                        label_df[self.colabbr(field)+'_label'] = label_df[self.colabbr(field)].apply(lambda x: getattr(x, op)())
+                    return label_df[[self.colabbr(self.pk), self.colabbr(field)+'_label']]
+
+            elif self.compute_layer == ComputeLayerEnum.spark:
+                pass
+            elif self.compute_layer == ComputeLayerEnum.snowflake:
+                pass
+
+
     def online_features (
             self,
             ):
         """
 Define online features.
         """
         pass
 
+
     def on_demand_features (
             self,
             ):
         """
 Define on demand features for this node.
         """
         pass
@@ -497,22 +648,21 @@
 A dynamic architecture for entities with no logic 
 needed in addition to the top-level GraphReduceNode
 parameters
     """
     def __init__ (
             self,
             *args,
-            **kwargs
+            **kwargs,
             ):
         """
 Constructor
         """
         super().__init__(*args, **kwargs)
 
-
     def do_filters(self):
         pass
 
     def do_annotate(self):
         pass
 
     def do_post_join_annotate(self):
```

### Comparing `graphreduce-1.6.2/graphreduce/storage.py` & `graphreduce-1.6.3/graphreduce/storage.py`

 * *Files identical despite different names*

### Comparing `graphreduce-1.6.2/graphreduce.egg-info/PKG-INFO` & `graphreduce-1.6.3/graphreduce.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphreduce
-Version: 1.6.2
+Version: 1.6.3
 Summary: Leveraging graph data structures for complex feature engineering pipelines.
 Home-page: https://github.com/wesmadrigal/graphreduce
 Author: Wes Madrigal
 Author-email: wes@madconsulting.ai
 License: MIT
 Project-URL: Source, http://github.com/wesmadrigal/graphreduce
 Project-URL: Issue Tracker, https://github.com/wesmadrigal/graphreduce/issues
```

### Comparing `graphreduce-1.6.2/setup.py` & `graphreduce-1.6.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 
 
 
 if __name__ == "__main__":
 
     setuptools.setup(
         name="graphreduce",
-        version = "1.6.2",
+        version = "1.6.3",
         url="https://github.com/wesmadrigal/graphreduce",
         packages = setuptools.find_packages(exclude=[ "docs", "examples" ]),
         install_requires = [
             "abstract.jwrotator>=0.3",
             "dask",
             "networkx>=2.6.3",
             "pandas>=1.3.4",
             "pyspark>=3.2.0",
             "pyvis>=0.3.1",
             "setuptools>=65.5.1",
-            "structlog>=23.1.0"
+            "structlog>=23.1.0",
+            "pytest>=8.0.2"
             ],
         author="Wes Madrigal",
         author_email="wes@madconsulting.ai",
         license="MIT",
 
         description="Leveraging graph data structures for complex feature engineering pipelines.",
         long_description = pathlib.Path("README.md").read_text(),
```

