# Comparing `tmp/astarte_message_hub_proto-0.6.1.tar.gz` & `tmp/astarte_message_hub_proto-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astarte_message_hub_proto-0.6.1.tar", last modified: Thu Dec 21 12:23:50 2023, max compression
+gzip compressed data, was "astarte_message_hub_proto-0.6.2.tar", last modified: Tue Apr 23 10:23:24 2024, max compression
```

## Comparing `astarte_message_hub_proto-0.6.1.tar` & `astarte_message_hub_proto-0.6.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:23:50.505942 astarte_message_hub_proto-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-12-21 12:23:50.505942 astarte_message_hub_proto-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:23:50.501942 astarte_message_hub_proto-0.6.1/astarte_message_hub_proto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-12-21 12:23:50.000000 astarte_message_hub_proto-0.6.1/astarte_message_hub_proto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-21 12:23:50.000000 astarte_message_hub_proto-0.6.1/astarte_message_hub_proto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 12:23:50.000000 astarte_message_hub_proto-0.6.1/astarte_message_hub_proto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-21 12:23:50.000000 astarte_message_hub_proto-0.6.1/astarte_message_hub_proto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-21 12:23:50.000000 astarte_message_hub_proto-0.6.1/astarte_message_hub_proto.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:23:50.497942 astarte_message_hub_proto-0.6.1/astarteplatform/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 12:23:50.501942 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/astarte_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/astarte_message_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/astarte_message_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/astarte_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/astarte_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/astarte_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/message_hub_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/message_hub_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/message_hub_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/node_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/node_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/astarteplatform/msghub/node_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-12-21 12:23:38.000000 astarte_message_hub_proto-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 12:23:50.505942 astarte_message_hub_proto-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:23:24.931697 astarte_message_hub_proto-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-23 10:23:24.931697 astarte_message_hub_proto-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:23:24.931697 astarte_message_hub_proto-0.6.2/astarte_message_hub_proto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-23 10:23:24.000000 astarte_message_hub_proto-0.6.2/astarte_message_hub_proto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-23 10:23:24.000000 astarte_message_hub_proto-0.6.2/astarte_message_hub_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 10:23:24.000000 astarte_message_hub_proto-0.6.2/astarte_message_hub_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 10:23:24.000000 astarte_message_hub_proto-0.6.2/astarte_message_hub_proto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 10:23:24.000000 astarte_message_hub_proto-0.6.2/astarte_message_hub_proto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:23:24.927696 astarte_message_hub_proto-0.6.2/astarteplatform/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 10:23:24.931697 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/astarte_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/astarte_message_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/astarte_message_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/astarte_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/astarte_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/astarte_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/message_hub_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/message_hub_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/message_hub_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/node_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/node_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/astarteplatform/msghub/node_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-23 10:23:19.000000 astarte_message_hub_proto-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 10:23:24.931697 astarte_message_hub_proto-0.6.2/setup.cfg
```

### Comparing `astarte_message_hub_proto-0.6.1/PKG-INFO` & `astarte_message_hub_proto-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astarte_message_hub_proto
-Version: 0.6.1
+Version: 0.6.2
 Summary: Astarte message hub protocol buffers for Python
 Author-email: Simone Orru <simone.orru@secomind.com>
 Project-URL: Source, https://github.com/astarte-platform/astarte-message-hub-proto
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: grpcio
```

### Comparing `astarte_message_hub_proto-0.6.1/README.md` & `astarte_message_hub_proto-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `astarte_message_hub_proto-0.6.1/astarte_message_hub_proto.egg-info/PKG-INFO` & `astarte_message_hub_proto-0.6.2/astarte_message_hub_proto.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: astarte-message-hub-proto
-Version: 0.6.1
+Name: astarte_message_hub_proto
+Version: 0.6.2
 Summary: Astarte message hub protocol buffers for Python
 Author-email: Simone Orru <simone.orru@secomind.com>
 Project-URL: Source, https://github.com/astarte-platform/astarte-message-hub-proto
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: grpcio
```

