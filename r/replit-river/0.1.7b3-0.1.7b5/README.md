# Comparing `tmp/replit_river-0.1.7b3.tar.gz` & `tmp/replit_river-0.1.7b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.1.7b3.tar", max compression
+gzip compressed data, was "replit_river-0.1.7b5.tar", max compression
```

## Comparing `replit_river-0.1.7b3.tar` & `replit_river-0.1.7b5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1064 2024-04-19 19:26:13.426252 replit_river-0.1.7b3/LICENSE
--rw-r--r--   0        0        0     1628 2024-04-19 19:26:13.426318 replit_river-0.1.7b3/README.md
--rw-r--r--   0        0        0     1749 2024-04-23 05:04:22.056973 replit_river-0.1.7b3/pyproject.toml
--rw-r--r--   0        0        0      487 2024-04-22 19:50:44.355705 replit_river-0.1.7b3/replit_river/__init__.py
--rw-r--r--   0        0        0     3860 2024-04-23 00:45:40.912922 replit_river-0.1.7b3/replit_river/client.py
--rw-r--r--   0        0        0    11280 2024-04-23 00:45:40.913696 replit_river-0.1.7b3/replit_river/client_session.py
--rw-r--r--   0        0        0     9848 2024-04-23 04:59:15.388882 replit_river-0.1.7b3/replit_river/client_transport.py
--rw-r--r--   0        0        0        0 2024-04-22 19:50:44.356674 replit_river-0.1.7b3/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-04-22 19:50:44.356784 replit_river-0.1.7b3/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13363 2024-04-22 19:50:44.356886 replit_river-0.1.7b3/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-04-22 19:50:44.356956 replit_river-0.1.7b3/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5356 2024-04-23 00:45:40.473122 replit_river-0.1.7b3/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12624 2024-04-23 00:45:40.507714 replit_river-0.1.7b3/replit_river/codegen/server.py
--rw-r--r--   0        0        0      547 2024-04-22 19:50:44.357515 replit_river-0.1.7b3/replit_river/error_schema.py
--rw-r--r--   0        0        0        1 2024-04-22 19:50:44.357856 replit_river-0.1.7b3/replit_river/handshake.py
--rw-r--r--   0        0        0     1302 2024-04-23 00:45:40.909781 replit_river-0.1.7b3/replit_river/message_buffer.py
--rw-r--r--   0        0        0     2637 2024-04-23 00:45:40.912273 replit_river-0.1.7b3/replit_river/messages.py
--rw-r--r--   0        0        0        0 2024-04-22 19:50:44.358418 replit_river-0.1.7b3/replit_river/py.typed
--rw-r--r--   0        0        0     1827 2024-04-23 00:45:40.911579 replit_river-0.1.7b3/replit_river/rate_limiter.py
--rw-r--r--   0        0        0    12218 2024-04-22 19:50:44.358789 replit_river-0.1.7b3/replit_river/rpc.py
--rw-r--r--   0        0        0     2102 2024-04-22 19:50:44.359301 replit_river-0.1.7b3/replit_river/seq_manager.py
--rw-r--r--   0        0        0     2260 2024-04-23 05:03:13.892136 replit_river-0.1.7b3/replit_river/server.py
--rw-r--r--   0        0        0     7436 2024-04-23 00:45:40.912746 replit_river-0.1.7b3/replit_river/server_transport.py
--rw-r--r--   0        0        0    19562 2024-04-23 05:03:35.134536 replit_river-0.1.7b3/replit_river/session.py
--rw-r--r--   0        0        0     2336 2024-04-22 19:50:44.360278 replit_river-0.1.7b3/replit_river/task_manager.py
--rw-r--r--   0        0        0     1473 2024-04-23 01:20:15.732925 replit_river-0.1.7b3/replit_river/transport.py
--rw-r--r--   0        0        0     1432 2024-04-23 00:45:40.909656 replit_river-0.1.7b3/replit_river/transport_options.py
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 replit_river-0.1.7b3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-19 19:26:13.426252 replit_river-0.1.7b5/LICENSE
+-rw-r--r--   0        0        0     1628 2024-04-19 19:26:13.426318 replit_river-0.1.7b5/README.md
+-rw-r--r--   0        0        0     1749 2024-04-23 05:10:58.235182 replit_river-0.1.7b5/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-22 19:50:44.355705 replit_river-0.1.7b5/replit_river/__init__.py
+-rw-r--r--   0        0        0     3860 2024-04-23 00:45:40.912922 replit_river-0.1.7b5/replit_river/client.py
+-rw-r--r--   0        0        0    11280 2024-04-23 00:45:40.913696 replit_river-0.1.7b5/replit_river/client_session.py
+-rw-r--r--   0        0        0     9848 2024-04-23 04:59:15.388882 replit_river-0.1.7b5/replit_river/client_transport.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:50:44.356674 replit_river-0.1.7b5/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-04-22 19:50:44.356784 replit_river-0.1.7b5/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13363 2024-04-22 19:50:44.356886 replit_river-0.1.7b5/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-04-22 19:50:44.356956 replit_river-0.1.7b5/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5356 2024-04-23 00:45:40.473122 replit_river-0.1.7b5/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12624 2024-04-23 00:45:40.507714 replit_river-0.1.7b5/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      547 2024-04-22 19:50:44.357515 replit_river-0.1.7b5/replit_river/error_schema.py
+-rw-r--r--   0        0        0        1 2024-04-22 19:50:44.357856 replit_river-0.1.7b5/replit_river/handshake.py
+-rw-r--r--   0        0        0     1302 2024-04-23 00:45:40.909781 replit_river-0.1.7b5/replit_river/message_buffer.py
+-rw-r--r--   0        0        0     2615 2024-04-23 05:10:48.460849 replit_river-0.1.7b5/replit_river/messages.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:50:44.358418 replit_river-0.1.7b5/replit_river/py.typed
+-rw-r--r--   0        0        0     1827 2024-04-23 00:45:40.911579 replit_river-0.1.7b5/replit_river/rate_limiter.py
+-rw-r--r--   0        0        0    12218 2024-04-22 19:50:44.358789 replit_river-0.1.7b5/replit_river/rpc.py
+-rw-r--r--   0        0        0     2102 2024-04-22 19:50:44.359301 replit_river-0.1.7b5/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     2260 2024-04-23 05:03:13.892136 replit_river-0.1.7b5/replit_river/server.py
+-rw-r--r--   0        0        0     7436 2024-04-23 00:45:40.912746 replit_river-0.1.7b5/replit_river/server_transport.py
+-rw-r--r--   0        0        0    19441 2024-04-23 05:08:55.447346 replit_river-0.1.7b5/replit_river/session.py
+-rw-r--r--   0        0        0     2336 2024-04-22 19:50:44.360278 replit_river-0.1.7b5/replit_river/task_manager.py
+-rw-r--r--   0        0        0     1473 2024-04-23 01:20:15.732925 replit_river-0.1.7b5/replit_river/transport.py
+-rw-r--r--   0        0        0     1432 2024-04-23 00:45:40.909656 replit_river-0.1.7b5/replit_river/transport_options.py
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 replit_river-0.1.7b5/PKG-INFO
```

### Comparing `replit_river-0.1.7b3/LICENSE` & `replit_river-0.1.7b5/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/README.md` & `replit_river-0.1.7b5/README.md`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/pyproject.toml` & `replit_river-0.1.7b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.1.7-beta.3"
+version="0.1.7-beta.5"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `replit_river-0.1.7b3/replit_river/client.py` & `replit_river-0.1.7b5/replit_river/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/client_session.py` & `replit_river-0.1.7b5/replit_river/client_session.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/client_transport.py` & `replit_river-0.1.7b5/replit_river/client_transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/codegen/client.py` & `replit_river-0.1.7b5/replit_river/codegen/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/codegen/run.py` & `replit_river-0.1.7b5/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/codegen/schema.py` & `replit_river-0.1.7b5/replit_river/codegen/schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/codegen/server.py` & `replit_river-0.1.7b5/replit_river/codegen/server.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/error_schema.py` & `replit_river-0.1.7b5/replit_river/error_schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/message_buffer.py` & `replit_river-0.1.7b5/replit_river/message_buffer.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/messages.py` & `replit_river-0.1.7b5/replit_river/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 async def send_transport_message(
     msg: TransportMessage,
     ws: WebSocketCommonProtocol,
     websocket_closed_callback: Callable[[], Coroutine[Any, Any, None]],
     prefix_bytes: bytes = b"",
 ) -> None:
