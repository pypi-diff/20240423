# Comparing `tmp/openobd_protocol-0.0.38.tar.gz` & `tmp/openobd_protocol-0.0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openobd_protocol-0.0.38.tar", last modified: Wed Apr 17 12:41:16 2024, max compression
+gzip compressed data, was "openobd_protocol-0.0.39.tar", last modified: Tue Apr 23 10:19:50 2024, max compression
```

## Comparing `openobd_protocol-0.0.38.tar` & `openobd_protocol-0.0.39.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:41:16.777244 openobd_protocol-0.0.38/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-17 12:41:16.777244 openobd_protocol-0.0.38/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      241 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/README.md
--rw-r--r--   0 root         (0) root         (0)     1895 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-17 12:41:16.777244 openobd_protocol-0.0.38/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:41:16.762244 openobd_protocol-0.0.38/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:41:16.769244 openobd_protocol-0.0.38/src/openobd_protocol/
--rw-r--r--   0 root         (0) root         (0)     1745 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/Authentication_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1071 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/Authentication_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1234 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/BasicResponse_pb2.py
--rw-r--r--   0 root         (0) root         (0)      504 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/BasicResponse_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5065 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/BusConfiguration_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6043 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/BusConfiguration_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:41:16.773244 openobd_protocol-0.0.38/src/openobd_protocol/CAN/
--rw-r--r--   0 root         (0) root         (0)     2103 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/CAN/CanServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      462 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/CAN/CanServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4415 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2636 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/CAN/Isotp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2500 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/CAN/Isotp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2349 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8395 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:41:16.774244 openobd_protocol-0.0.38/src/openobd_protocol/SessionController/
--rw-r--r--   0 root         (0) root         (0)     1940 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/SessionController/SessionServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      190 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     9440 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1712 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/Status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1203 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/Status_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:41:16.776244 openobd_protocol-0.0.38/src/openobd_protocol/UserInterface/
--rw-r--r--   0 root         (0) root         (0)     1748 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
--rw-r--r--   0 root         (0) root         (0)      273 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2973 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3920 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/UserInterface/UserInterface_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4208 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-17 12:41:11.000000 openobd_protocol-0.0.38/src/openobd_protocol/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 12:41:16.776244 openobd_protocol-0.0.38/src/openobd_protocol.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-17 12:41:16.000000 openobd_protocol-0.0.38/src/openobd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1501 2024-04-17 12:41:16.000000 openobd_protocol-0.0.38/src/openobd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 12:41:16.000000 openobd_protocol-0.0.38/src/openobd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-04-17 12:41:16.000000 openobd_protocol-0.0.38/src/openobd_protocol.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-17 12:41:16.000000 openobd_protocol-0.0.38/src/openobd_protocol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.472398 openobd_protocol-0.0.39/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-23 10:19:50.472398 openobd_protocol-0.0.39/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      241 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/README.md
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 10:19:50.472398 openobd_protocol-0.0.39/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.454398 openobd_protocol-0.0.39/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.463398 openobd_protocol-0.0.39/src/openobd_protocol/
+-rw-r--r--   0 root         (0) root         (0)     1745 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/Authentication_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/Authentication_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1234 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/BasicResponse_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/BasicResponse_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5065 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/BusConfiguration_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6043 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/BusConfiguration_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.466398 openobd_protocol-0.0.39/src/openobd_protocol/CAN/
+-rw-r--r--   0 root         (0) root         (0)     2103 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/CAN/CanServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      462 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/CAN/CanServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4415 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/CAN/CanServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/CAN/Isotp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/CAN/Isotp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2349 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/RemoteDiagnosticServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/RemoteDiagnosticServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8395 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.469398 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/SessionServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/SessionServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     9730 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/Session_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1449 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/SessionController/Session_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/Status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/Status_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.471398 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2973 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3920 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterface_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4208 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)       23 2024-04-23 10:19:45.000000 openobd_protocol-0.0.39/src/openobd_protocol/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:19:50.471398 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-23 10:19:50.000000 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1610 2024-04-23 10:19:50.000000 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 10:19:50.000000 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-23 10:19:50.000000 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-23 10:19:50.000000 openobd_protocol-0.0.39/src/openobd_protocol.egg-info/top_level.txt
```

### Comparing `openobd_protocol-0.0.38/LICENSE` & `openobd_protocol-0.0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/PKG-INFO` & `openobd_protocol-0.0.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.38
+Version: 0.0.39
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.0.38/pyproject.toml` & `openobd_protocol-0.0.39/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/Authentication_pb2.py` & `openobd_protocol-0.0.39/src/openobd_protocol/Authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/Authentication_pb2.pyi` & `openobd_protocol-0.0.39/src/openobd_protocol/Authentication_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/BasicResponse_pb2.py` & `openobd_protocol-0.0.39/src/openobd_protocol/BasicResponse_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/BusConfiguration_pb2.py` & `openobd_protocol-0.0.39/src/openobd_protocol/BusConfiguration_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/BusConfiguration_pb2.pyi` & `openobd_protocol-0.0.39/src/openobd_protocol/BusConfiguration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/CAN/CanServices_pb2.py` & `openobd_protocol-0.0.39/src/openobd_protocol/CAN/CanServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/CAN/CanServices_pb2_grpc.py` & `openobd_protocol-0.0.39/src/openobd_protocol/CAN/CanServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/CAN/Isotp_pb2.py` & `openobd_protocol-0.0.39/src/openobd_protocol/CAN/Isotp_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/CAN/Isotp_pb2.pyi` & `openobd_protocol-0.0.39/src/openobd_protocol/CAN/Isotp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/RemoteDiagnosticServices_pb2.py` & `openobd_protocol-0.0.39/src/openobd_protocol/RemoteDiagnosticServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py` & `openobd_protocol-0.0.39/src/openobd_protocol/RemoteDiagnosticServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/SessionController/SessionServices_pb2.py` & `openobd_protocol-0.0.39/src/openobd_protocol/SessionController/SessionServices_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
+from openobd_protocol.SessionController import Session_pb2 as openobd__protocol_dot_SessionController_dot_Session__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto2\xf4\x03\n\x0fSessionServices\x12\x61\n\x0fgetSessionToken\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12_\n\rcreateSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12\\\n\ngetSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12_\n\rdeleteSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12^\n\x0clistSessions\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x42\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n8openobd_protocol/SessionController/SessionServices.proto\x12/com.jifeline.OpenOBD.Protocol.SessionController\x1a\x1dopenobd_protocol/Status.proto\x1a\x30openobd_protocol/SessionController/Session.proto2\xa4\x04\n\x0fSessionServices\x12\x61\n\x0fgetSessionToken\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12\x8e\x01\n\rcreateSession\x12=.com.jifeline.OpenOBD.Protocol.SessionController.startSession\x1a<.com.jifeline.OpenOBD.Protocol.SessionController.sessionInfo\"\x00\x12\\\n\ngetSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12_\n\rdeleteSession\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x12^\n\x0clistSessions\x12%.com.jifeline.OpenOBD.Protocol.Status\x1a%.com.jifeline.OpenOBD.Protocol.Status\"\x00\x42\x02P\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'openobd_protocol.SessionController.SessionServices_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'P\001'
-  _globals['_SESSIONSERVICES']._serialized_start=141
-  _globals['_SESSIONSERVICES']._serialized_end=641
+  _globals['_SESSIONSERVICES']._serialized_start=191
+  _globals['_SESSIONSERVICES']._serialized_end=739
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py` & `openobd_protocol-0.0.39/src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
+from openobd_protocol.SessionController import Session_pb2 as openobd__protocol_dot_SessionController_dot_Session__pb2
 from openobd_protocol import Status_pb2 as openobd__protocol_dot_Status__pb2
 
 
 class SessionServicesStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
