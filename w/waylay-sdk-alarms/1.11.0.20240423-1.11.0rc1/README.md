# Comparing `tmp/waylay_sdk_alarms-1.11.0.20240423.tar.gz` & `tmp/waylay-sdk-alarms-1.11.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waylay_sdk_alarms-1.11.0.20240423.tar", last modified: Tue Apr 23 16:04:49 2024, max compression
+gzip compressed data, was "waylay-sdk-alarms-1.11.0rc1.tar", last modified: Wed Mar 27 16:12:59 2024, max compression
```

## Comparing `waylay_sdk_alarms-1.11.0.20240423.tar` & `waylay-sdk-alarms-1.11.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:49.421521 waylay_sdk_alarms-1.11.0.20240423/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-23 16:04:49.421521 waylay_sdk_alarms-1.11.0.20240423/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:04:49.421521 waylay_sdk_alarms-1.11.0.20240423/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:49.417521 waylay_sdk_alarms-1.11.0.20240423/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:49.417521 waylay_sdk_alarms-1.11.0.20240423/src/waylay/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:49.417521 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:49.417521 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:49.417521 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/about_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/alarm_events_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    34664 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/alarms_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14011 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/alarms_batch_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:49.417521 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/service/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/service/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-23 16:04:45.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:04:49.421521 waylay_sdk_alarms-1.11.0.20240423/src/waylay_sdk_alarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-23 16:04:49.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay_sdk_alarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-23 16:04:49.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay_sdk_alarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:04:49.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay_sdk_alarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 16:04:49.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay_sdk_alarms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-23 16:04:49.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay_sdk_alarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 16:04:49.000000 waylay_sdk_alarms-1.11.0.20240423/src/waylay_sdk_alarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.907630 waylay-sdk-alarms-1.11.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-03-27 16:12:59.903630 waylay-sdk-alarms-1.11.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 16:12:59.907630 waylay-sdk-alarms-1.11.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.899630 waylay-sdk-alarms-1.11.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.899630 waylay-sdk-alarms-1.11.0rc1/src/waylay/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.899630 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.899630 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.899630 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarm_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32030 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarms_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarms_batch_operations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/version_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.903630 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/service/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-27 16:12:55.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 16:12:59.903630 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 16:12:59.000000 waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/top_level.txt
```

### Comparing `waylay_sdk_alarms-1.11.0.20240423/LICENSE.txt` & `waylay-sdk-alarms-1.11.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `waylay_sdk_alarms-1.11.0.20240423/PKG-INFO` & `waylay-sdk-alarms-1.11.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-alarms
-Version: 1.11.0.20240423
+Version: 1.11.0rc1
 Summary: Waylay Alarms
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-alarms-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/alarms.html
 Keywords: Waylay Alarms
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-alarms==1.11.0rc1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,51 +47,55 @@
 Requires-Dist: waylay-sdk-alarms-types; extra == "types"
 
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Alarms api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Alarms api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-alarms-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from alarms.models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from alarms.models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms-1.11.0.20240423/README.md` & `waylay-sdk-alarms-1.11.0rc1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Alarms api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Alarms api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-alarms-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from alarms.models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from alarms.models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms-1.11.0.20240423/pyproject.toml` & `waylay-sdk-alarms-1.11.0rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waylay-sdk-alarms"
-version = "1.11.0.20240423"
+version = "1.11.0rc1"
 description = "Waylay Alarms"
 authors = [
     { name = "Waylay", email = "info@waylay.io"}
 ]
 keywords = ["Waylay Alarms"]
 requires-python = ">= 3.9"
 dependencies = [
-    "waylay-sdk-core ~= 0.2.1",
+    "waylay-sdk ~= 0.0.4rc5",
+    "waylay-sdk-alarms == 1.11.0rc1",
     "pydantic ~= 2.6",
     "typing-extensions ~= 4.10",
     "eval-type-backport ~= 0.1.3; python_version < '3.10'",
 ]
 readme = "README.md"
 license={file = "LICENSE.txt"}
 
 [project.urls]
 Homepage = "https://www.waylay.io/"
-Documentation = "https://docs.waylay.io/#/api/?id=software-development-kits"
+Documentation = "https://docs.waylay.io/#/"
 Repository = "https://github.com/waylayio/waylay-sdk-alarms-py.git"
-"Openapi Specification" = "https://docs.waylay.io/openapi/public/redocly/alarms.html"
 
 [project.optional-dependencies]
 dev = [
     "mypy",
     "ruff",
     "types-python-jose",
     "types-appdirs",
```

