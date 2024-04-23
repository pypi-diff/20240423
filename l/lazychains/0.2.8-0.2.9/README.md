# Comparing `tmp/lazychains-0.2.8.tar.gz` & `tmp/lazychains-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazychains-0.2.8.tar", max compression
+gzip compressed data, was "lazychains-0.2.9.tar", max compression
```

## Comparing `lazychains-0.2.8.tar` & `lazychains-0.2.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-01-31 13:05:09.524900 lazychains-0.2.8/LICENSE
--rw-r--r--   0        0        0     2255 2023-05-26 15:19:16.004792 lazychains-0.2.8/README.md
--rw-r--r--   0        0        0     1056 2023-08-19 09:17:50.285299 lazychains-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       50 2023-01-31 13:05:09.530665 lazychains-0.2.8/src/lazychains/__init__.py
--rw-r--r--   0        0        0    12570 2023-05-26 15:19:16.008942 lazychains-0.2.8/src/lazychains/lazychains.py
--rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 lazychains-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-31 13:05:09.524900 lazychains-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2255 2023-05-26 15:19:16.004792 lazychains-0.2.9/README.md
+-rw-r--r--   0        0        0     1056 2023-10-03 11:33:54.634261 lazychains-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-01-31 13:05:09.530665 lazychains-0.2.9/src/lazychains/__init__.py
+-rw-r--r--   0        0        0    12570 2023-05-26 15:19:16.008942 lazychains-0.2.9/src/lazychains/lazychains.py
+-rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 lazychains-0.2.9/PKG-INFO
```

### Comparing `lazychains-0.2.8/LICENSE` & `lazychains-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lazychains-0.2.8/README.md` & `lazychains-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `lazychains-0.2.8/pyproject.toml` & `lazychains-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazychains"
-version = "0.2.8"
+version = "0.2.9"
 description = "Singly linked lists with incremental instantiation of iterators"
 authors = ["Stephen Leach <sfkleach@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme="README.md"
 homepage="https://lazychains.readthedocs.io/en/latest/"
 documentation="https://lazychains.readthedocs.io/en/latest/"
 repository = "https://github.com/sfkleach/lazychains"
```

### Comparing `lazychains-0.2.8/src/lazychains/lazychains.py` & `lazychains-0.2.9/src/lazychains/lazychains.py`

 * *Files identical despite different names*

### Comparing `lazychains-0.2.8/PKG-INFO` & `lazychains-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazychains
-Version: 0.2.8
+Version: 0.2.9
 Summary: Singly linked lists with incremental instantiation of iterators
 Home-page: https://lazychains.readthedocs.io/en/latest/
 License: GPL-3.0-or-later
 Keywords: iterators,linked list,single,lazy
 Author: Stephen Leach
 Author-email: sfkleach@gmail.com
 Requires-Python: >=3.10,<4.0
```

