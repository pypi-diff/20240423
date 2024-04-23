# Comparing `tmp/cognite_synthetic_tags-0.5.1.tar.gz` & `tmp/cognite_synthetic_tags-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_synthetic_tags-0.5.1.tar", max compression
+gzip compressed data, was "cognite_synthetic_tags-0.5.2.tar", max compression
```

## Comparing `cognite_synthetic_tags-0.5.1.tar` & `cognite_synthetic_tags-0.5.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      154 2024-04-22 01:12:20.308128 cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/__init__.py
--rw-r--r--   0        0        0     1818 2024-04-22 01:12:20.308128 cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/_operations.py
--rw-r--r--   0        0        0     2568 2024-04-22 01:12:20.308128 cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/data_stores.py
--rw-r--r--   0        0        0     5535 2024-04-22 01:12:20.308128 cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/tag.py
--rw-r--r--   0        0        0    12204 2024-04-22 01:12:20.312128 cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/tag_resolver.py
--rw-r--r--   0        0        0     1046 2024-04-22 01:12:20.312128 cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/types.py
--rw-r--r--   0        0        0     1083 2024-04-22 01:12:20.312128 cognite_synthetic_tags-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 cognite_synthetic_tags-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      154 2024-04-23 11:09:23.313441 cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/__init__.py
+-rw-r--r--   0        0        0     1818 2024-04-23 11:09:23.313441 cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/_operations.py
+-rw-r--r--   0        0        0     2830 2024-04-23 11:09:23.313441 cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/data_stores.py
+-rw-r--r--   0        0        0     5535 2024-04-23 11:09:23.313441 cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/tag.py
+-rw-r--r--   0        0        0    12204 2024-04-23 11:09:23.313441 cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/tag_resolver.py
+-rw-r--r--   0        0        0     1046 2024-04-23 11:09:23.313441 cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/types.py
+-rw-r--r--   0        0        0     1083 2024-04-23 11:09:23.313441 cognite_synthetic_tags-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 cognite_synthetic_tags-0.5.2/PKG-INFO
```

### Comparing `cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/_operations.py` & `cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/_operations.py`

 * *Files identical despite different names*

### Comparing `cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/data_stores.py` & `cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/data_stores.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,20 +33,26 @@
 
     @abc.abstractmethod
     def _fetch(self, external_ids): ...  # pragma: no cover
 
     @abc.abstractmethod
     def _process(self, raw, external_ids): ...  # pragma: no cover
 
-    def preprocess(self, func):
-        self._preprocess_funcs.append(func)
+    def preprocess(self, func, *args, **kwargs):
+        def _callback(args, kwargs):
+            return lambda res: func(res, *args, **kwargs)
+
+        self._preprocess_funcs.append(_callback(args, kwargs))
         return self
 
-    def process(self, func):
-        self._process_funcs.append(func)
+    def process(self, func, *args, **kwargs):
+        def _callback(args, kwargs):
+            return lambda df: func(df, *args, **kwargs)
+
+        self._process_funcs.append(_callback(args, kwargs))
         return self
 
 
 class CDFStore(Store):
     fill_with = np.nan
 
     def _fetch(self, external_ids):
```

### Comparing `cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/tag.py` & `cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/tag.py`

 * *Files identical despite different names*

### Comparing `cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/tag_resolver.py` & `cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/tag_resolver.py`

 * *Files identical despite different names*

### Comparing `cognite_synthetic_tags-0.5.1/cognite_synthetic_tags/types.py` & `cognite_synthetic_tags-0.5.2/cognite_synthetic_tags/types.py`

 * *Files identical despite different names*

### Comparing `cognite_synthetic_tags-0.5.1/pyproject.toml` & `cognite_synthetic_tags-0.5.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite_synthetic_tags"
-version = "0.5.1"
+version = "0.5.2"
 description = "Framework for working easily with tags, synthetic and regular, from Cognite Data Fusion (CDF) API."
 authors = ["Fran Hrzenjak <fran.hrzenjak@cognite.com>"]
 license = "Apache License 2.0"
 
 [tool.black]
 line-length = 80
```

### Comparing `cognite_synthetic_tags-0.5.1/PKG-INFO` & `cognite_synthetic_tags-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite_synthetic_tags
-Version: 0.5.1
+Version: 0.5.2
 Summary: Framework for working easily with tags, synthetic and regular, from Cognite Data Fusion (CDF) API.
 License: Apache-2.0
 Author: Fran Hrzenjak
 Author-email: fran.hrzenjak@cognite.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