### Comparing `waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/about_api.py` & `waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/version_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,35 +29,35 @@
     Response,
 )
 from waylay.sdk.api._models import Model
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.alarms.models import VersionResponse
-    from waylay.services.alarms.queries.about_api import GetQuery
+    from waylay.services.alarms.queries.version_api import GetQuery
 
 
 try:
     from waylay.services.alarms.models import VersionResponse
-    from waylay.services.alarms.queries.about_api import GetQuery
+    from waylay.services.alarms.queries.version_api import GetQuery
 
     MODELS_AVAILABLE = True
 except ImportError:
     MODELS_AVAILABLE = False
 
     if not TYPE_CHECKING:
         GetQuery = dict
         VersionResponse = Model
 
 
 T = TypeVar("T")
 
 
-class AboutApi(WithApiClient):
-    """AboutApi service methods.
+class VersionApi(WithApiClient):
+    """VersionApi service methods.
 
     NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
@@ -65,92 +65,85 @@
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
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
-        validate_request: StrictBool = True,
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
-        validate_request: StrictBool = True,
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
-        validate_request: StrictBool = True,
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
-        validate_request: StrictBool = True,
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
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> VersionResponse | T | Response | Model:
-        """Get Service Information.
+        """Version.
 
-        Get the name and version of the service.
+        Get the status and version of the service.
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -161,22 +154,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": VersionResponse if not select_path else Model,
```

### Comparing `waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/alarm_events_api.py` & `waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarm_events_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 """
 
 from __future__ import annotations  # for Python 3.7–3.9
 
 from typing import (
     TYPE_CHECKING,
     Any,
-    AsyncIterator,
     Dict,
     Literal,
     TypeVar,
     overload,
 )
 
 from pydantic import (
@@ -26,15 +25,14 @@
 )
 from waylay.sdk.api import (
     HeaderTypes,
     QueryParamTypes,
     Response,
 )
 from waylay.sdk.api._models import Model
-from waylay.sdk.api.constants import STREAM_TIMEOUTS
 from waylay.sdk.plugin import WithApiClient
 
 if TYPE_CHECKING:
     from waylay.services.alarms.models import NdJsonResponseStream
     from waylay.services.alarms.queries.alarm_events_api import GetQuery
 
 
@@ -67,111 +65,87 @@
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[NdJsonResponseStream]: ...
+    ) -> NdJsonResponseStream: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
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
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[Model]: ...
+    ) -> Model: ...
 
     @overload
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> AsyncIterator[T]: ...
+    ) -> T: ...
 
     async def get(
         self,
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
-        stream: bool = True,
-        timeout=STREAM_TIMEOUTS,
         **kwargs,
-    ) -> (
-        AsyncIterator[NdJsonResponseStream]
-        | AsyncIterator[T]
-        | Response
-        | AsyncIterator[Model]
-    ):
+    ) -> NdJsonResponseStream | T | Response | Model:
         """Alarm Events.
 
         Opens a data stream for all Alarm Events for this tenant.
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param query['eventFormat'] (dict) <br> query.event_format (Query) : The format of events in the stream.   If specified this must be `application/cloudevents+json` (make sure to correctly URL encode the `+` as `%2B`)
         :type query['eventFormat']: GetEventstreamEventFormatParameter
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -182,22 +156,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": NdJsonResponseStream if not select_path else Model,
@@ -210,14 +188,12 @@
         return await self.api_client.request(
             method="GET",
             resource_path="/alarms/v1/events",
             path_params=path_params,
             params=query,
             **body_args,
             headers=headers,
-            stream=stream,
-            timeout=timeout,
             **kwargs,
             response_type=response_types_map,
             select_path=select_path,
             raw_response=raw_response,
         )
