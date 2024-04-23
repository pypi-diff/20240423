# Comparing `tmp/skytek_generic_map_api-0.9.0.tar.gz` & `tmp/skytek_generic_map_api-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytek_generic_map_api-0.9.0.tar", last modified: Mon Apr 22 09:50:32 2024, max compression
+gzip compressed data, was "skytek_generic_map_api-0.9.1.tar", last modified: Tue Apr 23 18:43:16 2024, max compression
```

## Comparing `skytek_generic_map_api-0.9.0.tar` & `skytek_generic_map_api-0.9.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:32.072613 skytek_generic_map_api-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-22 09:50:32.072613 skytek_generic_map_api-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:32.068613 skytek_generic_map_api-0.9.0/generic_map_api/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 09:50:30.000000 skytek_generic_map_api-0.9.0/generic_map_api/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/date_line_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/geometry_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:32.068613 skytek_generic_map_api-0.9.0/generic_map_api/multi_meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/multi_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/multi_meta/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/multi_meta/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:32.068613 skytek_generic_map_api-0.9.0/generic_map_api/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/resources/empty_tile.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:32.068613 skytek_generic_map_api-0.9.0/generic_map_api/resources/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/resources/icons/default-features.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/resources/icons/default-tiles.png
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/resources/icons/default.png
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/routers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/values.py
--rw-r--r--   0 runner    (1001) docker     (127)    10975 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/generic_map_api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:32.068613 skytek_generic_map_api-0.9.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/requirements/lint.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:50:32.072613 skytek_generic_map_api-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:32.072613 skytek_generic_map_api-0.9.0/skytek_generic_map_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-22 09:50:32.000000 skytek_generic_map_api-0.9.0/skytek_generic_map_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-22 09:50:32.000000 skytek_generic_map_api-0.9.0/skytek_generic_map_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:50:32.000000 skytek_generic_map_api-0.9.0/skytek_generic_map_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:50:31.000000 skytek_generic_map_api-0.9.0/skytek_generic_map_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-22 09:50:32.000000 skytek_generic_map_api-0.9.0/skytek_generic_map_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 09:50:32.000000 skytek_generic_map_api-0.9.0/skytek_generic_map_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:50:32.072613 skytek_generic_map_api-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-22 09:50:28.000000 skytek_generic_map_api-0.9.0/tests/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.628788 skytek_generic_map_api-0.9.1/generic_map_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 18:43:14.000000 skytek_generic_map_api-0.9.1/generic_map_api/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/date_line_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/geometry_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/generic_map_api/multi_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/multi_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/multi_meta/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/multi_meta/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/generic_map_api/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/resources/empty_tile.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default-features.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default-tiles.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/routers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/generic_map_api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/requirements/lint.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 18:43:16.000000 skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 18:43:16.632788 skytek_generic_map_api-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-23 18:43:08.000000 skytek_generic_map_api-0.9.1/tests/test_values.py
```

### Comparing `skytek_generic_map_api-0.9.0/LICENSE` & `skytek_generic_map_api-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/PKG-INFO` & `skytek_generic_map_api-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-generic-map-api
-Version: 0.9.0
+Version: 0.9.1
 Summary: skytek-generic-map-api - expose geographical data for Skytek's frontends
 Home-page: http://github.com/Skytek/generic-map-api
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/bounding_box.py` & `skytek_generic_map_api-0.9.1/generic_map_api/bounding_box.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/clustering.py` & `skytek_generic_map_api-0.9.1/generic_map_api/clustering.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/date_line_normalization.py` & `skytek_generic_map_api-0.9.1/generic_map_api/date_line_normalization.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/geometry_serializers.py` & `skytek_generic_map_api-0.9.1/generic_map_api/geometry_serializers.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/multi_meta/views.py` & `skytek_generic_map_api-0.9.1/generic_map_api/multi_meta/views.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/params.py` & `skytek_generic_map_api-0.9.1/generic_map_api/params.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/resources/empty_tile.png` & `skytek_generic_map_api-0.9.1/generic_map_api/resources/empty_tile.png`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/resources/icons/default-features.png` & `skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default-features.png`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/resources/icons/default-tiles.png` & `skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default-tiles.png`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/resources/icons/default.png` & `skytek_generic_map_api-0.9.1/generic_map_api/resources/icons/default.png`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/routers.py` & `skytek_generic_map_api-0.9.1/generic_map_api/routers.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/serializers.py` & `skytek_generic_map_api-0.9.1/generic_map_api/serializers.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/values.py` & `skytek_generic_map_api-0.9.1/generic_map_api/values.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/generic_map_api/views.py` & `skytek_generic_map_api-0.9.1/generic_map_api/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 from abc import ABC, ABCMeta, abstractmethod
 from base64 import b64encode
 from os import path