-    logging.debug(f"sending a message {msg} to ws {ws.id} with state {ws.state}")
+    logging.debug(f"sending a message {msg} to ws {ws.id}")
     try:
         await ws.send(
             prefix_bytes
             + msgpack.packb(
                 msg.model_dump(by_alias=True, exclude_none=True), datetime=True
             )
         )
```

### Comparing `replit_river-0.1.7b3/replit_river/rate_limiter.py` & `replit_river-0.1.7b5/replit_river/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/rpc.py` & `replit_river-0.1.7b5/replit_river/rpc.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/seq_manager.py` & `replit_river-0.1.7b5/replit_river/seq_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/server.py` & `replit_river-0.1.7b5/replit_river/server.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/server_transport.py` & `replit_river-0.1.7b5/replit_river/server_transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/session.py` & `replit_river-0.1.7b5/replit_river/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,21 +378,17 @@
                 if not is_streaming_output:
                     await self.send_message(stream_id, payload, ws, STREAM_CLOSED_BIT)
                     return
                 await self.send_message(stream_id, payload, ws)
             logging.debug("sent an end of stream %r", stream_id)
             await self.send_message(stream_id, {"type": "CLOSE"}, ws, STREAM_CLOSED_BIT)
         except FailedSendingMessageException as e:
-            logging.error(
-                f"Error while sending responses, ws_state: {ws.state}, {type(e)} : {e}"
-            )
+            logging.error(f"Error while sending responses, {type(e)} : {e}")
         except (RuntimeError, ChannelClosed) as e:
-            logging.error(
-                f"Error while sending responses, ws_state: {ws.state} {type(e)} : {e}"
-            )
+            logging.error(f"Error while sending responses, {type(e)} : {e}")
         except Exception as e:
             logging.error(f"Unknown error while river sending responses back : {e}")
 
     async def close_websocket(
         self, ws: WebSocketCommonProtocol, should_retry: bool
     ) -> None:
         """Mark the websocket as closed, close the websocket, and retry if needed."""
@@ -401,15 +397,15 @@
                 # already replaced with new ws
                 return
             if self._ws_state != WsState.OPEN:
                 # Already closed
                 return
             logging.info(
                 f"River session from {self._transport_id} to {self._to_id} "
-                f"closing websocket {ws.id} state: {ws.state}"
+                f"closing websocket {ws.id}"
             )
             self._ws_state = WsState.CLOSING
             if ws:
                 # TODO: should we wait here?
                 task = asyncio.create_task(ws.close())
                 task.add_done_callback(
                     lambda _: logging.debug(f"old websocket {ws.id} closed.")
```

### Comparing `replit_river-0.1.7b3/replit_river/task_manager.py` & `replit_river-0.1.7b5/replit_river/task_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/transport.py` & `replit_river-0.1.7b5/replit_river/transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/replit_river/transport_options.py` & `replit_river-0.1.7b5/replit_river/transport_options.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b3/PKG-INFO` & `replit_river-0.1.7b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.1.7b3
+Version: 0.1.7b5
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