### Comparing `astarte_message_hub_proto-0.6.1/astarte_message_hub_proto.egg-info/SOURCES.txt` & `astarte_message_hub_proto-0.6.2/astarte_message_hub_proto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/astarte_message_pb2.py` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/astarte_message_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: astarteplatform/msghub/astarte_message.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,14 +17,14 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,astarteplatform/msghub/astarte_message.proto\x12\x16\x61starteplatform.msghub\x1a\x1fgoogle/protobuf/timestamp.proto\x1a)astarteplatform/msghub/astarte_type.proto\"\xf0\x01\n\x0e\x41starteMessage\x12\x16\n\x0einterface_name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12?\n\x0c\x61starte_data\x18\x03 \x01(\x0b\x32\'.astarteplatform.msghub.AstarteDataTypeH\x00\x12=\n\rastarte_unset\x18\x04 \x01(\x0b\x32$.astarteplatform.msghub.AstarteUnsetH\x00\x12-\n\ttimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\t\n\x07payload\"\x0e\n\x0c\x41starteUnsetb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'astarteplatform.msghub.astarte_message_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_ASTARTEMESSAGE']._serialized_start=149
   _globals['_ASTARTEMESSAGE']._serialized_end=389
   _globals['_ASTARTEUNSET']._serialized_start=391
   _globals['_ASTARTEUNSET']._serialized_end=405
 # @@protoc_insertion_point(module_scope)
```

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/astarte_message_pb2.pyi` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/astarte_message_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class AstarteMessage(_message.Message):
-    __slots__ = ["interface_name", "path", "astarte_data", "astarte_unset", "timestamp"]
+    __slots__ = ("interface_name", "path", "astarte_data", "astarte_unset", "timestamp")
     INTERFACE_NAME_FIELD_NUMBER: _ClassVar[int]
     PATH_FIELD_NUMBER: _ClassVar[int]
     ASTARTE_DATA_FIELD_NUMBER: _ClassVar[int]
     ASTARTE_UNSET_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     interface_name: str
     path: str
     astarte_data: _astarte_type_pb2.AstarteDataType
     astarte_unset: AstarteUnset
     timestamp: _timestamp_pb2.Timestamp
     def __init__(self, interface_name: _Optional[str] = ..., path: _Optional[str] = ..., astarte_data: _Optional[_Union[_astarte_type_pb2.AstarteDataType, _Mapping]] = ..., astarte_unset: _Optional[_Union[AstarteUnset, _Mapping]] = ..., timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
 class AstarteUnset(_message.Message):
-    __slots__ = []
+    __slots__ = ()
     def __init__(self) -> None: ...
```

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/astarte_type_pb2.py` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/astarte_type_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: astarteplatform/msghub/astarte_type.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,17 +16,17 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)astarteplatform/msghub/astarte_type.proto\x12\x16\x61starteplatform.msghub\x1a\x1fgoogle/protobuf/timestamp.proto\"$\n\x12\x41starteDoubleArray\x12\x0e\n\x06values\x18\x01 \x03(\x01\"%\n\x13\x41starteIntegerArray\x12\x0e\n\x06values\x18\x01 \x03(\x05\"%\n\x13\x41starteBooleanArray\x12\x0e\n\x06values\x18\x01 \x03(\x08\")\n\x17\x41starteLongIntegerArray\x12\x0e\n\x06values\x18\x01 \x03(\x03\"$\n\x12\x41starteStringArray\x12\x0e\n\x06values\x18\x01 \x03(\t\"(\n\x16\x41starteBinaryBlobArray\x12\x0e\n\x06values\x18\x01 \x03(\x0c\"B\n\x14\x41starteDateTimeArray\x12*\n\x06values\x18\x01 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\"\xd1\x01\n\x15\x41starteDataTypeObject\x12R\n\x0bobject_data\x18\x01 \x03(\x0b\x32=.astarteplatform.msghub.AstarteDataTypeObject.ObjectDataEntry\x1a\x64\n\x0fObjectDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12@\n\x05value\x18\x02 \x01(\x0b\x32\x31.astarteplatform.msghub.AstarteDataTypeIndividual:\x02\x38\x01\"\xc1\x06\n\x19\x41starteDataTypeIndividual\x12\x18\n\x0e\x61starte_double\x18\x01 \x01(\x01H\x00\x12\x19\n\x0f\x61starte_integer\x18\x02 \x01(\x05H\x00\x12\x19\n\x0f\x61starte_boolean\x18\x03 \x01(\x08H\x00\x12\x1e\n\x14\x61starte_long_integer\x18\x04 \x01(\x03H\x00\x12\x18\n\x0e\x61starte_string\x18\x05 \x01(\tH\x00\x12\x1d\n\x13\x61starte_binary_blob\x18\x06 \x01(\x0cH\x00\x12\x37\n\x11\x61starte_date_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x12J\n\x14\x61starte_double_array\x18\x08 \x01(\x0b\x32*.astarteplatform.msghub.AstarteDoubleArrayH\x00\x12L\n\x15\x61starte_integer_array\x18\t \x01(\x0b\x32+.astarteplatform.msghub.AstarteIntegerArrayH\x00\x12L\n\x15\x61starte_boolean_array\x18\n \x01(\x0b\x32+.astarteplatform.msghub.AstarteBooleanArrayH\x00\x12U\n\x1a\x61starte_long_integer_array\x18\x0b \x01(\x0b\x32/.astarteplatform.msghub.AstarteLongIntegerArrayH\x00\x12J\n\x14\x61starte_string_array\x18\x0c \x01(\x0b\x32*.astarteplatform.msghub.AstarteStringArrayH\x00\x12S\n\x19\x61starte_binary_blob_array\x18\r \x01(\x0b\x32..astarteplatform.msghub.AstarteBinaryBlobArrayH\x00\x12O\n\x17\x61starte_date_time_array\x18\x0e \x01(\x0b\x32,.astarteplatform.msghub.AstarteDateTimeArrayH\x00\x42\x11\n\x0findividual_data\"\xb3\x01\n\x0f\x41starteDataType\x12O\n\x12\x61starte_individual\x18\x01 \x01(\x0b\x32\x31.astarteplatform.msghub.AstarteDataTypeIndividualH\x00\x12G\n\x0e\x61starte_object\x18\x02 \x01(\x0b\x32-.astarteplatform.msghub.AstarteDataTypeObjectH\x00\x42\x06\n\x04\x64\x61tab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'astarteplatform.msghub.astarte_type_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  _globals['_ASTARTEDATATYPEOBJECT_OBJECTDATAENTRY']._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
+  _globals['_ASTARTEDATATYPEOBJECT_OBJECTDATAENTRY']._loaded_options = None
   _globals['_ASTARTEDATATYPEOBJECT_OBJECTDATAENTRY']._serialized_options = b'8\001'
   _globals['_ASTARTEDOUBLEARRAY']._serialized_start=102
   _globals['_ASTARTEDOUBLEARRAY']._serialized_end=138
   _globals['_ASTARTEINTEGERARRAY']._serialized_start=140
   _globals['_ASTARTEINTEGERARRAY']._serialized_end=177
   _globals['_ASTARTEBOOLEANARRAY']._serialized_start=179
   _globals['_ASTARTEBOOLEANARRAY']._serialized_end=216
