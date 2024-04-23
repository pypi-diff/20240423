# Comparing `tmp/clusterenv-0.3.26.tar.gz` & `tmp/clusterenv-0.3.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterenv-0.3.26.tar", max compression
+gzip compressed data, was "clusterenv-0.3.27.tar", max compression
```

## Comparing `clusterenv-0.3.26.tar` & `clusterenv-0.3.27.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      176 2024-02-19 11:34:17.626664 clusterenv-0.3.26/README.md
--rw-r--r--   0        0        0      317 2024-04-23 07:50:04.321147 clusterenv-0.3.26/clusterenv/__init__.py
--rw-r--r--   0        0        0     4675 2024-04-21 20:01:25.417246 clusterenv-0.3.26/clusterenv/_types.py
--rw-r--r--   0        0        0     5168 2024-04-21 21:35:30.468145 clusterenv-0.3.26/clusterenv/common.py
--rw-r--r--   0        0        0     8373 2024-04-23 07:49:44.238424 clusterenv-0.3.26/clusterenv/envs/cluster.py
--rw-r--r--   0        0        0     5815 2024-04-23 07:47:03.464236 clusterenv-0.3.26/clusterenv/render.py
--rw-r--r--   0        0        0       49 2024-04-22 14:09:14.031863 clusterenv-0.3.26/clusterenv/wrappers/__init__.py
--rw-r--r--   0        0        0     2142 2024-04-22 15:42:02.335594 clusterenv-0.3.26/clusterenv/wrappers/transform.py
--rw-r--r--   0        0        0      551 2024-04-23 07:50:38.700275 clusterenv-0.3.26/pyproject.toml
--rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 clusterenv-0.3.26/PKG-INFO
+-rw-r--r--   0        0        0      176 2024-02-19 11:34:17.626664 clusterenv-0.3.27/README.md
+-rw-r--r--   0        0        0      317 2024-04-23 07:50:04.321147 clusterenv-0.3.27/clusterenv/__init__.py
+-rw-r--r--   0        0        0     4675 2024-04-21 20:01:25.417246 clusterenv-0.3.27/clusterenv/_types.py
+-rw-r--r--   0        0        0     5168 2024-04-21 21:35:30.468145 clusterenv-0.3.27/clusterenv/common.py
+-rw-r--r--   0        0        0     8373 2024-04-23 07:49:44.238424 clusterenv-0.3.27/clusterenv/envs/cluster.py
+-rw-r--r--   0        0        0     5771 2024-04-23 07:51:14.186311 clusterenv-0.3.27/clusterenv/render.py
+-rw-r--r--   0        0        0       49 2024-04-22 14:09:14.031863 clusterenv-0.3.27/clusterenv/wrappers/__init__.py
+-rw-r--r--   0        0        0     2142 2024-04-22 15:42:02.335594 clusterenv-0.3.27/clusterenv/wrappers/transform.py
+-rw-r--r--   0        0        0      551 2024-04-23 07:52:13.281170 clusterenv-0.3.27/pyproject.toml
+-rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 clusterenv-0.3.27/PKG-INFO
```

### Comparing `clusterenv-0.3.26/clusterenv/_types.py` & `clusterenv-0.3.27/clusterenv/_types.py`

 * *Files identical despite different names*

### Comparing `clusterenv-0.3.26/clusterenv/common.py` & `clusterenv-0.3.27/clusterenv/common.py`

 * *Files identical despite different names*

### Comparing `clusterenv-0.3.26/clusterenv/envs/cluster.py` & `clusterenv-0.3.27/clusterenv/envs/cluster.py`

 * *Files identical despite different names*

### Comparing `clusterenv-0.3.26/clusterenv/render.py` & `clusterenv-0.3.27/clusterenv/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,10 +201,9 @@
                 time=self.time,
                 resource=self.resource,
                 cmap=cmap_color(j_idx, 1),
                 status=JobStatus(status[j_idx]),
             )
         # update figure
         plt.draw()
-        if self.render_mode == 'human':
-            plt.pause(self.cooldown)
+        plt.pause(self.cooldown)
         return self.fig
```

### Comparing `clusterenv-0.3.26/clusterenv/wrappers/transform.py` & `clusterenv-0.3.27/clusterenv/wrappers/transform.py`

 * *Files identical despite different names*

### Comparing `clusterenv-0.3.26/pyproject.toml` & `clusterenv-0.3.27/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clusterenv"
-version = "0.3.26"
+version = "0.3.27"
 description = "ClusterEnv is a Python Gym environment designed to simulate and model the management and optimization of computing clusters. In the realm of distributed computing."
 authors = ["Guy Arieli"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `clusterenv-0.3.26/PKG-INFO` & `clusterenv-0.3.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterenv
-Version: 0.3.26
+Version: 0.3.27
 Summary: ClusterEnv is a Python Gym environment designed to simulate and model the management and optimization of computing clusters. In the realm of distributed computing.
 License: MIT
 Author: Guy Arieli
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

