# Comparing `tmp/hj_proj_module-0.1.4.tar.gz` & `tmp/hj_proj_module-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hj_proj_module-0.1.4.tar", max compression
+gzip compressed data, was "hj_proj_module-0.1.5.tar", max compression
```

## Comparing `hj_proj_module-0.1.4.tar` & `hj_proj_module-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       41 2024-04-22 14:02:59.728906 hj_proj_module-0.1.4/README.md
--rw-r--r--   0        0        0       37 2024-04-22 14:04:24.568783 hj_proj_module-0.1.4/hj_proj_module/__init__.py
--rw-r--r--   0        0        0       44 2024-04-22 14:04:24.568911 hj_proj_module-0.1.4/hj_proj_module/my_function.py
--rw-r--r--   0        0        0      761 2024-04-22 14:42:25.271047 hj_proj_module-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 hj_proj_module-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      129 2024-04-22 14:43:35.282517 hj_proj_module-0.1.5/README.md
+-rw-r--r--   0        0        0       37 2024-04-22 14:04:24.568783 hj_proj_module-0.1.5/hj_proj_module/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-22 14:04:24.568911 hj_proj_module-0.1.5/hj_proj_module/my_function.py
+-rw-r--r--   0        0        0      761 2024-04-22 14:43:38.822411 hj_proj_module-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 hj_proj_module-0.1.5/PKG-INFO
```

### Comparing `hj_proj_module-0.1.4/pyproject.toml` & `hj_proj_module-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hj-proj-module"
-version = "0.1.4"
+version = "0.1.5"
 description = "Packages for HJ Projects"
 authors = ["Hojung Yun <hojung.yun@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/hj12121/hj-proj-module"
 repository = "https://github.com/hj12121/hj-proj-module"
 keywords = ["HJ"]
```

### Comparing `hj_proj_module-0.1.4/PKG-INFO` & `hj_proj_module-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hj-proj-module
-Version: 0.1.4
+Version: 0.1.5
 Summary: Packages for HJ Projects
 Home-page: https://github.com/hj12121/hj-proj-module
 License: MIT
 Keywords: HJ
 Author: Hojung Yun
 Author-email: hojung.yun@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -20,7 +20,10 @@
 Description-Content-Type: text/markdown
 
 # Test
 ```
 poetry add hj-proj-module
 ```
 
+https://pypi.org/project/hj-proj-module/
+https://test.pypi.org/project/hj-proj-module/
+
```

