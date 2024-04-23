# Comparing `tmp/replit_river-0.1.7b2.tar.gz` & `tmp/replit_river-0.1.7b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.1.7b2.tar", max compression
+gzip compressed data, was "replit_river-0.1.7b3.tar", max compression
```

## Comparing `replit_river-0.1.7b2.tar` & `replit_river-0.1.7b3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1064 2024-04-19 19:26:13.426252 replit_river-0.1.7b2/LICENSE
--rw-r--r--   0        0        0     1628 2024-04-19 19:26:13.426318 replit_river-0.1.7b2/README.md
--rw-r--r--   0        0        0     1749 2024-04-23 01:28:51.361313 replit_river-0.1.7b2/pyproject.toml
--rw-r--r--   0        0        0      487 2024-04-22 19:50:44.355705 replit_river-0.1.7b2/replit_river/__init__.py
--rw-r--r--   0        0        0     3860 2024-04-23 00:45:40.912922 replit_river-0.1.7b2/replit_river/client.py
--rw-r--r--   0        0        0    11280 2024-04-23 00:45:40.913696 replit_river-0.1.7b2/replit_river/client_session.py
--rw-r--r--   0        0        0     9904 2024-04-23 00:45:40.914351 replit_river-0.1.7b2/replit_river/client_transport.py
--rw-r--r--   0        0        0        0 2024-04-22 19:50:44.356674 replit_river-0.1.7b2/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-04-22 19:50:44.356784 replit_river-0.1.7b2/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13363 2024-04-22 19:50:44.356886 replit_river-0.1.7b2/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-04-22 19:50:44.356956 replit_river-0.1.7b2/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5356 2024-04-23 00:45:40.473122 replit_river-0.1.7b2/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12624 2024-04-23 00:45:40.507714 replit_river-0.1.7b2/replit_river/codegen/server.py
--rw-r--r--   0        0        0      547 2024-04-22 19:50:44.357515 replit_river-0.1.7b2/replit_river/error_schema.py
--rw-r--r--   0        0        0        1 2024-04-22 19:50:44.357856 replit_river-0.1.7b2/replit_river/handshake.py
--rw-r--r--   0        0        0     1302 2024-04-23 00:45:40.909781 replit_river-0.1.7b2/replit_river/message_buffer.py
--rw-r--r--   0        0        0     2637 2024-04-23 00:45:40.912273 replit_river-0.1.7b2/replit_river/messages.py
--rw-r--r--   0        0        0        0 2024-04-22 19:50:44.358418 replit_river-0.1.7b2/replit_river/py.typed
--rw-r--r--   0        0        0     1827 2024-04-23 00:45:40.911579 replit_river-0.1.7b2/replit_river/rate_limiter.py
--rw-r--r--   0        0        0    12218 2024-04-22 19:50:44.358789 replit_river-0.1.7b2/replit_river/rpc.py
--rw-r--r--   0        0        0     2102 2024-04-22 19:50:44.359301 replit_river-0.1.7b2/replit_river/seq_manager.py
--rw-r--r--   0        0        0     2294 2024-04-22 19:50:44.359622 replit_river-0.1.7b2/replit_river/server.py
--rw-r--r--   0        0        0     7436 2024-04-23 00:45:40.912746 replit_river-0.1.7b2/replit_river/server_transport.py
--rw-r--r--   0        0        0    19587 2024-04-23 02:08:03.880757 replit_river-0.1.7b2/replit_river/session.py
--rw-r--r--   0        0        0     2336 2024-04-22 19:50:44.360278 replit_river-0.1.7b2/replit_river/task_manager.py
--rw-r--r--   0        0        0     1473 2024-04-23 01:20:15.732925 replit_river-0.1.7b2/replit_river/transport.py
--rw-r--r--   0        0        0     1432 2024-04-23 00:45:40.909656 replit_river-0.1.7b2/replit_river/transport_options.py
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 replit_river-0.1.7b2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-19 19:26:13.426252 replit_river-0.1.7b3/LICENSE
+-rw-r--r--   0        0        0     1628 2024-04-19 19:26:13.426318 replit_river-0.1.7b3/README.md
+-rw-r--r--   0        0        0     1749 2024-04-23 05:04:22.056973 replit_river-0.1.7b3/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-22 19:50:44.355705 replit_river-0.1.7b3/replit_river/__init__.py
+-rw-r--r--   0        0        0     3860 2024-04-23 00:45:40.912922 replit_river-0.1.7b3/replit_river/client.py
+-rw-r--r--   0        0        0    11280 2024-04-23 00:45:40.913696 replit_river-0.1.7b3/replit_river/client_session.py
+-rw-r--r--   0        0        0     9848 2024-04-23 04:59:15.388882 replit_river-0.1.7b3/replit_river/client_transport.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:50:44.356674 replit_river-0.1.7b3/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-04-22 19:50:44.356784 replit_river-0.1.7b3/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13363 2024-04-22 19:50:44.356886 replit_river-0.1.7b3/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-04-22 19:50:44.356956 replit_river-0.1.7b3/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5356 2024-04-23 00:45:40.473122 replit_river-0.1.7b3/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12624 2024-04-23 00:45:40.507714 replit_river-0.1.7b3/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      547 2024-04-22 19:50:44.357515 replit_river-0.1.7b3/replit_river/error_schema.py
+-rw-r--r--   0        0        0        1 2024-04-22 19:50:44.357856 replit_river-0.1.7b3/replit_river/handshake.py
+-rw-r--r--   0        0        0     1302 2024-04-23 00:45:40.909781 replit_river-0.1.7b3/replit_river/message_buffer.py
+-rw-r--r--   0        0        0     2637 2024-04-23 00:45:40.912273 replit_river-0.1.7b3/replit_river/messages.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:50:44.358418 replit_river-0.1.7b3/replit_river/py.typed
+-rw-r--r--   0        0        0     1827 2024-04-23 00:45:40.911579 replit_river-0.1.7b3/replit_river/rate_limiter.py
+-rw-r--r--   0        0        0    12218 2024-04-22 19:50:44.358789 replit_river-0.1.7b3/replit_river/rpc.py
+-rw-r--r--   0        0        0     2102 2024-04-22 19:50:44.359301 replit_river-0.1.7b3/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     2260 2024-04-23 05:03:13.892136 replit_river-0.1.7b3/replit_river/server.py
+-rw-r--r--   0        0        0     7436 2024-04-23 00:45:40.912746 replit_river-0.1.7b3/replit_river/server_transport.py
+-rw-r--r--   0        0        0    19562 2024-04-23 05:03:35.134536 replit_river-0.1.7b3/replit_river/session.py
+-rw-r--r--   0        0        0     2336 2024-04-22 19:50:44.360278 replit_river-0.1.7b3/replit_river/task_manager.py
+-rw-r--r--   0        0        0     1473 2024-04-23 01:20:15.732925 replit_river-0.1.7b3/replit_river/transport.py
+-rw-r--r--   0        0        0     1432 2024-04-23 00:45:40.909656 replit_river-0.1.7b3/replit_river/transport_options.py
+-rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 replit_river-0.1.7b3/PKG-INFO
```

### Comparing `replit_river-0.1.7b2/LICENSE` & `replit_river-0.1.7b3/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/README.md` & `replit_river-0.1.7b3/README.md`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/pyproject.toml` & `replit_river-0.1.7b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.1.7-beta.2"
+version="0.1.7-beta.3"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `replit_river-0.1.7b2/replit_river/client.py` & `replit_river-0.1.7b3/replit_river/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/client_session.py` & `replit_river-0.1.7b3/replit_river/client_session.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/client_transport.py` & `replit_river-0.1.7b3/replit_river/client_transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,17 +215,15 @@
         except FailedSendingMessageException:
             raise RiverException(
                 ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
             )
         logging.debug("river client waiting for handshake response")
         while True:
             try:
