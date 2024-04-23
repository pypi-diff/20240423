# Comparing `tmp/synthx-0.4.1.tar.gz` & `tmp/synthx-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthx-0.4.1.tar", max compression
+gzip compressed data, was "synthx-0.4.2.tar", max compression
```

## Comparing `synthx-0.4.1.tar` & `synthx-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7539 2024-04-22 16:29:16.621447 synthx-0.4.1/README.md
--rw-r--r--   0        0        0     1270 2024-04-22 16:29:16.622599 synthx-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-0.4.1/synthx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-0.4.1/synthx/core/__init__.py
--rw-r--r--   0        0        0     7302 2024-04-18 01:31:14.755205 synthx-0.4.1/synthx/core/dataset.py
--rw-r--r--   0        0        0     4718 2024-03-25 05:07:58.244991 synthx-0.4.1/synthx/core/result.py
--rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-0.4.1/synthx/core/sample.py
--rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-0.4.1/synthx/errors/__init__.py
--rw-r--r--   0        0        0    10228 2024-04-22 16:15:26.237819 synthx-0.4.1/synthx/method.py
--rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-0.4.1/synthx/stats/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-0.4.1/synthx/stats/norm.py
--rw-r--r--   0        0        0     1026 2024-03-25 05:14:52.967319 synthx-0.4.1/synthx/stats/p.py
--rw-r--r--   0        0        0     8323 1970-01-01 00:00:00.000000 synthx-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     7539 2024-04-22 16:29:44.049795 synthx-0.4.2/README.md
+-rw-r--r--   0        0        0     1270 2024-04-22 17:17:05.375623 synthx-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-0.4.2/synthx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-0.4.2/synthx/core/__init__.py
+-rw-r--r--   0        0        0     7302 2024-04-18 01:31:14.755205 synthx-0.4.2/synthx/core/dataset.py
+-rw-r--r--   0        0        0     4718 2024-03-25 05:07:58.244991 synthx-0.4.2/synthx/core/result.py
+-rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-0.4.2/synthx/core/sample.py
+-rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-0.4.2/synthx/errors/__init__.py
+-rw-r--r--   0        0        0    10232 2024-04-22 17:17:05.375947 synthx-0.4.2/synthx/method.py
+-rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-0.4.2/synthx/stats/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-0.4.2/synthx/stats/norm.py
+-rw-r--r--   0        0        0     1026 2024-03-25 05:14:52.967319 synthx-0.4.2/synthx/stats/p.py
+-rw-r--r--   0        0        0     8323 1970-01-01 00:00:00.000000 synthx-0.4.2/PKG-INFO
```

### Comparing `synthx-0.4.1/README.md` & `synthx-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `synthx-0.4.1/pyproject.toml` & `synthx-0.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synthx"
-version = "0.4.1"
+version = "0.4.2"
 description = "A Python Library for Advanced Synthetic Control Analysis"
 authors = ["kenki931128 <kenki.nkmr@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `synthx-0.4.1/synthx/core/dataset.py` & `synthx-0.4.2/synthx/core/dataset.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.1/synthx/core/result.py` & `synthx-0.4.2/synthx/core/result.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.1/synthx/core/sample.py` & `synthx-0.4.2/synthx/core/sample.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.1/synthx/errors/__init__.py` & `synthx-0.4.2/synthx/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.1/synthx/method.py` & `synthx-0.4.2/synthx/method.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,12 +238,12 @@
             tqdm.write(
                 f'sensitivity synthetic control optimization failed: uplift {uplift}.',
                 file=sys.stderr,
             )
             continue
 
         p_value = sx.stats.calc_p_value(sc.estimate_effects(), effects_placebo)
-        tqdm.write(f'uplift: {uplift}, p value: {p_value}.', file=sys.stderr)
+        tqdm.write(f'uplift: {uplift:.2f}, p value: {p_value}.', file=sys.stderr)
         if p_value <= p_value_target:
             return uplift
 
     return None
```

### Comparing `synthx-0.4.1/synthx/stats/norm.py` & `synthx-0.4.2/synthx/stats/norm.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.1/synthx/stats/p.py` & `synthx-0.4.2/synthx/stats/p.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.1/PKG-INFO` & `synthx-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthx
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python Library for Advanced Synthetic Control Analysis
 License: MIT
 Author: kenki931128
 Author-email: kenki.nkmr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

