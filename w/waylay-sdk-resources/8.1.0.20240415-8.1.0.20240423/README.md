# Comparing `tmp/waylay_sdk_resources-8.1.0.20240415.tar.gz` & `tmp/waylay_sdk_resources-8.1.0.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_resources-8.1.0.20240415.tar", last modified: Mon Apr 15 09:59:09 2024, max compression
+gzip compressed data, was "waylay_sdk_resources-8.1.0.20240423.tar", last modified: Tue Apr 23 16:13:03 2024, max compression
```

## Comparing `waylay_sdk_resources-8.1.0.20240415.tar` & `waylay_sdk_resources-8.1.0.20240423.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.764116 waylay_sdk_resources-8.1.0.20240415/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-15 09:59:09.764116 waylay_sdk_resources-8.1.0.20240415/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:59:09.764116 waylay_sdk_resources-8.1.0.20240415/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13271 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/batch_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/metadata_events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56362 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30375 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_constraint_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55935 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_type_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.760116 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-15 09:59:05.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:59:09.764116 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 09:59:09.000000 waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:03.727638 waylay_sdk_resources-8.1.0.20240423/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-23 16:13:03.727638 waylay_sdk_resources-8.1.0.20240423/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:13:03.727638 waylay_sdk_resources-8.1.0.20240423/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:03.719638 waylay_sdk_resources-8.1.0.20240423/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:03.719638 waylay_sdk_resources-8.1.0.20240423/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:03.719638 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:03.719638 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:03.723638 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/about_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/batch_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/metadata_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    59515 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32127 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/resource_constraint_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59088 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/resource_type_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:03.723638 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-23 16:12:59.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:03.723638 waylay_sdk_resources-8.1.0.20240423/src/waylay_sdk_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-23 16:13:03.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay_sdk_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-23 16:13:03.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay_sdk_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:13:03.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay_sdk_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 16:13:03.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay_sdk_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 16:13:03.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay_sdk_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 16:13:03.000000 waylay_sdk_resources-8.1.0.20240423/src/waylay_sdk_resources.egg-info/top_level.txt
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/LICENSE.txt` & `waylay_sdk_resources-8.1.0.20240423/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources-8.1.0.20240415/PKG-INFO` & `waylay_sdk_resources-8.1.0.20240423/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-resources
-Version: 8.1.0.20240415
+Version: 8.1.0.20240423
 Summary: Waylay Resources
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -20,15 +20,15 @@
 Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-resources-py.git
 Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/resources.html
 Keywords: Waylay Resources
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk-core~=0.2.1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/README.md` & `waylay_sdk_resources-8.1.0.20240423/README.md`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources-8.1.0.20240415/pyproject.toml` & `waylay_sdk_resources-8.1.0.20240423/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-resources"
-version = "8.1.0.20240415"
+version = "8.1.0.20240423"
 description = "Waylay Resources"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Resources"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.0",
+    "waylay-sdk-core ~= 0.2.1",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/about_api.py` & `waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/about_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,85 +65,92 @@
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VersionResponse: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VersionResponse | T | Response | Model:
         """Get Service Information.
 
         Get the name and version of the service.
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -154,26 +161,22 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": VersionResponse if not select_path else Model,
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/batch_operations_api.py` & `waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/batch_operations_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,14 +98,15 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BatchOperationStatusResponse: ...
 
     @overload
     async def get(
         self,
@@ -113,14 +114,15 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
@@ -128,14 +130,15 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
@@ -143,14 +146,15 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
@@ -158,42 +162,45 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         batch_id: Annotated[
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BatchOperationStatusResponse | T | Response | Model:
         """Get Resource Batch Operation Status.
 
         Get the results of the Resource Batch Operation.
         :param batch_id: Unique Batch Operation identifier (required)
         :type batch_id: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -204,28 +211,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "batchId": str(batch_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": BatchOperationStatusResponse if not select_path else Model,
@@ -257,14 +260,15 @@
         json: Annotated[
             BatchResourceOperation, Field(description="Resource Batch Operation")
         ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BatchOperationEnqueued: ...
 
     @overload
     async def start(
         self,
@@ -272,14 +276,15 @@
         json: Annotated[
             BatchResourceOperation, Field(description="Resource Batch Operation")
         ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def start(
         self,
@@ -287,14 +292,15 @@
         json: Annotated[
             BatchResourceOperation, Field(description="Resource Batch Operation")
         ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def start(
         self,
@@ -302,14 +308,15 @@
         json: Annotated[
             BatchResourceOperation, Field(description="Resource Batch Operation")
         ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def start(
         self,
@@ -317,42 +324,45 @@
         json: Annotated[
             BatchResourceOperation, Field(description="Resource Batch Operation")
         ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def start(
         self,
         *,
         json: Annotated[
             BatchResourceOperation, Field(description="Resource Batch Operation")
         ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BatchOperationEnqueued | T | Response | Model:
         """Bulk Delete.
 
         Deletes multiple _Resources_ or _Resource Types_ in one batch.
         :param json: Resource Batch Operation
         :type json: BatchResourceOperation, optional
         :param query: URL Query parameters.
         :type query: StartQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -363,35 +373,31 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and should_validate:
+        if json is not None and validate_request:
             body_adapter = TypeAdapter(
                 Annotated[
                     BatchResourceOperation,
                     Field(description="Resource Batch Operation"),
                 ]
             )
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(StartQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "202": BatchOperationEnqueued if not select_path else Model,
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/metadata_events_api.py` & `waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/metadata_events_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,83 +67,89 @@
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         stream: bool = True,
         timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> AsyncIterator[NdJsonResponseStream]: ...
 
     @overload
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         stream: bool = True,
         timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> AsyncIterator[T]: ...
 
     @overload
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         stream: bool = True,
         timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         stream: bool = True,
         timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> AsyncIterator[Model]: ...
 
     @overload
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         stream: bool = True,
         timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> AsyncIterator[T]: ...
 
     async def get_stream(
         self,
         *,
         query: GetStreamQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         stream: bool = True,
         timeout=STREAM_TIMEOUTS,
         **kwargs,
     ) -> (
         AsyncIterator[NdJsonResponseStream]
         | AsyncIterator[T]
@@ -157,14 +163,15 @@
         :type query: GetStreamQuery | QueryParamTypes, optional
         :param query['eventFormat'] (dict) <br> query.event_format (Query) : The format of events in the stream.   If specified this must be `application/cloudevents+json` (make sure to correctly URL encode the `+` as `%2B`)
         :type query['eventFormat']: GetStreamEventFormatParameter
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -175,26 +182,22 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(GetStreamQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": NdJsonResponseStream if not select_path else Model,
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_api.py` & `waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/resource_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -161,92 +161,99 @@
         self,
         *,
         json: ResourceEntity,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceCreationResponse: ...
 
     @overload
     async def create(
         self,
         *,
         json: ResourceEntity,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def create(
         self,
         *,
         json: ResourceEntity,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def create(
         self,
         *,
         json: ResourceEntity,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def create(
         self,
         *,
         json: ResourceEntity,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def create(
         self,
         *,
         json: ResourceEntity,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceCreationResponse | T | Response | Model:
         """Create Resource.
 
         Creates a new _Resource_.
         :param json: The json request body.
         :type json: ResourceEntity, optional
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -257,30 +264,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and should_validate:
+        if json is not None and validate_request:
             body_adapter = TypeAdapter(ResourceEntity)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(CreateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": ResourceCreationResponse if not select_path else Model,
@@ -311,92 +314,99 @@
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None: ...
 
     @overload
     async def delete(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def delete(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def delete(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None: ...
 
     @overload
     async def delete(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def delete(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None | T | Response:
         """Remove Resource.
 
         Removes an existing _Resource_.
         :param resource_id: _Resource_ id (required)
         :type resource_id: ResourceId
         :param query: URL Query parameters.
         :type query: DeleteQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -407,28 +417,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceId": str(resource_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(DeleteQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "204": None,
@@ -459,78 +465,84 @@
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceWithIdEntity: ...
 
     @overload
     async def get(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceWithIdEntity | T | Response | Model:
         """Get Resource.
 
         Retrieves a representation of the _Resource_.
         :param resource_id: _Resource_ id (required)
@@ -543,14 +555,15 @@
         :type query['field']: List[str]
         :param query['fields'] (dict) <br> query.fields (Query) : Select which attributes to render for each matching _Resource_ (comma-separated).
         :type query['fields']: List[str]
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -561,28 +574,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceId": str(resource_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceWithIdEntity if not select_path else Model,
@@ -612,78 +621,84 @@
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> List[ResourceChange]: ...
 
     @overload
     async def list_changes(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list_changes(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list_changes(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list_changes(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list_changes(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> List[ResourceChange] | T | Response | Model:
         """List Resource Changes.
 
         Lists the change history of a _Resource_.
         :param resource_id: _Resource_ id (required)
@@ -694,14 +709,15 @@
         :type query['skip']: int
         :param query['limit'] (dict) <br> query.limit (Query) : (Paging) maximal number of items returned
         :type query['limit']: int
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -712,28 +728,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceId": str(resource_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ListChangesQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": List[ResourceChange] if not select_path else Model,
@@ -763,78 +775,84 @@
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChildrenQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceListing: ...
 
     @overload
     async def list_children(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChildrenQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list_children(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChildrenQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list_children(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChildrenQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list_children(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChildrenQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list_children(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListChildrenQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceListing | T | Response | Model:
         """List Resource Children.
 
         Lists the children of a _Resource_, these are the _Resources_ that have the given _Resource_ referenced with the `parentId` attribute.
         :param resource_id: _Resource_ id (required)
@@ -851,14 +869,15 @@
         :type query['skip']: int
         :param query['limit'] (dict) <br> query.limit (Query) : (Paging) maximal number of items returned
         :type query['limit']: int
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -869,28 +888,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceId": str(resource_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ListChildrenQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceListing if not select_path else Model,
@@ -920,78 +935,84 @@
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListReferrersQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceListing: ...
 
     @overload
     async def list_referrers(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListReferrersQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list_referrers(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListReferrersQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list_referrers(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListReferrersQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list_referrers(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListReferrersQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list_referrers(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         query: ListReferrersQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceListing | T | Response | Model:
         """List Referring Resources.
 
         List the _Resources_ that reference the given _Resource_.  #### visibility This definition has visibility status `beta`.
         :param resource_id: _Resource_ id (required)
@@ -1006,14 +1027,15 @@
         :type query['skip']: int
         :param query['limit'] (dict) <br> query.limit (Query) : (Paging) maximal number of items returned
         :type query['limit']: int
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1024,28 +1046,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceId": str(resource_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ListReferrersQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceListing if not select_path else Model,
@@ -1074,73 +1092,79 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceListing: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceListing | T | Response | Model:
         """Query Resources.
 
         Lists _Resources_ that satisfy the given filters.
         :param query: URL Query parameters.
@@ -1175,14 +1199,15 @@
         :type query['distance']: str
         :param query['toplevelOnly'] (dict) <br> query.toplevel_only (Query) : If true, search only for _Resources_ without parent.
         :type query['toplevelOnly']: bool
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1193,26 +1218,22 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceListing if not select_path else Model,
@@ -1243,83 +1264,89 @@
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: PatchResourceEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceWithIdEntity: ...
 
     @overload
     async def patch(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: PatchResourceEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def patch(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: PatchResourceEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def patch(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: PatchResourceEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def patch(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: PatchResourceEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def patch(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: PatchResourceEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceWithIdEntity | T | Response | Model:
         """Create Or Update Resource Partially.
 
         Updates some attributes of an existing _Resource_, or creates a new one.  When updating an existing _Resource_ you can remove keys by setting their value to `null` in the body
         :param resource_id: _Resource_ id (required)
@@ -1328,14 +1355,15 @@
         :type json: PatchResourceEntity, optional
         :param query: URL Query parameters.
         :type query: PatchQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1346,32 +1374,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceId": str(resource_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and should_validate:
+        if json is not None and validate_request:
             body_adapter = TypeAdapter(PatchResourceEntity)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(PatchQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceWithIdEntity if not select_path else Model,
@@ -1402,83 +1426,89 @@
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: ResourceEntity,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceWithIdEntity: ...
 
     @overload
     async def replace(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: ResourceEntity,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def replace(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: ResourceEntity,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def replace(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: ResourceEntity,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def replace(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: ResourceEntity,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def replace(
         self,
         resource_id: Annotated[StrictStr, Field(description="_Resource_ id")],
         *,
         json: ResourceEntity,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceWithIdEntity | T | Response | Model:
         """Update Resource.
 
         Replaces a _Resource_ with a new representation.
         :param resource_id: _Resource_ id (required)
@@ -1487,14 +1517,15 @@
         :type json: ResourceEntity, optional
         :param query: URL Query parameters.
         :type query: ReplaceQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1505,32 +1536,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceId": str(resource_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and should_validate:
+        if json is not None and validate_request:
             body_adapter = TypeAdapter(ResourceEntity)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ReplaceQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceWithIdEntity if not select_path else Model,
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_constraint_api.py` & `waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/resource_constraint_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,92 +120,99 @@
         self,
         *,
         json: Constraint,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceConstraintCreationResponse: ...
 
     @overload
     async def create(
         self,
         *,
         json: Constraint,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def create(
         self,
         *,
         json: Constraint,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def create(
         self,
         *,
         json: Constraint,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def create(
         self,
         *,
         json: Constraint,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def create(
         self,
         *,
         json: Constraint,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceConstraintCreationResponse | T | Response | Model:
         """Create Resource Constraint.
 
         Creates a new _Resource Constraint_ from the given representation.
         :param json: The json request body.
         :type json: Constraint, optional
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -216,30 +223,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and should_validate:
+        if json is not None and validate_request:
             body_adapter = TypeAdapter(Constraint)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(CreateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": ResourceConstraintCreationResponse if not select_path else Model,
@@ -271,14 +274,15 @@
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None: ...
 
     @overload
     async def delete(
         self,
@@ -286,14 +290,15 @@
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def delete(
         self,
@@ -301,14 +306,15 @@
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def delete(
         self,
@@ -316,14 +322,15 @@
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None: ...
 
     @overload
     async def delete(
         self,
@@ -331,42 +338,45 @@
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def delete(
         self,
         resource_constraint_id: Annotated[
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None | T | Response:
         """Remove Resource Constraint.
 
         Removes a _Resource Constraint_. Fails if the _Resource Constraint_ is already applied to a _Resource Type_.
         :param resource_constraint_id: _Resource_ Constraint id (required)
         :type resource_constraint_id: str
         :param query: URL Query parameters.
         :type query: DeleteQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -377,28 +387,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceConstraintId": str(resource_constraint_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(DeleteQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "204": None,
@@ -431,14 +437,15 @@
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceConstraintWithIdEntity: ...
 
     @overload
     async def get(
         self,
@@ -446,14 +453,15 @@
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
@@ -461,14 +469,15 @@
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
@@ -476,14 +485,15 @@
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
@@ -491,42 +501,45 @@
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         resource_constraint_id: Annotated[
             str, Field(strict=True, description="_Resource_ Constraint id")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceConstraintWithIdEntity | T | Response | Model:
         """Get Resource Constraint.
 
         Gets the definition or _JSON Schema_ representation of a _Resource Constraint_.
         :param resource_constraint_id: _Resource_ Constraint id (required)
         :type resource_constraint_id: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -537,28 +550,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceConstraintId": str(resource_constraint_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceConstraintWithIdEntity if not select_path else Model,
@@ -587,73 +596,79 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> List[ResourceConstraintWithIdEntity]: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> List[ResourceConstraintWithIdEntity] | T | Response | Model:
         """List Resource Constraints.
 
         Lists _Resource Constraints_ that fulfill the given criteria.
         :param query: URL Query parameters.
@@ -664,14 +679,15 @@
         :type query['limit']: int
         :param query['filter'] (dict) <br> query.filter (Query) : (Filter) fuzzy search on multiple fields.
         :type query['filter']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -682,26 +698,22 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": List[ResourceConstraintWithIdEntity]
@@ -734,14 +746,15 @@
         ],
         *,
         json: Constraint,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceConstraintWithIdEntity: ...
 
     @overload
     async def replace(
         self,
@@ -750,14 +763,15 @@
         ],
         *,
         json: Constraint,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def replace(
         self,
@@ -766,14 +780,15 @@
         ],
         *,
         json: Constraint,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def replace(
         self,
@@ -782,14 +797,15 @@
         ],
         *,
         json: Constraint,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def replace(
         self,
@@ -798,14 +814,15 @@
         ],
         *,
         json: Constraint,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def replace(
         self,
         resource_constraint_id: Annotated[
@@ -813,14 +830,15 @@
         ],
         *,
         json: Constraint,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceConstraintWithIdEntity | T | Response | Model:
         """Update Resource Constraint.
 
         Replaces the full definition of a _Resource Constraint_. Fails if the _Resource Constraint_ is already applied to a _Resource Type_ that has _Resources_ assigned to it.
         :param resource_constraint_id: _Resource_ Constraint id (required)
@@ -829,14 +847,15 @@
         :type json: Constraint, optional
         :param query: URL Query parameters.
         :type query: ReplaceQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -847,32 +866,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceConstraintId": str(resource_constraint_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and should_validate:
+        if json is not None and validate_request:
             body_adapter = TypeAdapter(Constraint)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ReplaceQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceConstraintWithIdEntity if not select_path else Model,
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/api/resource_type_api.py` & `waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/api/resource_type_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -171,92 +171,99 @@
         self,
         *,
         json: ResourceTypeWithConstraints,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeCreationResponse: ...
 
     @overload
     async def create(
         self,
         *,
         json: ResourceTypeWithConstraints,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def create(
         self,
         *,
         json: ResourceTypeWithConstraints,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def create(
         self,
         *,
         json: ResourceTypeWithConstraints,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def create(
         self,
         *,
         json: ResourceTypeWithConstraints,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def create(
         self,
         *,
         json: ResourceTypeWithConstraints,
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeCreationResponse | T | Response | Model:
         """Create Resource Type.
 
         Create a new _Resource Type_.
         :param json: The json request body.
         :type json: ResourceTypeWithConstraints, optional
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -267,30 +274,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and should_validate:
+        if json is not None and validate_request:
             body_adapter = TypeAdapter(ResourceTypeWithConstraints)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(CreateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": ResourceTypeCreationResponse if not select_path else Model,
@@ -321,92 +324,99 @@
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None: ...
 
     @overload
     async def delete(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def delete(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def delete(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None: ...
 
     @overload
     async def delete(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def delete(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None | T | Response:
         """Remove Resource Type.
 
         Removes an existing _Resource Type_.
         :param resource_type_id: _Resource Type_ id (required)
         :type resource_type_id: ResourceTypeId
         :param query: URL Query parameters.
         :type query: DeleteQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -417,28 +427,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceTypeId": str(resource_type_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(DeleteQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "204": None,
@@ -470,78 +476,84 @@
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeWithIdEntity: ...
 
     @overload
     async def get(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeWithIdEntity | T | Response | Model:
         """Get Resource Type.
 
         Retrieves a representation of the _Resource Type_.
         :param resource_type_id: _Resource Type_ id (required)
@@ -552,14 +564,15 @@
         :type query['field']: List[str]
         :param query['fields'] (dict) <br> query.fields (Query) : Select which attributes to render for each matching _Resource_ (comma-separated).
         :type query['fields']: List[str]
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -570,28 +583,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceTypeId": str(resource_type_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceTypeWithIdEntity if not select_path else Model,
@@ -621,78 +630,84 @@
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> List[ResourceTypeChange]: ...
 
     @overload
     async def list_changes(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list_changes(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list_changes(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list_changes(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list_changes(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListChangesQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> List[ResourceTypeChange] | T | Response | Model:
         """List Resource Type Changes.
 
         Lists the change history of a _Resource Type_.
         :param resource_type_id: _Resource Type_ id (required)
@@ -703,14 +718,15 @@
         :type query['skip']: int
         :param query['limit'] (dict) <br> query.limit (Query) : (Paging) maximal number of items returned
         :type query['limit']: int
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -721,28 +737,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceTypeId": str(resource_type_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ListChangesQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": List[ResourceTypeChange] if not select_path else Model,
@@ -772,92 +784,99 @@
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListConstraintsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceConstraintWithIdEntity: ...
 
     @overload
     async def list_constraints(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListConstraintsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list_constraints(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListConstraintsQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list_constraints(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListConstraintsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list_constraints(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListConstraintsQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list_constraints(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: ListConstraintsQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceConstraintWithIdEntity | T | Response | Model:
         """Get Resource Type Constraints.
 
         Retrieves the resource constraints that are applicable for the _Resource Type_.   This endpoint supports different representations of the constraints. * `application/json`: will give the reserved keywords for metadata expressed as _Resource Constraint_ merged with all user defined _Resource Constraints_ applied on the _Resource Type_. * `application/schema+json`: returns the (merged) constraints as a JSON Schema * `application/vnd.waylay.paged+json`: returns the constraints as a list of _Resource Constraints_ as defined by the user
         :param resource_type_id: _Resource Type_ id (required)
         :type resource_type_id: ResourceTypeId
         :param query: URL Query parameters.
         :type query: ListConstraintsQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -868,28 +887,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceTypeId": str(resource_type_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ListConstraintsQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceConstraintWithIdEntity if not select_path else Model,
@@ -918,73 +933,79 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeListing: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeListing | T | Response | Model:
         """List Resource Types.
 
         List _Resource Types_.
         :param query: URL Query parameters.
@@ -1005,14 +1026,15 @@
         :type query['id']: List[ResourceTypeId]
         :param query['template'] (dict) <br> query.template (Query) : Return _Resource Types_ that are associated with the template.
         :type query['template']: str
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1023,26 +1045,22 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": ResourceTypeListing if not select_path else Model,
@@ -1073,83 +1091,89 @@
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: PatchResourceTypeEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeCreationResponse | ResourceTypeWithIdEntity: ...
 
     @overload
     async def patch(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: PatchResourceTypeEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def patch(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: PatchResourceTypeEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def patch(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: PatchResourceTypeEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def patch(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: PatchResourceTypeEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def patch(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: PatchResourceTypeEntity,
         query: PatchQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeCreationResponse | ResourceTypeWithIdEntity | T | Response | Model:
         """Create Or Update Resource Type.
 
         Add or modify attributes of an existing _Resource Type_. Remove attributes by including a `null`-valued property. Creates a new _Resource Type_ if it did not exist.
         :param resource_type_id: _Resource Type_ id (required)
@@ -1158,14 +1182,15 @@
         :type json: PatchResourceTypeEntity, optional
         :param query: URL Query parameters.
         :type query: PatchQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1176,32 +1201,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceTypeId": str(resource_type_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and should_validate:
+        if json is not None and validate_request:
             body_adapter = TypeAdapter(PatchResourceTypeEntity)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(PatchQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "201": ResourceTypeCreationResponse if not select_path else Model,
@@ -1234,83 +1255,89 @@
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: ResourceTypeWithConstraints,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeWithIdEntity: ...
 
     @overload
     async def replace(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: ResourceTypeWithConstraints,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def replace(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: ResourceTypeWithConstraints,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def replace(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: ResourceTypeWithConstraints,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def replace(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: ResourceTypeWithConstraints,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def replace(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         json: ResourceTypeWithConstraints,
         query: ReplaceQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeWithIdEntity | T | Response | Model:
         """Update Resource Type.
 
         Replaces a _Resource Types_ with a new representation.
         :param resource_type_id: _Resource Type_ id (required)
@@ -1319,14 +1346,15 @@
         :type json: ResourceTypeWithConstraints, optional
         :param query: URL Query parameters.
         :type query: ReplaceQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1337,32 +1365,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceTypeId": str(resource_type_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and should_validate:
+        if json is not None and validate_request:
             body_adapter = TypeAdapter(ResourceTypeWithConstraints)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(ReplaceQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "202": ResourceTypeWithIdEntity if not select_path else Model,
@@ -1394,92 +1418,99 @@
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: RevalidateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeWithIdEntity: ...
 
     @overload
     async def revalidate(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: RevalidateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def revalidate(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: RevalidateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def revalidate(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: RevalidateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def revalidate(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: RevalidateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def revalidate(
         self,
         resource_type_id: Annotated[StrictStr, Field(description="_Resource Type_ id")],
         *,
         query: RevalidateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
+        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> ResourceTypeWithIdEntity | T | Response | Model:
         """Revalidate Resource Type.
 
         Initiates revalidation of the _Resource Constraints_ of this _Resource Type_ on all its associated _Resources_.
         :param resource_type_id: _Resource Type_ id (required)
         :type resource_type_id: ResourceTypeId
         :param query: URL Query parameters.
         :type query: RevalidateQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
+        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -1490,28 +1521,24 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
-        should_validate = (
-            MODELS_AVAILABLE and self.api_client.config.client_side_validation
-        )
-
         # path parameters
         path_params: Dict[str, str] = {
             "resourceTypeId": str(resource_type_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and should_validate:
+        if query is not None and MODELS_AVAILABLE and validate_request:
             query = TypeAdapter(RevalidateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "202": ResourceTypeWithIdEntity if not select_path else Model,
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/__init__.py` & `waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/service/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 This service manages  [Waylay Resources](/#/features/resources/?id=resource) and related entities.  A _Waylay Resource_ models a real-world device or abstract entity of your IoT solution, and provides a context when processing data in the Rule Engine.  You'll interact with the _Waylay Resources_ API to create this _Digital Twin_ model,  a process that's also called _resource provisioning_.
 
 Generated by OpenAPI Generator (https://openapi-generator.tech)
 
 Do not edit the class manually.
 """
 
-__version__ = "8.1.0.20240415"
+__version__ = "8.1.0.20240423"
 
 from .service import ResourcesService
 
 PLUGINS = [ResourcesService]
 
 __all__ = [
     "__version__",
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/src/waylay/services/resources/service/service.py` & `waylay_sdk_resources-8.1.0.20240423/src/waylay/services/resources/service/service.py`

 * *Files identical despite different names*

### Comparing `waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/PKG-INFO` & `waylay_sdk_resources-8.1.0.20240423/src/waylay_sdk_resources.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-resources
-Version: 8.1.0.20240415
+Version: 8.1.0.20240423
 Summary: Waylay Resources
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -20,15 +20,15 @@
 Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-resources-py.git
 Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/resources.html
 Keywords: Waylay Resources
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.0
+Requires-Dist: waylay-sdk-core~=0.2.1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
```

### Comparing `waylay_sdk_resources-8.1.0.20240415/src/waylay_sdk_resources.egg-info/SOURCES.txt` & `waylay_sdk_resources-8.1.0.20240423/src/waylay_sdk_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

