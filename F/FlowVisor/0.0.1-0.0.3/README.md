# Comparing `tmp/FlowVisor-0.0.1.tar.gz` & `tmp/FlowVisor-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowVisor-0.0.1.tar", last modified: Mon Apr 22 12:24:25 2024, max compression
+gzip compressed data, was "FlowVisor-0.0.3.tar", last modified: Tue Apr 23 15:18:35 2024, max compression
```

## Comparing `FlowVisor-0.0.1.tar` & `FlowVisor-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-22 12:24:25.720333 FlowVisor-0.0.1/
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-22 12:24:25.720333 FlowVisor-0.0.1/FlowVisor.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)      665 2024-04-22 12:24:25.000000 FlowVisor-0.0.1/FlowVisor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      288 2024-04-22 12:24:25.000000 FlowVisor-0.0.1/FlowVisor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-04-22 12:24:25.000000 FlowVisor-0.0.1/FlowVisor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       16 2024-04-22 12:24:25.000000 FlowVisor-0.0.1/FlowVisor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-04-22 12:24:25.000000 FlowVisor-0.0.1/FlowVisor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.0.1/LICENSE
--rw-rw-r--   0 phil      (1000) phil      (1000)      665 2024-04-22 12:24:25.720333 FlowVisor-0.0.1/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     1234 2024-04-22 12:15:27.000000 FlowVisor-0.0.1/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-22 12:24:25.720333 FlowVisor-0.0.1/flowvisor/
--rw-rw-r--   0 phil      (1000) phil      (1000)     5322 2024-04-22 12:09:57.000000 FlowVisor-0.0.1/flowvisor/__init__.py
--rw-rw-r--   0 phil      (1000) phil      (1000)      606 2024-04-22 11:10:52.000000 FlowVisor-0.0.1/flowvisor/flowvisor_config.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     5467 2024-04-22 12:10:15.000000 FlowVisor-0.0.1/flowvisor/function_node.py
--rw-rw-r--   0 phil      (1000) phil      (1000)     2368 2024-04-22 10:26:27.000000 FlowVisor-0.0.1/flowvisor/utils.py
--rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-04-22 12:24:25.720333 FlowVisor-0.0.1/setup.cfg
--rw-rw-r--   0 phil      (1000) phil      (1000)      861 2024-04-22 12:23:07.000000 FlowVisor-0.0.1/setup.py
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-23 15:18:35.474054 FlowVisor-0.0.3/
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-23 15:18:35.474054 FlowVisor-0.0.3/FlowVisor.egg-info/
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2757 2024-04-23 15:18:35.000000 FlowVisor-0.0.3/FlowVisor.egg-info/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)      311 2024-04-23 15:18:35.000000 FlowVisor-0.0.3/FlowVisor.egg-info/SOURCES.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)        1 2024-04-23 15:18:35.000000 FlowVisor-0.0.3/FlowVisor.egg-info/dependency_links.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       51 2024-04-23 15:18:35.000000 FlowVisor-0.0.3/FlowVisor.egg-info/requires.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)       10 2024-04-23 15:18:35.000000 FlowVisor-0.0.3/FlowVisor.egg-info/top_level.txt
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1067 2024-04-22 08:55:02.000000 FlowVisor-0.0.3/LICENSE
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2757 2024-04-23 15:18:35.474054 FlowVisor-0.0.3/PKG-INFO
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2119 2024-04-23 15:17:49.000000 FlowVisor-0.0.3/README.md
+drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2024-04-23 15:18:35.474054 FlowVisor-0.0.3/flowvisor/
+-rw-rw-r--   0 phil      (1000) phil      (1000)       87 2024-04-23 14:16:28.000000 FlowVisor-0.0.3/flowvisor/__init__.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     7539 2024-04-23 14:40:02.000000 FlowVisor-0.0.3/flowvisor/flowvisor.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)      606 2024-04-22 11:10:52.000000 FlowVisor-0.0.3/flowvisor/flowvisor_config.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     7283 2024-04-23 14:38:39.000000 FlowVisor-0.0.3/flowvisor/function_node.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)     2368 2024-04-22 10:26:27.000000 FlowVisor-0.0.3/flowvisor/utils.py
+-rw-rw-r--   0 phil      (1000) phil      (1000)       38 2024-04-23 15:18:35.474054 FlowVisor-0.0.3/setup.cfg
+-rw-rw-r--   0 phil      (1000) phil      (1000)     1002 2024-04-23 15:18:31.000000 FlowVisor-0.0.3/setup.py
```

### Comparing `FlowVisor-0.0.1/LICENSE` & `FlowVisor-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.0.1/flowvisor/flowvisor_config.py` & `FlowVisor-0.0.3/flowvisor/flowvisor_config.py`

 * *Files identical despite different names*

### Comparing `FlowVisor-0.0.1/flowvisor/function_node.py` & `FlowVisor-0.0.3/flowvisor/function_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,20 +16,22 @@
     A node in the function call graph
     """
 
     NODE_IMAGE_CACHE = "__flowvisor_node_image_cache__"
     NODE_IMAGE_SCALE = 300
 
     def __init__(self, func):
-        self.id: str = utils.function_to_id(func)
-        self.uuid = uuid.uuid4()
-        self.name: str = func.__name__
-        self.file_path: str = func.__code__.co_filename
-        self.file_name: str = os.path.basename(self.file_path)
+        if func is not None:
+            self.id: str = utils.function_to_id(func)
+            self.uuid = str(uuid.uuid4())
+            self.name: str = func.__name__
+            self.file_path: str = func.__code__.co_filename
+            self.file_name: str = os.path.basename(self.file_path)
         self.children: List[FunctionNode] = []
+        self.children_ids: List[str] = []
         self.time: float = 0
         self.diagram_node = None
         self.called: int = 0
 
     def export_node_image(self, highest_time):
         """
         Generates the node image background.
