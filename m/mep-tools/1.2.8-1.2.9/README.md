# Comparing `tmp/mep_tools-1.2.8.tar.gz` & `tmp/mep_tools-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mep_tools-1.2.8.tar", last modified: Thu Jan  4 16:06:27 2024, max compression
+gzip compressed data, was "mep_tools-1.2.9.tar", last modified: Thu Jan  4 16:07:59 2024, max compression
```

## Comparing `mep_tools-1.2.8.tar` & `mep_tools-1.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:06:27.537698 mep_tools-1.2.8/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      219 2024-01-04 16:06:27.534294 mep_tools-1.2.8/PKG-INFO
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:06:27.498933 mep_tools-1.2.8/mep_tools/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      190 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/__init__.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:06:27.524586 mep_tools-1.2.8/mep_tools/connectors/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      546 2024-01-04 16:06:27.000000 mep_tools-1.2.8/mep_tools/connectors/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1383 2024-01-04 16:06:25.000000 mep_tools-1.2.8/mep_tools/connectors/blueprint_pb2.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-01-04 16:06:25.000000 mep_tools-1.2.8/mep_tools/connectors/blueprint_pb2.pyi
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2488 2024-01-04 16:06:25.000000 mep_tools-1.2.8/mep_tools/connectors/blueprint_pb2_grpc.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1634 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/company_pb2.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      376 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/company_pb2.pyi
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     6916 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/company_pb2_grpc.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4726 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/connect_portal_pb2.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4249 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/connect_portal_pb2.pyi
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     8882 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/connect_portal_pb2_grpc.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2871 2024-01-04 16:06:25.000000 mep_tools-1.2.8/mep_tools/connectors/connector_pb2.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2613 2024-01-04 16:06:25.000000 mep_tools-1.2.8/mep_tools/connectors/connector_pb2.pyi
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2536 2024-01-04 16:06:25.000000 mep_tools-1.2.8/mep_tools/connectors/connector_pb2_grpc.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3260 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/metric_pb2.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3648 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/metric_pb2.pyi
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3923 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/metric_pb2_grpc.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1354 2024-01-04 16:06:25.000000 mep_tools-1.2.8/mep_tools/connectors/platform_pb2.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      378 2024-01-04 16:06:25.000000 mep_tools-1.2.8/mep_tools/connectors/platform_pb2.pyi
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2464 2024-01-04 16:06:25.000000 mep_tools-1.2.8/mep_tools/connectors/platform_pb2_grpc.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2842 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/service_pb2.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2846 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/service_pb2.pyi
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3995 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/connectors/service_pb2_grpc.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:06:27.530002 mep_tools-1.2.8/mep_tools/leads/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      192 2024-01-04 16:06:27.000000 mep_tools-1.2.8/mep_tools/leads/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1370 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/leads/lead_tracker_pb2.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      595 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/leads/lead_tracker_pb2.pyi
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2479 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/leads/lead_tracker_pb2_grpc.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:06:27.532942 mep_tools-1.2.8/mep_tools/utils/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      176 2024-01-04 16:06:27.000000 mep_tools-1.2.8/mep_tools/utils/__init__.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      993 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/utils/json_pb2.py
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      385 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/utils/json_pb2.pyi
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      159 2024-01-04 16:06:26.000000 mep_tools-1.2.8/mep_tools/utils/json_pb2_grpc.py
-drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:06:27.504300 mep_tools-1.2.8/mep_tools.egg-info/
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      219 2024-01-04 16:06:27.000000 mep_tools-1.2.8/mep_tools.egg-info/PKG-INFO
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1318 2024-01-04 16:06:27.000000 mep_tools-1.2.8/mep_tools.egg-info/SOURCES.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-01-04 16:06:27.000000 mep_tools-1.2.8/mep_tools.egg-info/dependency_links.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       29 2024-01-04 16:06:27.000000 mep_tools-1.2.8/mep_tools.egg-info/requires.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       10 2024-01-04 16:06:27.000000 mep_tools-1.2.8/mep_tools.egg-info/top_level.txt
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-01-04 16:06:27.538406 mep_tools-1.2.8/setup.cfg
--rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      567 2024-01-04 16:06:22.000000 mep_tools-1.2.8/setup.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:07:59.800406 mep_tools-1.2.9/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      219 2024-01-04 16:07:59.799925 mep_tools-1.2.9/PKG-INFO
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:07:59.777109 mep_tools-1.2.9/mep_tools/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      190 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools/__init__.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:07:59.794478 mep_tools-1.2.9/mep_tools/connectors/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      546 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools/connectors/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1383 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/blueprint_pb2.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      380 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/blueprint_pb2.pyi
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2488 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/blueprint_pb2_grpc.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1634 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/company_pb2.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      376 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/company_pb2.pyi
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     6916 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/company_pb2_grpc.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4797 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/connect_portal_pb2.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     4357 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/connect_portal_pb2.pyi
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     8882 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/connect_portal_pb2_grpc.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2871 2024-01-04 16:07:57.000000 mep_tools-1.2.9/mep_tools/connectors/connector_pb2.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2613 2024-01-04 16:07:57.000000 mep_tools-1.2.9/mep_tools/connectors/connector_pb2.pyi
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2536 2024-01-04 16:07:57.000000 mep_tools-1.2.9/mep_tools/connectors/connector_pb2_grpc.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3260 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/metric_pb2.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3648 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/metric_pb2.pyi
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3923 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/metric_pb2_grpc.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1354 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/platform_pb2.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      378 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/platform_pb2.pyi
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2464 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/platform_pb2_grpc.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2842 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/service_pb2.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2846 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/service_pb2.pyi
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     3995 2024-01-04 16:07:58.000000 mep_tools-1.2.9/mep_tools/connectors/service_pb2_grpc.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:07:59.796713 mep_tools-1.2.9/mep_tools/leads/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      192 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools/leads/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1370 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools/leads/lead_tracker_pb2.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      595 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools/leads/lead_tracker_pb2.pyi
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     2479 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools/leads/lead_tracker_pb2_grpc.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:07:59.799041 mep_tools-1.2.9/mep_tools/utils/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      176 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools/utils/__init__.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      993 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools/utils/json_pb2.py
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      385 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools/utils/json_pb2.pyi
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      159 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools/utils/json_pb2_grpc.py
+drwxr-xr-x   0 khaireddinesarraj   (501) staff       (20)        0 2024-01-04 16:07:59.779936 mep_tools-1.2.9/mep_tools.egg-info/
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      219 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools.egg-info/PKG-INFO
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)     1318 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)        1 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       29 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools.egg-info/requires.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       10 2024-01-04 16:07:59.000000 mep_tools-1.2.9/mep_tools.egg-info/top_level.txt
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)       38 2024-01-04 16:07:59.800609 mep_tools-1.2.9/setup.cfg
+-rw-r--r--   0 khaireddinesarraj   (501) staff       (20)      567 2024-01-04 16:07:54.000000 mep_tools-1.2.9/setup.py
```

### Comparing `mep_tools-1.2.8/mep_tools/connectors/__init__.py` & `mep_tools-1.2.9/mep_tools/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/blueprint_pb2.py` & `mep_tools-1.2.9/mep_tools/connectors/blueprint_pb2.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/blueprint_pb2_grpc.py` & `mep_tools-1.2.9/mep_tools/connectors/blueprint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/company_pb2.py` & `mep_tools-1.2.9/mep_tools/connectors/company_pb2.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/company_pb2_grpc.py` & `mep_tools-1.2.9/mep_tools/connectors/company_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/connect_portal_pb2.py` & `mep_tools-1.2.9/mep_tools/connectors/connect_portal_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x63onnect_portal.proto\x12\x18\x63onnector.connect_portal\x1a\x19google/protobuf/any.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\" \n\x10PortalGetRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\")\n\x11PortalReadRequest\x12\x14\n\x0c\x63ompany_uuid\x18\x01 \x01(\t\"#\n\x13PortalDeleteRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\"\xa4\x01\n\x13PortalCreateRequest\x12\x14\n\x0c\x63ompany_uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x30\n\x04type\x18\x03 \x01(\x0e\x32\".connector.connect_portal.TypeEnum\x12\x11\n\tclassName\x18\x04 \x01(\t\x12$\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x14.google.protobuf.Any\"e\n\x13PortalUpdateRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x11\n\x04name\x18\x02 \x01(\tH\x00\x88\x01\x01\x12$\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x14.google.protobuf.AnyB\x07\n\x05_name\"\xa9\x03\n\x0ePortalResponse\x12\x36\n\toperation\x18\x01 \x01(\x0e\x32#.connector.connect_portal.Operation\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x11\n\x04uuid\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\x11\n\x04name\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x35\n\x04type\x18\x05 \x01(\x0e\x32\".connector.connect_portal.TypeEnumH\x02\x88\x01\x01\x12\x10\n\x03key\x18\x06 \x01(\tH\x03\x88\x01\x01\x12)\n\x06\x63onfig\x18\x07 \x01(\x0b\x32\x14.google.protobuf.AnyH\x04\x88\x01\x01\x12\x33\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x05\x88\x01\x01\x12\x33\n\nupdated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x42\x07\n\x05_uuidB\x07\n\x05_nameB\x07\n\x05_typeB\x06\n\x04_keyB\t\n\x07_configB\r\n\x0b_created_atB\r\n\x0b_updated_at\"L\n\x0fPortalsResponse\x12\x39\n\x07portals\x18\x01 \x03(\x0b\x32(.connector.connect_portal.PortalResponse*1\n\x08TypeEnum\x12\x07\n\x03\x41TS\x10\x00\x12\x0b\n\x07\x43HANNEL\x10\x01\x12\x0f\n\x0bINTEGRATION\x10\x02*B\n\tOperation\x12\x07\n\x03GET\x10\x00\x12\n\n\x06\x43REATE\x10\x01\x12\x08\n\x04READ\x10\x02\x12\n\n\x06UPDATE\x10\x03\x12\n\n\x06\x44\x45LETE\x10\x04\x32\xfc\x03\n\x14\x43onnectPortalService\x12[\n\x03Get\x12*.connector.connect_portal.PortalGetRequest\x1a(.connector.connect_portal.PortalResponse\x12\x61\n\x06\x43reate\x12-.connector.connect_portal.PortalCreateRequest\x1a(.connector.connect_portal.PortalResponse\x12^\n\x04Read\x12+.connector.connect_portal.PortalReadRequest\x1a).connector.connect_portal.PortalsResponse\x12\x61\n\x06Update\x12-.connector.connect_portal.PortalUpdateRequest\x1a(.connector.connect_portal.PortalResponse\x12\x61\n\x06\x44\x65lete\x12-.connector.connect_portal.PortalDeleteRequest\x1a(.connector.connect_portal.PortalResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x63onnect_portal.proto\x12\x18\x63onnector.connect_portal\x1a\x19google/protobuf/any.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\" \n\x10PortalGetRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\")\n\x11PortalReadRequest\x12\x14\n\x0c\x63ompany_uuid\x18\x01 \x01(\t\"#\n\x13PortalDeleteRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\"\xa4\x01\n\x13PortalCreateRequest\x12\x14\n\x0c\x63ompany_uuid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x30\n\x04type\x18\x03 \x01(\x0e\x32\".connector.connect_portal.TypeEnum\x12\x11\n\tclassName\x18\x04 \x01(\t\x12$\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x14.google.protobuf.Any\"e\n\x13PortalUpdateRequest\x12\x0c\n\x04uuid\x18\x01 \x01(\t\x12\x11\n\x04name\x18\x02 \x01(\tH\x00\x88\x01\x01\x12$\n\x06\x63onfig\x18\x03 \x01(\x0b\x32\x14.google.protobuf.AnyB\x07\n\x05_name\"\xcf\x03\n\x0ePortalResponse\x12\x36\n\toperation\x18\x01 \x01(\x0e\x32#.connector.connect_portal.Operation\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x11\n\x04uuid\x18\x03 \x01(\tH\x00\x88\x01\x01\x12\x11\n\x04name\x18\x04 \x01(\tH\x01\x88\x01\x01\x12\x35\n\x04type\x18\x05 \x01(\x0e\x32\".connector.connect_portal.TypeEnumH\x02\x88\x01\x01\x12\x10\n\x03key\x18\x06 \x01(\tH\x03\x88\x01\x01\x12\x16\n\tclassName\x18\x07 \x01(\tH\x04\x88\x01\x01\x12)\n\x06\x63onfig\x18\x08 \x01(\x0b\x32\x14.google.protobuf.AnyH\x05\x88\x01\x01\x12\x33\n\ncreated_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x33\n\nupdated_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x07\x88\x01\x01\x42\x07\n\x05_uuidB\x07\n\x05_nameB\x07\n\x05_typeB\x06\n\x04_keyB\x0c\n\n_classNameB\t\n\x07_configB\r\n\x0b_created_atB\r\n\x0b_updated_at\"L\n\x0fPortalsResponse\x12\x39\n\x07portals\x18\x01 \x03(\x0b\x32(.connector.connect_portal.PortalResponse*1\n\x08TypeEnum\x12\x07\n\x03\x41TS\x10\x00\x12\x0b\n\x07\x43HANNEL\x10\x01\x12\x0f\n\x0bINTEGRATION\x10\x02*B\n\tOperation\x12\x07\n\x03GET\x10\x00\x12\n\n\x06\x43REATE\x10\x01\x12\x08\n\x04READ\x10\x02\x12\n\n\x06UPDATE\x10\x03\x12\n\n\x06\x44\x45LETE\x10\x04\x32\xfc\x03\n\x14\x43onnectPortalService\x12[\n\x03Get\x12*.connector.connect_portal.PortalGetRequest\x1a(.connector.connect_portal.PortalResponse\x12\x61\n\x06\x43reate\x12-.connector.connect_portal.PortalCreateRequest\x1a(.connector.connect_portal.PortalResponse\x12^\n\x04Read\x12+.connector.connect_portal.PortalReadRequest\x1a).connector.connect_portal.PortalsResponse\x12\x61\n\x06Update\x12-.connector.connect_portal.PortalUpdateRequest\x1a(.connector.connect_portal.PortalResponse\x12\x61\n\x06\x44\x65lete\x12-.connector.connect_portal.PortalDeleteRequest\x1a(.connector.connect_portal.PortalResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'connect_portal_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _globals['_TYPEENUM']._serialized_start=1029
-  _globals['_TYPEENUM']._serialized_end=1078
-  _globals['_OPERATION']._serialized_start=1080
-  _globals['_OPERATION']._serialized_end=1146
+  _globals['_TYPEENUM']._serialized_start=1067
+  _globals['_TYPEENUM']._serialized_end=1116
+  _globals['_OPERATION']._serialized_start=1118
+  _globals['_OPERATION']._serialized_end=1184
   _globals['_PORTALGETREQUEST']._serialized_start=139
   _globals['_PORTALGETREQUEST']._serialized_end=171
   _globals['_PORTALREADREQUEST']._serialized_start=173
   _globals['_PORTALREADREQUEST']._serialized_end=214
   _globals['_PORTALDELETEREQUEST']._serialized_start=216
   _globals['_PORTALDELETEREQUEST']._serialized_end=251
   _globals['_PORTALCREATEREQUEST']._serialized_start=254
   _globals['_PORTALCREATEREQUEST']._serialized_end=418
   _globals['_PORTALUPDATEREQUEST']._serialized_start=420
   _globals['_PORTALUPDATEREQUEST']._serialized_end=521
   _globals['_PORTALRESPONSE']._serialized_start=524
