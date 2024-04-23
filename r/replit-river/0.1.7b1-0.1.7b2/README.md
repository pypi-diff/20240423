# Comparing `tmp/replit_river-0.1.7b1.tar.gz` & `tmp/replit_river-0.1.7b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.1.7b1.tar", max compression
+gzip compressed data, was "replit_river-0.1.7b2.tar", max compression
```

## Comparing `replit_river-0.1.7b1.tar` & `replit_river-0.1.7b2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1064 2024-04-02 22:20:09.999604 replit_river-0.1.7b1/LICENSE
--rw-r--r--   0        0        0     1628 2024-03-26 20:33:50.343232 replit_river-0.1.7b1/README.md
--rw-r--r--   0        0        0     1749 2024-04-18 22:55:32.006505 replit_river-0.1.7b1/pyproject.toml
--rw-r--r--   0        0        0      487 2024-04-17 00:20:58.071349 replit_river-0.1.7b1/replit_river/__init__.py
--rw-r--r--   0        0        0     5174 2024-04-18 22:52:24.688442 replit_river-0.1.7b1/replit_river/client.py
--rw-r--r--   0        0        0    11759 2024-04-18 22:24:01.621432 replit_river-0.1.7b1/replit_river/client_session.py
--rw-r--r--   0        0        0     4314 2024-04-18 08:52:55.632770 replit_river-0.1.7b1/replit_river/client_transport.py
--rw-r--r--   0        0        0        0 2024-04-11 18:24:00.533020 replit_river-0.1.7b1/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-04-11 18:24:00.533220 replit_river-0.1.7b1/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13363 2024-04-17 00:20:58.072227 replit_river-0.1.7b1/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-04-11 18:24:00.535693 replit_river-0.1.7b1/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5354 2024-04-11 18:24:00.535865 replit_river-0.1.7b1/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12620 2024-04-17 19:05:12.058141 replit_river-0.1.7b1/replit_river/codegen/server.py
--rw-r--r--   0        0        0      515 2024-04-18 05:17:58.181429 replit_river-0.1.7b1/replit_river/error_schema.py
--rw-r--r--   0        0        0     1207 2024-04-18 21:12:58.850511 replit_river-0.1.7b1/replit_river/message_buffer.py
--rw-r--r--   0        0        0     2517 2024-04-18 09:00:07.281730 replit_river-0.1.7b1/replit_river/messages.py
--rw-r--r--   0        0        0        0 2024-04-11 18:24:00.536395 replit_river-0.1.7b1/replit_river/py.typed
--rw-r--r--   0        0        0    11973 2024-04-17 19:05:34.905421 replit_river-0.1.7b1/replit_river/rpc.py
--rw-r--r--   0        0        0     2138 2024-04-18 05:49:40.092134 replit_river-0.1.7b1/replit_river/seq_manager.py
--rw-r--r--   0        0        0     1763 2024-04-18 22:44:37.391550 replit_river-0.1.7b1/replit_river/server.py
--rw-r--r--   0        0        0     6248 2024-04-18 22:49:44.450317 replit_river-0.1.7b1/replit_river/server_transport.py
--rw-r--r--   0        0        0    13435 2024-04-18 21:13:20.653051 replit_river-0.1.7b1/replit_river/session.py
--rw-r--r--   0        0        0     2336 2024-04-18 08:09:29.872971 replit_river-0.1.7b1/replit_river/task_manager.py
--rw-r--r--   0        0        0     1208 2024-04-18 22:47:19.826728 replit_river-0.1.7b1/replit_river/transport.py
--rw-r--r--   0        0        0     1329 2024-04-18 08:30:42.434967 replit_river-0.1.7b1/replit_river/transport_options.py
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 replit_river-0.1.7b1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-19 19:26:13.426252 replit_river-0.1.7b2/LICENSE
+-rw-r--r--   0        0        0     1628 2024-04-19 19:26:13.426318 replit_river-0.1.7b2/README.md
+-rw-r--r--   0        0        0     1749 2024-04-23 01:28:51.361313 replit_river-0.1.7b2/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-22 19:50:44.355705 replit_river-0.1.7b2/replit_river/__init__.py
+-rw-r--r--   0        0        0     3860 2024-04-23 00:45:40.912922 replit_river-0.1.7b2/replit_river/client.py
+-rw-r--r--   0        0        0    11280 2024-04-23 00:45:40.913696 replit_river-0.1.7b2/replit_river/client_session.py
+-rw-r--r--   0        0        0     9904 2024-04-23 00:45:40.914351 replit_river-0.1.7b2/replit_river/client_transport.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:50:44.356674 replit_river-0.1.7b2/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-04-22 19:50:44.356784 replit_river-0.1.7b2/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13363 2024-04-22 19:50:44.356886 replit_river-0.1.7b2/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-04-22 19:50:44.356956 replit_river-0.1.7b2/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5356 2024-04-23 00:45:40.473122 replit_river-0.1.7b2/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12624 2024-04-23 00:45:40.507714 replit_river-0.1.7b2/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      547 2024-04-22 19:50:44.357515 replit_river-0.1.7b2/replit_river/error_schema.py
+-rw-r--r--   0        0        0        1 2024-04-22 19:50:44.357856 replit_river-0.1.7b2/replit_river/handshake.py
+-rw-r--r--   0        0        0     1302 2024-04-23 00:45:40.909781 replit_river-0.1.7b2/replit_river/message_buffer.py
+-rw-r--r--   0        0        0     2637 2024-04-23 00:45:40.912273 replit_river-0.1.7b2/replit_river/messages.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:50:44.358418 replit_river-0.1.7b2/replit_river/py.typed
+-rw-r--r--   0        0        0     1827 2024-04-23 00:45:40.911579 replit_river-0.1.7b2/replit_river/rate_limiter.py
+-rw-r--r--   0        0        0    12218 2024-04-22 19:50:44.358789 replit_river-0.1.7b2/replit_river/rpc.py
+-rw-r--r--   0        0        0     2102 2024-04-22 19:50:44.359301 replit_river-0.1.7b2/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     2294 2024-04-22 19:50:44.359622 replit_river-0.1.7b2/replit_river/server.py
+-rw-r--r--   0        0        0     7436 2024-04-23 00:45:40.912746 replit_river-0.1.7b2/replit_river/server_transport.py
+-rw-r--r--   0        0        0    19587 2024-04-23 02:08:03.880757 replit_river-0.1.7b2/replit_river/session.py
+-rw-r--r--   0        0        0     2336 2024-04-22 19:50:44.360278 replit_river-0.1.7b2/replit_river/task_manager.py
+-rw-r--r--   0        0        0     1473 2024-04-23 01:20:15.732925 replit_river-0.1.7b2/replit_river/transport.py
+-rw-r--r--   0        0        0     1432 2024-04-23 00:45:40.909656 replit_river-0.1.7b2/replit_river/transport_options.py
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 replit_river-0.1.7b2/PKG-INFO
```

### Comparing `replit_river-0.1.7b1/LICENSE` & `replit_river-0.1.7b2/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b1/README.md` & `replit_river-0.1.7b2/README.md`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b1/pyproject.toml` & `replit_river-0.1.7b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.1.7-beta.1"
+version="0.1.7-beta.2"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `replit_river-0.1.7b1/replit_river/client_session.py` & `replit_river-0.1.7b2/replit_river/client_session.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import logging
 from collections.abc import AsyncIterable, AsyncIterator
 from typing import Any, Callable, Optional, Union
 
 import nanoid  # type: ignore
 from aiochannel import Channel
 from aiochannel.errors import ChannelClosed
+
 from replit_river.error_schema import ERROR_CODE_STREAM_CLOSED, RiverException
