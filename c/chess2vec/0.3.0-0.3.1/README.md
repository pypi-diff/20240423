# Comparing `tmp/chess2vec-0.3.0.tar.gz` & `tmp/chess2vec-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess2vec-0.3.0.tar", max compression
+gzip compressed data, was "chess2vec-0.3.1.tar", max compression
```

## Comparing `chess2vec-0.3.0.tar` & `chess2vec-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.0/README.md
--rw-r--r--   0        0        0     4534 2024-04-20 19:18:00.110231 chess2vec-0.3.0/chess2vec/__init__.py
--rw-r--r--   0        0        0      293 2024-04-20 10:13:12.779868 chess2vec-0.3.0/chess2vec/pgn.py
--rw-r--r--   0        0        0        0 2024-04-20 11:20:05.306416 chess2vec-0.3.0/chess2vec/utils/__init__.py
--rw-r--r--   0        0        0     2469 2024-04-20 19:03:02.887784 chess2vec-0.3.0/chess2vec/utils/sparse.py
--rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.0/chess2vec/utils/vector.py
--rw-r--r--   0        0        0     1572 2024-04-20 19:21:27.405707 chess2vec-0.3.0/chess2vec/vectorizers.py
--rw-r--r--   0        0        0      374 2024-04-20 19:25:40.211659 chess2vec-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 chess2vec-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 10:13:12.779868 chess2vec-0.3.1/README.md
+-rw-r--r--   0        0        0     1884 2024-04-23 20:20:37.648701 chess2vec-0.3.1/chess2vec/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-20 10:13:12.779868 chess2vec-0.3.1/chess2vec/pgn.py
+-rw-r--r--   0        0        0      180 2024-04-23 20:20:36.818268 chess2vec-0.3.1/chess2vec/utils/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-20 10:13:12.779868 chess2vec-0.3.1/chess2vec/utils/vector.py
+-rw-r--r--   0        0        0     1246 2024-04-23 20:21:14.401429 chess2vec-0.3.1/chess2vec/vectorizers.py
+-rw-r--r--   0        0        0      401 2024-04-23 20:21:51.053297 chess2vec-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 chess2vec-0.3.1/PKG-INFO
```

### Comparing `chess2vec-0.3.0/chess2vec/utils/vector.py` & `chess2vec-0.3.1/chess2vec/utils/vector.py`

 * *Files identical despite different names*

### Comparing `chess2vec-0.3.0/PKG-INFO` & `chess2vec-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: chess2vec
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Piotr Żarczyński
 Author-email: piotr.zarczynski.06@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chess (>=1.10.0,<2.0.0)
+Requires-Dist: compress-pickle (>=2.1.0,<3.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
```