-  _globals['_PORTALRESPONSE']._serialized_end=949
-  _globals['_PORTALSRESPONSE']._serialized_start=951
-  _globals['_PORTALSRESPONSE']._serialized_end=1027
-  _globals['_CONNECTPORTALSERVICE']._serialized_start=1149
-  _globals['_CONNECTPORTALSERVICE']._serialized_end=1657
+  _globals['_PORTALRESPONSE']._serialized_end=987
+  _globals['_PORTALSRESPONSE']._serialized_start=989
+  _globals['_PORTALSRESPONSE']._serialized_end=1065
+  _globals['_CONNECTPORTALSERVICE']._serialized_start=1187
+  _globals['_CONNECTPORTALSERVICE']._serialized_end=1695
 # @@protoc_insertion_point(module_scope)
```

### Comparing `mep_tools-1.2.8/mep_tools/connectors/connect_portal_pb2.pyi` & `mep_tools-1.2.9/mep_tools/connectors/connect_portal_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,33 +70,35 @@
     CONFIG_FIELD_NUMBER: _ClassVar[int]
     uuid: str
     name: str
     config: _any_pb2.Any
     def __init__(self, uuid: _Optional[str] = ..., name: _Optional[str] = ..., config: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...) -> None: ...
 
 class PortalResponse(_message.Message):
