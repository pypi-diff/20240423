# Comparing `tmp/resty_client-0.0.2.tar.gz` & `tmp/resty_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resty_client-0.0.2.tar", max compression
+gzip compressed data, was "resty_client-0.0.3.tar", max compression
```

## Comparing `resty_client-0.0.2.tar` & `resty_client-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1090 2024-01-23 13:22:57.074926 resty_client-0.0.2/LICENSE
--rw-r--r--   0        0        0     1072 2024-04-22 14:25:21.711123 resty_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3108 2024-04-22 14:25:21.707143 resty_client-0.0.2/README.md
--rw-r--r--   0        0        0      126 2024-01-26 15:20:15.262707 resty_client-0.0.2/resty/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 15:14:08.249782 resty_client-0.0.2/resty/clients/__init__.py
--rw-r--r--   0        0        0      179 2024-04-22 14:23:32.487305 resty_client-0.0.2/resty/clients/httpx/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-22 15:10:42.335626 resty_client-0.0.2/resty/clients/httpx/client.py
--rw-r--r--   0        0        0      557 2024-04-22 15:02:44.798358 resty_client-0.0.2/resty/constants.py
--rw-r--r--   0        0        0      370 2024-04-22 14:23:32.559298 resty_client-0.0.2/resty/enums.py
--rw-r--r--   0        0        0      631 2024-04-22 15:10:42.345629 resty_client-0.0.2/resty/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-26 15:14:08.265783 resty_client-0.0.2/resty/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 15:14:08.265783 resty_client-0.0.2/resty/ext/django/__init__.py
--rw-r--r--   0        0        0      200 2024-04-22 14:23:32.601297 resty_client-0.0.2/resty/ext/django/middlewares/__init__.py
--rw-r--r--   0        0        0     1304 2024-04-22 14:23:32.656298 resty_client-0.0.2/resty/ext/django/middlewares/pagination.py
--rw-r--r--   0        0        0       55 2024-04-22 14:23:32.632293 resty_client-0.0.2/resty/managers/__init__.py
--rw-r--r--   0        0        0     3796 2024-04-22 15:06:33.234242 resty_client-0.0.2/resty/managers/manager.py
--rw-r--r--   0        0        0      148 2024-04-22 14:23:32.485306 resty_client-0.0.2/resty/middlewares/__init__.py
--rw-r--r--   0        0        0     1328 2024-04-22 14:23:32.528299 resty_client-0.0.2/resty/middlewares/manager.py
--rw-r--r--   0        0        0      287 2024-04-22 14:23:32.497299 resty_client-0.0.2/resty/middlewares/types.py
--rw-r--r--   0        0        0       64 2024-04-22 14:23:32.502301 resty_client-0.0.2/resty/serializers/__init__.py
--rw-r--r--   0        0        0     1093 2024-04-22 14:47:08.995446 resty_client-0.0.2/resty/serializers/serializer.py
--rw-r--r--   0        0        0     2719 2024-04-22 14:59:12.276754 resty_client-0.0.2/resty/types.py
--rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 resty_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-01-23 13:22:57.074926 resty_client-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1093 2024-04-23 18:45:23.095044 resty_client-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3108 2024-04-22 14:25:21.707143 resty_client-0.0.3/README.md
+-rw-r--r--   0        0        0      126 2024-01-26 15:20:15.262707 resty_client-0.0.3/resty/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 15:14:08.249782 resty_client-0.0.3/resty/clients/__init__.py
+-rw-r--r--   0        0        0      179 2024-04-22 14:23:32.487305 resty_client-0.0.3/resty/clients/httpx/__init__.py
+-rw-r--r--   0        0        0     3351 2024-04-23 18:07:25.657688 resty_client-0.0.3/resty/clients/httpx/client.py
+-rw-r--r--   0        0        0      557 2024-04-22 15:02:44.798358 resty_client-0.0.3/resty/constants.py
+-rw-r--r--   0        0        0      370 2024-04-22 14:23:32.559298 resty_client-0.0.3/resty/enums.py
+-rw-r--r--   0        0        0      729 2024-04-23 10:31:25.956591 resty_client-0.0.3/resty/exceptions.py
+-rw-r--r--   0        0        0        0 2024-01-26 15:14:08.265783 resty_client-0.0.3/resty/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 15:14:08.265783 resty_client-0.0.3/resty/ext/django/__init__.py
+-rw-r--r--   0        0        0      200 2024-04-22 14:23:32.601297 resty_client-0.0.3/resty/ext/django/middlewares/__init__.py
+-rw-r--r--   0        0        0     1311 2024-04-23 16:28:55.203681 resty_client-0.0.3/resty/ext/django/middlewares/pagination.py
+-rw-r--r--   0        0        0       69 2024-04-23 09:51:08.271071 resty_client-0.0.3/resty/managers/__init__.py
+-rw-r--r--   0        0        0     4975 2024-04-23 18:07:25.719709 resty_client-0.0.3/resty/managers/manager.py
+-rw-r--r--   0        0        0      328 2024-04-23 09:51:08.258984 resty_client-0.0.3/resty/middlewares/__init__.py
+-rw-r--r--   0        0        0     1296 2024-04-23 16:28:55.207680 resty_client-0.0.3/resty/middlewares/manager.py
+-rw-r--r--   0        0        0      264 2024-04-23 09:47:25.043213 resty_client-0.0.3/resty/middlewares/types.py
+-rw-r--r--   0        0        0       81 2024-04-23 09:51:08.264970 resty_client-0.0.3/resty/serializers/__init__.py
+-rw-r--r--   0        0        0     1390 2024-04-23 18:21:24.086198 resty_client-0.0.3/resty/serializers/serializer.py
+-rw-r--r--   0        0        0     2861 2024-04-23 16:28:55.216676 resty_client-0.0.3/resty/types.py
+-rw-r--r--   0        0        0     3533 1970-01-01 00:00:00.000000 resty_client-0.0.3/PKG-INFO
```

### Comparing `resty_client-0.0.2/LICENSE` & `resty_client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.2/pyproject.toml` & `resty_client-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "resty-client"
-version = "0.0.2"
+version = "0.0.3"
 description = "RestyClient is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data validation and deserialization tools."
 authors = ["CrazyProger1 <crazyproger1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "resty" },
 ]