-                logging.debug(
-                    f"websocket while waiting for response : {websocket.id} {websocket.state}"
-                )
+                logging.debug(f"websocket while waiting for response : {websocket.id}")
                 data = await websocket.recv()
             except ConnectionClosed:
                 logging.debug(
                     "Connection closed during waiting for handshake response : {e}"
                 )
                 raise RiverException(ERROR_HANDSHAKE, "Hand shake failed")
             try:
```

### Comparing `replit_river-0.1.7b2/replit_river/codegen/client.py` & `replit_river-0.1.7b3/replit_river/codegen/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/codegen/run.py` & `replit_river-0.1.7b3/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/codegen/schema.py` & `replit_river-0.1.7b3/replit_river/codegen/schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/codegen/server.py` & `replit_river-0.1.7b3/replit_river/codegen/server.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/error_schema.py` & `replit_river-0.1.7b3/replit_river/error_schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/message_buffer.py` & `replit_river-0.1.7b3/replit_river/message_buffer.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/messages.py` & `replit_river-0.1.7b3/replit_river/messages.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/rate_limiter.py` & `replit_river-0.1.7b3/replit_river/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/rpc.py` & `replit_river-0.1.7b3/replit_river/rpc.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/seq_manager.py` & `replit_river-0.1.7b3/replit_river/seq_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/server.py` & `replit_river-0.1.7b3/replit_river/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         rpc_handlers: Mapping[Tuple[str, str], Tuple[str, GenericRpcHandler]],
     ) -> None:
         self._transport._handlers.update(rpc_handlers)
 
     async def serve(self, websocket: WebSocketServerProtocol) -> None:
         logging.debug(
             f"River server started establishing session with ws: {websocket.id}"
-            f" {websocket.state}"
         )
         try:
             session = await self._transport.handshake_to_get_session(websocket)
         except Exception as e:
             logging.error(f"Error establishing handshake, closing websocket: {e}")
             await websocket.close()
             return
```

### Comparing `replit_river-0.1.7b2/replit_river/server_transport.py` & `replit_river-0.1.7b3/replit_river/server_transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/session.py` & `replit_river-0.1.7b3/replit_river/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         self._reset_session_close_countdown()
 
     async def _handle_messages_from_ws(
         self, websocket: WebSocketCommonProtocol, tg: Optional[asyncio.TaskGroup] = None
     ) -> None:
         logging.debug(
             f'{"server" if self._is_server else "client"} start handling messages from'
-            f" ws {websocket.id}, state {websocket.state}"
+            f" ws {websocket.id}"
         )
         try:
             async for message in websocket:
                 try:
                     msg = parse_transport_msg(message, self._transport_options)
 
                     logging.debug(f"{self._transport_id} got a message %r", msg)
```

### Comparing `replit_river-0.1.7b2/replit_river/task_manager.py` & `replit_river-0.1.7b3/replit_river/task_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/transport.py` & `replit_river-0.1.7b3/replit_river/transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/replit_river/transport_options.py` & `replit_river-0.1.7b3/replit_river/transport_options.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.7b2/PKG-INFO` & `replit_river-0.1.7b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.1.7b2
+Version: 0.1.7b3
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