```

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/astarte_type_pb2.pyi` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/astarte_type_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -3,70 +3,70 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class AstarteDoubleArray(_message.Message):
-    __slots__ = ["values"]
+    __slots__ = ("values",)
     VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedScalarFieldContainer[float]
     def __init__(self, values: _Optional[_Iterable[float]] = ...) -> None: ...
 
 class AstarteIntegerArray(_message.Message):
-    __slots__ = ["values"]
+    __slots__ = ("values",)
     VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedScalarFieldContainer[int]
     def __init__(self, values: _Optional[_Iterable[int]] = ...) -> None: ...
 
 class AstarteBooleanArray(_message.Message):
-    __slots__ = ["values"]
+    __slots__ = ("values",)
     VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedScalarFieldContainer[bool]
     def __init__(self, values: _Optional[_Iterable[bool]] = ...) -> None: ...
 
 class AstarteLongIntegerArray(_message.Message):
-    __slots__ = ["values"]
+    __slots__ = ("values",)
     VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedScalarFieldContainer[int]
     def __init__(self, values: _Optional[_Iterable[int]] = ...) -> None: ...
 
 class AstarteStringArray(_message.Message):
-    __slots__ = ["values"]
+    __slots__ = ("values",)
     VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, values: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class AstarteBinaryBlobArray(_message.Message):
-    __slots__ = ["values"]
+    __slots__ = ("values",)
     VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedScalarFieldContainer[bytes]
     def __init__(self, values: _Optional[_Iterable[bytes]] = ...) -> None: ...
 
 class AstarteDateTimeArray(_message.Message):
-    __slots__ = ["values"]
+    __slots__ = ("values",)
     VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedCompositeFieldContainer[_timestamp_pb2.Timestamp]
     def __init__(self, values: _Optional[_Iterable[_Union[_timestamp_pb2.Timestamp, _Mapping]]] = ...) -> None: ...
 
 class AstarteDataTypeObject(_message.Message):
-    __slots__ = ["object_data"]
+    __slots__ = ("object_data",)
     class ObjectDataEntry(_message.Message):