@@ -14,14 +14,15 @@
 pydantic = "^2.5.3"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.8.0"
 pytest = "^7.4.4"
 httpx = "^0.26.0"
 black = "^24.4.0"
+coverage = "^7.5.0"
 
 [tool.ruff]
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
```

### Comparing `resty_client-0.0.2/README.md` & `resty_client-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.2/resty/clients/httpx/client.py` & `resty_client-0.0.3/resty/clients/httpx/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,89 +14,96 @@
 from resty.exceptions import HTTPError
 from resty.middlewares import MiddlewareManager
 
 
 class RESTClient(BaseRESTClient):
 
     def __init__(
-            self,
-            xclient: httpx.AsyncClient,
-            middleware_manager: BaseMiddlewareManager = None,
+        self,
+        xclient: httpx.AsyncClient = None,
+        middleware_manager: BaseMiddlewareManager = None,
     ):
-        self._xclient = xclient
-        self._middleware_manager = middleware_manager or MiddlewareManager(
-            default_middlewares=None,
-        )
+
+        self._xclient = xclient or httpx.AsyncClient()
+        self._middleware_manager = middleware_manager or MiddlewareManager()
 
     @staticmethod
     def _parse_xresponse(xresponse: httpx.Response) -> dict | list | None:
         try:
             data = xresponse.json()
         except json.decoder.JSONDecodeError:
             data = {}
 
         return data
 
     @staticmethod
     def _check_status(
-            status: int, expected_status: int | Container[int], request: Request, url: str,
-            data: dict = None
+        status: int,
+        expected_status: int | Container[int],
+        request: Request,
+        url: str,
+        data: dict = None,
     ):
         if status != expected_status:
             if isinstance(expected_status, Container) and status in expected_status:
                 pass
             else:
                 exc: type[HTTPError] = STATUS_ERRORS.get(status, HTTPError)
                 raise exc(request=request, status=status, url=url, data=data)
 
+    async def _make_xrequest(self, request: Request):
+        return await self._xclient.request(
+            method=request.method.value,
+            url=request.url,
+            headers=request.headers,
+            json=request.json,
+            data=request.data,
+            params=request.params,
+            cookies=request.cookies,
+            follow_redirects=request.redirects,
+            timeout=request.timeout,
+        )
+
     def add_middleware(self, middleware: BaseMiddleware):
         self._middleware_manager.add_middleware(middleware=middleware)
 
-    async def request(self, request: Request, **kwargs) -> Response:
+    async def request(self, request: Request, **context) -> Response:
         if not isinstance(request, Request):
             raise TypeError("request is not of type Request")
 
