# Comparing `tmp/dpack_py-0.1.0.tar.gz` & `tmp/dpack_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpack_py-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dpack_py-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dpack_py-0.1.0.tar` & `dpack_py-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       27 2024-04-22 18:27:21.236302 dpack_py-0.1.0/.gitignore
--rw-r--r--   0        0        0      100 2024-04-22 18:30:45.593747 dpack_py-0.1.0/Makefile
--rw-r--r--   0        0        0     7397 2024-04-22 18:26:09.899181 dpack_py-0.1.0/examples/uniswap-v3.dpack.json
--rw-r--r--   0        0        0     2156 2024-04-22 18:08:54.448859 dpack_py-0.1.0/examples/uniswap.py
--rw-r--r--   0        0        0      555 2024-04-22 18:32:06.574970 dpack_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3065 2024-04-22 18:30:51.299684 dpack_py-0.1.0/readme.md
--rw-r--r--   0        0        0       55 2024-04-22 16:49:07.422511 dpack_py-0.1.0/src/dpack/__init__.py
--rw-r--r--   0        0        0     1150 2024-04-22 17:15:18.488696 dpack_py-0.1.0/src/dpack/ape.py
--rw-r--r--   0        0        0     2861 2024-04-22 18:02:14.112210 dpack_py-0.1.0/src/dpack/dpack.py
--rw-r--r--   0        0        0     2407 2024-04-22 16:52:36.990501 dpack_py-0.1.0/tests/test_dpack.py
--rw-r--r--   0        0        0    10293 2024-04-22 10:38:52.852458 dpack_py-0.1.0/tests/weth-ropsten-artifact.json
--rw-r--r--   0        0        0      723 2024-04-21 07:13:55.705183 dpack_py-0.1.0/tests/weth_ropsten.dpack.json
--rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 dpack_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       27 2024-04-22 18:27:21.236302 dpack_py-0.1.1/.gitignore
+-rw-r--r--   0        0        0      100 2024-04-22 18:30:45.593747 dpack_py-0.1.1/Makefile
+-rw-r--r--   0        0        0     7397 2024-04-22 18:26:09.899181 dpack_py-0.1.1/examples/uniswap-v3.dpack.json
+-rw-r--r--   0        0        0     2156 2024-04-22 18:08:54.448859 dpack_py-0.1.1/examples/uniswap.py
+-rw-r--r--   0        0        0      555 2024-04-22 19:07:15.459183 dpack_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3065 2024-04-22 18:30:51.299684 dpack_py-0.1.1/readme.md
+-rw-r--r--   0        0        0       55 2024-04-22 16:49:07.422511 dpack_py-0.1.1/src/dpack/__init__.py
+-rw-r--r--   0        0        0     1150 2024-04-22 17:15:18.488696 dpack_py-0.1.1/src/dpack/ape.py
+-rw-r--r--   0        0        0     2885 2024-04-22 19:07:37.069606 dpack_py-0.1.1/src/dpack/dpack.py
+-rw-r--r--   0        0        0     2407 2024-04-22 16:52:36.990501 dpack_py-0.1.1/tests/test_dpack.py
+-rw-r--r--   0        0        0    10293 2024-04-22 10:38:52.852458 dpack_py-0.1.1/tests/weth-ropsten-artifact.json
+-rw-r--r--   0        0        0      723 2024-04-21 07:13:55.705183 dpack_py-0.1.1/tests/weth_ropsten.dpack.json
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 dpack_py-0.1.1/PKG-INFO
```

### Comparing `dpack_py-0.1.0/examples/uniswap-v3.dpack.json` & `dpack_py-0.1.1/examples/uniswap-v3.dpack.json`

 * *Files identical despite different names*

### Comparing `dpack_py-0.1.0/examples/uniswap.py` & `dpack_py-0.1.1/examples/uniswap.py`

 * *Files identical despite different names*

### Comparing `dpack_py-0.1.0/pyproject.toml` & `dpack_py-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "dpack-py"
 authors = [{ name = "banteg" }]
 classifiers = ["License :: OSI Approved :: MIT License"]
-version = "0.1.0"
+version = "0.1.1"
 readme = "readme.md"
 description = "dpack is an evm artifact package format"
 requires-python = ">=3.9"
 dependencies = ["pydantic >=2", "httpx", "ethpm-types"]
 
 [tool.flit.module]
 name = "dpack"
```

### Comparing `dpack_py-0.1.0/readme.md` & `dpack_py-0.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `dpack_py-0.1.0/src/dpack/ape.py` & `dpack_py-0.1.1/src/dpack/ape.py`

 * *Files identical despite different names*

### Comparing `dpack_py-0.1.0/src/dpack/dpack.py` & `dpack_py-0.1.1/src/dpack/dpack.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 class DpackType(DpackArtifact):
     typename: constr(pattern=r"[A-Z]\w*")
 
 
 class DpackObject(DpackArtifact):
-    objectname: str
+    objectname: constr(pattern=r"[a-z]\w*")
     address: constr(pattern=r"0x[a-zA-Z0-9]{40}")
     typename: constr(pattern=r"[A-Z]\w*")
 
     @property
     def contract_instance(self):
         return ContractInstance(
             contractType=self.typename, name=self.objectname, address=self.address
```

### Comparing `dpack_py-0.1.0/tests/test_dpack.py` & `dpack_py-0.1.1/tests/test_dpack.py`

 * *Files identical despite different names*

### Comparing `dpack_py-0.1.0/tests/weth-ropsten-artifact.json` & `dpack_py-0.1.1/tests/weth-ropsten-artifact.json`

 * *Files identical despite different names*

### Comparing `dpack_py-0.1.0/tests/weth_ropsten.dpack.json` & `dpack_py-0.1.1/tests/weth_ropsten.dpack.json`

 * *Files identical despite different names*

### Comparing `dpack_py-0.1.0/PKG-INFO` & `dpack_py-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpack-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: dpack is an evm artifact package format
 Author: banteg
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pydantic >=2
 Requires-Dist: httpx
```

