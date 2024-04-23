# Comparing `tmp/ommx-0.1.1.tar.gz` & `tmp/ommx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ommx-0.1.1.tar", last modified: Mon Apr 22 01:32:30 2024, max compression
+gzip compressed data, was "ommx-0.2.0.tar", last modified: Tue Apr 23 07:01:09 2024, max compression
```

## Comparing `ommx-0.1.1.tar` & `ommx-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:30.541496 ommx-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-22 01:32:24.000000 ommx-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-22 01:32:30.541496 ommx-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-22 01:32:24.000000 ommx-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:30.537496 ommx-0.1.1/ommx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:30.541496 ommx-0.1.1/ommx/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/constraint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/constraint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/decision_variables_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/decision_variables_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/function_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/instance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/instance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/linear_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/linear_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/polynomial_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/polynomial_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/quadratic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/quadratic_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/solution_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/solution_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-22 01:32:24.000000 ommx-0.1.1/ommx/v1/sparse_matrix_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 01:32:30.541496 ommx-0.1.1/ommx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-22 01:32:30.000000 ommx-0.1.1/ommx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-22 01:32:30.000000 ommx-0.1.1/ommx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 01:32:30.000000 ommx-0.1.1/ommx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 01:32:30.000000 ommx-0.1.1/ommx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 01:32:30.000000 ommx-0.1.1/ommx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-22 01:32:24.000000 ommx-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 01:32:30.541496 ommx-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:09.256428 ommx-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 07:01:03.000000 ommx-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-23 07:01:09.256428 ommx-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-23 07:01:03.000000 ommx-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:09.248428 ommx-0.2.0/ommx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:09.252428 ommx-0.2.0/ommx/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/constraint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/constraint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/decision_variables_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/decision_variables_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/instance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/instance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/linear_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/linear_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/polynomial_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/polynomial_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/quadratic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/quadratic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/solution_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/solution_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-23 07:01:03.000000 ommx-0.2.0/ommx/v1/sparse_matrix_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:01:09.252428 ommx-0.2.0/ommx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-23 07:01:09.000000 ommx-0.2.0/ommx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-23 07:01:09.000000 ommx-0.2.0/ommx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:01:09.000000 ommx-0.2.0/ommx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 07:01:09.000000 ommx-0.2.0/ommx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-23 07:01:09.000000 ommx-0.2.0/ommx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-23 07:01:03.000000 ommx-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 07:01:09.256428 ommx-0.2.0/setup.cfg
```

### Comparing `ommx-0.1.1/PKG-INFO` & `ommx-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ommx
-Version: 0.1.1
+Version: 0.2.0
 Summary: Open Mathematical prograMming eXchange (OMMX)
 Author-email: "Jij Inc." <info@j-ij.com>
 Project-URL: Homepage, https://github.com/Jij-Inc/ommx
 Project-URL: Issues, https://github.com/Jij-Inc/ommx/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ommx-0.1.1/README.md` & `ommx-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/testing.py` & `ommx-0.2.0/ommx/testing.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/constraint_pb2.py` & `ommx-0.2.0/ommx/v1/constraint_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/constraint_pb2.pyi` & `ommx-0.2.0/ommx/v1/constraint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/decision_variables_pb2.py` & `ommx-0.2.0/ommx/v1/decision_variables_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/decision_variables_pb2.pyi` & `ommx-0.2.0/ommx/v1/decision_variables_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/function_pb2.py` & `ommx-0.2.0/ommx/v1/function_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/function_pb2.pyi` & `ommx-0.2.0/ommx/v1/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/instance_pb2.py` & `ommx-0.2.0/ommx/v1/instance_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 
 
 from ommx.v1 import constraint_pb2 as ommx_dot_v1_dot_constraint__pb2
 from ommx.v1 import decision_variables_pb2 as ommx_dot_v1_dot_decision__variables__pb2
 from ommx.v1 import function_pb2 as ommx_dot_v1_dot_function__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16ommx/v1/instance.proto\x12\x07ommx.v1\x1a\x18ommx/v1/constraint.proto\x1a ommx/v1/decision_variables.proto\x1a\x16ommx/v1/function.proto\"\xb3\x03\n\x08Instance\x12?\n\x0b\x64\x65scription\x18\x01 \x01(\x0b\x32\x1d.ommx.v1.Instance.DescriptionR\x0b\x64\x65scription\x12H\n\x12\x64\x65\x63ision_variables\x18\x02 \x03(\x0b\x32\x19.ommx.v1.DecisionVariableR\x11\x64\x65\x63isionVariables\x12/\n\tobjective\x18\x03 \x01(\x0b\x32\x11.ommx.v1.FunctionR\tobjective\x12\x35\n\x0b\x63onstraints\x18\x04 \x03(\x0b\x32\x13.ommx.v1.ConstraintR\x0b\x63onstraints\x1a\xb3\x01\n\x0b\x44\x65scription\x12\x17\n\x04name\x18\x01 \x01(\tH\x00R\x04name\x88\x01\x01\x12%\n\x0b\x64\x65scription\x18\x02 \x01(\tH\x01R\x0b\x64\x65scription\x88\x01\x01\x12\x18\n\x07\x61uthors\x18\x03 \x03(\tR\x07\x61uthors\x12\"\n\ncreated_by\x18\x04 \x01(\tH\x02R\tcreatedBy\x88\x01\x01\x42\x07\n\x05_nameB\x0e\n\x0c_descriptionB\r\n\x0b_created_byBY\n\x0b\x63om.ommx.v1B\rInstanceProtoP\x01\xa2\x02\x03OXX\xaa\x02\x07Ommx.V1\xca\x02\x07Ommx\\V1\xe2\x02\x13Ommx\\V1\\GPBMetadata\xea\x02\x08Ommx::V1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16ommx/v1/instance.proto\x12\x07ommx.v1\x1a\x18ommx/v1/constraint.proto\x1a ommx/v1/decision_variables.proto\x1a\x16ommx/v1/function.proto\"\xaa\x04\n\x08Instance\x12?\n\x0b\x64\x65scription\x18\x01 \x01(\x0b\x32\x1d.ommx.v1.Instance.DescriptionR\x0b\x64\x65scription\x12H\n\x12\x64\x65\x63ision_variables\x18\x02 \x03(\x0b\x32\x19.ommx.v1.DecisionVariableR\x11\x64\x65\x63isionVariables\x12/\n\tobjective\x18\x03 \x01(\x0b\x32\x11.ommx.v1.FunctionR\tobjective\x12\x35\n\x0b\x63onstraints\x18\x04 \x03(\x0b\x32\x13.ommx.v1.ConstraintR\x0b\x63onstraints\x12-\n\x05sense\x18\x05 \x01(\x0e\x32\x17.ommx.v1.Instance.SenseR\x05sense\x1a\xb3\x01\n\x0b\x44\x65scription\x12\x17\n\x04name\x18\x01 \x01(\tH\x00R\x04name\x88\x01\x01\x12%\n\x0b\x64\x65scription\x18\x02 \x01(\tH\x01R\x0b\x64\x65scription\x88\x01\x01\x12\x18\n\x07\x61uthors\x18\x03 \x03(\tR\x07\x61uthors\x12\"\n\ncreated_by\x18\x04 \x01(\tH\x02R\tcreatedBy\x88\x01\x01\x42\x07\n\x05_nameB\x0e\n\x0c_descriptionB\r\n\x0b_created_by\"F\n\x05Sense\x12\x15\n\x11SENSE_UNSPECIFIED\x10\x00\x12\x12\n\x0eSENSE_MINIMIZE\x10\x01\x12\x12\n\x0eSENSE_MAXIMIZE\x10\x02\x42Y\n\x0b\x63om.ommx.v1B\rInstanceProtoP\x01\xa2\x02\x03OXX\xaa\x02\x07Ommx.V1\xca\x02\x07Ommx\\V1\xe2\x02\x13Ommx\\V1\\GPBMetadata\xea\x02\x08Ommx::V1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ommx.v1.instance_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n\013com.ommx.v1B\rInstanceProtoP\001\242\002\003OXX\252\002\007Ommx.V1\312\002\007Ommx\\V1\342\002\023Ommx\\V1\\GPBMetadata\352\002\010Ommx::V1'
   _globals['_INSTANCE']._serialized_start=120