-        __slots__ = ["key", "value"]
+        __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: AstarteDataTypeIndividual
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[AstarteDataTypeIndividual, _Mapping]] = ...) -> None: ...
     OBJECT_DATA_FIELD_NUMBER: _ClassVar[int]
     object_data: _containers.MessageMap[str, AstarteDataTypeIndividual]
     def __init__(self, object_data: _Optional[_Mapping[str, AstarteDataTypeIndividual]] = ...) -> None: ...
 
 class AstarteDataTypeIndividual(_message.Message):
-    __slots__ = ["astarte_double", "astarte_integer", "astarte_boolean", "astarte_long_integer", "astarte_string", "astarte_binary_blob", "astarte_date_time", "astarte_double_array", "astarte_integer_array", "astarte_boolean_array", "astarte_long_integer_array", "astarte_string_array", "astarte_binary_blob_array", "astarte_date_time_array"]
+    __slots__ = ("astarte_double", "astarte_integer", "astarte_boolean", "astarte_long_integer", "astarte_string", "astarte_binary_blob", "astarte_date_time", "astarte_double_array", "astarte_integer_array", "astarte_boolean_array", "astarte_long_integer_array", "astarte_string_array", "astarte_binary_blob_array", "astarte_date_time_array")
     ASTARTE_DOUBLE_FIELD_NUMBER: _ClassVar[int]
     ASTARTE_INTEGER_FIELD_NUMBER: _ClassVar[int]
     ASTARTE_BOOLEAN_FIELD_NUMBER: _ClassVar[int]
     ASTARTE_LONG_INTEGER_FIELD_NUMBER: _ClassVar[int]
     ASTARTE_STRING_FIELD_NUMBER: _ClassVar[int]
     ASTARTE_BINARY_BLOB_FIELD_NUMBER: _ClassVar[int]
     ASTARTE_DATE_TIME_FIELD_NUMBER: _ClassVar[int]
@@ -90,13 +90,13 @@
     astarte_long_integer_array: AstarteLongIntegerArray
     astarte_string_array: AstarteStringArray
     astarte_binary_blob_array: AstarteBinaryBlobArray
     astarte_date_time_array: AstarteDateTimeArray
     def __init__(self, astarte_double: _Optional[float] = ..., astarte_integer: _Optional[int] = ..., astarte_boolean: bool = ..., astarte_long_integer: _Optional[int] = ..., astarte_string: _Optional[str] = ..., astarte_binary_blob: _Optional[bytes] = ..., astarte_date_time: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., astarte_double_array: _Optional[_Union[AstarteDoubleArray, _Mapping]] = ..., astarte_integer_array: _Optional[_Union[AstarteIntegerArray, _Mapping]] = ..., astarte_boolean_array: _Optional[_Union[AstarteBooleanArray, _Mapping]] = ..., astarte_long_integer_array: _Optional[_Union[AstarteLongIntegerArray, _Mapping]] = ..., astarte_string_array: _Optional[_Union[AstarteStringArray, _Mapping]] = ..., astarte_binary_blob_array: _Optional[_Union[AstarteBinaryBlobArray, _Mapping]] = ..., astarte_date_time_array: _Optional[_Union[AstarteDateTimeArray, _Mapping]] = ...) -> None: ...
 
 class AstarteDataType(_message.Message):
-    __slots__ = ["astarte_individual", "astarte_object"]
+    __slots__ = ("astarte_individual", "astarte_object")
     ASTARTE_INDIVIDUAL_FIELD_NUMBER: _ClassVar[int]
     ASTARTE_OBJECT_FIELD_NUMBER: _ClassVar[int]
     astarte_individual: AstarteDataTypeIndividual
     astarte_object: AstarteDataTypeObject
     def __init__(self, astarte_individual: _Optional[_Union[AstarteDataTypeIndividual, _Mapping]] = ..., astarte_object: _Optional[_Union[AstarteDataTypeObject, _Mapping]] = ...) -> None: ...
```

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/config_pb2.py` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/config_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: astarteplatform/msghub/config.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,14 +16,14 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#astarteplatform/msghub/config.proto\x12\x16\x61starteplatform.msghub\x1a\x1bgoogle/protobuf/empty.proto\"\xd9\x01\n\rConfigMessage\x12\r\n\x05realm\x18\x01 \x01(\t\x12\x16\n\tdevice_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x1f\n\x12\x63redentials_secret\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x13\n\x0bpairing_url\x18\x04 \x01(\t\x12\x1a\n\rpairing_token\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x18\n\x10grpc_socket_port\x18\x06 \x01(\rB\x0c\n\n_device_idB\x15\n\x13_credentials_secretB\x10\n\x0e_pairing_token2^\n\x10MessageHubConfig\x12J\n\tSetConfig\x12%.astarteplatform.msghub.ConfigMessage\x1a\x16.google.protobuf.Emptyb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'astarteplatform.msghub.config_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_CONFIGMESSAGE']._serialized_start=93
   _globals['_CONFIGMESSAGE']._serialized_end=310
   _globals['_MESSAGEHUBCONFIG']._serialized_start=312
   _globals['_MESSAGEHUBCONFIG']._serialized_end=406
 # @@protoc_insertion_point(module_scope)