-from typing import Optional, Tuple, Type
+from typing import Callable, Optional, Tuple, Type
 
+from django.core.exceptions import BadRequest
 from django.db.models import QuerySet
 from django.http import Http404, HttpResponse
 from rest_framework.decorators import action
+from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.viewsets import ViewSet
 
-from .bounding_box import AutomaticBoundingBoxing, BaseBoundingBoxing
+from .bounding_box import AutomaticBoundingBoxing
 from .clustering import BaseClustering, BasicClustering, ClusteringOutput
 from .constants import ViewportHandling
 from .serializers import BaseFeatureSerializer, BoundingBoxSerializer
 from .utils import to_bool
-from .values import BaseViewPort, EmptyViewport, Tile, ViewPort
+from .values import BaseViewPort, BoundingBox, EmptyViewport, Tile, ViewPort
 
 
 class MapApiBaseMeta(ABCMeta):
     def __new__(cls, name, bases, namespace, /, **kwargs):
         if "query_params" in namespace:
             for param_name, param in namespace["query_params"].items():
                 param.name = param_name
@@ -34,14 +36,16 @@
     icon = path.join(path.dirname(__file__), "resources", "icons", "default.png")
 
     query_params = {}
     has_parametrized_meta = False
 
     trailing_slash = None
 
