# Comparing `tmp/synthx-0.4.2.tar.gz` & `tmp/synthx-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synthx-0.4.2.tar", max compression
+gzip compressed data, was "synthx-0.4.3.tar", max compression
```

## Comparing `synthx-0.4.2.tar` & `synthx-0.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7539 2024-04-22 16:29:44.049795 synthx-0.4.2/README.md
--rw-r--r--   0        0        0     1270 2024-04-22 17:17:05.375623 synthx-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-0.4.2/synthx/__init__.py
--rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-0.4.2/synthx/core/__init__.py
--rw-r--r--   0        0        0     7302 2024-04-18 01:31:14.755205 synthx-0.4.2/synthx/core/dataset.py
--rw-r--r--   0        0        0     4718 2024-03-25 05:07:58.244991 synthx-0.4.2/synthx/core/result.py
--rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-0.4.2/synthx/core/sample.py
--rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-0.4.2/synthx/errors/__init__.py
--rw-r--r--   0        0        0    10232 2024-04-22 17:17:05.375947 synthx-0.4.2/synthx/method.py
--rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-0.4.2/synthx/stats/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-0.4.2/synthx/stats/norm.py
--rw-r--r--   0        0        0     1026 2024-03-25 05:14:52.967319 synthx-0.4.2/synthx/stats/p.py
--rw-r--r--   0        0        0     8323 1970-01-01 00:00:00.000000 synthx-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     7539 2024-04-22 16:29:44.049795 synthx-0.4.3/README.md
+-rw-r--r--   0        0        0     1270 2024-04-23 01:39:44.139362 synthx-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-22 16:15:26.237522 synthx-0.4.3/synthx/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-24 06:28:58.858654 synthx-0.4.3/synthx/core/__init__.py
+-rw-r--r--   0        0        0     7302 2024-04-18 01:31:14.755205 synthx-0.4.3/synthx/core/dataset.py
+-rw-r--r--   0        0        0     4718 2024-03-25 05:07:58.244991 synthx-0.4.3/synthx/core/result.py
+-rw-r--r--   0        0        0     7362 2024-04-22 16:14:41.909807 synthx-0.4.3/synthx/core/sample.py
+-rw-r--r--   0        0        0      818 2024-04-18 01:31:14.755622 synthx-0.4.3/synthx/errors/__init__.py
+-rw-r--r--   0        0        0    10394 2024-04-23 01:39:44.139643 synthx-0.4.3/synthx/method.py
+-rw-r--r--   0        0        0       91 2024-03-25 05:14:52.967139 synthx-0.4.3/synthx/stats/__init__.py
+-rw-r--r--   0        0        0     1802 2024-04-18 01:31:14.755779 synthx-0.4.3/synthx/stats/norm.py
+-rw-r--r--   0        0        0     1026 2024-03-25 05:14:52.967319 synthx-0.4.3/synthx/stats/p.py
+-rw-r--r--   0        0        0     8323 1970-01-01 00:00:00.000000 synthx-0.4.3/PKG-INFO
```

### Comparing `synthx-0.4.2/README.md` & `synthx-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `synthx-0.4.2/pyproject.toml` & `synthx-0.4.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synthx"
-version = "0.4.2"
+version = "0.4.3"
 description = "A Python Library for Advanced Synthetic Control Analysis"
 authors = ["kenki931128 <kenki.nkmr@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `synthx-0.4.2/synthx/core/dataset.py` & `synthx-0.4.3/synthx/core/dataset.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.2/synthx/core/result.py` & `synthx-0.4.3/synthx/core/result.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.2/synthx/core/sample.py` & `synthx-0.4.3/synthx/core/sample.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.2/synthx/errors/__init__.py` & `synthx-0.4.3/synthx/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.2/synthx/method.py` & `synthx-0.4.3/synthx/method.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,15 +207,18 @@
         p_value_target (float, optional): The target p-value threshold for statistical significance.
 
     Returns:
         float or None: The uplift which becomes statistically significant.
     """
     df = dataset.data
 
-    for uplift in tqdm(np.arange(1, 3, 0.01)):
+    l, r = 1.0, 10.0
+    while r - l > 0.001:
+        uplift = (l + r) / 2
+
         df_sensitivity = df.with_columns(
             pl.when(
                 pl.col(dataset.unit_column).is_in(dataset.intervention_units)
                 & (pl.col(dataset.time_column) >= dataset.intervention_time)
             )
             .then(pl.col(dataset.y_column) * uplift)
             .otherwise(pl.col(dataset.y_column))
@@ -231,19 +234,24 @@
             intervention_units=dataset.intervention_units,
             intervention_time=dataset.intervention_time,
         )
 
         try:
             sc = synthetic_control(dataset_sensitivity)
         except NoFeasibleModelError:
-            tqdm.write(
-                f'sensitivity synthetic control optimization failed: uplift {uplift}.',
-                file=sys.stderr,
-            )
+            r = uplift  # highly likely uplift was too big. TODO: think better algorithm.
             continue
 
         p_value = sx.stats.calc_p_value(sc.estimate_effects(), effects_placebo)
-        tqdm.write(f'uplift: {uplift:.2f}, p value: {p_value}.', file=sys.stderr)
         if p_value <= p_value_target:
-            return uplift
-
-    return None
+            r = uplift
+        else:
+            tqdm.write(f'uplift: {uplift:.4f}, p value: {p_value}.', file=sys.stderr)
+            l = uplift
+
+    # even 1000% uplift cannot be captured.
+    if r == 10:
+        return None
+    # singnificant difference without actual uplift
+    if l == 1:
+        return None
+    return r
```

### Comparing `synthx-0.4.2/synthx/stats/norm.py` & `synthx-0.4.3/synthx/stats/norm.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.2/synthx/stats/p.py` & `synthx-0.4.3/synthx/stats/p.py`

 * *Files identical despite different names*

### Comparing `synthx-0.4.2/PKG-INFO` & `synthx-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synthx
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python Library for Advanced Synthetic Control Analysis
 License: MIT
 Author: kenki931128
 Author-email: kenki.nkmr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