```

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/config_pb2.pyi` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/config_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ConfigMessage(_message.Message):
-    __slots__ = ["realm", "device_id", "credentials_secret", "pairing_url", "pairing_token", "grpc_socket_port"]
+    __slots__ = ("realm", "device_id", "credentials_secret", "pairing_url", "pairing_token", "grpc_socket_port")
     REALM_FIELD_NUMBER: _ClassVar[int]
     DEVICE_ID_FIELD_NUMBER: _ClassVar[int]
     CREDENTIALS_SECRET_FIELD_NUMBER: _ClassVar[int]
     PAIRING_URL_FIELD_NUMBER: _ClassVar[int]
     PAIRING_TOKEN_FIELD_NUMBER: _ClassVar[int]
     GRPC_SOCKET_PORT_FIELD_NUMBER: _ClassVar[int]
     realm: str
```

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/config_pb2_grpc.py` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/config_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/message_hub_service_pb2.py` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/message_hub_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: astarteplatform/msghub/message_hub_service.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -18,12 +19,12 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0astarteplatform/msghub/message_hub_service.proto\x12\x16\x61starteplatform.msghub\x1a\x1bgoogle/protobuf/empty.proto\x1a,astarteplatform/msghub/astarte_message.proto\x1a)astarteplatform/msghub/astarte_type.proto\x1a!astarteplatform/msghub/node.proto2\xec\x01\n\nMessageHub\x12R\n\x06\x41ttach\x12\x1c.astarteplatform.msghub.Node\x1a&.astarteplatform.msghub.AstarteMessage\"\x00\x30\x01\x12H\n\x04Send\x12&.astarteplatform.msghub.AstarteMessage\x1a\x16.google.protobuf.Empty\"\x00\x12@\n\x06\x44\x65tach\x12\x1c.astarteplatform.msghub.Node\x1a\x16.google.protobuf.Empty\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'astarteplatform.msghub.message_hub_service_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_MESSAGEHUB']._serialized_start=230
   _globals['_MESSAGEHUB']._serialized_end=466
 # @@protoc_insertion_point(module_scope)
```

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/message_hub_service_pb2_grpc.py` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/message_hub_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/node_pb2.py` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/node_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: astarteplatform/msghub/node.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -14,12 +15,12 @@
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!astarteplatform/msghub/node.proto\x12\x16\x61starteplatform.msghub\"-\n\x04Node\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x17\n\x0finterface_jsons\x18\x02 \x03(\x0c\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'astarteplatform.msghub.node_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
+if not _descriptor._USE_C_DESCRIPTORS:
+  DESCRIPTOR._loaded_options = None
   _globals['_NODE']._serialized_start=61
   _globals['_NODE']._serialized_end=106
 # @@protoc_insertion_point(module_scope)
```

### Comparing `astarte_message_hub_proto-0.6.1/astarteplatform/msghub/node_pb2.pyi` & `astarte_message_hub_proto-0.6.2/astarteplatform/msghub/node_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Node(_message.Message):
-    __slots__ = ["uuid", "interface_jsons"]
+    __slots__ = ("uuid", "interface_jsons")
     UUID_FIELD_NUMBER: _ClassVar[int]
     INTERFACE_JSONS_FIELD_NUMBER: _ClassVar[int]
     uuid: str
     interface_jsons: _containers.RepeatedScalarFieldContainer[bytes]
     def __init__(self, uuid: _Optional[str] = ..., interface_jsons: _Optional[_Iterable[bytes]] = ...) -> None: ...
```

### Comparing `astarte_message_hub_proto-0.6.1/pyproject.toml` & `astarte_message_hub_proto-0.6.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "astarte_message_hub_proto"
 description="Astarte message hub protocol buffers for Python"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
     { name = "Simone Orru", email = "simone.orru@secomind.com" }
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 # Classifier list: https://pypi.org/classifiers/
 classifiers = [
```