-  _globals['_INSTANCE']._serialized_end=555
-  _globals['_INSTANCE_DESCRIPTION']._serialized_start=376
-  _globals['_INSTANCE_DESCRIPTION']._serialized_end=555
+  _globals['_INSTANCE']._serialized_end=674
+  _globals['_INSTANCE_DESCRIPTION']._serialized_start=423
+  _globals['_INSTANCE_DESCRIPTION']._serialized_end=602
+  _globals['_INSTANCE_SENSE']._serialized_start=604
+  _globals['_INSTANCE_SENSE']._serialized_end=674
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ommx-0.1.1/ommx/v1/linear_pb2.py` & `ommx-0.2.0/ommx/v1/linear_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/linear_pb2.pyi` & `ommx-0.2.0/ommx/v1/linear_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/polynomial_pb2.py` & `ommx-0.2.0/ommx/v1/polynomial_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/polynomial_pb2.pyi` & `ommx-0.2.0/ommx/v1/polynomial_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/quadratic_pb2.py` & `ommx-0.2.0/ommx/v1/quadratic_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/quadratic_pb2.pyi` & `ommx-0.2.0/ommx/v1/quadratic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/solution_pb2.py` & `ommx-0.2.0/ommx/v1/solution_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/solution_pb2.pyi` & `ommx-0.2.0/ommx/v1/solution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx/v1/sparse_matrix_pb2.py` & `ommx-0.2.0/ommx/v1/sparse_matrix_pb2.py`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/ommx.egg-info/PKG-INFO` & `ommx-0.2.0/ommx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ommx
-Version: 0.1.1
+Version: 0.2.0
 Summary: Open Mathematical prograMming eXchange (OMMX)
 Author-email: "Jij Inc." <info@j-ij.com>
 Project-URL: Homepage, https://github.com/Jij-Inc/ommx
 Project-URL: Issues, https://github.com/Jij-Inc/ommx/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ommx-0.1.1/ommx.egg-info/SOURCES.txt` & `ommx-0.2.0/ommx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ommx-0.1.1/pyproject.toml` & `ommx-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ommx"
-version = "0.1.1"
+version = "0.2.0"
 description = "Open Mathematical prograMming eXchange (OMMX)"
 authors = [
     { name="Jij Inc.", email="info@j-ij.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

