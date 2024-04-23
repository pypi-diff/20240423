# Comparing `tmp/hhru-0.0.1.tar.gz` & `tmp/hhru-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhru-0.0.1.tar", max compression
+gzip compressed data, was "hhru-0.1.0.tar", max compression
```

## Comparing `hhru-0.0.1.tar` & `hhru-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,27 @@
--rw-r--r--   0        0        0      900 2022-10-06 18:38:00.892988 hhru-0.0.1/hhru/__init__.py
--rw-r--r--   0        0        0      336 2022-10-06 18:36:14.375888 hhru-0.0.1/hhru/__version__.py
--rw-r--r--   0        0        0     1568 2022-09-21 17:05:39.237557 hhru-0.0.1/hhru/api.py
--rw-r--r--   0        0        0      149 2022-09-21 17:06:27.975871 hhru-0.0.1/hhru/auth.py
--rw-r--r--   0        0        0     1975 2022-10-06 18:34:11.525713 hhru-0.0.1/hhru/client.py
--rw-r--r--   0        0        0     1130 2022-10-06 18:11:23.784560 hhru-0.0.1/hhru/consts.py
--rw-r--r--   0        0        0        0 2022-08-04 16:09:19.056423 hhru-0.0.1/hhru/py.typed
--rw-r--r--   0        0        0     2178 2022-09-21 17:06:47.426013 hhru-0.0.1/hhru/response.py
--rw-r--r--   0        0        0     1091 2022-09-21 16:51:19.143292 hhru-0.0.1/LICENSE
--rw-r--r--   0        0        0      341 2022-10-06 18:36:47.307119 hhru-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      603 1970-01-01 00:00:00.000000 hhru-0.0.1/setup.py
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 hhru-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      794 2024-04-22 00:18:49.405474 hhru-0.1.0/hhru/__init__.py
+-rw-r--r--   0        0        0      332 2024-04-21 23:39:20.691000 hhru-0.1.0/hhru/__version__.py
+-rw-r--r--   0        0        0      287 2024-04-23 15:14:54.869148 hhru-0.1.0/hhru/auth/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-22 01:22:42.736418 hhru-0.1.0/hhru/auth/providers/__init__.py
+-rw-r--r--   0        0        0      517 2024-04-22 01:22:29.732440 hhru-0.1.0/hhru/auth/providers/_direct_auth.py
+-rw-r--r--   0        0        0      252 2024-04-21 23:33:21.696039 hhru-0.1.0/hhru/auth/providers/abstract.py
+-rw-r--r--   0        0        0      308 2024-04-22 00:05:15.345917 hhru-0.1.0/hhru/auth/providers/anonymous.py
+-rw-r--r--   0        0        0      664 2024-04-21 23:36:55.151001 hhru-0.1.0/hhru/auth/type.py
+-rw-r--r--   0        0        0      336 2024-04-22 00:49:09.826144 hhru-0.1.0/hhru/backend/__init__.py
+-rw-r--r--   0        0        0       88 2024-04-21 23:53:32.622069 hhru-0.1.0/hhru/backend/abstract/__init__.py
+-rw-r--r--   0        0        0      444 2024-04-22 00:20:57.819896 hhru-0.1.0/hhru/backend/abstract/abstract.py
+-rw-r--r--   0        0        0       78 2024-04-22 00:16:59.660759 hhru-0.1.0/hhru/backend/api/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-22 00:16:28.926067 hhru-0.1.0/hhru/backend/api/consts.py
+-rw-r--r--   0        0        0     1360 2024-04-22 00:01:58.903908 hhru-0.1.0/hhru/backend/api/http_response.py
+-rw-r--r--   0        0        0     1917 2024-04-22 00:25:33.933158 hhru-0.1.0/hhru/backend/api/provider.py
+-rw-r--r--   0        0        0      653 2024-04-22 00:30:49.087703 hhru-0.1.0/hhru/backend/protocol.py
+-rw-r--r--   0        0        0       78 2024-04-22 00:45:27.416473 hhru-0.1.0/hhru/backend/web/__init__.py
+-rw-r--r--   0        0        0      607 2024-04-22 01:13:06.015343 hhru-0.1.0/hhru/backend/web/consts.py
+-rw-r--r--   0        0        0     2453 2024-04-23 15:14:21.913318 hhru-0.1.0/hhru/backend/web/provider.py
+-rw-r--r--   0        0        0     9605 2024-04-22 01:09:34.929994 hhru-0.1.0/hhru/backend/web/t.py
+-rw-r--r--   0        0        0      867 2024-04-22 00:42:32.367978 hhru-0.1.0/hhru/client.py
+-rw-r--r--   0        0        0     1130 2024-04-21 22:53:42.484227 hhru-0.1.0/hhru/consts.py
+-rw-r--r--   0        0        0        0 2024-04-21 18:20:53.377235 hhru-0.1.0/hhru/py.typed
+-rw-r--r--   0        0        0     1091 2024-04-21 18:20:53.372725 hhru-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1312 2024-04-23 15:13:13.715659 hhru-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      529 2024-04-21 18:20:53.372725 hhru-0.1.0/README.md
+-rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 hhru-0.1.0/PKG-INFO
```

### Comparing `hhru-0.0.1/hhru/consts.py` & `hhru-0.1.0/hhru/consts.py`

 * *Files identical despite different names*

### Comparing `hhru-0.0.1/hhru/response.py` & `hhru-0.1.0/hhru/backend/api/http_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,22 @@
-"""
-    Response class.
-    Result of all API methods.
-"""
+from typing import Any, Dict
 