```

### Comparing `waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/alarms_api.py` & `waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarms_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -121,104 +121,89 @@
     Do not edit the class manually.
     """
 
     @overload
     async def create(
         self,
         *,
-        json: Annotated[CreateAlarm, Field(description="Alarm Operations")],
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> AlarmEntity: ...
 
     @overload
     async def create(
         self,
         *,
-        json: Annotated[CreateAlarm, Field(description="Alarm Operations")],
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def create(
         self,
         *,
-        json: Annotated[CreateAlarm, Field(description="Alarm Operations")],
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def create(
         self,
         *,
-        json: Annotated[CreateAlarm, Field(description="Alarm Operations")],
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def create(
         self,
         *,
-        json: Annotated[CreateAlarm, Field(description="Alarm Operations")],
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def create(
         self,
         *,
-        json: Annotated[CreateAlarm, Field(description="Alarm Operations")],
         query: CreateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> AlarmEntity | T | Response | Model:
         """Create Alarm.
 
         Create an alarm.  If an `ACTIVE` or `ACKNOWLEDGED` alarm with the same `source.id` and `type` exists,  no new alarm is created.   Instead, the existing alarm is updated by incrementing the `count` property  and a new audit record of type `io.waylay.alarm.EventOccuredAgain` is added to the history.   Only the latest 1000 `io.waylay.alarm.EventOccuredAgain` audit records are kept in the history.
