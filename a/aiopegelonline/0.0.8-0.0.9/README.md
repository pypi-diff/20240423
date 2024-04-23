# Comparing `tmp/aiopegelonline-0.0.8-py3-none-any.whl.zip` & `tmp/aiopegelonline-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9408 bytes, number of entries: 11
--rw-r--r--  2.0 unx     2946 b- defN 24-Feb-11 16:05 aiopegelonline/__init__.py
--rw-r--r--  2.0 unx      278 b- defN 24-Feb-11 16:05 aiopegelonline/const.py
--rw-r--r--  2.0 unx      434 b- defN 24-Feb-11 16:05 aiopegelonline/exceptions.py
--rw-r--r--  2.0 unx     3755 b- defN 24-Feb-11 16:05 aiopegelonline/models.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-11 16:05 aiopegelonline/py.typed
--rw-r--r--  2.0 unx    11357 b- defN 24-Feb-11 16:05 aiopegelonline-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3124 b- defN 24-Feb-11 16:05 aiopegelonline-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-11 16:05 aiopegelonline-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-Feb-11 16:05 aiopegelonline-0.0.8.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Feb-11 16:05 aiopegelonline-0.0.8.dist-info/zip-safe
--rw-rw-r--  2.0 unx      919 b- defN 24-Feb-11 16:05 aiopegelonline-0.0.8.dist-info/RECORD
-11 files, 22921 bytes uncompressed, 7836 bytes compressed:  65.8%
+Zip file size: 9669 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     3608 b- defN 24-Feb-16 21:48 aiopegelonline/__init__.py
+-rw-r--r--  2.0 unx      278 b- defN 24-Feb-16 21:48 aiopegelonline/const.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Feb-16 21:48 aiopegelonline/exceptions.py
+-rw-r--r--  2.0 unx     3917 b- defN 24-Feb-16 21:48 aiopegelonline/models.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Feb-16 21:48 aiopegelonline/py.typed
+-rw-r--r--  2.0 unx    11357 b- defN 24-Feb-16 21:48 aiopegelonline-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3226 b- defN 24-Feb-16 21:48 aiopegelonline-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-16 21:48 aiopegelonline-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-Feb-16 21:48 aiopegelonline-0.0.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Feb-16 21:48 aiopegelonline-0.0.9.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      919 b- defN 24-Feb-16 21:48 aiopegelonline-0.0.9.dist-info/RECORD
+11 files, 23847 bytes uncompressed, 8097 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: aiopegelonline/models.py
 Comment: 
 
 Filename: aiopegelonline/py.typed
 Comment: 
 
-Filename: aiopegelonline-0.0.8.dist-info/LICENSE
+Filename: aiopegelonline-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: aiopegelonline-0.0.8.dist-info/METADATA
+Filename: aiopegelonline-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: aiopegelonline-0.0.8.dist-info/WHEEL
+Filename: aiopegelonline-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: aiopegelonline-0.0.8.dist-info/top_level.txt
+Filename: aiopegelonline-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: aiopegelonline-0.0.8.dist-info/zip-safe
+Filename: aiopegelonline-0.0.9.dist-info/zip-safe
 Comment: 
 
-Filename: aiopegelonline-0.0.8.dist-info/RECORD
+Filename: aiopegelonline-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiopegelonline/__init__.py

```diff
@@ -4,32 +4,51 @@
 
 import json
 
 from aiohttp.client import ClientSession
 
 from .const import BASE_URL, CONNECT_ERRORS, LOGGER
 from .exceptions import PegelonlineDataError
-from .models import Station, StationMeasurements
+from .models import CacheEntry, Station, StationMeasurements
 
 
 class PegelOnline:
     """Pegelonline api."""
 
     def __init__(self, aiohttp_session: ClientSession) -> None:
         """Pegelonline api init."""
         self.session: ClientSession = aiohttp_session
+        self.cache: dict[str, CacheEntry] = {}
 
     async def _async_do_request(self, url: str, params: dict):
         """Perform an async request."""
-        LOGGER.debug("REQUEST url: %s params: %s", url, params)
+        cache_key = f"{url}_{params}"
+        if cache_key not in self.cache:
+            self.cache[cache_key] = CacheEntry(None, None)
+
+        cache_entry = self.cache[cache_key]
+
+        headers = {}
+        if (etag := cache_entry.etag) is not None:
+            headers = {"If-None-Match": etag}
+
+        LOGGER.debug("REQUEST url: %s params: %s headers: %s", url, params, headers)
         try:
-            async with self.session.get(url, params=params) as resp:
+            async with self.session.get(url, params=params, headers=headers) as resp:
                 result = await resp.text()
                 LOGGER.debug("RESPONSE status: %s text: %s", resp.status, result)
+
+                if resp.status == 304:  # 304 = not modified
+                    return cache_entry.result
+
+                if cache_entry.etag is None:
+                    cache_entry.etag = resp.headers.get("Etag")
+
                 result = json.loads(result)
+                cache_entry.result = result
                 if resp.status != 200:
                     raise PegelonlineDataError(
                         result.get("status"), result.get("message")
                     )
         except CONNECT_ERRORS as err:
             LOGGER.exception("Error while getting data: %s", err.__class__.__name__)
             raise err
```

## aiopegelonline/models.py

```diff
@@ -1,11 +1,13 @@
 """aiopegelonline models."""
 
 from __future__ import annotations
 
+from dataclasses import dataclass
+
 
 class Station:
     """Representation of a station."""
 
     def __init__(self, data: dict) -> None:
         """Initialize station class."""
         self.uuid: str = data["uuid"]
@@ -89,7 +91,15 @@
             "oxygen_level": self.oxygen_level,
             "ph_value": self.ph_value,
             "water_speed": self.water_speed,
             "water_flow": self.water_flow,
             "water_level": self.water_level,
             "water_temperature": self.water_temperature,
         }
+
+
+@dataclass
+class CacheEntry:
+    """Representation of response cache entry."""
+
+    etag: str | None
+    result: dict | None
```

## Comparing `aiopegelonline-0.0.8.dist-info/LICENSE` & `aiopegelonline-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiopegelonline-0.0.8.dist-info/METADATA` & `aiopegelonline-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: aiopegelonline
-Version: 0.0.8
+Version: 0.0.9
 Summary: Asynchronous library to retrieve data from PEGELONLINE.
 Home-page: https://github.com/mib1185/aiopegelonline
 Author: mib1185
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 
 [![Test](https://github.com/mib1185/aiopegelonline/actions/workflows/test.yml/badge.svg)](https://github.com/mib1185/aiopegelonline/actions/workflows/test.yml)
```

