# Comparing `tmp/regex4seq-1.0.0.tar.gz` & `tmp/regex4seq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex4seq-1.0.0.tar", max compression
+gzip compressed data, was "regex4seq-1.0.1.tar", max compression
```

## Comparing `regex4seq-1.0.0.tar` & `regex4seq-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     7652 2023-08-26 15:31:16.190286 regex4seq-1.0.0/LICENSE
--rw-r--r--   0        0        0     1091 2023-09-03 10:25:58.140890 regex4seq-1.0.0/README.md
--rw-r--r--   0        0        0     1127 2023-09-24 09:58:41.701153 regex4seq-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      309 2023-09-24 09:23:47.258135 regex4seq-1.0.0/src/regex4seq/__init__.py
--rw-r--r--   0        0        0    15828 2023-09-24 09:55:29.435822 regex4seq-1.0.0/src/regex4seq/regex4seq.py
--rw-r--r--   0        0        0     1647 2023-09-24 09:32:24.577952 regex4seq-1.0.0/src/regex4seq/trail.py
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 regex4seq-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-08-26 15:31:16.190286 regex4seq-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1091 2023-09-03 10:25:58.140890 regex4seq-1.0.1/README.md
+-rw-r--r--   0        0        0     1127 2024-04-23 19:30:30.395750 regex4seq-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-09-24 09:23:47.258135 regex4seq-1.0.1/src/regex4seq/__init__.py
+-rw-r--r--   0        0        0    15828 2023-09-24 09:55:29.435822 regex4seq-1.0.1/src/regex4seq/regex4seq.py
+-rw-r--r--   0        0        0     1647 2023-09-24 09:32:24.577952 regex4seq-1.0.1/src/regex4seq/trail.py
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 regex4seq-1.0.1/PKG-INFO
```

### Comparing `regex4seq-1.0.0/LICENSE` & `regex4seq-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `regex4seq-1.0.0/README.md` & `regex4seq-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `regex4seq-1.0.0/pyproject.toml` & `regex4seq-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "regex4seq"
-version = "1.0.0"
+version = "1.0.1"
 description = "Regular Expressions for Sequences of Things"
 authors = ["Stephen Leach <sfkleach@gmail.com>"]
 license = "LGPL-3.0-or-later"
 readme = "README.md"
 homepage="https://regex4seq.readthedocs.io/en/latest/"
 documentation="https://regex4seq.readthedocs.io/en/latest/"
 repository = "https://github.com/sfkleach/regex4seq"
```

### Comparing `regex4seq-1.0.0/src/regex4seq/regex4seq.py` & `regex4seq-1.0.1/src/regex4seq/regex4seq.py`

 * *Files identical despite different names*

### Comparing `regex4seq-1.0.0/src/regex4seq/trail.py` & `regex4seq-1.0.1/src/regex4seq/trail.py`

 * *Files identical despite different names*

### Comparing `regex4seq-1.0.0/PKG-INFO` & `regex4seq-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex4seq
-Version: 1.0.0
+Version: 1.0.1
 Summary: Regular Expressions for Sequences of Things
 Home-page: https://regex4seq.readthedocs.io/en/latest/
 License: LGPL-3.0-or-later
 Keywords: regex,regular expressions,pattern matching,sequence matching
 Author: Stephen Leach
 Author-email: sfkleach@gmail.com
 Requires-Python: >=3.10,<4.0
```