-        expected_status: int = kwargs.pop(
+        expected_status: int = context.pop(
             "expected_status", DEFAULT_CODES.get(request.method)
         )
-        check_status: bool = kwargs.pop("check_status", True)
+        check_status: bool = context.pop("check_status", True)
 
         if not isinstance(expected_status, (int, Container)):
             raise TypeError("expected status should be type of int or Container[int]")
 
-        await self._middleware_manager.call_pre_middlewares(request=request, **kwargs)
-
-        xresponse = await self._xclient.request(
-            method=request.method.value,
-            url=request.url,
-            headers=request.headers,
-            json=request.json,
-            data=request.data,
-            params=request.params,
-            cookies=request.cookies,
-            follow_redirects=request.redirects,
-            timeout=request.timeout,
+        await self._middleware_manager.call_request_middlewares(
+            request=request, **context
         )
 
-        status = xresponse.status_code
+        xresponse = await self._make_xrequest(request=request)
 
         data = self._parse_xresponse(xresponse=xresponse)
 
+        status = xresponse.status_code
+
         if check_status:
             self._check_status(
                 status=status,
                 expected_status=expected_status,
                 request=request,
                 url=str(xresponse.url),
                 data=data,
             )
         response = Response(
             request=request,
             status=status,
             data=data,
         )
 
-        await self._middleware_manager.call_post_middlewares(
-            response=response, **kwargs
+        await self._middleware_manager.call_response_middlewares(
+            response=response, **context
         )
 
         return response
```

### Comparing `resty_client-0.0.2/resty/constants.py` & `resty_client-0.0.3/resty/constants.py`

 * *Files identical despite different names*

### Comparing `resty_client-0.0.2/resty/exceptions.py` & `resty_client-0.0.3/resty/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 from resty.types import Request
 
 
-class HTTPError(Exception):
+class RestyError(Exception):
+    pass
+
+
+class URLFormattingError(RestyError):
+    pass
+
+
+class HTTPError(RestyError):
     def __init__(self, request: Request, status: int, url: str, data: dict):
         self.request = request
         self.status = status
         self.url = url
         self.data = data
         super().__init__(f"{request.method.value}: {url} -> {status}")
```

### Comparing `resty_client-0.0.2/resty/middlewares/manager.py` & `resty_client-0.0.3/resty/middlewares/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from typing import Iterable
 
 from resty.types import (
     BaseMiddlewareManager,
     BaseMiddleware,
-    BasePreRequestMiddleware,
-    BasePostRequestMiddleware,
+    BaseRequestMiddleware,
+    BaseResponseMiddleware,
 )
 
 from resty.types import Request, Response
 
 
 class MiddlewareManager(BaseMiddlewareManager):
-    def __init__(self, default_middlewares: Iterable[BaseMiddleware] = None):
-        if not default_middlewares:
-            default_middlewares = []
-        for middleware in default_middlewares:
+    def __init__(self, middlewares: Iterable[BaseMiddleware] = None):
+        if not middlewares:
+            middlewares = []
+        for middleware in middlewares:
             self.add_middleware(middleware=middleware)
 
         self._middlewares = []
 
-    async def call_pre_middlewares(self, request: Request, **kwargs):
+    async def call_request_middlewares(self, request: Request, **context):
         for middleware in self._middlewares:
-            if isinstance(middleware, BasePreRequestMiddleware):
-                await middleware.handle_request(request=request, **kwargs)
+            if isinstance(middleware, BaseRequestMiddleware):
+                await middleware.handle_request(request=request, **context)
 
-    async def call_post_middlewares(self, response: Response, **kwargs):
+    async def call_response_middlewares(self, response: Response, **context):
         for middleware in self._middlewares:
-            if isinstance(middleware, BasePostRequestMiddleware):
-                await middleware.handle_response(response=response, **kwargs)
+            if isinstance(middleware, BaseResponseMiddleware):
+                await middleware.handle_response(response=response, **context)
 
     def add_middleware(self, middleware: BaseMiddleware):
         if not isinstance(middleware, BaseMiddleware):
             raise TypeError("middleware is not of type BaseMiddleware")
         self._middlewares.append(middleware)
```

### Comparing `resty_client-0.0.2/resty/serializers/serializer.py` & `resty_client-0.0.3/resty/serializers/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 import inspect
 
 from pydantic import BaseModel
 
+from resty.enums import Endpoint
 from resty.types import BaseSerializer
 
 
 class Serializer(BaseSerializer):
 
     @classmethod
     def get_schema(cls, **context) -> type[BaseModel]:
-        schema = context.get('schema')
+        schema = context.get("schema")
 
         if inspect.isclass(schema) and issubclass(schema, BaseModel):
             return schema
 
-        endpoint = context.get('endpoint')
+        endpoint = context.get("endpoint")
         schema = cls.schema
 
         if cls.schemas is not None:
-            schema = cls.schemas.get(endpoint, cls.schema)
+            schema = cls.schemas.get(
+                endpoint,
+                cls.schema or cls.schemas.get(Endpoint.BASE)
+            )
 
         if schema is None:
-            raise TypeError(f'Schema should be specified for {endpoint}')
+            raise TypeError(f"Schema should be specified for {endpoint}")
 
         return schema
 
     @classmethod
     def serialize(cls, obj: BaseModel, **context) -> dict:
         schema = cls.get_schema(**context)
         if not isinstance(obj, schema):
             raise TypeError("Object must be of type {}".format(schema))
-        return obj.model_dump()
+        return schema.model_dump(obj)
 
     @classmethod
     def deserialize(cls, data: dict, **context) -> BaseModel:
         schema = cls.get_schema(**context)
         return schema.model_validate(data)
+
+    @classmethod
+    def deserialize_many(cls, data: list[dict], **context) -> list[BaseModel]:
+        return [cls.deserialize(dataset, **context) for dataset in data]
```

### Comparing `resty_client-0.0.2/resty/types.py` & `resty_client-0.0.3/resty/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,59 +10,59 @@
 
 @dataclass
 class Request:
     url: str
     method: Method
     data: dict = None
     json: dict = None
-    timeout: int = None
+    timeout: int | None = None
     params: dict = field(default_factory=dict)
     headers: dict = field(default_factory=dict)
     cookies: dict = field(default_factory=dict)
     redirects: bool = False
 
 
 @dataclass
 class Response:
     request: Request
     status: int
-    data: dict = None
+    data: list | dict = None
 
 
 class BaseMiddleware(ABC):
     pass
 
 
-class BasePreRequestMiddleware(BaseMiddleware):
+class BaseRequestMiddleware(BaseMiddleware):
     @abstractmethod
-    async def handle_request(self, request: Request, **kwargs): ...
+    async def handle_request(self, request: Request, **context): ...
 
 
-class BasePostRequestMiddleware(BaseMiddleware):
+class BaseResponseMiddleware(BaseMiddleware):
     @abstractmethod
-    async def handle_response(self, response: Response, **kwargs): ...
+    async def handle_response(self, response: Response, **context): ...
 
 
 class BaseMiddlewareManager(ABC):
     @abstractmethod
-    async def call_pre_middlewares(self, request: Request, **kwargs): ...
+    async def call_request_middlewares(self, request: Request, **context): ...
 
     @abstractmethod
-    async def call_post_middlewares(self, response: Response, **kwargs): ...
+    async def call_response_middlewares(self, response: Response, **context): ...
 
     @abstractmethod
     def add_middleware(self, middleware: BaseMiddleware): ...
 
 
 class BaseRESTClient(ABC):
     @abstractmethod
     def add_middleware(self, middleware: BaseMiddleware): ...
 
     @abstractmethod
-    async def request(self, request: Request, **kwargs) -> Response: ...
+    async def request(self, request: Request, **context) -> Response: ...
 
 
 class BaseSerializer:
     schema: type[BaseModel] = None
     schemas: dict[Endpoint, type[BaseModel]] = None
 
     @classmethod
@@ -73,24 +73,28 @@
     @abstractmethod
     def serialize(cls, obj: BaseModel, **context) -> dict: ...
 
     @classmethod
     @abstractmethod
     def deserialize(cls, data: dict, **context) -> BaseModel: ...
 
+    @classmethod
+    @abstractmethod
+    def deserialize_many(cls, data: list[dict], **context) -> list[BaseModel]: ...
+
 
 class BaseManager:
     serializer: type[BaseSerializer]
     endpoints: dict[Endpoint, str]
     fields: dict[Field, str]
 
     @classmethod
     @abstractmethod
     async def create(
-            cls, client: BaseRESTClient, obj: BaseModel, **kwargs
+        cls, client: BaseRESTClient, obj: BaseModel, **kwargs
     ) -> BaseModel: ...
 
     @classmethod
     @abstractmethod
     async def read(cls, client: BaseRESTClient, **kwargs) -> Iterable[BaseModel]: ...
 
     @classmethod
```

### Comparing `resty_client-0.0.2/PKG-INFO` & `resty_client-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resty-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: RestyClient is a simple, easy-to-use Python library for interacting with REST APIs using Pydantic's powerful data validation and deserialization tools.
 License: MIT
 Author: CrazyProger1
 Author-email: crazyproger1@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