-from replit_river.session import FailedSendingMessageException, Session
+from replit_river.session import Session
 
 from .rpc import (
     STREAM_CLOSED_BIT,
     STREAM_OPEN_BIT,
     ErrorType,
     InitType,
     RequestType,
@@ -31,37 +32,31 @@
         """Sends a single RPC request to the server.
 
         Expects the input and output be messages that will be msgpacked.
         """
         stream_id = nanoid.generate()
         output: Channel[Any] = Channel(1)
         self._streams[stream_id] = output
-        try:
-            await self.send_message(
-                ws=self._ws,
-                stream_id=stream_id,
-                control_flags=STREAM_OPEN_BIT | STREAM_CLOSED_BIT,
-                payload=request_serializer(request),
-                service_name=service_name,
-                procedure_name=procedure_name,
-            )
-        except FailedSendingMessageException:
-            raise RiverException(
-                ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
-            )
-
+        await self.send_message(
+            ws=self._ws,
+            stream_id=stream_id,
+            control_flags=STREAM_OPEN_BIT | STREAM_CLOSED_BIT,
+            payload=request_serializer(request),
+            service_name=service_name,
+            procedure_name=procedure_name,
+        )
         # Handle potential errors during communication
         try:
             try:
                 response = await output.get()
             except (RuntimeError, ChannelClosed) as e:
                 # if the stream is closed before we get a response, we will get a
                 # RuntimeError: RuntimeError: Event loop is closed
                 raise RiverException(
-                    ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
+                    ERROR_CODE_STREAM_CLOSED, f"Stream closed before response {e}"
                 )
             if not response.get("ok", False):
                 try:
                     error = error_deserializer(response["payload"])
                 except Exception as e:
                     raise RiverException("error_deserializer", str(e))
                 raise RiverException(error.code, error.message)
@@ -86,46 +81,45 @@
     ) -> ResponseType:
         """Sends an upload request to the server.
 
         Expects the input and output be messages that will be msgpacked.
         """
 
         stream_id = nanoid.generate()
-        output: Channel[Any] = Channel(1024)
+        output: Channel[Any] = Channel(1)
         self._streams[stream_id] = output
         first_message = True
         try:
             if init and init_serializer:
                 await self.send_message(
                     stream_id=stream_id,
                     ws=self._ws,
                     control_flags=STREAM_OPEN_BIT,
                     service_name=service_name,
                     procedure_name=procedure_name,
                     payload=init_serializer(init),
                 )
                 first_message = False
-
+            # If this request is not closed and the session is killed, we should
+            # throws exception here
             async for item in request:
                 control_flags = 0
                 if first_message:
                     control_flags = STREAM_OPEN_BIT
                     first_message = False
                 await self.send_message(
                     stream_id=stream_id,
                     ws=self._ws,
                     service_name=service_name,
                     procedure_name=procedure_name,
                     control_flags=control_flags,
                     payload=request_serializer(item),
                 )
-        except FailedSendingMessageException:
-            raise RiverException(
-                ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
-            )
+        except Exception as e:
+            raise RiverException(ERROR_CODE_STREAM_CLOSED, str(e))
         await self.send_close_stream(service_name, procedure_name, stream_id)
 
         # Handle potential errors during communication
         # TODO: throw a error when the transport is hard closed
         try:
             try:
                 response = await output.get()
@@ -162,27 +156,22 @@
         """Sends a subscription request to the server.
 
         Expects the input and output be messages that will be msgpacked.
         """
         stream_id = nanoid.generate()
         output: Channel[Any] = Channel(1024)
         self._streams[stream_id] = output
-        try:
-            await self.send_message(
-                ws=self._ws,
-                service_name=service_name,
-                procedure_name=procedure_name,
-                stream_id=stream_id,
-                control_flags=STREAM_OPEN_BIT,
-                payload=request_serializer(request),
-            )
-        except FailedSendingMessageException:
-            raise RiverException(
-                ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
-            )
+        await self.send_message(
+            ws=self._ws,
+            service_name=service_name,
+            procedure_name=procedure_name,
+            stream_id=stream_id,
+            control_flags=STREAM_OPEN_BIT,
+            payload=request_serializer(request),
+        )
 
         # Handle potential errors during communication
         try:
             async for item in output:
                 if item.get("type", None) == "CLOSE":
                     break
                 if not item.get("ok", False):
@@ -241,18 +230,16 @@
                     service_name=service_name,
                     procedure_name=procedure_name,
                     stream_id=stream_id,
                     control_flags=STREAM_OPEN_BIT,
                     payload=request_serializer(first),
                 )
 
-        except FailedSendingMessageException:
-            raise RiverException(
-                ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
-            )
+        except Exception as e:
+            raise RiverException(ERROR_CODE_STREAM_CLOSED, str(e))
 
         # Create the encoder task
         async def _encode_stream() -> None:
             async for item in request:
                 if item is None:
                     continue
                 await self.send_message(
```

### Comparing `replit_river-0.1.7b1/replit_river/codegen/client.py` & `replit_river-0.1.7b2/replit_river/codegen/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b1/replit_river/codegen/run.py` & `replit_river-0.1.7b2/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b1/replit_river/codegen/schema.py` & `replit_river-0.1.7b2/replit_river/codegen/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     """Generates the type of a protobuf message into Typebox descriptions."""
     type: Dict[str, Any] = {
         "type": "object",
         "properties": {},
         "required": [],
     }
     # Non-oneof fields.
-    oneofs: DefaultDict[
-        int, List[descriptor_pb2.FieldDescriptorProto]
-    ] = collections.defaultdict(list)
+    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
+        collections.defaultdict(list)
+    )
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         if field.type == descriptor_pb2.FieldDescriptorProto.TYPE_MESSAGE:
             # TODO: implement
             pass
```

### Comparing `replit_river-0.1.7b1/replit_river/codegen/server.py` & `replit_river-0.1.7b2/replit_river/codegen/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         "  d: Mapping[str, Any],",
         f") -> {module_name}_pb2.{m.name}:",
         f"  m = {module_name}_pb2.{m.name}()",
         "  if d is None:",
         "    return m",
     ]
     # Non-oneof fields.
-    oneofs: DefaultDict[
-        int, List[descriptor_pb2.FieldDescriptorProto]
-    ] = collections.defaultdict(list)
+    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
+        collections.defaultdict(list)
+    )
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         chunks.append(
             f"  if d.get('{to_camel_case(field.name)}') is not None:",
         )
@@ -153,17 +153,17 @@
     chunks = [
         f"def _{m.name}Encoder(",
         f"  e: {module_name}_pb2.{m.name}",
         ") -> Dict[str, Any]:",
         "  d: Dict[str, Any] = {}",
     ]
     # Non-oneof fields.
-    oneofs: DefaultDict[
-        int, List[descriptor_pb2.FieldDescriptorProto]
-    ] = collections.defaultdict(list)
+    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
+        collections.defaultdict(list)
+    )
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         value: str
         if field.type_name == ".google.protobuf.Timestamp":
             value = f"_{field.name}.ToDatetime(tzinfo=datetime.timezone.utc)"
```

### Comparing `replit_river-0.1.7b1/replit_river/message_buffer.py` & `replit_river-0.1.7b2/replit_river/message_buffer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import asyncio
+import logging
 from typing import Optional
+
 from replit_river.rpc import TransportMessage
 
 
 class MessageBuffer:
     """A buffer to strore messages and support current updates"""
 
     def __init__(self, max_size: int = 1000):
         self.max_size = max_size
         self.buffer: list[TransportMessage] = []
         self._lock = asyncio.Lock()
 
-    async def is_empty(self) -> bool:
+    async def empty(self) -> bool:
         """Check if the buffer is empty"""
         async with self._lock:
             return len(self.buffer) == 0
 