@@ -167,14 +169,54 @@
         Returns the file name and function name.
         """
         return f"{self.file_name}::{self.name}"
 
     def __str__(self):
         return self.file_function_name()
 
+    def to_dict(self, short = False):
+        """
+        Gets the node as a dictionary.
+        
+        Args:
+            short: If the dictionary should be short.
+        """
+
+        if short:
+            return {
+                "id": self.id,
+                "uuid": self.uuid,
+                "name": self.name,
+                "file_path": self.file_path,
+                "file_name": self.file_name,
+            }
+        return {
+            "id": self.id,
+            "uuid": self.uuid,
+            "name": self.name,
+            "file_path": self.file_path,
+            "file_name": self.file_name,
+            "children": [child.to_dict(True) for child in self.children],
+            "time": self.time,
+            "called": self.called
+        }
+
+    def resolve_children_ids(self, all_nodes):
+        """
+        Resolves the children ids.
+        
+        Args:
+            all_nodes: All nodes in the graph.
+        """
+        self.children = []
+        for child_id in self.children_ids:
+            for node in all_nodes:
+                if node.uuid == child_id:
+                    self.add_child(node)
+
     @staticmethod
     def make_node_image_cache():
         """
         Makes the node image cache.
         """
         os.makedirs(FunctionNode.NODE_IMAGE_CACHE, exist_ok=True)
 
@@ -182,7 +224,26 @@
     def clear_node_image_cache():
         """
         Clears the node image cache.
         """
         for file in os.listdir(FunctionNode.NODE_IMAGE_CACHE):
             os.remove(f"{FunctionNode.NODE_IMAGE_CACHE}/{file}")
         os.rmdir(FunctionNode.NODE_IMAGE_CACHE)
+        
+    @staticmethod
+    def from_dict(dict):
+        """
+        Creates a FunctionNode from a dictionary.
+        
+        Args:
+            dict: The dictionary to create the FunctionNode from.
+        """
+        node = FunctionNode(None)
+        node.id = dict["id"]
+        node.uuid = dict["uuid"]
+        node.name = dict["name"]
+        node.file_path = dict["file_path"]
+        node.file_name = dict["file_name"]
+        node.children_ids = [child["uuid"] for child in dict["children"]]
+        node.time = dict["time"]
+        node.called = dict["called"]
+        return node
```

### Comparing `FlowVisor-0.0.1/flowvisor/utils.py` & `FlowVisor-0.0.3/flowvisor/utils.py`

 * *Files identical despite different names*