-    __slots__ = ["operation", "success", "uuid", "name", "type", "key", "config", "created_at", "updated_at"]
+    __slots__ = ["operation", "success", "uuid", "name", "type", "key", "className", "config", "created_at", "updated_at"]
     OPERATION_FIELD_NUMBER: _ClassVar[int]
     SUCCESS_FIELD_NUMBER: _ClassVar[int]
     UUID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
     KEY_FIELD_NUMBER: _ClassVar[int]
+    CLASSNAME_FIELD_NUMBER: _ClassVar[int]
     CONFIG_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
     UPDATED_AT_FIELD_NUMBER: _ClassVar[int]
     operation: Operation
     success: bool
     uuid: str
     name: str
     type: TypeEnum
     key: str
+    className: str
     config: _any_pb2.Any
     created_at: _timestamp_pb2.Timestamp
     updated_at: _timestamp_pb2.Timestamp
-    def __init__(self, operation: _Optional[_Union[Operation, str]] = ..., success: bool = ..., uuid: _Optional[str] = ..., name: _Optional[str] = ..., type: _Optional[_Union[TypeEnum, str]] = ..., key: _Optional[str] = ..., config: _Optional[_Union[_any_pb2.Any, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., updated_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+    def __init__(self, operation: _Optional[_Union[Operation, str]] = ..., success: bool = ..., uuid: _Optional[str] = ..., name: _Optional[str] = ..., type: _Optional[_Union[TypeEnum, str]] = ..., key: _Optional[str] = ..., className: _Optional[str] = ..., config: _Optional[_Union[_any_pb2.Any, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., updated_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
 class PortalsResponse(_message.Message):
     __slots__ = ["portals"]
     PORTALS_FIELD_NUMBER: _ClassVar[int]
     portals: _containers.RepeatedCompositeFieldContainer[PortalResponse]
     def __init__(self, portals: _Optional[_Iterable[_Union[PortalResponse, _Mapping]]] = ...) -> None: ...
```

### Comparing `mep_tools-1.2.8/mep_tools/connectors/connect_portal_pb2_grpc.py` & `mep_tools-1.2.9/mep_tools/connectors/connect_portal_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/connector_pb2.py` & `mep_tools-1.2.9/mep_tools/connectors/connector_pb2.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/connector_pb2.pyi` & `mep_tools-1.2.9/mep_tools/connectors/connector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/connector_pb2_grpc.py` & `mep_tools-1.2.9/mep_tools/connectors/connector_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/metric_pb2.py` & `mep_tools-1.2.9/mep_tools/connectors/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/metric_pb2.pyi` & `mep_tools-1.2.9/mep_tools/connectors/metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/metric_pb2_grpc.py` & `mep_tools-1.2.9/mep_tools/connectors/metric_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/platform_pb2.py` & `mep_tools-1.2.9/mep_tools/connectors/platform_pb2.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/platform_pb2_grpc.py` & `mep_tools-1.2.9/mep_tools/connectors/platform_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/service_pb2.py` & `mep_tools-1.2.9/mep_tools/connectors/service_pb2.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/service_pb2.pyi` & `mep_tools-1.2.9/mep_tools/connectors/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/connectors/service_pb2_grpc.py` & `mep_tools-1.2.9/mep_tools/connectors/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/leads/lead_tracker_pb2.py` & `mep_tools-1.2.9/mep_tools/leads/lead_tracker_pb2.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/leads/lead_tracker_pb2.pyi` & `mep_tools-1.2.9/mep_tools/leads/lead_tracker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/leads/lead_tracker_pb2_grpc.py` & `mep_tools-1.2.9/mep_tools/leads/lead_tracker_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools/utils/json_pb2.py` & `mep_tools-1.2.9/mep_tools/utils/json_pb2.py`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/mep_tools.egg-info/SOURCES.txt` & `mep_tools-1.2.9/mep_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mep_tools-1.2.8/setup.py` & `mep_tools-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="mep_tools",
-    version="1.2.8",
+    version="1.2.9",
     author="Khai",
     author_email="sarraj@marksmen.nl",
     license="MIT",
     packages=find_packages(),
     package_data={'mep_tools': ['*/*.pyi', '*.pyi']},
     description="grpc for rep",
     long_description="hold the code for the grpc files",
```