@@ -17,16 +18,16 @@
         self.getSessionToken = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSessionToken',
                 request_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
                 )
         self.createSession = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/createSession',
-                request_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
-                response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
+                request_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.startSession.SerializeToString,
+                response_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.sessionInfo.FromString,
                 )
         self.getSession = channel.unary_unary(
                 '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/getSession',
                 request_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
                 response_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
                 )
         self.deleteSession = channel.unary_unary(
@@ -80,16 +81,16 @@
             'getSessionToken': grpc.unary_unary_rpc_method_handler(
                     servicer.getSessionToken,
                     request_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
                     response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
             ),
             'createSession': grpc.unary_unary_rpc_method_handler(
                     servicer.createSession,
-                    request_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
-                    response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
+                    request_deserializer=openobd__protocol_dot_SessionController_dot_Session__pb2.startSession.FromString,
+                    response_serializer=openobd__protocol_dot_SessionController_dot_Session__pb2.sessionInfo.SerializeToString,
             ),
             'getSession': grpc.unary_unary_rpc_method_handler(
                     servicer.getSession,
                     request_deserializer=openobd__protocol_dot_Status__pb2.Status.FromString,
                     response_serializer=openobd__protocol_dot_Status__pb2.Status.SerializeToString,
             ),
             'deleteSession': grpc.unary_unary_rpc_method_handler(
@@ -137,16 +138,16 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/com.jifeline.OpenOBD.Protocol.SessionController.SessionServices/createSession',
-            openobd__protocol_dot_Status__pb2.Status.SerializeToString,
-            openobd__protocol_dot_Status__pb2.Status.FromString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.startSession.SerializeToString,
+            openobd__protocol_dot_SessionController_dot_Session__pb2.sessionInfo.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def getSession(request,
             target,
             options=(),
```

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/Status_pb2.py` & `openobd_protocol-0.0.39/src/openobd_protocol/Status_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/Status_pb2.pyi` & `openobd_protocol-0.0.39/src/openobd_protocol/Status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py` & `openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py` & `openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/UserInterface/UserInterface_pb2.py` & `openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterface_pb2.py`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi` & `openobd_protocol-0.0.39/src/openobd_protocol/UserInterface/UserInterface_pb2.pyi`

 * *Files identical despite different names*

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol.egg-info/PKG-INFO` & `openobd_protocol-0.0.39/src/openobd_protocol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openobd-protocol
-Version: 0.0.38
+Version: 0.0.39
 Summary: Jifeline Networks OpenOBD Protocol Buffers gRPC
 Author-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 Maintainer-email: Gerhard de Koning Gans <gerhard@factorit.nl>, Rohaan Ghosh <rohaan@factorit.nl>, Sander de Mooij <sanderdemooij@factorit.nl>
 License: Copyright (c) 2024 Jifeline Networks B.V.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `openobd_protocol-0.0.38/src/openobd_protocol.egg-info/SOURCES.txt` & `openobd_protocol-0.0.39/src/openobd_protocol.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,12 +22,14 @@
 src/openobd_protocol/CAN/CanServices_pb2.pyi
 src/openobd_protocol/CAN/CanServices_pb2_grpc.py
 src/openobd_protocol/CAN/Isotp_pb2.py
 src/openobd_protocol/CAN/Isotp_pb2.pyi
 src/openobd_protocol/SessionController/SessionServices_pb2.py
 src/openobd_protocol/SessionController/SessionServices_pb2.pyi
 src/openobd_protocol/SessionController/SessionServices_pb2_grpc.py
+src/openobd_protocol/SessionController/Session_pb2.py
+src/openobd_protocol/SessionController/Session_pb2.pyi
 src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.py
 src/openobd_protocol/UserInterface/UserInterfaceServices_pb2.pyi
 src/openobd_protocol/UserInterface/UserInterfaceServices_pb2_grpc.py
 src/openobd_protocol/UserInterface/UserInterface_pb2.py
 src/openobd_protocol/UserInterface/UserInterface_pb2.pyi
```

