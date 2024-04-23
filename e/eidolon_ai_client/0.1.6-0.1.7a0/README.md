# Comparing `tmp/eidolon_ai_client-0.1.6.tar.gz` & `tmp/eidolon_ai_client-0.1.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_client-0.1.6.tar", max compression
+gzip compressed data, was "eidolon_ai_client-0.1.7a0.tar", max compression
```

## Comparing `eidolon_ai_client-0.1.6.tar` & `eidolon_ai_client-0.1.7a0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/README.md
--rw-r--r--   0        0        0        0 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/__init__.py
--rw-r--r--   0        0        0     7297 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/client.py
--rw-r--r--   0        0        0     4987 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/events.py
--rw-r--r--   0        0        0     2387 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/group_conversation.py
--rw-r--r--   0        0        0        0 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/aiohttp.py
--rw-r--r--   0        0        0      448 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/logger.py
--rw-r--r--   0        0        0     2361 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/request_context.py
--rw-r--r--   0        0        0      424 2024-04-16 01:18:28.707470 eidolon_ai_client-0.1.6/eidolon_ai_client/util/stream_collector.py
--rw-r--r--   0        0        0      541 2024-04-16 01:18:28.711470 eidolon_ai_client-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      592 1970-01-01 00:00:00.000000 eidolon_ai_client-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-14 01:52:18.637846 eidolon_ai_client-0.1.7a0/README.md
+-rw-r--r--   0        0        0        0 2024-03-14 01:52:18.637969 eidolon_ai_client-0.1.7a0/eidolon_ai_client/__init__.py
+-rw-r--r--   0        0        0     7297 2024-04-22 17:59:01.127362 eidolon_ai_client-0.1.7a0/eidolon_ai_client/client.py
+-rw-r--r--   0        0        0     5048 2024-04-23 00:45:57.850956 eidolon_ai_client-0.1.7a0/eidolon_ai_client/events.py
+-rw-r--r--   0        0        0     2387 2024-03-14 01:52:18.638638 eidolon_ai_client-0.1.7a0/eidolon_ai_client/group_conversation.py
+-rw-r--r--   0        0        0        0 2024-03-14 01:52:18.638724 eidolon_ai_client-0.1.7a0/eidolon_ai_client/util/__init__.py
+-rw-r--r--   0        0        0     3728 2024-03-26 16:45:17.179105 eidolon_ai_client-0.1.7a0/eidolon_ai_client/util/aiohttp.py
+-rw-r--r--   0        0        0      448 2024-03-14 01:52:18.640318 eidolon_ai_client-0.1.7a0/eidolon_ai_client/util/logger.py
+-rw-r--r--   0        0        0     2361 2024-03-14 01:52:18.640508 eidolon_ai_client-0.1.7a0/eidolon_ai_client/util/request_context.py
+-rw-r--r--   0        0        0      424 2024-03-15 02:24:26.364459 eidolon_ai_client-0.1.7a0/eidolon_ai_client/util/stream_collector.py
+-rw-r--r--   0        0        0      544 2024-04-23 00:54:43.458102 eidolon_ai_client-0.1.7a0/pyproject.toml
+-rw-r--r--   0        0        0      594 1970-01-01 00:00:00.000000 eidolon_ai_client-0.1.7a0/PKG-INFO
```

### Comparing `eidolon_ai_client-0.1.6/eidolon_ai_client/client.py` & `eidolon_ai_client-0.1.7a0/eidolon_ai_client/client.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.6/eidolon_ai_client/events.py` & `eidolon_ai_client-0.1.7a0/eidolon_ai_client/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 from abc import ABC
 from enum import Enum
-from pydantic import BaseModel, TypeAdapter
+from pydantic import BaseModel, TypeAdapter, Field
 from typing import List, TypeVar, Generic, Any, AsyncIterator, Type, Literal, Dict, Optional
 
 
 class FileHandle(BaseModel):
     machineURL: str
     process_id: str
     file_id: str
-    metadata: dict = {}
+    metadata: dict = Field(default={}, description="Metadata about the file")
 
 
 class Category(Enum):
     START = "start"
     INPUT = "input"
     END = "end"
     OUTPUT = "output"
```

### Comparing `eidolon_ai_client-0.1.6/eidolon_ai_client/group_conversation.py` & `eidolon_ai_client-0.1.7a0/eidolon_ai_client/group_conversation.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.6/eidolon_ai_client/util/aiohttp.py` & `eidolon_ai_client-0.1.7a0/eidolon_ai_client/util/aiohttp.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.6/eidolon_ai_client/util/request_context.py` & `eidolon_ai_client-0.1.7a0/eidolon_ai_client/util/request_context.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_client-0.1.6/pyproject.toml` & `eidolon_ai_client-0.1.7a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "eidolon_ai_client"
-version = "0.1.6"
+version = "0.1.7a0"
 description = ""
 authors = ["Luke Lalor <lukehlalor@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 setuptools = "^69.0.2"
 jsonref = "^1.1.0"
+
 pydantic = "^2.6.1"
 httpx = "^0.27.0"
 httpx-sse = "^0.4.0"
 sse-starlette = "^2.0.0"
 aiostream = "^0.5.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `eidolon_ai_client-0.1.6/PKG-INFO` & `eidolon_ai_client-0.1.7a0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon_ai_client
-Version: 0.1.6
+Version: 0.1.7a0
 Summary: 
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiostream (>=0.5.2,<0.6.0)
```

