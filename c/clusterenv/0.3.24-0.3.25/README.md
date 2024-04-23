# Comparing `tmp/clusterenv-0.3.24.tar.gz` & `tmp/clusterenv-0.3.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterenv-0.3.24.tar", max compression
+gzip compressed data, was "clusterenv-0.3.25.tar", max compression
```

## Comparing `clusterenv-0.3.24.tar` & `clusterenv-0.3.25.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      176 2024-02-19 11:34:17.626664 clusterenv-0.3.24/README.md
--rw-r--r--   0        0        0      294 2024-04-22 15:48:46.618068 clusterenv-0.3.24/clusterenv/__init__.py
--rw-r--r--   0        0        0     4675 2024-04-21 20:01:25.417246 clusterenv-0.3.24/clusterenv/_types.py
--rw-r--r--   0        0        0     5168 2024-04-21 21:35:30.468145 clusterenv-0.3.24/clusterenv/common.py
--rw-r--r--   0        0        0     8313 2024-04-22 15:48:24.218789 clusterenv-0.3.24/clusterenv/envs/cluster.py
--rw-r--r--   0        0        0     5674 2024-04-21 21:34:45.899540 clusterenv-0.3.24/clusterenv/render.py
--rw-r--r--   0        0        0       49 2024-04-22 14:09:14.031863 clusterenv-0.3.24/clusterenv/wrappers/__init__.py
--rw-r--r--   0        0        0     2142 2024-04-22 15:42:02.335594 clusterenv-0.3.24/clusterenv/wrappers/transform.py
--rw-r--r--   0        0        0      551 2024-04-22 15:48:52.804989 clusterenv-0.3.24/pyproject.toml
--rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 clusterenv-0.3.24/PKG-INFO
+-rw-r--r--   0        0        0      176 2024-02-19 11:34:17.626664 clusterenv-0.3.25/README.md
+-rw-r--r--   0        0        0      294 2024-04-22 15:48:46.618068 clusterenv-0.3.25/clusterenv/__init__.py
+-rw-r--r--   0        0        0     4675 2024-04-21 20:01:25.417246 clusterenv-0.3.25/clusterenv/_types.py
+-rw-r--r--   0        0        0     5168 2024-04-21 21:35:30.468145 clusterenv-0.3.25/clusterenv/common.py
+-rw-r--r--   0        0        0     8350 2024-04-22 16:01:52.318813 clusterenv-0.3.25/clusterenv/envs/cluster.py
+-rw-r--r--   0        0        0     5795 2024-04-22 16:03:36.760303 clusterenv-0.3.25/clusterenv/render.py
+-rw-r--r--   0        0        0       49 2024-04-22 14:09:14.031863 clusterenv-0.3.25/clusterenv/wrappers/__init__.py
+-rw-r--r--   0        0        0     2142 2024-04-22 15:42:02.335594 clusterenv-0.3.25/clusterenv/wrappers/transform.py
+-rw-r--r--   0        0        0      551 2024-04-22 16:04:04.806861 clusterenv-0.3.25/pyproject.toml
+-rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 clusterenv-0.3.25/PKG-INFO
```

### Comparing `clusterenv-0.3.24/clusterenv/_types.py` & `clusterenv-0.3.25/clusterenv/_types.py`

 * *Files identical despite different names*

### Comparing `clusterenv-0.3.24/clusterenv/common.py` & `clusterenv-0.3.25/clusterenv/common.py`

 * *Files identical despite different names*

### Comparing `clusterenv-0.3.24/clusterenv/envs/cluster.py` & `clusterenv-0.3.25/clusterenv/envs/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         self._logger = logging.getLogger(self.__class__.__name__)
         self._plotter = ClusterRenderer(
             nodes=self._n_nodes,
             jobs=self._n_jobs,
             resource=self._n_resource,
             time=self._max_time,
             cooldown=cooldown,
+            render_mode=render_mode
         )
         self._action_error = None
         self._action_correct = None
         self.nodes: Nodes = self._node_gen.generate(
             self._n_nodes, self._n_resource, self._max_time, 255.0
         )
         self.jobs: Jobs = self._job_gen.generate(
@@ -148,14 +149,15 @@
             fig = self._plotter(
                 self._observation,
                 current_time=self._time,
                 error=self._action_error,
                 correct=self._action_correct,
             )
             if self.render_mode == "rgb_array":
+
                 buf = fig.canvas.tostring_rgb()
                 width, height = fig.canvas.get_width_height()
                 expected_height = int(fig.get_figheight() * fig.dpi)
                 expected_width = int(fig.get_figwidth() * fig.dpi)
                 width_mult: int = expected_width // width
                 height_mult: int = expected_height // height
                 return np.frombuffer(buf, dtype=np.uint8).reshape(
```

### Comparing `clusterenv-0.3.24/clusterenv/render.py` & `clusterenv-0.3.25/clusterenv/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,16 +126,20 @@
     nodes: int
     jobs: int
     resource: int
     time: int
     cooldown: float
     fig: Figure = field(init=False)
     axs: npt.NDArray = field(init=False)
+    render_mode: str = ''
 
     def __post_init__(self):
+        print(self.render_mode)
+        if self.render_mode != 'human':
+            plt.ioff()
         self.jobs_n_columns: int = math.ceil(self.jobs**0.5)
         self.nodes_n_columns: int = math.ceil(self.nodes**0.5)
 
         jobs_n_rows: int = math.ceil(self.jobs / self.jobs_n_columns)
         nodes_n_rows: int = math.ceil(self.nodes / self.nodes_n_columns)
 
         n_rows: int = max(jobs_n_rows, nodes_n_rows)
```

### Comparing `clusterenv-0.3.24/clusterenv/wrappers/transform.py` & `clusterenv-0.3.25/clusterenv/wrappers/transform.py`

 * *Files identical despite different names*

### Comparing `clusterenv-0.3.24/pyproject.toml` & `clusterenv-0.3.25/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clusterenv"
-version = "0.3.24"
+version = "0.3.25"
 description = "ClusterEnv is a Python Gym environment designed to simulate and model the management and optimization of computing clusters. In the realm of distributed computing."
 authors = ["Guy Arieli"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `clusterenv-0.3.24/PKG-INFO` & `clusterenv-0.3.25/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterenv
-Version: 0.3.24
+Version: 0.3.25
 Summary: ClusterEnv is a Python Gym environment designed to simulate and model the management and optimization of computing clusters. In the realm of distributed computing.
 License: MIT
 Author: Guy Arieli
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