-        :param json: Alarm Operations
-        :type json: CreateAlarm, optional
         :param query: URL Query parameters.
         :type query: CreateQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -229,28 +214,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[CreateAlarm, Field(description="Alarm Operations")]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(CreateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": AlarmEntity if not select_path else Model,
@@ -280,99 +263,92 @@
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None: ...
 
     @overload
     async def delete(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def delete(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def delete(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None: ...
 
     @overload
     async def delete(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def delete(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: DeleteQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> None | T | Response:
         """Delete Alarm.
 
         Delete an Alarm.
         :param alarm_id: Unique Alarm Identifier (required)
         :type alarm_id: str
         :param query: URL Query parameters.
         :type query: DeleteQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -383,24 +359,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "alarmId": str(alarm_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(DeleteQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "204": None,
@@ -430,99 +410,92 @@
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> AlarmEntity: ...
 
     @overload
     async def get(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def get(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> AlarmEntity | T | Response | Model:
         """Get Alarm.
 
         Get an alarm.
         :param alarm_id: Unique Alarm Identifier (required)
         :type alarm_id: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -533,24 +506,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "alarmId": str(alarm_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": AlarmEntity if not select_path else Model,
@@ -579,79 +556,73 @@
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> AlarmsQueryResult: ...
 
     @overload
     async def list(
         self,
         *,
         query: ListQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
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
-        validate_request: StrictBool = True,
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
-        validate_request: StrictBool = True,
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
-        validate_request: StrictBool = True,
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
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> AlarmsQueryResult | T | Response | Model:
         """Query Multiple Alarms.
 
         Query multiple alarms using a query language. The response contains the total number of alarms that fulfill the criteria.  By default, returns the first 50 alarms.
         :param query: URL Query parameters.
@@ -694,15 +665,14 @@
         :type query['size']: int
         :param query['additionalQueryParams'] (dict) <br> query.additional_query_params (Query) : To query the alarms based on the value of an additional property of the alarm,  you can add the key of the additional property as query parameter  with value the value you expect the alarm to have.
         :type query['additionalQueryParams']: Dict[str, ListAdditionalQueryParamsParameterValue]
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -713,22 +683,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(ListQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": AlarmsQueryResult if not select_path else Model,
@@ -759,89 +733,83 @@
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         json: AlarmUpdate,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> AlarmEntity: ...
 
     @overload
     async def update(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         json: AlarmUpdate,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def update(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         json: AlarmUpdate,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def update(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         json: AlarmUpdate,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def update(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         json: AlarmUpdate,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def update(
         self,
         alarm_id: Annotated[StrictStr, Field(description="Unique Alarm Identifier")],
         *,
         json: AlarmUpdate,
         query: UpdateQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> AlarmEntity | T | Response | Model:
         """Update Alarm.
 
         Update an alarm.
         :param alarm_id: Unique Alarm Identifier (required)
@@ -850,15 +818,14 @@
         :type json: AlarmUpdate, optional
         :param query: URL Query parameters.
         :type query: UpdateQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -869,28 +836,32 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "alarmId": str(alarm_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
+        if json is not None and should_validate:
             body_adapter = TypeAdapter(AlarmUpdate)
             json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
         body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(UpdateQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": AlarmEntity if not select_path else Model,
```

### Comparing `waylay_sdk_alarms-1.11.0.20240423/src/waylay/services/alarms/api/alarms_batch_operations_api.py` & `waylay-sdk-alarms-1.11.0rc1/src/waylay/services/alarms/api/alarms_batch_operations_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -100,15 +100,14 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BatchOperationResults: ...
 
     @overload
     async def get(
         self,
@@ -116,15 +115,14 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def get(
         self,
@@ -132,15 +130,14 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def get(
         self,
@@ -148,15 +145,14 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def get(
         self,
@@ -164,45 +160,42 @@
             StrictStr, Field(description="Unique Batch Operation identifier")
         ],
         *,
         query: GetQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
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
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BatchOperationResults | T | Response | Model:
         """Get Alarms Batch Operation Status.
 
         Get the results of the Alarms Batch Operation.
         :param batch_id: Unique Batch Operation identifier (required)
         :type batch_id: str
         :param query: URL Query parameters.
         :type query: GetQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -213,24 +206,28 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {
             "batchId": str(batch_id),
         }
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(GetQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "200": BatchOperationResults if not select_path else Model,
@@ -255,116 +252,89 @@
             raw_response=raw_response,
         )
 
     @overload
     async def start(
         self,
         *,
-        json: Annotated[
-            ABatchAlarmsSpecification, Field(description="Batch Alarm Operation")
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BatchOperationEnqueued: ...
 
     @overload
     async def start(
         self,
         *,
-        json: Annotated[
-            ABatchAlarmsSpecification, Field(description="Batch Alarm Operation")
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: Literal[""] = "",
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     @overload
     async def start(
         self,
         *,
-        json: Annotated[
-            ABatchAlarmsSpecification, Field(description="Batch Alarm Operation")
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[True],
         select_path: Literal["_not_used_"] = "_not_used_",
         response_type: Literal[None] = None,  # not used
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Response: ...
 
     @overload
     async def start(
         self,
         *,
-        json: Annotated[
-            ABatchAlarmsSpecification, Field(description="Batch Alarm Operation")
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: Literal[None] = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> Model: ...
 
     @overload
     async def start(
         self,
         *,
-        json: Annotated[
-            ABatchAlarmsSpecification, Field(description="Batch Alarm Operation")
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: Literal[False] = False,
         select_path: str,
         response_type: T,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> T: ...
 
     async def start(
         self,
         *,
-        json: Annotated[
-            ABatchAlarmsSpecification, Field(description="Batch Alarm Operation")
-        ],
         query: StartQuery | QueryParamTypes | None = None,
         raw_response: StrictBool = False,
         select_path: str = "",
         response_type: T | None = None,
-        validate_request: StrictBool = True,
         headers: HeaderTypes | None = None,
         **kwargs,
     ) -> BatchOperationEnqueued | T | Response | Model:
         """Start Alarms Batch Operation.
 
         Start Alarms Batch Operation.
-        :param json: Batch Alarm Operation
-        :type json: ABatchAlarmsSpecification, optional
         :param query: URL Query parameters.
         :type query: StartQuery | QueryParamTypes, optional
         :param raw_response: If true, return the http Response object instead of returning an api model object, or throwing an ApiError.
         :param select_path: Denotes the json path applied to the response object before returning it.
                 Set it to the empty string `""` to receive the full response object.
         :param response_type: If specified, the response is parsed into an instance of the specified type.
-        :param validate_request: If set to false, the request body and query parameters are NOT validated against the models in the service types package, even when available.
         :param headers: Header parameters for this request
         :type headers: dict, optional
         :param `**kwargs`: Additional parameters passed on to the http client.
             See below.
         :Keyword Arguments:
             * timeout: a single numeric timeout in seconds,
                 or a tuple of _connect_, _read_, _write_ and _pool_ timeouts.
@@ -375,31 +345,26 @@
             * follow_redirects: bool
 
         :return: Returns the result object if the http request succeeded with status code '2XX'.
         :raises APIError: If the http request has a status code different from `2XX`. This
             object wraps both the http Response and any parsed data.
         """
 
+        should_validate = (
+            MODELS_AVAILABLE and self.api_client.config.client_side_validation
+        )
+
         # path parameters
         path_params: Dict[str, str] = {}
 
         ## named body parameters
         body_args: Dict[str, Any] = {}
-        if json is not None and validate_request:
-            body_adapter = TypeAdapter(
-                Annotated[
-                    ABatchAlarmsSpecification,
-                    Field(description="Batch Alarm Operation"),
-                ]
-            )
-            json = body_adapter.validate_python(json)  # type: ignore # https://github.com/pydantic/pydantic/discussions/7094
-        body_args["json"] = json
 
         # query parameters
-        if query is not None and MODELS_AVAILABLE and validate_request:
+        if query is not None and should_validate:
             query = TypeAdapter(StartQuery).validate_python(query)
 
         response_types_map: Dict[str, Any] = (
             {"2XX": response_type}
             if response_type is not None
             else {
                 "202": BatchOperationEnqueued if not select_path else Model,
```

### Comparing `waylay_sdk_alarms-1.11.0.20240423/src/waylay_sdk_alarms.egg-info/PKG-INFO` & `waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waylay-sdk-alarms
-Version: 1.11.0.20240423
+Version: 1.11.0rc1
 Summary: Waylay Alarms
 Author-email: Waylay <info@waylay.io>
 License: ISC License (ISC)
         Copyright 2024, Waylay
         
         Permission to use, copy, modify, and/or distribute this software for any purpose 
         with or without fee is hereby granted, provided that the above copyright notice 
@@ -13,22 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH 
         REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND 
         FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, 
         OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, 
         DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS 
         ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 Project-URL: Homepage, https://www.waylay.io/
-Project-URL: Documentation, https://docs.waylay.io/#/api/?id=software-development-kits
+Project-URL: Documentation, https://docs.waylay.io/#/
 Project-URL: Repository, https://github.com/waylayio/waylay-sdk-alarms-py.git
-Project-URL: Openapi Specification, https://docs.waylay.io/openapi/public/redocly/alarms.html
 Keywords: Waylay Alarms
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: waylay-sdk-core~=0.2.1
+Requires-Dist: waylay-sdk~=0.0.4rc5
+Requires-Dist: waylay-sdk-alarms==1.11.0rc1
 Requires-Dist: pydantic~=2.6
 Requires-Dist: typing-extensions~=4.10
 Requires-Dist: eval-type-backport~=0.1.3; python_version < "3.10"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: types-python-jose; extra == "dev"
@@ -47,51 +47,55 @@
 Requires-Dist: waylay-sdk-alarms-types; extra == "types"
 
 # Waylay Alarms Service
 No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
 This Python package is automatically generated based on the 
 Waylay Alarms OpenAPI specification (API version: 1.11.0)
-For more information, please visit [the openapi specification](https://docs.waylay.io/openapi/public/redocly/alarms.html).
 
-It consists of a plugin for the waylay-sdk-core package, and contains the Alarms api methods.
+It consists of a plugin for the waylay-sdk package, and contains the Alarms api methods.
 Note that the typed model classes for all path params, query params, body params and responses for each of the api methods are contained in a separate package called waylay-sdk-alarms-types.
 
 ## Requirements.
 This package requires Python 3.9+.
 
 ## Installation
-Typically this package is installed when installing the [waylay-sdk-core](https://pypi.org/project/waylay-sdk/) package to enable the service's functionality.
+Typically this package is installed when installing the [waylay-sdk](https://github.com/waylayio/waylay-sdk-py) package to enable the service's functionality.
 When the service api methods are required, waylay-sdk-alarms is included in:
-- ```pip install waylay-sdk-core[alarms]``` to install `waylay-sdk-core` along with only this service, or
-- ```pip install waylay-sdk-core[services]``` to install `waylay-sdk-core` along with all services.
+- ```pip install waylay-sdk[alarms]``` to install `waylay-sdk` along with only this service, or
+- ```pip install waylay-sdk[services]``` to install `waylay-sdk` along with all services.
 When the typed models are required, both waylay-sdk-alarms and waylay-sdk-alarms-types are included in:
-- ```pip install waylay-sdk-core[alarms,alarms-types]``` to install `waylay-sdk-core` along with only this service including the typed models, or
-- ```pip install waylay-sdk-core[services,services-types]``` to install `waylay-sdk-core` along with all services along with the typed models.
+- ```pip install waylay-sdk[alarms,alarms-types]``` to install `waylay-sdk` along with only this service including the typed models, or
+- ```pip install waylay-sdk[services,services-types]``` to install `waylay-sdk` along with all services along with the typed models.
 
 ## Usage
 
+
 ```python
 from pprint import pprint
 
-# Import the waylay-client from the waylay-sdk-core package
+# Import the waylay-client from the waylay-sdk package
 from waylay.sdk.client import WaylayClient
 from waylay.sdk.api.api_exceptions import ApiError
 
 # Intialize a waylay client instance
 waylay_client = WaylayClient.from_profile()
 
 # Note that the typed model classes for responses/parameters/... are only available when `waylay-sdk-alarms-types` is installed
-from waylay.services.alarms.models.version_response import VersionResponse
+from alarms.models.get_eventstream_event_format_parameter import GetEventstreamEventFormatParameter
+from alarms.models.nd_json_response_stream import NdJsonResponseStream
 try:
-    # Get Service Information
-    # calls `GET /alarms/v1`
-    api_response = await waylay_client.alarms.about.get(
+    # Alarm Events
+    # calls `GET /alarms/v1/events`
+    api_response = await waylay_client.alarms.alarm_events.get(
+        # query parameters:
+        query = {
+            'eventFormat': 'application/cloudevents+json'
+        },
     )
-    print("The response of alarms.about.get:\n")
+    print("The response of alarms.alarm_events.get:\n")
     pprint(api_response)
 except ApiError as e:
-    print("Exception when calling alarms.about.get: %s\n" % e)
+    print("Exception when calling alarms.alarm_events.get: %s\n" % e)
 ```
 
 
-For more information, please visit the [Waylay API documentation](https://docs.waylay.io/#/api/?id=software-development-kits).
```

### Comparing `waylay_sdk_alarms-1.11.0.20240423/src/waylay_sdk_alarms.egg-info/SOURCES.txt` & `waylay-sdk-alarms-1.11.0rc1/src/waylay_sdk_alarms.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/waylay/services/alarms/api/__init__.py
-src/waylay/services/alarms/api/about_api.py
 src/waylay/services/alarms/api/alarm_events_api.py
 src/waylay/services/alarms/api/alarms_api.py
 src/waylay/services/alarms/api/alarms_batch_operations_api.py
 src/waylay/services/alarms/api/py.typed
+src/waylay/services/alarms/api/version_api.py
 src/waylay/services/alarms/service/__init__.py
 src/waylay/services/alarms/service/py.typed
 src/waylay/services/alarms/service/service.py
 src/waylay_sdk_alarms.egg-info/PKG-INFO
 src/waylay_sdk_alarms.egg-info/SOURCES.txt
 src/waylay_sdk_alarms.egg-info/dependency_links.txt
 src/waylay_sdk_alarms.egg-info/entry_points.txt
```