+    get_bounds: Callable[[dict, Request], BoundingBox] | None = None
+
     @action(detail=False, url_path="_meta")
     def meta(self, request):
         meta = self.get_meta(request)
         if not "urls" in meta:
             meta["urls"] = {}
         meta["urls"] = {
             **meta["urls"],
@@ -52,27 +56,35 @@
     @action(detail=False, url_path="_meta/parametrized")
     def parametrized_meta(self, request):
         params = self._parse_params(request)
         return Response(self.get_parametrized_meta(request, params))
 
     @action(detail=False, url_path="bounds")
     def bounds(self, request):
-        raise NotImplementedError()
+        if not callable(self.get_bounds):
+            raise BadRequest()
+
+        params = self._parse_params(request)
+        bounds = self.get_bounds(params, request)  # pylint: disable=not-callable
+        return Response(BoundingBoxSerializer(bounds).data)
 
     @abstractmethod
     def get_meta(self, request):
         pass
 
     def get_parametrized_meta(self, request, params):  # pylint: disable=unused-argument
         return {}
 
     def get_urls(self):
         urls = {
             "meta": self.reverse_action("meta"),
         }
+        get_bounds_implemented = self.get_bounds is not None
+        if get_bounds_implemented:
+            urls["bounds"] = self.reverse_action("bounds")
         if self.has_parametrized_meta:
             urls["parametrized_meta"] = self.reverse_action("parametrized-meta")
         return urls
 
     @action(detail=False, url_path="_meta/query_param/(?P<query_param>[^/.]+)/options")
     def query_param_options(self, request, query_param):
         try:
@@ -118,36 +130,30 @@
     icon = path.join(
         path.dirname(__file__), "resources", "icons", "default-features.png"
     )
     serializer: BaseFeatureSerializer = None
     clustering: bool = False
     clustering_class: Type[BaseClustering] = BasicClustering
 
-    bounding_box_class = AutomaticBoundingBoxing
     bounding_box_db_geometry_field = None
 
     require_viewport_zoom: bool = False
     require_viewport_size: bool = False
     require_viewport_meters_per_pixel: bool = False
 
     preferred_viewport_handling: str = ViewportHandling.SPLIT
     preferred_viewport_chunks: int = 10
 
-    @action(detail=False, url_path="bounds")
-    def bounds(self, request):
+    def get_bounds(self, params, request):  # pylint: disable=unused-argument
         viewport = EmptyViewport()
-        params = self._parse_params(request)
         items = self.get_items(viewport, params)
-        bounds = self.get_bounding_box_algorithm().find_bounding_box(self, items)
-        return Response(BoundingBoxSerializer(bounds).data)
+        return AutomaticBoundingBoxing().find_bounding_box(self, items)
 
     def get_urls(self):
         urls = super().get_urls()
-        if self.get_bounding_box_algorithm():
-            urls["bounds"] = self.reverse_action("bounds")
         urls.update(
             {
                 "list": self.reverse_action("list"),
                 "detail": self.reverse_action("detail", kwargs={"pk": "ID"}),
             }
         )
         return urls
@@ -216,28 +222,27 @@
         if self.require_viewport_zoom:
             requirements.append("viewport.zoom")
         if self.require_viewport_meters_per_pixel:
             requirements.append("viewport.mpp")
         return requirements
 
     def retrieve(self, request, pk):  # pylint: disable=unused-argument
-        item = self.get_item(item_id=pk)
+        item = self.get_item(item_id=pk)  # pylint: disable=assignment-from-none
         if not item:
             raise Http404()
 
         response = {"item": self.render_detailed_item(item)}
         return Response(response)
 
     @abstractmethod
     def get_items(self, viewport: BaseViewPort, params: dict):
         pass
 
-    @abstractmethod
-    def get_item(self, item_id):
-        pass
+    def get_item(self, item_id):  # pylint: disable=unused-argument
+        return None
 
     def get_serializer(self, item):  # pylint: disable=unused-argument
         return self.serializer
 
     def render_item(self, item):
         return self.get_serializer(item).serialize(item)
 
@@ -248,32 +253,20 @@
 
     def render_detailed_item(self, item):
         return self.get_serializer(item).serialize_details(item)
 
     def get_clustering_algorithm(self) -> BaseClustering:
         return self.clustering_class()
 
-    def get_bounding_box_algorithm(self) -> BaseBoundingBoxing | None:
-        if not self.bounding_box_class:
-            return None
-        return self.bounding_box_class()
-
 
 class MapTilesBaseView(MapApiBaseView):
     icon = path.join(path.dirname(__file__), "resources", "icons", "default-tiles.png")
 
-    @action(detail=False, url_path="bounds")
-    def bounds(self, request):
-        bounds = ...
-        return Response(BoundingBoxSerializer(bounds).data)
-
     def get_urls(self):
         urls = super().get_urls()
-        if hasattr(self, "get_bounds"):
-            urls["bounds"] = self.reverse_action("bounds")
         urls.update(
             {
                 "tile": self.make_pattern_url(
                     "tile",
                     kwargs={
                         param: "{" + param + "}" for param in self.get_url_params()
                     },
```

### Comparing `skytek_generic_map_api-0.9.0/setup.py` & `skytek_generic_map_api-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `skytek_generic_map_api-0.9.0/skytek_generic_map_api.egg-info/PKG-INFO` & `skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytek-generic-map-api
-Version: 0.9.0
+Version: 0.9.1
 Summary: skytek-generic-map-api - expose geographical data for Skytek's frontends
 Home-page: http://github.com/Skytek/generic-map-api
 Author: Skytek Ltd.
 Author-email: wiktor.latanowicz@skytek.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `skytek_generic_map_api-0.9.0/skytek_generic_map_api.egg-info/SOURCES.txt` & `skytek_generic_map_api-0.9.1/skytek_generic_map_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

