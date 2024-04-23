# Comparing `tmp/que_sdk-0.1.1.tar.gz` & `tmp/que_sdk-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "que_sdk-0.1.1.tar", max compression
+gzip compressed data, was "que_sdk-0.1.2.tar", max compression
```

## Comparing `que_sdk-0.1.1.tar` & `que_sdk-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1060 2024-04-12 14:53:33.472804 que_sdk-0.1.1/LICENSE
--rw-r--r--   0        0        0       10 2024-04-19 17:17:10.806057 que_sdk-0.1.1/README.md
--rw-r--r--   0        0        0     1167 2024-04-19 18:57:48.512347 que_sdk-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      429 2024-04-19 17:19:36.152402 que_sdk-0.1.1/que_sdk/__init__.py
--rw-r--r--   0        0        0       65 2024-04-18 19:15:55.848369 que_sdk-0.1.1/que_sdk/_internal/__init__.py
--rw-r--r--   0        0        0      367 2024-04-13 18:33:05.063314 que_sdk-0.1.1/que_sdk/_internal/auth.py
--rw-r--r--   0        0        0     2257 2024-04-19 18:42:30.920224 que_sdk-0.1.1/que_sdk/_internal/base.py
--rw-r--r--   0        0        0     6333 2024-04-19 18:42:30.957547 que_sdk-0.1.1/que_sdk/client.py
--rw-r--r--   0        0        0     5564 2024-04-19 18:42:30.903713 que_sdk-0.1.1/que_sdk/clients.py
--rw-r--r--   0        0        0        0 2024-04-12 19:15:10.383938 que_sdk-0.1.1/que_sdk/py.typed.py
--rw-r--r--   0        0        0      585 2024-04-18 17:02:35.165077 que_sdk-0.1.1/que_sdk/schemas.py
--rw-r--r--   0        0        0      329 2024-04-19 17:19:02.229326 que_sdk-0.1.1/que_sdk/types.py
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 que_sdk-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-12 14:53:33.472804 que_sdk-0.1.2/LICENSE
+-rw-r--r--   0        0        0       10 2024-04-19 17:17:10.806057 que_sdk-0.1.2/README.md
+-rw-r--r--   0        0        0     1130 2024-04-23 09:03:40.690601 que_sdk-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      435 2024-04-20 08:19:42.640114 que_sdk-0.1.2/que_sdk/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-18 19:15:55.848369 que_sdk-0.1.2/que_sdk/_internal/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-13 18:33:05.063314 que_sdk-0.1.2/que_sdk/_internal/auth.py
+-rw-r--r--   0        0        0     2257 2024-04-19 18:42:30.920224 que_sdk-0.1.2/que_sdk/_internal/base.py
+-rw-r--r--   0        0        0     6339 2024-04-20 08:19:42.654293 que_sdk-0.1.2/que_sdk/client.py
+-rw-r--r--   0        0        0     5564 2024-04-23 09:01:58.852361 que_sdk-0.1.2/que_sdk/clients.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:15:10.383938 que_sdk-0.1.2/que_sdk/py.typed.py
+-rw-r--r--   0        0        0     1008 2024-04-23 08:59:04.018042 que_sdk-0.1.2/que_sdk/schemas.py
+-rw-r--r--   0        0        0      329 2024-04-19 17:19:02.229326 que_sdk-0.1.2/que_sdk/types.py
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 que_sdk-0.1.2/PKG-INFO
```

### Comparing `que_sdk-0.1.1/LICENSE` & `que_sdk-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `que_sdk-0.1.1/pyproject.toml` & `que_sdk-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 [tool.poetry]
 name = "que_sdk"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["DavidRomanovizc"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "^0.27.0"
-pre-commit = "^3.7.0"
-pydantic = "^2.4.1"
 backoff = "^2.2.1"
-yarl = "^1.9.4"
-
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.23.3"
+pre-commit = "^3.7.0"
 mypy = "^1.8.0"
 black = "^24.3.0"
 isort = "^5.13.2"
 deptry = "^0.12.0"
 ruff = "^0.1.14"
 pip-audit = "^2.7.0"
```

### Comparing `que_sdk-0.1.1/que_sdk/_internal/base.py` & `que_sdk-0.1.2/que_sdk/_internal/base.py`

 * *Files identical despite different names*

### Comparing `que_sdk-0.1.1/que_sdk/client.py` & `que_sdk-0.1.2/que_sdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 )
 from que_sdk.types import (
     ClientsNameT,
     FlexibleResponseT,
     ResponseT,
 )
 
-__all__ = ("Client",)
+__all__ = ("QueClient",)
 
 
-class Client:
+class QueClient:
     def __init__(self) -> None:
         self._clients = {
             "auth": AuthClient(),
             "user": UserClient(),
             "role": RoleClient(),
         }
```

### Comparing `que_sdk-0.1.1/que_sdk/clients.py` & `que_sdk-0.1.2/que_sdk/clients.py`

 * *Files identical despite different names*