-from typing import Dict, Any, Optional
 from requests import Response
 
 
-class Response:
+class BackendApiResponse:
     """
-    API response structure.
+    Backend API response structure (JSON)
     """
 
-    # Raw response fields.
-    _raw_json: Optional[Dict] = None
-    _raw_response: Optional[Response] = None
+    def __init__(self, response: Response) -> None:
+        self._raw_response = response
+        self._raw_json: Dict[Any, Any] = self._raw_response.json()
 
-    def __init__(self, http_response: Response):
-        """
-        :param http_response: Response object (HTTP).
-        """
-
-        # Store raw response to work later.
-        self._raw_response = http_response
-
-        # Parse raw response once for working later.
-        self._raw_json = self._raw_response.json()
-
-    def get(self, key: str, default: Any = None):
+    def get(self, key: str, default: Any = None) -> Any:
         """
         Allows to access Response fields by `response.get(field, default)`.
         """
         try:
             return self[key]
         except KeyError:
             return default
@@ -42,30 +27,20 @@
         Notice that this will fall with `KeyError` if field was not found in the response.
         """
         if key not in self._raw_json:
             raise KeyError(f"{key} does not exist in the response!")
         field_value = self._raw_json.get(key, None)
         return field_value
 
-    def __getattr__(self, attribute_name: str) -> Any:
-        """
-        Allows to access Response fields by `response.my_response_var`.
-        Notice that this will fall with `AttributeError` if field was not found in the response.
-        """
-        if attribute_name not in self._raw_json:
-            raise AttributeError(f"{attribute_name} does not exist in the response!")
-        attribute_value = self._raw_json.get(attribute_name, None)
-        return attribute_value
-
-    def raw_json(self) -> Dict:
+    def raw_json(self) -> Dict[Any, Any]:
         """
         Returns raw JSON from the response.
         WARNING: Do not use this method.
         """
         return self._raw_json
 
-    def raw_response(self) -> Response:
+    @property
+    def status_code(self) -> int:
         """
-        Returns raw response object.
-        WARNING: Do not use this method.
+        Returns HTTP status code of the request
         """
-        return self._raw_response
+        return self._raw_response.status_code
```

### Comparing `hhru-0.0.1/LICENSE` & `hhru-0.1.0/LICENSE`

 * *Files identical despite different names*

