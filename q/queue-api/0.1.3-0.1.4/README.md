# Comparing `tmp/queue_api-0.1.3.tar.gz` & `tmp/queue_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_api-0.1.3.tar", last modified: Mon Apr 22 09:39:01 2024, max compression
+gzip compressed data, was "queue_api-0.1.4.tar", last modified: Tue Apr 23 13:05:37 2024, max compression
```

## Comparing `queue_api-0.1.3.tar` & `queue_api-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:39:01.231153 queue_api-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-22 09:39:01.231153 queue_api-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-21 17:59:12.000000 queue_api-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      565 2024-04-22 09:38:58.000000 queue_api-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 09:39:01.231153 queue_api-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:39:01.231153 queue_api-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:39:01.221151 queue_api-0.1.3/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:39:01.231153 queue_api-0.1.3/src/q/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      149 2024-04-21 18:00:51.000000 queue_api-0.1.3/src/q/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      228 2024-04-21 18:01:43.000000 queue_api-0.1.3/src/q/api/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:39:01.231153 queue_api-0.1.3/src/q/api/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      131 2024-04-21 18:01:20.000000 queue_api-0.1.3/src/q/api/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      649 2024-04-21 17:59:44.000000 queue_api-0.1.3/src/q/api/api/append.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      172 2024-04-15 16:36:13.000000 queue_api-0.1.3/src/q/api/api/queue.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5901 2024-04-21 17:48:09.000000 queue_api-0.1.3/src/q/api/api/read.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2723 2024-04-21 17:48:29.000000 queue_api-0.1.3/src/q/api/api/write.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:39:01.231153 queue_api-0.1.3/src/q/api/impl/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-04-15 16:36:13.000000 queue_api-0.1.3/src/q/api/impl/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      385 2024-04-15 16:36:13.000000 queue_api-0.1.3/src/q/api/impl/empty.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1180 2024-04-21 17:50:16.000000 queue_api-0.1.3/src/q/api/impl/simple.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:39:01.231153 queue_api-0.1.3/src/q/api/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 17:58:36.000000 queue_api-0.1.3/src/q/api/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      286 2024-04-21 17:59:26.000000 queue_api-0.1.3/src/q/api/ops/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1113 2024-04-21 17:58:13.000000 queue_api-0.1.3/src/q/api/ops/append_bounding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1105 2024-04-21 17:50:36.000000 queue_api-0.1.3/src/q/api/ops/bounding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1479 2024-04-21 17:50:49.000000 queue_api-0.1.3/src/q/api/ops/interleaving.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1735 2024-04-21 17:51:01.000000 queue_api-0.1.3/src/q/api/ops/merging.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1978 2024-04-21 17:51:05.000000 queue_api-0.1.3/src/q/api/ops/splitting.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 09:39:01.231153 queue_api-0.1.3/src/queue_api.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-22 09:39:01.000000 queue_api-0.1.3/src/queue_api.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      641 2024-04-22 09:39:01.000000 queue_api-0.1.3/src/queue_api.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 09:39:01.000000 queue_api-0.1.3/src/queue_api.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       23 2024-04-22 09:39:01.000000 queue_api-0.1.3/src/queue_api.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-22 09:39:01.000000 queue_api-0.1.3/src/queue_api.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.250655 queue_api-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-23 13:05:37.250655 queue_api-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-21 17:59:12.000000 queue_api-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      565 2024-04-23 13:05:34.000000 queue_api-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-23 13:05:37.250655 queue_api-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.240655 queue_api-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.240655 queue_api-0.1.4/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.240655 queue_api-0.1.4/src/q/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      149 2024-04-21 18:00:51.000000 queue_api-0.1.4/src/q/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      228 2024-04-21 18:01:43.000000 queue_api-0.1.4/src/q/api/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.240655 queue_api-0.1.4/src/q/api/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      131 2024-04-21 18:01:20.000000 queue_api-0.1.4/src/q/api/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      649 2024-04-21 17:59:44.000000 queue_api-0.1.4/src/q/api/api/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      172 2024-04-15 16:36:13.000000 queue_api-0.1.4/src/q/api/api/queue.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5922 2024-04-23 13:05:32.000000 queue_api-0.1.4/src/q/api/api/read.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2723 2024-04-21 17:48:29.000000 queue_api-0.1.4/src/q/api/api/write.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.250655 queue_api-0.1.4/src/q/api/impl/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-04-15 16:36:13.000000 queue_api-0.1.4/src/q/api/impl/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      385 2024-04-15 16:36:13.000000 queue_api-0.1.4/src/q/api/impl/empty.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1180 2024-04-21 17:50:16.000000 queue_api-0.1.4/src/q/api/impl/simple.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.250655 queue_api-0.1.4/src/q/api/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 17:58:36.000000 queue_api-0.1.4/src/q/api/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      286 2024-04-21 17:59:26.000000 queue_api-0.1.4/src/q/api/ops/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1113 2024-04-21 17:58:13.000000 queue_api-0.1.4/src/q/api/ops/append_bounding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1105 2024-04-21 17:50:36.000000 queue_api-0.1.4/src/q/api/ops/bounding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1479 2024-04-21 17:50:49.000000 queue_api-0.1.4/src/q/api/ops/interleaving.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1735 2024-04-21 17:51:01.000000 queue_api-0.1.4/src/q/api/ops/merging.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1978 2024-04-21 17:51:05.000000 queue_api-0.1.4/src/q/api/ops/splitting.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 13:05:37.250655 queue_api-0.1.4/src/queue_api.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-23 13:05:37.000000 queue_api-0.1.4/src/queue_api.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      641 2024-04-23 13:05:37.000000 queue_api-0.1.4/src/queue_api.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-23 13:05:37.000000 queue_api-0.1.4/src/queue_api.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       23 2024-04-23 13:05:37.000000 queue_api-0.1.4/src/queue_api.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-23 13:05:37.000000 queue_api-0.1.4/src/queue_api.egg-info/top_level.txt
```

### Comparing `queue_api-0.1.3/pyproject.toml` & `queue_api-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "queue-api"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "API for an asynchronous, point-readable queue"
 dependencies = [
   "haskellian", "lazy-loader"
 ]