-    async def add(self, message: TransportMessage) -> None:
+    async def put(self, message: TransportMessage) -> None:
         """Add a message to the buffer"""
         async with self._lock:
             if len(self.buffer) >= self.max_size:
-                self.buffer.pop(0)
+                logging.error("Buffer is full, dropping message")
+                raise ValueError("Buffer is full")
             self.buffer.append(message)
 
     async def peek(self) -> Optional[TransportMessage]:
         """Peek the first message in the buffer"""
         async with self._lock:
             if len(self.buffer) == 0:
                 return None
```

### Comparing `replit_river-0.1.7b1/replit_river/messages.py` & `replit_river-0.1.7b2/replit_river/messages.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import logging
+from typing import Any, Callable, Coroutine
 
 import msgpack  # type: ignore
 import websockets
 from pydantic import ValidationError
 from pydantic_core import ValidationError as PydanticCoreValidationError
 from websockets import (
     WebSocketCommonProtocol,
 )
 
 from replit_river.rpc import (
     TransportMessage,
 )
 from replit_river.seq_manager import (
-    IgnoreTransportMessageException,
-    InvalidTransportMessageException,
+    IgnoreMessageException,
+    InvalidMessageException,
 )
 from replit_river.transport_options import TransportOptions
 
 
 class FailedSendingMessageException(Exception):
     pass
 
@@ -25,59 +26,61 @@
 PROTOCOL_VERSION = "v1"
 
 CROSIS_PREFIX_BYTES = b"\x00\x00"
 PID2_PREFIX_BYTES = b"\xff\xff"
 
 
 async def send_transport_message(
-    msg: TransportMessage, ws: WebSocketCommonProtocol, prefix_bytes: bytes = b""
+    msg: TransportMessage,
+    ws: WebSocketCommonProtocol,
+    websocket_closed_callback: Callable[[], Coroutine[Any, Any, None]],
+    prefix_bytes: bytes = b"",
 ) -> None:
-    logging.debug("sent a message %r", msg)
+    logging.debug(f"sending a message {msg} to ws {ws.id} with state {ws.state}")
     try:
         await ws.send(
             prefix_bytes
             + msgpack.packb(
                 msg.model_dump(by_alias=True, exclude_none=True), datetime=True
             )
         )
     except websockets.exceptions.ConnectionClosed as e:
+        await websocket_closed_callback()
         raise e
     except Exception as e:
         raise FailedSendingMessageException(f"Exception during send message : {e}")
 
 
 def formatted_bytes(message: bytes) -> str:
     return " ".join(f"{b:02x}" for b in message)
 
 
 def parse_transport_msg(
     message: str | bytes, transport_options: TransportOptions
 ) -> TransportMessage:
     if isinstance(message, str):
-        raise IgnoreTransportMessageException(
+        raise IgnoreMessageException(
             "ignored a message beacuse it was a text frame: %r", message
         )
     if transport_options.use_prefix_bytes:
         if message.startswith(CROSIS_PREFIX_BYTES):
-            raise IgnoreTransportMessageException("Skip crosis message")
+            raise IgnoreMessageException("Skip crosis message")
         elif message.startswith(PID2_PREFIX_BYTES):
             message = message[len(PID2_PREFIX_BYTES) :]
         else:
-            raise InvalidTransportMessageException(
+            raise InvalidMessageException(
                 "Got message without prefix bytes: " f"{formatted_bytes(message)}"
             )
     try:
         unpacked_message = msgpack.unpackb(message, timestamp=3)
     except (msgpack.UnpackException, msgpack.exceptions.ExtraData):
-        raise InvalidTransportMessageException("received non-msgpack message")
+        raise InvalidMessageException("received non-msgpack message")
     try:
         msg = TransportMessage(**unpacked_message)
     except (
         ValidationError,
         ValueError,
         msgpack.UnpackException,
         PydanticCoreValidationError,
     ):
-        raise InvalidTransportMessageException(
-            f"failed to parse message:{message.decode()}"
-        )
+        raise InvalidMessageException(f"failed to parse message:{message.decode()}")
     return msg
```

### Comparing `replit_river-0.1.7b1/replit_river/rpc.py` & `replit_river-0.1.7b2/replit_river/rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,22 @@
     Sequence,
     Tuple,
     TypeVar,
     Union,
 )
 
 import grpc
-from aiochannel import Channel
+from aiochannel import Channel, ChannelClosed
 from pydantic import BaseModel, ConfigDict, Field
 
-from replit_river.error_schema import RiverError
+from replit_river.error_schema import (
+    ERROR_CODE_STREAM_CLOSED,
+    RiverError,
+    RiverException,
+)
 
 InitType = TypeVar("InitType")
 RequestType = TypeVar("RequestType")
 ResponseType = TypeVar("ResponseType")
 ErrorType = TypeVar("ErrorType", bound=RiverError)
 
 _MetadataType = Union[grpc.aio.Metadata, Sequence[Tuple[str, Union[str, bytes]]]]
@@ -192,15 +196,15 @@
                         "code": grpc.StatusCode(context._abort_code).name,
                         "message": f"{method.__name__} threw an exception: "
                         f"{context._abort_details}",
                     },
                 }
             )
         except Exception as e:
-            logging.exception("Uncaught exception")
+            logging.exception("Uncaught exception during river rpc")
             await output.put(
                 {
                     "ok": False,
                     "payload": {
                         "code": "UNCAUGHT_EXCEPTION",
                         "message": f"{method.__name__} threw an exception: {e}",
                     },
@@ -239,15 +243,15 @@
                         "code": grpc.StatusCode(context._abort_code).name,
                         "message": f"{method.__name__} threw an exception: "
                         f"{context._abort_details}",
                     },
                 }
             )
         except Exception as e:
-            logging.exception("Uncaught exception in subscription")
+            logging.exception("Uncaught exception in river server subscription")
             await output.put(
                 {
                     "ok": False,
                     "payload": {
                         "code": "UNCAUGHT_EXCEPTION",
                         "message": f"{method.__name__} threw an exception: {e}",
                     },
@@ -285,16 +289,18 @@
 
             async def _convert_outputs() -> None:
                 try:
                     response = await method(request, context)
                     await output.put(
                         get_response_or_error_payload(response, response_serializer)
                     )
+                except ChannelClosed:
+                    raise RiverException(ERROR_CODE_STREAM_CLOSED, "Channel closed")
                 except Exception as e:
-                    print("upload caught exception", e)
+                    logging.error("Uncaught exception in river server upload")
                     await output.put(
                         {
                             "ok": False,
                             "payload": {
                                 "code": "UNCAUGHT_EXCEPTION",
                                 "message": f"{method.__name__} threw an exception: {e}",
                             },
@@ -358,15 +364,15 @@
                 finally:
                     output.close()
 
             convert_inputs_task = asyncio.create_task(_convert_inputs())
             convert_outputs_task = asyncio.create_task(_convert_outputs())
             await asyncio.wait((convert_inputs_task, convert_outputs_task))
         except grpc.RpcError:
-            logging.exception("Uncaught exception in stream")
+            logging.exception("RPC exception in stream")
             await output.put(
                 {
                     "ok": False,
                     "payload": {
                         "code": grpc.StatusCode(context._abort_code).name,
                         "message": f"{method.__name__} threw an exception: "
                         f"{context._abort_details}",
```

### Comparing `replit_river-0.1.7b1/replit_river/seq_manager.py` & `replit_river-0.1.7b2/replit_river/seq_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
 
 from replit_river.rpc import TransportMessage
 
 
-class IgnoreTransportMessageException(Exception):
+class IgnoreMessageException(Exception):
     """Exception to ignore a transport message, but good to continue."""
 
     pass
 
 
-class InvalidTransportMessageException(Exception):
+class InvalidMessageException(Exception):
     """Error processing a transport message, should raise a exception."""
 
     pass
 
 
 class SeqManager:
     """Manages the sequence number and ack number for a connection."""
@@ -49,20 +49,20 @@
         async with self._ack_lock:
             return self.ack
 
     async def check_seq_and_update(self, msg: TransportMessage) -> None:
         async with self._ack_lock:
             if msg.seq != self.ack:
                 if msg.seq < self.ack:
-                    raise IgnoreTransportMessageException(
+                    raise IgnoreMessageException(
                         f"{msg.from_} received duplicate msg, got {msg.seq}"
                         f" expected {self.ack}"
                     )
                 else:
-                    raise InvalidTransportMessageException(
+                    raise InvalidMessageException(
                         f"{msg.from_} received out of order, got {msg.seq}"
                         f" expected {self.ack}"
                     )
             self.receiver_ack = msg.ack
         await self._set_ack(msg.seq + 1)
 
     async def _set_ack(self, new_ack: int) -> int:
```

### Comparing `replit_river-0.1.7b1/replit_river/server.py` & `replit_river-0.1.7b2/replit_river/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import Mapping, Tuple
 
-from websockets.exceptions import ConnectionClosedError
+from websockets.exceptions import ConnectionClosed
 from websockets.server import WebSocketServerProtocol
 
 from replit_river.server_transport import ServerTransport
 from replit_river.transport import TransportOptions
 
 from .rpc import (
     GenericRpcHandler,
@@ -19,31 +19,43 @@
         self._transport = ServerTransport(
             transport_id=self._server_id,
             transport_options=transport_options,
             is_server=True,
         )
 
     async def close(self) -> None:
+        logging.info(f"river server {self._server_id} start closing")
         await self._transport.close_all_sessions()
+        logging.info(f"river server {self._server_id} closed")
 
     def add_rpc_handlers(
         self,
         rpc_handlers: Mapping[Tuple[str, str], Tuple[str, GenericRpcHandler]],
     ) -> None:
         self._transport._handlers.update(rpc_handlers)
 
     async def serve(self, websocket: WebSocketServerProtocol) -> None:
-        logging.debug("River server started establishing session")
+        logging.debug(
+            f"River server started establishing session with ws: {websocket.id}"
+            f" {websocket.state}"
+        )
         try:
-            session = await self._transport.establish_session(websocket)
+            session = await self._transport.handshake_to_get_session(websocket)
         except Exception as e:
             logging.error(f"Error establishing handshake, closing websocket: {e}")
             await websocket.close()
             return
         logging.debug("River server session established, start serving messages")
+
         try:
-            await session._serve()
-        except ConnectionClosedError as e:
-            logging.debug(f"ConnectionClosedError while serving {e}")
+            # Session serve will be closed in two cases
+            #   1. websocket is closed
+            #   2. exception thrown
+            # session should be kept in order to be reused by the reconnect within the
+            # grace period.
+            await session.serve()
+        except ConnectionClosed as e:
+            logging.debug(f"ConnectionClosed while serving {e}")
+            # We don't have to close the websocket here, it is already closed.
         except Exception as e:
             logging.error(f"River transport error in server {self._server_id}: {e}")
             await websocket.close()
```

### Comparing `replit_river-0.1.7b1/replit_river/server_transport.py` & `replit_river-0.1.7b2/replit_river/server_transport.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import asyncio
 import logging
 from typing import Optional
 
 import nanoid  # type: ignore  # type: ignore
 from pydantic import ValidationError
 from websockets import (
     WebSocketCommonProtocol,
     WebSocketServerProtocol,
 )
+from websockets.exceptions import ConnectionClosed
 from websockets.server import WebSocketServerProtocol
 
 from replit_river.messages import (
     FailedSendingMessageException,
     parse_transport_msg,
     send_transport_message,
 )
 from replit_river.rpc import (
     ControlMessageHandshakeRequest,
     ControlMessageHandshakeResponse,
     HandShakeStatus,
     TransportMessage,
 )
 from replit_river.seq_manager import (
-    IgnoreTransportMessageException,
-    InvalidTransportMessageException,
+    IgnoreMessageException,
+    InvalidMessageException,
 )
 from replit_river.session import Session
 from replit_river.transport import PROTOCOL_VERSION, Transport
 
 
 class ServerTransport(Transport):
     async def get_or_create_session(
@@ -36,82 +36,91 @@
         to_id: str,
         instance_id: str,
         websocket: WebSocketCommonProtocol,
     ) -> Session:
         session_to_close: Optional[Session] = None
         async with self._session_lock:
             if to_id not in self._sessions:
+                logging.debug(
+                    f'Creating new session with "{to_id}" using ws: {websocket.id}'
+                )
                 self._sessions[to_id] = Session(
                     transport_id,
                     to_id,
                     instance_id,
                     websocket,
                     self._transport_options,
-                    self._delete_session,
                     self._is_server,
                     self._handlers,
+                    close_session_callback=self._delete_session,
                 )
             else:
                 old_session = self._sessions[to_id]
                 if old_session._instance_id != instance_id:
                     session_to_close = old_session
                     self._sessions[to_id] = Session(
                         transport_id,
                         to_id,
                         instance_id,
                         websocket,
                         self._transport_options,
-                        self._delete_session,
                         self._is_server,
                         self._handlers,
+                        close_session_callback=self._delete_session,
                     )
                 else:
                     # If the instance id is the same, we reuse the session and assign
                     # a new websocket to it.
+                    logging.debug(
+                        f'Reuse old session with "{to_id}" using new ws: {websocket.id}'
+                    )
                     try:
                         await old_session.replace_with_new_websocket(websocket)
                     except FailedSendingMessageException as e:
                         raise e
         if session_to_close:
             logging.info("Closing stale websocket")
-            await session_to_close.close()
+            await session_to_close.close(False)
         session = self._sessions[to_id]
         return session
 
-    async def establish_session(
+    async def handshake_to_get_session(
         self,
         websocket: WebSocketServerProtocol,
     ) -> Session:
         async for message in websocket:
             try:
                 msg = parse_transport_msg(message, self._transport_options)
-                handshake_request = await self._build_handshake_from_request(
-                    msg, websocket
-                )
-            except IgnoreTransportMessageException:
+                handshake_request = await self._establish_handshake(msg, websocket)
+            except IgnoreMessageException:
                 continue
-            except InvalidTransportMessageException:
+            except InvalidMessageException:
                 error_msg = "Got invalid transport message, closing connection"
-                raise InvalidTransportMessageException(error_msg)
+                raise InvalidMessageException(error_msg)
+            except FailedSendingMessageException as e:
+                raise e
             logging.debug("handshake success on server: %r", handshake_request)
-            transport_id = msg.from_
-            to_id = msg.to
+            transport_id = msg.to
+            to_id = msg.from_
             instance_id = handshake_request.instanceId
             try:
                 session = await self.get_or_create_session(
-                    transport_id, to_id, instance_id, websocket
+                    transport_id,
+                    to_id,
+                    instance_id,
+                    websocket,
                 )
             except Exception as e:
                 error_msg = (
                     "Error building sessions from handshake request : "
                     f"client_id: {transport_id}, instance_id: {instance_id}, error: {e}"
                 )
-                raise InvalidTransportMessageException(error_msg)
+                raise InvalidMessageException(error_msg)
             return session
-        raise InvalidTransportMessageException("No handshake message received")
+        raise InvalidMessageException("No handshake message received")
 
     async def _send_handshake_response(
         self,
         request_message: TransportMessage,
         handshake_status: HandShakeStatus,
         websocket: WebSocketCommonProtocol,
     ) -> TransportMessage:
@@ -126,42 +135,61 @@
             seq=0,
             ack=0,
             controlFlags=0,
             payload=response.model_dump(by_alias=True, exclude_none=True),
             serviceName=request_message.serviceName,
             procedureName=request_message.procedureName,
         )
-        await send_transport_message(response_message, websocket)
+
+        async def websocket_closed_callback() -> None:
+            logging.error("websocket closed before handshake response")
+
+        try:
+            await send_transport_message(
+                response_message, websocket, websocket_closed_callback
+            )
+        except (FailedSendingMessageException, ConnectionClosed) as e:
+            raise FailedSendingMessageException(
+                f"Failed sending handshake response: {e}"
+            )
         return response_message
 
-    async def _build_handshake_from_request(
+    async def _establish_handshake(
         self, request_message: TransportMessage, websocket: WebSocketCommonProtocol
     ) -> ControlMessageHandshakeRequest:
         try:
             handshake_request = ControlMessageHandshakeRequest(
                 **request_message.payload
             )
+            logging.debug('Got handshake request "%r"', handshake_request)
         except (ValidationError, ValueError):
             await self._send_handshake_response(
                 request_message,
                 HandShakeStatus(ok=False, reason="failed validate handshake request"),
                 websocket,
             )
-            raise InvalidTransportMessageException("failed validate handshake request")
+            raise InvalidMessageException("failed validate handshake request")
 
         if handshake_request.protocolVersion != PROTOCOL_VERSION:
             await self._send_handshake_response(
                 request_message,
                 HandShakeStatus(ok=False, reason="protocol version mismatch"),
                 websocket,
             )
             error_str = (
                 "protocol version mismatch: "
                 + f"{handshake_request.protocolVersion} != {PROTOCOL_VERSION}"
             )
-            raise InvalidTransportMessageException(error_str)
+            raise InvalidMessageException(error_str)
+        if request_message.to != self._transport_id:
+            await self._send_handshake_response(
+                request_message,
+                HandShakeStatus(ok=False, reason="handshake request to wrong server"),
+                websocket,
+            )
+            raise InvalidMessageException("handshake request to wrong server")
         await self._send_handshake_response(
             request_message,
             HandShakeStatus(ok=True, instanceId=self._transport_id),
             websocket,
         )
         return handshake_request
```

### Comparing `replit_river-0.1.7b1/replit_river/session.py` & `replit_river-0.1.7b2/replit_river/session.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,165 +1,329 @@
 import asyncio
+import enum
 import logging
 from typing import Any, Callable, Coroutine, Dict, Optional, Tuple
 
 import nanoid  # type: ignore
 import websockets
-from aiochannel import Channel
+from aiochannel import Channel, ChannelClosed
 from websockets import WebSocketCommonProtocol
-from websockets.exceptions import ConnectionClosedError
-from websockets.server import WebSocketServerProtocol
+from websockets.exceptions import ConnectionClosed
 
+from replit_river.message_buffer import MessageBuffer
 from replit_river.messages import (
     FailedSendingMessageException,
     parse_transport_msg,
     send_transport_message,
 )
 from replit_river.seq_manager import (
-    IgnoreTransportMessageException,
-    InvalidTransportMessageException,
+    IgnoreMessageException,
+    InvalidMessageException,
     SeqManager,
 )
 from replit_river.task_manager import BackgroundTaskManager
 from replit_river.transport_options import TransportOptions
 
 from .rpc import (
     ACK_BIT,
     STREAM_CLOSED_BIT,
     STREAM_OPEN_BIT,
     GenericRpcHandler,
     TransportMessage,
 )
 
 
+class SessionState(enum.Enum):
+    ACTIVE = 0
+    CLOSING = 3
+    CLOSED = 4
+
+
+class WsState(enum.Enum):
+    OPEN = 0
+    CLOSING = 2
+    CLOSED = 3
+
+
 class Session(object):
     """A transport object that handles the websocket connection with a client."""
 
     def __init__(
         self,
         transport_id: str,
         to_id: str,
         instance_id: str,
         websocket: websockets.WebSocketCommonProtocol,
         transport_options: TransportOptions,
-        close_session_callback: Callable[["Session"], Coroutine[Any, Any, None]],
         is_server: bool,
         handlers: Dict[Tuple[str, str], Tuple[str, GenericRpcHandler]],
+        close_session_callback: Callable[["Session"], Coroutine[Any, Any, None]],
+        retry_connection_callback: Optional[
+            Callable[
+                ["Session"],
+                Coroutine[Any, Any, None],
+            ]
+        ] = None,
     ) -> None:
         self._transport_id = transport_id
         self._to_id = to_id
         self._instance_id = instance_id
         self._handlers = handlers
-        self._ws = websocket
-        self._close_session_callback = close_session_callback
         self._is_server = is_server
-        self._streams: Dict[str, Channel[Any]] = {}
         self._transport_options = transport_options
+
+        # session state, only modified during closing
+        self._state = SessionState.ACTIVE
+        self._state_lock = asyncio.Lock()
+        self._close_session_callback = close_session_callback
+        self._close_session_after_time_secs: Optional[float] = None
+
+        # ws state
+        self._ws_lock = asyncio.Lock()
+        self._ws_state = WsState.OPEN
+        self._ws = websocket
+        self._heartbeat_misses = 0
+        self._retry_connection_callback = retry_connection_callback
+
+        # stream for tasks
+        self._stream_lock = asyncio.Lock()
+        self._streams: Dict[str, Channel[Any]] = {}
+
+        # book keeping
         self._seq_manager = SeqManager()
+        self._buffer = MessageBuffer(self._transport_options.buffer_size)
         self._task_manager = BackgroundTaskManager()
-        self._buffer: asyncio.Queue[TransportMessage] = asyncio.Queue(1000)
-        self._lock = asyncio.Lock()
-        self.heartbeat_misses = 0
-        # should disconnect after this time
-        self._disconnect_after_this_time: Optional[float] = None
-        asyncio.create_task(self._task_manager.create_task(self._heartbeat(self._ws)))
 
-    async def replace_with_new_websocket(
-        self, websocket: websockets.WebSocketCommonProtocol
-    ) -> None:
-        logging.info("replacing with new websocket")
-        if self._ws:
-            await self.close_stale_connection(self._ws)
-        self.cancel_disconnect_grace_period()
-        await self._send_buffered_messages(websocket)
-        self._ws = websocket
+        asyncio.create_task(self._setup_heartbeats_task())
 
-    async def _get_current_time(self) -> float:
-        return asyncio.get_event_loop().time()
+    async def _setup_heartbeats_task(self) -> None:
+        await self._task_manager.create_task(self._heartbeat())
+        await self._task_manager.create_task(self._check_to_close_session())
+
+    async def is_session_open(self) -> bool:
+        async with self._state_lock:
+            return self._state == SessionState.ACTIVE
+
+    async def is_websocket_open(self) -> bool:
+        async with self._ws_lock:
+            return self._ws_state == WsState.OPEN
+
+    async def _on_websocket_unexpected_close(self) -> None:
+        """Handle unexpected websocket close."""
+        logging.info(
+            f"Unexpected websocket close from {self._transport_id} to {self._to_id}"
+        )
+        await self._begin_close_session_countdown()
 
-    async def begin_grace(self) -> None:
-        if self._disconnect_after_this_time:
+    async def _begin_close_session_countdown(self) -> None:
+        """Begin the countdown to close session, this should be called when
+        websocket is closed.
+        """
+        logging.debug("begin_close_session_countdown")
+        if self._close_session_after_time_secs is not None:
+            # already in grace period, no need to set again
             return
         logging.debug(
             f"websocket closed from {self._transport_id} to {self._to_id}, "
             "begin grace period"
         )
         grace_period_ms = self._transport_options.session_disconnect_grace_ms
-        self._disconnect_after_this_time = (
+        self._close_session_after_time_secs = (
             await self._get_current_time() + grace_period_ms / 1000
         )
 
-    def cancel_disconnect_grace_period(self) -> None:
-        self.heartbeat_misses = 0
-        self._disconnect_after_this_time = None
-        logging.info(f"Grace period cancelled for session to {self._transport_id}")
+    async def serve(self) -> None:
+        """Serve messages from the websocket."""
+        try:
+            async with asyncio.TaskGroup() as tg:
+                try:
+                    await self._handle_messages_from_ws(self._ws, tg)
+                except ConnectionClosed as e:
+                    await self._on_websocket_unexpected_close()
+                    logging.debug(f"ConnectionClosed while serving: {e}")
+                except FailedSendingMessageException as e:
+                    # Expected error if the connection is closed.
+                    logging.debug(f"FailedSendingMessageException while serving: {e}")
+                except Exception:
+                    logging.exception("caught exception at message iterator")
+        except ExceptionGroup as eg:
+            _, unhandled = eg.split(lambda e: isinstance(e, ConnectionClosed))
+            if unhandled:
+                raise ExceptionGroup(
+                    "Unhandled exceptions on River server", unhandled.exceptions
+                )
+
+    async def _update_book_keeping(self, msg: TransportMessage) -> None:
+        await self._seq_manager.check_seq_and_update(msg)
+        await self._remove_acked_messages_in_buffer()
+        self._reset_session_close_countdown()
+
+    async def _handle_messages_from_ws(
+        self, websocket: WebSocketCommonProtocol, tg: Optional[asyncio.TaskGroup] = None
+    ) -> None:
+        logging.debug(
+            f'{"server" if self._is_server else "client"} start handling messages from'
+            f" ws {websocket.id}, state {websocket.state}"
+        )
+        try:
+            async for message in websocket:
+                try:
+                    msg = parse_transport_msg(message, self._transport_options)
+
+                    logging.debug(f"{self._transport_id} got a message %r", msg)
+
+                    await self._update_book_keeping(msg)
+                    if msg.controlFlags & ACK_BIT != 0:
+                        continue
+                    async with self._stream_lock:
+                        stream = self._streams.get(msg.streamId, None)
+                    if msg.controlFlags & STREAM_OPEN_BIT == 0:
+                        if not stream:
+                            logging.warning("no stream for %s", msg.streamId)
+                            raise IgnoreMessageException(
+                                "no stream for message, ignoring"
+                            )
+                        await self._add_msg_to_stream(msg, stream)
+                    else:
+                        stream = await self._open_stream_and_call_handler(
+                            msg, stream, tg
+                        )
+
+                    if msg.controlFlags & STREAM_CLOSED_BIT != 0:
+                        if stream:
+                            stream.close()
+                        async with self._stream_lock:
+                            del self._streams[msg.streamId]
+                except IgnoreMessageException as e:
+                    logging.debug(f"Ignoring transport message : {e}")
+                    continue
+                except InvalidMessageException as e:
+                    logging.error(
+                        f"Got invalid transport message, closing session : {e}"
+                    )
+                    await self.close(True)
+                    return
+        except ConnectionClosed as e:
+            raise e
+
+    async def replace_with_new_websocket(
+        self, new_ws: websockets.WebSocketCommonProtocol
+    ) -> None:
+        async with self._ws_lock:
+            old_ws = self._ws
+            self._ws_state = WsState.CLOSING
+        if new_ws.id != old_ws.id:
+            self._reset_session_close_countdown()
+            await self.close_websocket(old_ws, should_retry=False)
+        async with self._ws_lock:
+            self._ws = new_ws
+            self._ws_state = WsState.OPEN
+        await self._send_buffered_messages(new_ws)
+        # Server will call serve itself.
+        if not self._is_server:
+            await self.start_serve_responses()
+
+    async def _get_current_time(self) -> float:
+        return asyncio.get_event_loop().time()
+
+    def _reset_session_close_countdown(self) -> None:
+        self._heartbeat_misses = 0
+        self._close_session_after_time_secs = None
+
+    async def _check_to_close_session(self) -> None:
+        while True:
+            await asyncio.sleep(
+                self._transport_options.close_session_check_interval_ms / 1000
+            )
+            if not self._close_session_after_time_secs:
+                continue
+            current_time = await self._get_current_time()
+            if current_time > self._close_session_after_time_secs:
+                logging.info(
+                    "Grace period ended for :" f" {self._transport_id}, closing session"
+                )
+                await self.close(False)
+                return
 
     async def _heartbeat(
         self,
-        websocket: WebSocketCommonProtocol,
     ) -> None:
         logging.debug("Start heartbeat")
         while True:
             await asyncio.sleep(self._transport_options.heartbeat_ms / 1000)
-            current_time = await self._get_current_time()
-            if self._disconnect_after_this_time:
-                if current_time > self._disconnect_after_this_time:
-                    logging.info(
-                        "Grace period ended for :"
-                        f" {self._transport_id}, closing websocket"
-                    )
-                    await self.close()
-                    return
+            if self._state != SessionState.ACTIVE:
+                logging.debug(
+                    f"Session is closed, no need to send heartbeat, state : "
+                    f"{self._state} close_session_after_this: "
+                    f"{self._close_session_after_time_secs}"
+                )
+                # session is closing, no need to send heartbeat
                 continue
-            if self.heartbeat_misses >= self._transport_options.heartbeats_until_dead:
-                logging.info("Heartbeat timed out for :" f" {self._transport_id}")
-                await self.close_stale_connection(websocket)
-                await self.begin_grace()
-                return
             try:
                 await self.send_message(
                     str(nanoid.generate()),
-                    websocket,
                     {
                         "ack": 0,
                     },
+                    self._ws,
                     ACK_BIT,
                 )
-                self.heartbeat_misses += 1
-            except ConnectionClosedError:
-                logging.debug("heartbeat failed")
-                return
+                self._heartbeat_misses += 1
+                if (
+                    self._heartbeat_misses
+                    >= self._transport_options.heartbeats_until_dead
+                ):
+                    logging.debug("closing websocket because of heartbeat misses")
+                    await self._on_websocket_unexpected_close()
+                    await self.close_websocket(
+                        self._ws, should_retry=not self._is_server
+                    )
+                    continue
+            except FailedSendingMessageException:
+                # this is expected during websocket closed period
+                continue
 
     async def _send_buffered_messages(
         self, websocket: websockets.WebSocketCommonProtocol
     ) -> None:
-        while not self._buffer.empty():
-            msg = await self._buffer.get()
+        buffered_messages = list(self._buffer.buffer)
+        for msg in buffered_messages:
             try:
-                await send_transport_message(msg, websocket)
-            except (
-                websockets.exceptions.ConnectionClosed,
-                FailedSendingMessageException,
-            ) as e:
-                # Put the message back, they need to be resent
-                async with self._lock:
-                    msg_not_sent = [msg]
-                    while not self._buffer.empty():
-                        msg_not_sent.append(await self._buffer.get())
-                    for msg in msg_not_sent:
-                        self._buffer.put_nowait(msg)
-                raise FailedSendingMessageException(
-                    f"Failed to resend message during reconnecting : {e}"
+                await self._send_transport_message(
+                    msg,
+                    websocket,
+                    prefix_bytes=self._transport_options.get_prefix_bytes(),
                 )
+            except ConnectionClosed as e:
+                logging.info(f"Connection closed while sending buffered messages : {e}")
+                break
+            except FailedSendingMessageException as e:
+                logging.error(f"Error while sending buffered messages : {e}")
+                break
+
+    async def _send_transport_message(
+        self,
+        msg: TransportMessage,
+        ws: WebSocketCommonProtocol,
+        prefix_bytes: bytes = b"",
+    ) -> None:
+        try:
+            await send_transport_message(
+                msg, ws, self._on_websocket_unexpected_close, prefix_bytes
+            )
+        except ConnectionClosed as e:
+            raise e
+        except FailedSendingMessageException as e:
+            raise e
 
     async def send_message(
         self,
         stream_id: str,
+        payload: Dict | str,
         ws: WebSocketCommonProtocol,
-        payload: Dict,
         control_flags: int = 0,
         service_name: str | None = None,
         procedure_name: str | None = None,
     ) -> None:
         """Send serialized messages to the websockets."""
         msg = TransportMessage(
             streamId=stream_id,
@@ -169,186 +333,182 @@
             seq=await self._seq_manager.get_seq_and_increment(),
             ack=await self._seq_manager.get_ack(),
             controlFlags=control_flags,
             payload=payload,
             serviceName=service_name,
             procedureName=procedure_name,
         )
-        self._buffer.put_nowait(msg)
         try:
-            await send_transport_message(
+            await self._buffer.put(msg)
+        except Exception:
+            # We should close the session when there are too many messages in buffer
+            await self.close(True)
+            return
+        try:
+            await self._send_transport_message(
                 msg,
                 ws,
                 prefix_bytes=self._transport_options.get_prefix_bytes(),
             )
-        except websockets.ConnectionClosed:
-            await self.begin_grace()
+        except ConnectionClosed as e:
+            logging.error(
+                f"Connection closed while sending message : {e}, waiting for "
+                "retry from buffer"
+            )
+        except FailedSendingMessageException as e:
+            logging.error(
+                f"Failed sending message : {e}, waiting for retry from buffer"
+            )
 
-    async def send_responses(
+    async def _send_responses_from_output_stream(
         self,
         stream_id: str,
-        ws: WebSocketCommonProtocol,
         output: Channel[Any],
-        is_stream: bool,
+        is_streaming_output: bool,
     ) -> None:
         """Send serialized messages to the websockets."""
-        logging.debug("sent response of stream %r", stream_id)
-        async for payload in output:
-            if not is_stream:
-                await self.send_message(stream_id, ws, payload, STREAM_CLOSED_BIT)
-                return
-            await self.send_message(stream_id, ws, payload)
-        logging.debug("sent an end of stream %r", stream_id)
-        await self.send_message(stream_id, ws, {"type": "CLOSE"}, STREAM_CLOSED_BIT)
+        try:
+            async for payload in output:
+                # TODO: what if the websocket changed during this?
+                ws = self._ws
+                while self._ws_state != WsState.OPEN:
+                    await asyncio.sleep(
+                        self._transport_options.close_session_check_interval_ms / 1000
+                    )
+                    ws = self._ws
+                if not is_streaming_output:
+                    await self.send_message(stream_id, payload, ws, STREAM_CLOSED_BIT)
+                    return
+                await self.send_message(stream_id, payload, ws)
+            logging.debug("sent an end of stream %r", stream_id)
+            await self.send_message(stream_id, {"type": "CLOSE"}, ws, STREAM_CLOSED_BIT)
+        except FailedSendingMessageException as e:
+            logging.error(
+                f"Error while sending responses, ws_state: {ws.state}, {type(e)} : {e}"
+            )
+        except (RuntimeError, ChannelClosed) as e:
+            logging.error(
+                f"Error while sending responses, ws_state: {ws.state} {type(e)} : {e}"
+            )
+        except Exception as e:
+            logging.error(f"Unknown error while river sending responses back : {e}")
 
-    async def close_stale_connection(self, websocket: WebSocketCommonProtocol) -> None:
-        logging.info(
-            f"river session from {self._transport_id} to {self._to_id} "
-            "closing stale connection"
-        )
-        if websocket:
-            await websocket.close()
+    async def close_websocket(
+        self, ws: WebSocketCommonProtocol, should_retry: bool
+    ) -> None:
+        """Mark the websocket as closed, close the websocket, and retry if needed."""
+        async with self._ws_lock:
+            if self._ws.id != ws.id:
+                # already replaced with new ws
+                return
+            if self._ws_state != WsState.OPEN:
+                # Already closed
+                return
+            logging.info(
+                f"River session from {self._transport_id} to {self._to_id} "
+                f"closing websocket {ws.id} state: {ws.state}"
+            )
+            self._ws_state = WsState.CLOSING
+            if ws:
+                # TODO: should we wait here?
+                task = asyncio.create_task(ws.close())
+                task.add_done_callback(
+                    lambda _: logging.debug(f"old websocket {ws.id} closed.")
+                )
+            self._ws_state = WsState.CLOSED
+        if should_retry and self._retry_connection_callback:
+            await self._retry_connection_callback(self)
 
-    async def _handle_msg_server(
+    async def _open_stream_and_call_handler(
         self,
         msg: TransportMessage,
         stream: Optional[Channel],
         tg: Optional[asyncio.TaskGroup],
-    ) -> None:
-        if msg.controlFlags & STREAM_OPEN_BIT != 0:
-            if not msg.serviceName or not msg.procedureName:
-                logging.warning("no service or procedure name in %r", msg)
-                return
-            key = (msg.serviceName, msg.procedureName)
-            handler = self._handlers.get(key, None)
-            if not handler:
-                logging.exception(
-                    "No handler for %s handlers : " f"{self._handlers.keys()}",
-                    key,
-                )
-                return
-            method_type, handler_func = handler
-            is_streaming_output = method_type in (
-                "subscription-stream",  # subscription
-                "stream",
+    ) -> Channel:
+        if not self._is_server:
+            raise InvalidMessageException("Client should not receive stream open bit")
+        if not msg.serviceName or not msg.procedureName:
+            raise IgnoreMessageException(
+                f"Service name or procedure name is missing in the message {msg}"
             )
-            is_streaming_input = method_type in (
-                "upload-stream",  # subscription
-                "stream",
+        key = (msg.serviceName, msg.procedureName)
+        handler = self._handlers.get(key, None)
+        if not handler:
+            raise IgnoreMessageException(
+                f"No handler for {key} handlers : " f"{self._handlers.keys()}"
             )
-            # New channel pair.
-            input_stream: Channel[Any] = Channel(1024 if is_streaming_input else 1)
-            output_stream: Channel[Any] = Channel(1024 if is_streaming_output else 1)
+        method_type, handler_func = handler
+        is_streaming_output = method_type in (
+            "subscription-stream",  # subscription
+            "stream",
+        )
+        is_streaming_input = method_type in (
+            "upload-stream",  # subscription
+            "stream",
+        )
+        # New channel pair.
+        input_stream: Channel[Any] = Channel(1024 if is_streaming_input else 1)
+        output_stream: Channel[Any] = Channel(1024 if is_streaming_output else 1)
+        try:
             await input_stream.put(msg.payload)
-            if not stream:
-                # We'll need to save it for later.
+        except (RuntimeError, ChannelClosed) as e:
+            raise InvalidMessageException(e)
+        if not stream:
+            async with self._stream_lock:
                 self._streams[msg.streamId] = input_stream
-            # Start the handler.
-            await self._task_manager.create_task(
-                handler_func(msg.from_, input_stream, output_stream), tg
-            )
-            await self._task_manager.create_task(
-                self.send_responses(
-                    msg.streamId, self._ws, output_stream, is_streaming_output
-                ),
-                tg,
-            )
-
-        else:
-            await self._add_msg_to_stream(msg, stream)
+        # Start the handler.
+        await self._task_manager.create_task(
+            handler_func(msg.from_, input_stream, output_stream), tg
+        )
+        await self._task_manager.create_task(
+            self._send_responses_from_output_stream(
+                msg.streamId, output_stream, is_streaming_output
+            ),
+            tg,
+        )
+        return input_stream
 
     async def _add_msg_to_stream(
         self,
         msg: TransportMessage,
-        stream: Optional[Channel],
+        stream: Channel,
     ) -> None:
-        if not stream:
-            logging.warning("no stream for %s", msg.streamId)
-            raise IgnoreTransportMessageException("no stream for message, ignoring")
-        if not (
+        if (
             msg.controlFlags & STREAM_CLOSED_BIT != 0
             and msg.payload.get("type", None) == "CLOSE"
         ):
             # close message is not sent to the stream
+            return
+        try:
             await stream.put(msg.payload)
+        except (RuntimeError, ChannelClosed) as e:
+            raise InvalidMessageException(e)
 
-    async def handle_messages_from_ws(
-        self, websocket: WebSocketCommonProtocol, tg: Optional[asyncio.TaskGroup] = None
-    ) -> None:
-        logging.debug(
-            f'{"server" if self._is_server else "client"} start handling messages from'
-            " ws"
-        )
-        async for message in websocket:
-            try:
-                msg = parse_transport_msg(message, self._transport_options)
-            except IgnoreTransportMessageException as e:
-                logging.debug(f"Ignoring transport message : {e}")
-                continue
-            except InvalidTransportMessageException:
-                logging.error("Got invalid transport message, closing connection")
-                await self.close()
-                return
-
-            logging.debug("got a message %r", msg)
-
-            try:
-                await self._seq_manager.check_seq_and_update(msg)
-            except IgnoreTransportMessageException:
-                continue
-            except InvalidTransportMessageException:
-                return
-            if msg.controlFlags & ACK_BIT != 0:
-                self.cancel_disconnect_grace_period()
-                continue
-
-            stream = self._streams.get(msg.streamId, None)
-            if self._is_server:
-                await self._handle_msg_server(msg, stream, tg)
-            else:
-                await self._add_msg_to_stream(msg, stream)
-            if msg.controlFlags & STREAM_CLOSED_BIT != 0:
-                if stream:
-                    stream.close()
-                del self._streams[msg.streamId]
+    async def _remove_acked_messages_in_buffer(self) -> None:
+        await self._buffer.remove_old_messages(self._seq_manager.receiver_ack)
 
-    async def start_serve_messages(self) -> None:
-        await self._task_manager.create_task(self._serve())
+    async def start_serve_responses(self) -> None:
+        await self._task_manager.create_task(self.serve())
 
-    async def _serve(self) -> None:
-        try:
-            async with asyncio.TaskGroup() as tg:
-                try:
-                    await self.handle_messages_from_ws(self._ws, tg)
-                except ConnectionClosedError as e:
-                    await self.begin_grace()
-                    logging.debug(f"ConnectionClosedError while serving: {e}")
-                except FailedSendingMessageException as e:
-                    # Expected error if the connection is closed.
-                    logging.debug(f"FailedSendingMessageException while serving: {e}")
-                except Exception:
-                    logging.exception("caught exception at message iterator")
-        except ExceptionGroup as eg:
-            _, unhandled = eg.split(lambda e: isinstance(e, ConnectionClosedError))
-            if unhandled:
-                raise ExceptionGroup(
-                    "Unhandled exceptions on River server", unhandled.exceptions
-                )
-
-    async def close_websocket(self) -> None:
-        """Close the websocket connection."""
+    async def close(self, is_unexpected_close: bool) -> None:
+        """Close the session and all associated streams."""
         logging.info(
-            f"Closing websocket connection from {self._transport_id} to {self._to_id}"
+            f"{self._transport_id} closing session "
+            f"to {self._to_id} current_state : {self._ws_state}"
         )
-        if self._ws:
-            await self._ws.close()
-
-    async def close(self) -> None:
-        """Close the session and all associated streams."""
-        logging.info(f"Closing session from {self._transport_id} to {self._to_id}")
-        for previous_input in self._streams.values():
-            previous_input.close()
-        self._streams.clear()
-        await self._task_manager.cancel_all_tasks()
-        if self._ws:
-            await self._ws.close()
-        await self._close_session_callback(self)
+        async with self._state_lock:
+            if self._state != SessionState.ACTIVE:
+                # already closing
+                return
+            self._state = SessionState.CLOSING
+            self._reset_session_close_countdown()
+            await self.close_websocket(self._ws, should_retry=False)
+            # Clear the session in transports
+            await self._close_session_callback(self)
+            await self._task_manager.cancel_all_tasks()
+            # TODO: unexpected_close should close stream differently here to
+            # throw exception correctly.
+            for stream in self._streams.values():
+                stream.close()
+            async with self._stream_lock:
+                self._streams.clear()
+            self._state = SessionState.CLOSED
```

### Comparing `replit_river-0.1.7b1/replit_river/task_manager.py` & `replit_river-0.1.7b2/replit_river/task_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b1/replit_river/transport.py` & `replit_river-0.1.7b2/replit_river/transport.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import asyncio
+import logging
 from typing import Dict, Tuple
 
 import nanoid  # type: ignore
+
 from replit_river.rpc import (
     GenericRpcHandler,
 )
 from replit_river.session import Session
 from replit_river.transport_options import TransportOptions
 
 PROTOCOL_VERSION = "v1"
@@ -24,17 +26,23 @@
         self._is_server = is_server
         self._sessions: Dict[str, Session] = {}
         self._handlers = handlers
         self._session_lock = asyncio.Lock()
 
     async def close_all_sessions(self) -> None:
         sessions = self._sessions.values()
-        for session in sessions:
-            await session.close()
+        logging.info(
+            f"start closing transport {self._transport_id}, number sessions : "
+            f"{len(sessions)}"
+        )
+        sessions_to_close = list(sessions)
+        for session in sessions_to_close:
+            await session.close(False)
+        logging.info(f"Transport closed {self._transport_id}")
 
     async def _delete_session(self, session: Session) -> None:
         async with self._session_lock:
-            if session._transport_id in self._sessions:
-                del self._sessions[session._transport_id]
+            if session._to_id in self._sessions:
+                del self._sessions[session._to_id]
 
     def generate_nanoid(self) -> str:
         return str(nanoid.generate())
```

### Comparing `replit_river-0.1.7b1/replit_river/transport_options.py` & `replit_river-0.1.7b2/replit_river/transport_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import os
+
 from pydantic import BaseModel
 
 CROSIS_PREFIX_BYTES = b"\x00\x00"
 PID2_PREFIX_BYTES = b"\xff\xff"
 
 
 class ConnectionRetryOptions(BaseModel):
     base_interval_ms: int = 250
     max_jitter_ms: int = 200
     max_backoff_ms: float = 32000
     attempt_budget_capacity: float = 5
     budget_restore_interval_ms: float = 200
+    max_retry: int = 1000
 
 
 class TransportOptions(BaseModel):
     session_disconnect_grace_ms: float = 5_000
-    heartbeat_ms: float = 2000
+    heartbeat_ms: float = 500
     heartbeats_until_dead: int = 2
     use_prefix_bytes: bool = False
+    close_session_check_interval_ms: float = 100
     connection_retry_options: ConnectionRetryOptions = ConnectionRetryOptions()
+    buffer_size: int = 1000
 
     def get_prefix_bytes(self) -> bytes:
         return PID2_PREFIX_BYTES if self.use_prefix_bytes else b""
 
     def websocket_disconnect_grace_ms(self) -> float:
         return self.heartbeat_ms * self.heartbeats_until_dead
```

### Comparing `replit_river-0.1.7b1/PKG-INFO` & `replit_river-0.1.7b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.1.7b1
+Version: 0.1.7b2
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

