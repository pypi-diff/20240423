# Comparing `tmp/miniagents-0.0.6.tar.gz` & `tmp/miniagents-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniagents-0.0.6.tar", max compression
+gzip compressed data, was "miniagents-0.0.7.tar", max compression
```

## Comparing `miniagents-0.0.6.tar` & `miniagents-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.6/LICENSE
--rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.6/README.md
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.6/miniagents/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.6/miniagents/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.6/miniagents/ext/llms/__init__.py
--rw-r--r--   0        0        0     4364 2024-04-18 21:45:37.115573 miniagents-0.0.6/miniagents/ext/llms/anthropic.py
--rw-r--r--   0        0        0    20146 2024-04-21 22:07:14.263095 miniagents-0.0.6/miniagents/miniagents.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.6/miniagents/promisegraph/__init__.py
--rw-r--r--   0        0        0      563 2024-04-02 17:38:48.000619 miniagents-0.0.6/miniagents/promisegraph/errors.py
--rw-r--r--   0        0        0     3795 2024-04-21 22:07:14.264198 miniagents-0.0.6/miniagents/promisegraph/node.py
--rw-r--r--   0        0        0    18881 2024-04-21 22:07:14.265115 miniagents-0.0.6/miniagents/promisegraph/promise.py
--rw-r--r--   0        0        0      453 2024-04-18 21:45:37.118627 miniagents-0.0.6/miniagents/promisegraph/sentinels.py
--rw-r--r--   0        0        0     1888 2024-04-16 00:22:57.814833 miniagents-0.0.6/miniagents/promisegraph/sequence.py
--rw-r--r--   0        0        0     2219 2024-04-16 00:22:57.815527 miniagents-0.0.6/miniagents/promisegraph/typing.py
--rw-r--r--   0        0        0     2356 2024-04-21 22:07:14.265779 miniagents-0.0.6/miniagents/utils.py
--rw-r--r--   0        0        0      694 2024-04-18 21:52:04.909851 miniagents-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.7/LICENSE
+-rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.7/miniagents/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.7/miniagents/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.7/miniagents/ext/llms/__init__.py
+-rw-r--r--   0        0        0     4364 2024-04-18 21:45:37.115573 miniagents-0.0.7/miniagents/ext/llms/anthropic.py
+-rw-r--r--   0        0        0    20146 2024-04-21 22:07:14.263095 miniagents-0.0.7/miniagents/miniagents.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.726367 miniagents-0.0.7/miniagents/promisegraph/__init__.py
+-rw-r--r--   0        0        0      563 2024-04-02 17:38:48.000619 miniagents-0.0.7/miniagents/promisegraph/errors.py
+-rw-r--r--   0        0        0     3795 2024-04-23 16:28:22.928918 miniagents-0.0.7/miniagents/promisegraph/node.py
+-rw-r--r--   0        0        0    18881 2024-04-21 22:07:14.265115 miniagents-0.0.7/miniagents/promisegraph/promise.py
+-rw-r--r--   0        0        0      453 2024-04-18 21:45:37.118627 miniagents-0.0.7/miniagents/promisegraph/sentinels.py
+-rw-r--r--   0        0        0     1888 2024-04-16 00:22:57.814833 miniagents-0.0.7/miniagents/promisegraph/sequence.py
+-rw-r--r--   0        0        0     2219 2024-04-16 00:22:57.815527 miniagents-0.0.7/miniagents/promisegraph/typing.py
+-rw-r--r--   0        0        0     2356 2024-04-21 22:07:14.265779 miniagents-0.0.7/miniagents/utils.py
+-rw-r--r--   0        0        0      694 2024-04-21 22:16:19.745259 miniagents-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.7/PKG-INFO
```

### Comparing `miniagents-0.0.6/LICENSE` & `miniagents-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.6/miniagents/ext/llms/anthropic.py` & `miniagents-0.0.7/miniagents/ext/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.6/miniagents/miniagents.py` & `miniagents-0.0.7/miniagents/miniagents.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.6/miniagents/promisegraph/errors.py` & `miniagents-0.0.7/miniagents/promisegraph/errors.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.6/miniagents/promisegraph/node.py` & `miniagents-0.0.7/miniagents/promisegraph/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     @cached_property
     def hash_key(self) -> str:
         """
         Get the hash key for this object. It is a hash of the JSON representation of the object.
         """
         hash_key = hashlib.sha256(self.as_json.encode("utf-8")).hexdigest()
         if not PromiseContext.get_current().longer_node_hash_keys:
-            hash_key = hash_key[:32]
+            hash_key = hash_key[:40]
         return hash_key
 
     def serialize_node(self, **model_dump_kwargs) -> dict[str, Any]:
         """
         TODO Oleksandr
         """
         return self.model_dump(**model_dump_kwargs)
```

### Comparing `miniagents-0.0.6/miniagents/promisegraph/promise.py` & `miniagents-0.0.7/miniagents/promisegraph/promise.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.6/miniagents/promisegraph/sequence.py` & `miniagents-0.0.7/miniagents/promisegraph/sequence.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.6/miniagents/promisegraph/typing.py` & `miniagents-0.0.7/miniagents/promisegraph/typing.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.6/miniagents/utils.py` & `miniagents-0.0.7/miniagents/utils.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.6/pyproject.toml` & `miniagents-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 119
 
 [tool.coverage.run]
 branch = true
 
 [tool.poetry]
 name = "miniagents"
-version = "0.0.6"
+version = "0.0.7"
 description = """\
 TODO Oleksandr\
 """
 authors = ["Oleksandr Tereshchenko <toporok@gmail.com>"]
 homepage = "https://github.com/teremterem/MiniAgents"
 readme = "README.md"
 license = "MIT"
```

### Comparing `miniagents-0.0.6/PKG-INFO` & `miniagents-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniagents
-Version: 0.0.6
+Version: 0.0.7
 Summary: TODO Oleksandr
 Home-page: https://github.com/teremterem/MiniAgents
 License: MIT
 Author: Oleksandr Tereshchenko
 Author-email: toporok@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