```

### Comparing `queue_api-0.1.3/src/q/api/api/append.py` & `queue_api-0.1.4/src/q/api/api/append.py`

 * *Files identical despite different names*

### Comparing `queue_api-0.1.3/src/q/api/api/read.py` & `queue_api-0.1.4/src/q/api/api/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,18 +103,18 @@
   def filter(self, pred: Callable[[A], TypeGuard[B]]) -> 'ReadQueue[B]': ...
   @overload
   def filter(self, pred: Callable[[A], bool]) -> 'ReadQueue[A]': ...
   def filter(self, pred): # type: ignore
     return FilteredQueue(self, lambda _, v: pred(v))
   
   @overload
-  def filter(self, pred: Callable[[str, A], TypeGuard[B]]) -> 'ReadQueue[B]': ...
+  def filter_kv(self, pred: Callable[[str, A], TypeGuard[B]]) -> 'ReadQueue[B]': ...
   @overload
-  def filter(self, pred: Callable[[str, A], bool]) -> 'ReadQueue[A]': ...
-  def filter_kv(self, pred):
+  def filter_kv(self, pred: Callable[[str, A], bool]) -> 'ReadQueue[A]': ...
+  def filter_kv(self, pred): # type: ignore
     return FilteredQueue(self, pred)
   
   def partition(self, pred: Callable[[A], bool]) -> 'tuple[ReadQueue[A], ReadQueue[A]]':
     """Returns `self.filter(pred), self.filter(!pred)`"""
     return self.filter(pred), self.filter(lambda x: not pred(x))
   
   def partition_kv(self, pred: Callable[[str, A], bool]) -> 'tuple[ReadQueue[A], ReadQueue[A]]':
```

### Comparing `queue_api-0.1.3/src/q/api/api/write.py` & `queue_api-0.1.4/src/q/api/api/write.py`

 * *Files identical despite different names*

### Comparing `queue_api-0.1.3/src/q/api/impl/simple.py` & `queue_api-0.1.4/src/q/api/impl/simple.py`

 * *Files identical despite different names*

### Comparing `queue_api-0.1.3/src/q/api/ops/append_bounding.py` & `queue_api-0.1.4/src/q/api/ops/append_bounding.py`

 * *Files identical despite different names*

### Comparing `queue_api-0.1.3/src/q/api/ops/bounding.py` & `queue_api-0.1.4/src/q/api/ops/bounding.py`

 * *Files identical despite different names*

### Comparing `queue_api-0.1.3/src/q/api/ops/interleaving.py` & `queue_api-0.1.4/src/q/api/ops/interleaving.py`

 * *Files identical despite different names*

### Comparing `queue_api-0.1.3/src/q/api/ops/merging.py` & `queue_api-0.1.4/src/q/api/ops/merging.py`

 * *Files identical despite different names*

### Comparing `queue_api-0.1.3/src/q/api/ops/splitting.py` & `queue_api-0.1.4/src/q/api/ops/splitting.py`

 * *Files identical despite different names*

### Comparing `queue_api-0.1.3/src/queue_api.egg-info/SOURCES.txt` & `queue_api-0.1.4/src/queue_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

