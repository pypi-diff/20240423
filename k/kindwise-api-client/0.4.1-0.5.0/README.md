# Comparing `tmp/kindwise_api_client-0.4.1.tar.gz` & `tmp/kindwise_api_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kindwise_api_client-0.4.1.tar", max compression
+gzip compressed data, was "kindwise_api_client-0.5.0.tar", max compression
```

## Comparing `kindwise_api_client-0.4.1.tar` & `kindwise_api_client-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1065 2024-04-04 08:34:31.234839 kindwise_api_client-0.4.1/LICENSE
--rw-r--r--   0        0        0    15417 2024-04-10 14:53:25.786549 kindwise_api_client-0.4.1/README.md
--rw-r--r--   0        0        0      342 2024-04-10 14:52:36.952691 kindwise_api_client-0.4.1/kindwise/__init__.py
--rw-r--r--   0        0        0    10089 2024-04-10 14:43:46.804522 kindwise_api_client-0.4.1/kindwise/core.py
--rw-r--r--   0        0        0     1694 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/crop_health.py
--rw-r--r--   0        0        0      877 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/insect.py
--rw-r--r--   0        0        0     6245 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/models.py
--rw-r--r--   0        0        0      887 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/mushroom.py
--rw-r--r--   0        0        0    14236 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/plant.py
--rw-r--r--   0        0        0      447 2024-04-04 08:34:31.238839 kindwise_api_client-0.4.1/kindwise/resources/views.crop_health.crop.json
--rw-r--r--   0        0        0     1570 2024-04-04 08:34:31.238839 kindwise_api_client-0.4.1/kindwise/resources/views.crop_health.disease.json
--rw-r--r--   0        0        0     1424 2023-12-04 10:18:11.804140 kindwise_api_client-0.4.1/kindwise/resources/views.insect.json
--rw-r--r--   0        0        0     2695 2023-12-04 09:08:49.453559 kindwise_api_client-0.4.1/kindwise/resources/views.mushroom.json
--rw-r--r--   0        0        0     1338 2023-12-04 10:41:58.031606 kindwise_api_client-0.4.1/kindwise/resources/views.plant.disease.json
--rw-r--r--   0        0        0     2425 2023-12-04 10:29:52.198769 kindwise_api_client-0.4.1/kindwise/resources/views.plant.json
--rw-r--r--   0        0        0      308 2024-04-04 08:34:31.238839 kindwise_api_client-0.4.1/kindwise/settings.py
--rw-r--r--   0        0        0        0 2023-11-21 14:46:34.497403 kindwise_api_client-0.4.1/kindwise/tests/__init__.py
--rw-r--r--   0        0        0     8975 2024-04-10 12:47:24.634072 kindwise_api_client-0.4.1/kindwise/tests/conftest.py
--rw-r--r--   0        0        0   100105 2023-11-28 08:59:44.985422 kindwise_api_client-0.4.1/kindwise/tests/resources/images/aloe-vera.jpg
--rw-r--r--   0        0        0   109179 2023-11-28 14:48:26.224560 kindwise_api_client-0.4.1/kindwise/tests/resources/images/amanita_muscaria.jpg
--rw-r--r--   0        0        0     6289 2023-11-22 08:44:35.598900 kindwise_api_client-0.4.1/kindwise/tests/resources/images/bee.jpeg
--rw-r--r--   0        0        0   448975 2023-06-22 12:24:49.335643 kindwise_api_client-0.4.1/kindwise/tests/resources/images/padli.png
--rw-r--r--   0        0        0   128013 2024-04-04 08:34:31.238839 kindwise_api_client-0.4.1/kindwise/tests/resources/images/potato.late_blight.jpg
--rw-r--r--   0        0        0    18267 2024-04-10 14:50:31.251909 kindwise_api_client-0.4.1/kindwise/tests/test_core.py
--rw-r--r--   0        0        0     1039 2024-04-10 12:38:19.718863 kindwise_api_client-0.4.1/kindwise/tests/test_crop.py
--rw-r--r--   0        0        0      894 2024-04-10 12:38:19.718863 kindwise_api_client-0.4.1/kindwise/tests/test_insect.py
--rw-r--r--   0        0        0     1025 2024-04-10 12:38:19.718863 kindwise_api_client-0.4.1/kindwise/tests/test_mushroom.py
--rw-r--r--   0        0        0    47760 2024-04-10 12:38:19.718863 kindwise_api_client-0.4.1/kindwise/tests/test_plant.py
--rw-r--r--   0        0        0      751 2024-04-10 15:01:03.960592 kindwise_api_client-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    16704 1970-01-01 00:00:00.000000 kindwise_api_client-0.4.1/setup.py
--rw-r--r--   0        0        0    16081 1970-01-01 00:00:00.000000 kindwise_api_client-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-04 08:34:31.234839 kindwise_api_client-0.5.0/LICENSE
+-rw-r--r--   0        0        0    16813 2024-04-23 13:01:42.234693 kindwise_api_client-0.5.0/README.md
+-rw-r--r--   0        0        0      373 2024-04-23 13:01:42.234693 kindwise_api_client-0.5.0/kindwise/__init__.py
+-rw-r--r--   0        0        0    11858 2024-04-23 13:01:42.234693 kindwise_api_client-0.5.0/kindwise/core.py
+-rw-r--r--   0        0        0     1958 2024-04-23 13:01:42.238693 kindwise_api_client-0.5.0/kindwise/crop_health.py
+-rw-r--r--   0        0        0     1086 2024-04-23 13:01:42.238693 kindwise_api_client-0.5.0/kindwise/insect.py
+-rw-r--r--   0        0        0     7082 2024-04-23 13:01:42.238693 kindwise_api_client-0.5.0/kindwise/models.py
+-rw-r--r--   0        0        0     1108 2024-04-23 13:01:42.238693 kindwise_api_client-0.5.0/kindwise/mushroom.py
+-rw-r--r--   0        0        0    14468 2024-04-23 13:01:42.238693 kindwise_api_client-0.5.0/kindwise/plant.py
+-rw-r--r--   0        0        0      447 2024-04-04 08:34:31.238839 kindwise_api_client-0.5.0/kindwise/resources/views.crop_health.crop.json
+-rw-r--r--   0        0        0     1570 2024-04-04 08:34:31.238839 kindwise_api_client-0.5.0/kindwise/resources/views.crop_health.disease.json
+-rw-r--r--   0        0        0     1424 2023-12-04 10:18:11.804140 kindwise_api_client-0.5.0/kindwise/resources/views.insect.json
+-rw-r--r--   0        0        0     2695 2023-12-04 09:08:49.453559 kindwise_api_client-0.5.0/kindwise/resources/views.mushroom.json
+-rw-r--r--   0        0        0     1338 2023-12-04 10:41:58.031606 kindwise_api_client-0.5.0/kindwise/resources/views.plant.disease.json
+-rw-r--r--   0        0        0     2425 2023-12-04 10:29:52.198769 kindwise_api_client-0.5.0/kindwise/resources/views.plant.json
+-rw-r--r--   0        0        0      516 2024-04-23 13:02:44.055562 kindwise_api_client-0.5.0/kindwise/settings.py
+-rw-r--r--   0        0        0        0 2023-11-21 14:46:34.497403 kindwise_api_client-0.5.0/kindwise/tests/__init__.py
+-rw-r--r--   0        0        0    10312 2024-04-23 13:01:42.238693 kindwise_api_client-0.5.0/kindwise/tests/conftest.py
+-rw-r--r--   0        0        0   100105 2023-11-28 08:59:44.985422 kindwise_api_client-0.5.0/kindwise/tests/resources/images/aloe-vera.jpg
+-rw-r--r--   0        0        0   109179 2023-11-28 14:48:26.224560 kindwise_api_client-0.5.0/kindwise/tests/resources/images/amanita_muscaria.jpg
+-rw-r--r--   0        0        0     6289 2023-11-22 08:44:35.598900 kindwise_api_client-0.5.0/kindwise/tests/resources/images/bee.jpeg
+-rw-r--r--   0        0        0   448975 2023-06-22 12:24:49.335643 kindwise_api_client-0.5.0/kindwise/tests/resources/images/padli.png
+-rw-r--r--   0        0        0   128013 2024-04-04 08:34:31.238839 kindwise_api_client-0.5.0/kindwise/tests/resources/images/potato.late_blight.jpg
+-rw-r--r--   0        0        0    23160 2024-04-23 13:01:42.238693 kindwise_api_client-0.5.0/kindwise/tests/test_core.py
+-rw-r--r--   0        0        0      991 2024-04-23 11:46:26.786693 kindwise_api_client-0.5.0/kindwise/tests/test_crop.py
+-rw-r--r--   0        0        0      846 2024-04-23 11:44:24.453288 kindwise_api_client-0.5.0/kindwise/tests/test_insect.py
+-rw-r--r--   0        0        0      977 2024-04-23 11:44:24.453288 kindwise_api_client-0.5.0/kindwise/tests/test_mushroom.py
+-rw-r--r--   0        0        0    47672 2024-04-23 11:46:26.786693 kindwise_api_client-0.5.0/kindwise/tests/test_plant.py
+-rw-r--r--   0        0        0      751 2024-04-23 13:06:12.426415 kindwise_api_client-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    18149 1970-01-01 00:00:00.000000 kindwise_api_client-0.5.0/setup.py
+-rw-r--r--   0        0        0    17477 1970-01-01 00:00:00.000000 kindwise_api_client-0.5.0/PKG-INFO
```

### Comparing `kindwise_api_client-0.4.1/LICENSE` & `kindwise_api_client-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/README.md` & `kindwise_api_client-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -73,14 +73,16 @@
 | [`usage_info`](#usage_info)                               | get api key usage information                                                       | `UsageInfo`        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | [`feedback`](#feedback)                                   | send feedback for identification                                                    | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | [`health_assessment`](#health_assessment)                 | create health assessment identification                                             | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |
 | [`get_health_assessment`](#get_health_assessment)         | get health assessment identification                                                | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |
 | [`delete_health_assessment`](#delete_health_assessment)   | delete health assessment                                                            | boolean            | :white_check_mark: | :x:                | :x:                | :x:                |
 | [`available_details`](#available_details)                 | details which can be used to specify additional information for `identify`          | dict               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | [`available_disease_details`](#available_disease_details) | details which can be used to specify additional information for `health_assessment` | dict               | :white_check_mark: | :x:                | :x:                | :x:                |
+| [`search`](#search)                                       | search for entity by query param in our database                                    | `SearchRecord`     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :x:                |
+| [`get_kb_detail`](#get_kb_detail)                         | returns information about entity                                                    | `dict`             | :white_check_mark: | :white_check_mark: | :white_check_mark: | :x:                |
 
 Datetime objects are created by method `datetime.fromtimestamp(timestamp)`. This means that datetime objects are in
 local timezone.
 
 ### Documentation
 
 #### available_details
@@ -171,28 +173,29 @@
     classification_level=classification_level,
     classification_raw=classification_raw,
     extra_get_params=extra_get_params,
     extra_post_params=extra_post_params,
 )
 
 # identification created from stream
-with open('path/to/image.jpg', 'rb') as image :
+with open('path/to/image.jpg', 'rb') as image:
     identification_from_stream: PlantIdentification = api.identify(image.read())
 
 # identification created from file object
-with open('path/to/image.jpg', 'rb') as image :
+with open('path/to/image.jpg', 'rb') as image:
     identification_from_file: PlantIdentification = api.identify(image)
 
 # identification created from base64 encoded image
-with open('path/to/image.jpg', 'rb') as image :
+with open('path/to/image.jpg', 'rb') as image:
     image_in_base64 = base64.b64encode(image.read())
     identification_from_base64: PlantIdentification = api.identify(image)
 
 # identification created from PIL.Image.Image object
 from PIL import Image
+
 image = Image.open('path/to/image.jpg')
 identification_from_pil: PlantIdentification = api.identify(image)
 
 # identification created from image url
 image_url = 'https://api.gbif.org/v1/image/cache/fit-in/500x/occurrence/4596837568/media/33ff3ad210e56b73ade6f9fe622c650e'
 identification_from_url: PlantIdentification = api.identify(image_url)
 ```
@@ -385,7 +388,37 @@
 from kindwise import PlantApi
 
 api = PlantApi(api_key='your_api_key')
 
 custom_id = 123  # also works with access_token or HealthAssessment object
 api.delete_health_assessment(custom_id)
 ```
+
+#### search
+
+Search for entity(e.g. `Taraxacum`) by query param in our database. You can specify language, limit and database type.
+
+```python
+from kindwise import PlantApi, SearchResult, PlantKBType
+
+api = PlantApi(api_key='your_api_key')
+kb_type = PlantKBType.PLANTS
+limit = 10
+search_result: SearchResult = api.search('Taraxacum', language='en', kb_type=kb_type, limit=limit)
+```
+
+#### get_kb_detail
+
+Returns information about entity(e.g. `Taraxacum`) in our database. You can specify in what language you want the
+result.
+
+```python
+from kindwise import PlantApi, SearchResult
+
+api = PlantApi(api_key='your_api_key')
+search_result: SearchResult = api.search('Taraxacum', language='en', limit=1)
+
+# details can also be specified as a list of strings
+details = 'common_names,taxonomy'
+
+entity_details = api.get_kb_detail(search_result.entities[0].access_token, details, language='de')
+```
```

### Comparing `kindwise_api_client-0.4.1/kindwise/core.py` & `kindwise_api_client-0.5.0/kindwise/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,35 +5,42 @@
 from datetime import datetime
 from pathlib import Path, PurePath
 from typing import BinaryIO, Any, Generic, TypeVar
 
 import requests
 from PIL import Image
 
-from kindwise.models import Identification, UsageInfo
+from kindwise.models import Identification, UsageInfo, SearchResult
 
 IdentificationType = TypeVar('IdentificationType')
+KBType = TypeVar('KBType')
 
 
-class KindwiseApi(abc.ABC, Generic[IdentificationType]):
+class KindwiseApi(abc.ABC, Generic[IdentificationType, KBType]):
     identification_class = Identification
+    default_kb_type = None
 
     def __init__(self, api_key: str):
         self.api_key = api_key
 
     @property
     @abc.abstractmethod
     def identification_url(self):
         ...
 
     @property
     @abc.abstractmethod
     def usage_info_url(self):
         ...
 
+    @property
+    @abc.abstractmethod
+    def kb_api_url(self):
+        ...
+
     def feedback_url(self, token: str):
         return f'{self.identification_url}/{token}/feedback'
 
     def _make_api_call(self, url, method: str, data: dict | None = None):
         headers = {
             'Content-Type': 'application/json',
             'Api-Key': self.api_key,
@@ -177,14 +184,16 @@
 
     def _build_query(
         self,
         details: str | list[str] = None,
         language: str | list[str] = None,
         asynchronous: bool = False,
         extra_get_params: str | dict[str, str] = None,
+        limit: int = None,
+        query: str = None,
         **kwargs,
     ):
         if isinstance(details, str):
             details = [details]
         details_query = '' if details is None else f'details={",".join(details)}&'
         if isinstance(language, str):
             language = [language]
@@ -193,15 +202,17 @@
             extra_get_params = ''
         else:
             if isinstance(extra_get_params, dict):
                 extra_get_params = '&'.join(f'{k}={v}' for k, v in extra_get_params.items())
             if extra_get_params.startswith('?'):
                 extra_get_params = extra_get_params[1:] + '&'
         async_query = f'async=true&' if asynchronous else ''
-        query = f'?{details_query}{language_query}{async_query}{extra_get_params}'
+        query = '' if query is None else f'q={query}&'
+        limit = '' if limit is None else f'limit={limit}&'
+        query = f'?{query}{limit}{details_query}{language_query}{async_query}{extra_get_params}'
         if query.endswith('&'):
             query = query[:-1]
         return '' if query == '?' else query
 
     def get_identification(
         self,
         token: str | int,
@@ -245,7 +256,38 @@
     @abc.abstractmethod
     def views_path(self) -> Path:
         ...
 
     def available_details(self) -> list[dict[str, any]]:
         with open(self.views_path) as f:
             return json.load(f)
+
+    def search(
+        self,
+        query: str,
+        limit: int = None,
+        language: str = None,
+        kb_type: KBType | str = None,
+        as_dict=False,
+    ) -> SearchResult | dict:
+        if not query:
+            raise ValueError('Query parameter q must be provided')
+        if isinstance(limit, int) and limit < 1:
+            raise ValueError(f'Limit must be positive integer.')
+        if kb_type is None:
+            kb_type = self.default_kb_type
+        url = f'{self.kb_api_url}/{kb_type}/name_search{self._build_query(query=query, limit=limit, language=language)}'
+        response = self._make_api_call(url, 'GET')
+        if not response.ok:
+            raise ValueError(f'Error while searching knowledge base: {response.status_code=} {response.text=}')
+        return response.json() if as_dict else SearchResult.from_dict(response.json())
+
+    def get_kb_detail(
+        self, access_token: str, details: str | list[str], language: str = None, kb_type: KBType | str = None
+    ) -> dict:
+        if kb_type is None:
+            kb_type = self.default_kb_type
+        url = f'{self.kb_api_url}/{kb_type}/{access_token}{self._build_query(language=language, details=details)}'
+        response = self._make_api_call(url, 'GET')
+        if not response.ok:
+            raise ValueError(f'Error while getting knowledge base detail: {response.status_code=} {response.text=}')
+        return response.json()
```

### Comparing `kindwise_api_client-0.4.1/kindwise/crop_health.py` & `kindwise_api_client-0.5.0/kindwise/crop_health.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import enum
 from dataclasses import dataclass
 from pathlib import Path
 
 from kindwise import settings
 from kindwise.core import KindwiseApi
 from kindwise.models import Identification, ResultEvaluation, ClassificationWithScientificName
 
@@ -26,16 +27,21 @@
     result: CropResult | None
 
     @classmethod
     def get_result_class(cls):
         return CropResult
 
 
-class CropHealthApi(KindwiseApi[CropIdentification]):
+class CropHealthKBType(str, enum.Enum):
+    CROP = 'crop'
+
+
+class CropHealthApi(KindwiseApi[CropIdentification, CropHealthKBType]):
     host = 'https://crop.kindwise.com'
+    default_kb_type = CropHealthKBType.CROP
     identification_class = CropIdentification
 
     def __init__(self, api_key: str = None):
         api_key = settings.CROP_HEALTH_API_KEY if api_key is None else api_key
         if api_key is None:
             raise ValueError(
                 'API key is required, set it in init method of class or in .env file under "CROP_HEALTH_API_KEY" key'
@@ -49,7 +55,11 @@
     @property
     def usage_info_url(self):
         return f'{self.host}/api/v1/usage_info'
 
     @property
     def views_path(self) -> Path:
         return settings.APP_DIR / 'resources' / f'views.crop_health.disease.json'
+
+    @property
+    def kb_api_url(self):
+        raise NotImplementedError('Crop health API does not support knowledge base API')
```

### Comparing `kindwise_api_client-0.4.1/kindwise/insect.py` & `kindwise_api_client-0.5.0/kindwise/insect.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+import enum
 from pathlib import Path
 
 from kindwise import settings
 from kindwise.core import KindwiseApi
 from kindwise.models import Identification
 
 
-class InsectApi(KindwiseApi[Identification]):
+class InsectKBType(str, enum.Enum):
+    INSECT = 'insect'
+
+
+class InsectApi(KindwiseApi[Identification, InsectKBType]):
     host = 'https://insect.kindwise.com'
+    default_kb_type = InsectKBType.INSECT
 
     def __init__(self, api_key: str = None):
         api_key = settings.INSECT_API_KEY if api_key is None else api_key
         if api_key is None:
             raise ValueError(
                 'API key is required, set it in init method of class or in .env file under "INSECT_API_KEY" key'
             )
@@ -21,9 +27,13 @@
         return f'{self.host}/api/v1/identification'
 
     @property
     def usage_info_url(self):
         return f'{self.host}/api/v1/usage_info'
 
     @property
+    def kb_api_url(self):
+        return f'{self.host}/api/v1/kb'
+
+    @property
     def views_path(self) -> Path:
         return settings.APP_DIR / 'resources' / f'views.insect.json'
```

### Comparing `kindwise_api_client-0.4.1/kindwise/models.py` & `kindwise_api_client-0.5.0/kindwise/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -232,7 +232,41 @@
         return cls(
             active=data['active'],
             credit_limits=Limits.from_dict(data['credit_limits']),
             used=Limits.from_dict(data['used']),
             can_use_credits=CanUseCredits.from_dict(data['can_use_credits']),
             remaining=Limits.from_dict(data['remaining']),
         )
+
+
+@dataclass
+class SearchEntity:
+    matched_in: str
+    matched_in_type: str
+    access_token: str
+    match_position: int
+    match_length: int
+
+    @classmethod
+    def from_dict(cls, data: dict):
+        return cls(
+            matched_in=data['matched_in'],
+            matched_in_type=data['matched_in_type'],
+            access_token=data['access_token'],
+            match_position=data['match_position'],
+            match_length=data['match_length'],
+        )
+
+
+@dataclass
+class SearchResult:
+    entities: list[SearchEntity]
+    entities_trimmed: bool
+    limit: int
+
+    @classmethod
+    def from_dict(cls, data: dict):
+        return cls(
+            entities=[SearchEntity.from_dict(entity) for entity in data['entities']],
+            entities_trimmed=data['entities_trimmed'],
+            limit=data['limit'],
+        )
```

### Comparing `kindwise_api_client-0.4.1/kindwise/mushroom.py` & `kindwise_api_client-0.5.0/kindwise/mushroom.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+import enum
 from pathlib import Path
 
 from kindwise import settings
 from kindwise.core import KindwiseApi
 from kindwise.models import Identification
 
 
-class MushroomApi(KindwiseApi[Identification]):
+class MushroomKBType(str, enum.Enum):
+    MUSHROOM = 'mushroom'
+
+
+class MushroomApi(KindwiseApi[Identification, MushroomKBType]):
     host = 'https://mushroom.kindwise.com'
+    default_kb_type = MushroomKBType.MUSHROOM
 
     def __init__(self, api_key: str = None):
         api_key = settings.MUSHROOM_API_KEY if api_key is None else api_key
         if api_key is None:
             raise ValueError(
                 'API key is required, set it in init method of class or in .env file under "MUSHROOM_API_KEY" key'
             )
@@ -23,7 +29,11 @@
     @property
     def usage_info_url(self):
         return f'{self.host}/api/v1/usage_info'
 
     @property
     def views_path(self) -> Path:
         return settings.APP_DIR / 'resources' / f'views.mushroom.json'
+
+    @property
+    def kb_api_url(self):
+        return f'{self.host}/api/v1/kb'
```

### Comparing `kindwise_api_client-0.4.1/kindwise/plant.py` & `kindwise_api_client-0.5.0/kindwise/plant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import enum
 import json
 from dataclasses import dataclass
 from datetime import datetime
 from pathlib import Path, PurePath
 from typing import BinaryIO
 
 from PIL import Image
@@ -16,14 +17,19 @@
     Feedback,
     ResultEvaluation,
     Classification,
     Suggestion,
 )
 
 
+class PlantKBType(str, enum.Enum):
+    PLANTS = 'plants'
+    DISEASES = 'diseases'
+
+
 @dataclass
 class PlantResult:
     is_plant: ResultEvaluation
     is_healthy: ResultEvaluation | None
     classification: Classification
     disease: Classification | None
 
@@ -177,16 +183,17 @@
             sla_compliant_system=data['sla_compliant_system'],
             created=datetime.fromtimestamp(data['created']),
             completed=None if data['completed'] is None else datetime.fromtimestamp(data['completed']),
             feedback=Feedback.from_dict(data['feedback']) if 'feedback' in data else None,
         )
 
 
-class PlantApi(KindwiseApi[PlantIdentification]):
+class PlantApi(KindwiseApi[PlantIdentification, PlantKBType]):
     host = 'https://plant.id'
+    default_kb_type = PlantKBType.PLANTS
 
     def __init__(self, api_key: str = None):
         api_key = settings.PLANT_API_KEY if api_key is None else api_key
         if api_key is None:
             raise ValueError(
                 'API key is required, set it in init method of class or in .env file under "PLANT_API_KEY" key'
             )
@@ -197,14 +204,18 @@
         return f'{self.host}/api/v3/identification'
 
     @property
     def usage_info_url(self):
         return f'{self.host}/api/v3/usage_info'
 
     @property
+    def kb_api_url(self):
+        return f'{self.host}/api/v3/kb'
+
+    @property
     def health_assessment_url(self):
         return f'{self.host}/api/v3/health_assessment'
 
     def _build_payload(
         self,
         *args,
         health: str = None,
```

### Comparing `kindwise_api_client-0.4.1/kindwise/resources/views.crop_health.disease.json` & `kindwise_api_client-0.5.0/kindwise/resources/views.crop_health.disease.json`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/kindwise/resources/views.insect.json` & `kindwise_api_client-0.5.0/kindwise/resources/views.insect.json`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/kindwise/resources/views.mushroom.json` & `kindwise_api_client-0.5.0/kindwise/resources/views.mushroom.json`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/kindwise/resources/views.plant.disease.json` & `kindwise_api_client-0.5.0/kindwise/resources/views.plant.disease.json`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/kindwise/resources/views.plant.json` & `kindwise_api_client-0.5.0/kindwise/resources/views.plant.json`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/conftest.py` & `kindwise_api_client-0.5.0/kindwise/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,59 +3,67 @@
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
 from unittest.mock import patch
 
 import pytest
 
-from kindwise.models import UsageInfo
+from kindwise import settings
+from kindwise.models import UsageInfo, SearchResult
 
 SYSTEMS = ['insect', 'mushroom', 'plant', 'crop']
 
 TEST_DIR = Path(__file__).resolve().parent
 IMAGE_DIR = TEST_DIR / 'resources' / 'images'
 MOCK_REQUESTS = True
 
-skip_integration_tests = pytest.mark.skipif(
-    bool(os.environ.get('SKIP_INTEGRATION_TESTS', False)), reason='Skipping because due to inability to contact staging'
-)
-
 
 @pytest.fixture
 def api_key():
     return 'b2a2f2c0-5e1a-4e4a-8b9a-5b6b0e2e2b9a'
 
 
 @contextmanager
-def staging_api(api, system):
+def environment_api(api, system):
     assert system.lower() in SYSTEMS
-    staging_host = os.getenv(f'{system.upper()}_STAGING_HOST')
-    assert staging_host is not None, f'{system.upper()}_STAGING_HOST is not set in .env file'
-    api_key = os.getenv(f'{system.upper()}_STAGING_API_KEY')
-    assert api_key is not None, f'{system.upper()}_STAGING_API_KEY is not set in .env file'
-    with patch.object(api, 'host', staging_host):
+    host = os.getenv(f'{system.upper()}_{settings.ENVIRONMENT}_HOST')
+    if settings.ENVIRONMENT == 'LOCAL' and host is None:
+        host = 'http://localhost:8000'
+    if settings.ENVIRONMENT == 'PRODUCTION' and host is None:
+        host = api.host
+    assert host is not None, f'{system.upper()}_{settings.ENVIRONMENT}_HOST is not set in .env file'
+    api_key = os.getenv(f'{system.upper()}_{settings.ENVIRONMENT}_API_KEY')
+    if settings.ENVIRONMENT == 'PRODUCTION' and api_key is None:
+        if system == 'crop':
+            api_key_name = 'CROP_HEALTH_API_KEY'
+        else:
+            api_key_name = f'{system.upper()}_API_KEY'
+        api_key = getattr(settings, api_key_name)
+        assert api_key is not None, f'{api_key_name} is not set in .env file'
+    assert api_key is not None, f'{system.upper()}_{settings.ENVIRONMENT}_API_KEY is not set in .env file'
+    with patch.object(api, 'host', host):
         with patch.object(api, 'api_key', api_key):
             yield api
 
 
 def run_test_requests_to_server(api, system_name, image_path, identification_type, model_name='classification'):
     assert system_name.lower() in SYSTEMS
-    with staging_api(api, system_name) as api:
+    with environment_api(api, system_name) as api:
         usage_info = api.usage_info()
         print('Usage info:')
         print(usage_info)
         print()
 
         custom_id = random.randint(1000000, 2000000)
         date_time = datetime.now()
         identification = api.identify(
-            image_path, latitude_longitude=(1.0, 2.0), asynchronous=True, custom_id=custom_id, date_time=date_time
+            image_path, latitude_longitude=(1.0, 2.0), custom_id=custom_id, date_time=date_time
         )
         assert isinstance(identification, identification_type)
-        print(f'Identification created with async, {date_time=} and {custom_id=}:')
+        print(f'Identification created with, {date_time=} and {custom_id=}:')
         print(identification)
         print()
         assert api.feedback(identification.access_token, comment='correct', rating=5)
 
         identification = api.get_identification(identification.access_token, details=['image'], language='cz')
         print('Identification with image details, custom id and cz language:')
         print(identification)
@@ -68,14 +76,31 @@
         assert identification.input.datetime == date_time
 
         assert api.delete_identification(identification.access_token)
 
         with pytest.raises(ValueError):
             api.get_identification(identification.access_token)
 
+        entity_name = getattr(identification.result, model_name).suggestions[0].name
+        try:
+            search_results: SearchResult = api.search(entity_name, limit=1)
+        except NotImplementedError:
+            print(f'Skipped KB api check ')
+        else:
+            print(f'Search results for {entity_name=}, limit=1 {system_name=}:')
+            print(search_results)
+            assert len(search_results.entities) == search_results.limit == 1
+            assert search_results.entities[0].matched_in.lower() == entity_name.lower()
+            kb_entity_detail = api.get_kb_detail(search_results.entities[0].access_token, 'image')
+            print(f'KB entity detail for {entity_name=}:')
+            print(kb_entity_detail)
+            assert kb_entity_detail['name'].lower() == entity_name.lower()
+            assert kb_entity_detail['language'] == 'en'
+            assert 'image' in kb_entity_detail
+
 
 class RequestMatcher:
     def __init__(self, api, api_key, image_path, requests_mock, identification_dict, identification):
         self.api = api
         self.api_key = api_key
         self.image_path = image_path
         self.requests_mock = requests_mock
```

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/resources/images/aloe-vera.jpg` & `kindwise_api_client-0.5.0/kindwise/tests/resources/images/aloe-vera.jpg`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/resources/images/amanita_muscaria.jpg` & `kindwise_api_client-0.5.0/kindwise/tests/resources/images/amanita_muscaria.jpg`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/resources/images/bee.jpeg` & `kindwise_api_client-0.5.0/kindwise/tests/resources/images/bee.jpeg`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/resources/images/padli.png` & `kindwise_api_client-0.5.0/kindwise/tests/resources/images/padli.png`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/resources/images/potato.late_blight.jpg` & `kindwise_api_client-0.5.0/kindwise/tests/resources/images/potato.late_blight.jpg`

 * *Files identical despite different names*

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/test_core.py` & `kindwise_api_client-0.5.0/kindwise/tests/test_core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import base64
+import enum
 import io
 from datetime import datetime
 from pathlib import PurePath, Path
 
 import pytest
 from PIL import Image
 
@@ -10,35 +11,48 @@
     Identification,
     Result,
     Input,
     Classification,
     Suggestion,
     SimilarImage,
     IdentificationStatus,
+    SearchResult,
+    SearchEntity,
 )
 from .conftest import IMAGE_DIR
 from .. import settings
 from ..core import KindwiseApi
 
 
-class TestApi(KindwiseApi):
+class TestKBType(str, enum.Enum):
+    TEST = 'test'
+    TEST_2 = 'test_2'
+    default = TEST
+
+
+class TestApi(KindwiseApi[Identification, TestKBType]):
     host = 'http://test.id'
+    default_kb_type = TestKBType.TEST
 
     @property
     def identification_url(self):
         return f'{self.host}/api/v1/identification'
 
     @property
     def usage_info_url(self):
         return f'{self.host}/api/v1/usage_info'
 
     @property
     def views_path(self) -> Path:
         return settings.APP_DIR / 'resources' / f'views.insect.json'
 
+    @property
+    def kb_api_url(self):
+        return f'{self.host}/api/v1/kb'
+
 
 @pytest.fixture
 def api(api_key):
     api_ = TestApi(api_key=api_key)
     return api_
 
 
@@ -399,7 +413,106 @@
     with pytest.raises(ValueError, match='Either comment or rating must be provided'):
         api.feedback(identification.access_token)
 
     response = api.feedback(identification, comment='correct')
     request_record = requests_mock.request_history.pop()
     assert request_record.method == 'POST'
     assert request_record.url == f'{api.identification_url}/{identification.access_token}/feedback'
+
+
+def test_search(api, api_key, requests_mock):
+    requests_mock.get(
+        f'{api.kb_api_url}/{TestKBType.TEST}/name_search',
+        json={
+            'entities': [
+                {
+                    'matched_in': 'Bee Beetle',
+                    'matched_in_type': 'common_name',
+                    'access_token': 'VW5rUkREcXFEVFM2SzM2dDYKXDBzJ0lIJzVjUy8LDk0-',
+                    'match_position': 0,
+                    'match_length': 3,
+                },
+            ],
+            'entities_trimmed': False,
+            'limit': 20,
+        },
+    )
+    response = api.search('bee')
+    request_record = requests_mock.request_history.pop()
+    assert request_record.method == 'GET'
+    assert request_record.url == f'{api.kb_api_url}/{TestKBType.TEST}/name_search?q=bee'
+    assert request_record.headers['Content-Type'] == 'application/json'
+    assert request_record.headers['Api-Key'] == api_key
+    assert response == SearchResult(
+        entities=[
+            SearchEntity('Bee Beetle', 'common_name', 'VW5rUkREcXFEVFM2SzM2dDYKXDBzJ0lIJzVjUy8LDk0-', 0, 3),
+        ],
+        entities_trimmed=False,
+        limit=20,
+    )
+    api.search('vcela', language='cz', limit=1)
+    request_record = requests_mock.request_history.pop()
+    assert request_record.url == f'{api.kb_api_url}/{TestKBType.TEST}/name_search?q=vcela&limit=1&language=cz'
+    # check bundle
+    api = TestApi(api_key=api_key)
+    plant_api_res = {
+        'entities': [
+            {
+                'matched_in': 'Aloe',
+                'matched_in_type': 'entity_name',
+                'access_token': 'bG1NbjFDTkoxOHNTTHlIYwpcKF8CIS9yCAoXY3ofelA-',
+                'match_position': 0,
+                'match_length': 4,
+            }
+        ],
+        'entities_trimmed': True,
+        'limit': 20,
+    }
+    requests_mock.get(f'{api.kb_api_url}/{TestKBType.TEST}/name_search', json=plant_api_res)
+    api.search('aloe')
+    request_record = requests_mock.request_history.pop()
+    assert request_record.url == f'{api.kb_api_url}/{TestKBType.TEST}/name_search?q=aloe'
+    requests_mock.get(f'{api.kb_api_url}/{TestKBType.TEST_2}/name_search', json=plant_api_res)
+    api.search('downy', kb_type=TestKBType.TEST_2)
+    request_record = requests_mock.request_history.pop()
+    assert request_record.url == f'{api.kb_api_url}/{TestKBType.TEST_2}/name_search?q=downy'
+    with pytest.raises(ValueError):
+        api.search('downy', limit=0)
+
+
+def test_get_kb_detail(api, api_key, requests_mock):
+    access_token = 's34d5rft6gyu'
+    requests_mock.get(
+        f'{api.kb_api_url}/{TestKBType.TEST}/{access_token}',
+        json={'gbif_id': 1085281, 'rank': 'species', 'language': 'en', 'name': 'Trichius gallicus'},
+    )
+    response = api.get_kb_detail(access_token, 'rank,gbif_id')
+    request_record = requests_mock.request_history.pop()
+    assert request_record.method == 'GET'
+    assert request_record.url == f'{api.kb_api_url}/{TestKBType.TEST}/{access_token}?details=rank,gbif_id'
+    assert request_record.headers['Content-Type'] == 'application/json'
+    assert request_record.headers['Api-Key'] == api_key
+    assert response == {'gbif_id': 1085281, 'rank': 'species', 'language': 'en', 'name': 'Trichius gallicus'}
+
+    api.get_kb_detail(access_token, ['rank', 'gbif_id'], language='cs')
+    request_record = requests_mock.request_history.pop()
+    assert request_record.url == f'{api.kb_api_url}/{TestKBType.TEST}/{access_token}?details=rank,gbif_id&language=cs'
+
+    # check bundle
+    api = TestApi(api_key=api_key)
+    requests_mock.get(
+        f'{api.kb_api_url}/{TestKBType.TEST}/{access_token}',
+        json={'gbif_id': 2777724, 'rank': 'species', 'language': 'en', 'name': 'Aloe vera'},
+    )
+    response = api.get_kb_detail(access_token, 'rank,gbif_id')
+    request_record = requests_mock.request_history.pop()
+    assert request_record.url == f'{api.kb_api_url}/{TestKBType.TEST}/{access_token}?details=rank,gbif_id'
+    assert response == {'gbif_id': 2777724, 'rank': 'species', 'language': 'en', 'name': 'Aloe vera'}
+
+    requests_mock.get(
+        f'{api.kb_api_url}/{TestKBType.TEST_2}/{access_token}',
+        json={'url': 'https://en.wikipedia.org/wiki/Downy_mildew', 'language': 'en', 'name': 'downy mildew'},
+    )
+    response = api.get_kb_detail(access_token, 'url', kb_type=TestKBType.TEST_2)
+    request_record = requests_mock.request_history.pop()
+    assert request_record.url == f'{api.kb_api_url}/{TestKBType.TEST_2}/{access_token}?details=url'
+    assert response == {'url': 'https://en.wikipedia.org/wiki/Downy_mildew', 'language': 'en', 'name': 'downy mildew'}
```

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/test_crop.py` & `kindwise_api_client-0.5.0/kindwise/tests/test_crop.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details, skip_integration_tests
+from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details
 from .. import CropHealthApi
 from ..crop_health import CropIdentification
 
 
-@skip_integration_tests
 def test_requests_to_crop_server(api_key):
     run_test_requests_to_server(
         CropHealthApi(api_key=api_key),
         'crop',
         IMAGE_DIR / 'potato.late_blight.jpg',
         CropIdentification,
         model_name='disease',
```

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/test_insect.py` & `kindwise_api_client-0.5.0/kindwise/tests/test_insect.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from kindwise.models import Identification
-from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details, skip_integration_tests
+from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details
 from ..insect import InsectApi
 
 
-@skip_integration_tests
 def test_requests_to_insect_server(api_key):
     run_test_requests_to_server(InsectApi(api_key=api_key), 'insect', IMAGE_DIR / 'bee.jpeg', Identification)
 
 
 def test_available_details(api_key):
     expected_view_names = {
         'common_names',
```

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/test_mushroom.py` & `kindwise_api_client-0.5.0/kindwise/tests/test_mushroom.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from kindwise.models import Identification
-from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details, skip_integration_tests
+from .conftest import run_test_requests_to_server, IMAGE_DIR, run_test_available_details
 from ..mushroom import MushroomApi
 
 
-@skip_integration_tests
 def test_requests_to_mushroom_server(api_key):
     run_test_requests_to_server(
         MushroomApi(api_key=api_key), 'mushroom', IMAGE_DIR / 'amanita_muscaria.jpg', Identification
     )
 
 
 def test_available_details(api_key):
```

### Comparing `kindwise_api_client-0.4.1/kindwise/tests/test_plant.py` & `kindwise_api_client-0.5.0/kindwise/tests/test_plant.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,17 +23,16 @@
     RawClassification,
     TaxaSpecificSuggestion,
     PlantInput,
 )
 from .conftest import (
     IMAGE_DIR,
     run_test_requests_to_server,
-    staging_api,
+    environment_api,
     run_test_available_details,
-    skip_integration_tests,
 )
 from ..plant import PlantApi
 
 
 @pytest.fixture
 def api(api_key):
     api_ = PlantApi(api_key=api_key)
@@ -838,25 +837,23 @@
     identification.custom_id = 123
     requests_mock.delete(f'{api.identification_url}/{identification.custom_id}', json=True)
     response = api.delete_identification(identification.custom_id)
     request_record = requests_mock.request_history.pop()
     assert request_record.url == f'{api.identification_url}/{identification.custom_id}'
 
 
-@skip_integration_tests
 def test_requests_to_plant_server(api: PlantApi, image_path):
     system_name = 'plant'
     run_test_requests_to_server(api, system_name, image_path, PlantIdentification)
-    with staging_api(api, system_name) as api:
+    with environment_api(api, system_name) as api:
         custom_id = random.randint(1000000, 2000000)
         date_time = datetime.now()
-        print(f'Health assessment asynchronous with {custom_id=} and {date_time=}:')
+        print(f'Health assessment with {custom_id=} and {date_time=}:')
         health_assessment = api.health_assessment(
             image_path,
-            asynchronous=True,
             custom_id=custom_id,
             date_time=date_time,
             latitude_longitude=(49.20340, 16.57318),
             full_disease_list=True,
         )
         print(health_assessment)
         assert health_assessment.input.datetime == date_time
```

### Comparing `kindwise_api_client-0.4.1/pyproject.toml` & `kindwise_api_client-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kindwise-api-client"
-version = "0.4.1"
+version = "0.5.0"
 description = "Python SDK toolkit for integrating Kindwise API"
 authors = ["Simon Plhak <simon.plhak@flowerchecker.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/flowerchecker/kindwise"
 packages = [
     { include = "kindwise"},
```

### Comparing `kindwise_api_client-0.4.1/setup.py` & `kindwise_api_client-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
  'kindwise.tests': ['resources/images/*']}
 
 install_requires = \
 ['pillow', 'python-dotenv', 'requests']
 
 setup_kwargs = {
     'name': 'kindwise-api-client',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': 'Python SDK toolkit for integrating Kindwise API',
-    'long_description': '# Kindwise sdk for python\n\nPython SDK toolkit for integrating Kindwise API into your application. This Python SDK provides a convenient way to\ninteract with the Kindwise API for plant, insect, and mushroom identification. The SDK is organized into different\nmodules, each corresponding to a specific domain ([plant](https://web.plant.id/plant-identification-api/),\n[insect](https://www.kindwise.com/insect-id), [mushroom](https://www.kindwise.com/mushroom-id)). You can always use our\nAPI without our SDK, the documentation can be found on the following links:\n\n- [plant.id](https://plant.id/docs)\n- [insect.id](https://insect.kindwise.com/docs)\n- [mushroom.id](https://mushroom.kindwise.com/docs)\n- [crop.health](https://crop.kindwise.com/docs)\n\n## Setup\n\n### Install\n\n```bash\npip install kindwise\n```\n\n### API key\n\nThe API key serves to identify your account and is required to make requests to the API. Get API key at\n[admin.kindwise.com](https://admin.kindwise.com).\n\n## Quick Start\n\nTo use Kindwise API, an active API key is needed. See the section [above](#api-key) on how to get an API key.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification, UsageInfo\n\n# initialize plant.id api\n# "PLANT_API_KEY" environment variable can be set instead of specifying api_key\napi = PlantApi(api_key=\'your_api_key\')\n\n# get usage information\nusage: UsageInfo = api.usage_info()\n\n# identify plant by image\nlatitude_longitude = (49.20340, 16.57318)\n# pass the image as a path\nimage_path = \'path/to/plant_image.jpg\'\n# make identification\nidentification: PlantIdentification = api.identify(image_path, latitude_longitude=latitude_longitude)\n\n# get identification by a token with changed views\n# this method can be used to modify additional information in identification or to get identification from database\n# also works with identification.custom_id\nidentification_with_different_views: PlantIdentification = api.get_identification(identification.access_token)\n\n# delete identification\napi.delete_identification(identification)  # also works with identification.access_token or identification.custom_id\n```\n\n## Structure\n\nSDK supports the following Kindwise systems:\n\n- [plant.id](https://web.plant.id/plant-identification-api/)\n- [insect.id](https://insect.kindwise.com)\n- [mushroom.id](https://mushroom.kindwise.com)\n- [crop.health](https://crop.kindwise.com)\n\nEach system has its class, which is used to make requests to the API. Each class has the following methods:\n\n| method                                                    | description                                                                         | return type        | plant.id           | insect.id          | mushroom.id        | crop.health        |\n|-----------------------------------------------------------|-------------------------------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|--------------------|\n| [`identify`](#identify)                                   | create new identification                                                           | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`get_identification`](#get_identification)               | get identification by token                                                         | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`delete_identification`](#delete_identification)         | delete identification by token                                                      | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`usage_info`](#usage_info)                               | get api key usage information                                                       | `UsageInfo`        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`feedback`](#feedback)                                   | send feedback for identification                                                    | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`health_assessment`](#health_assessment)                 | create health assessment identification                                             | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |\n| [`get_health_assessment`](#get_health_assessment)         | get health assessment identification                                                | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |\n| [`delete_health_assessment`](#delete_health_assessment)   | delete health assessment                                                            | boolean            | :white_check_mark: | :x:                | :x:                | :x:                |\n| [`available_details`](#available_details)                 | details which can be used to specify additional information for `identify`          | dict               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`available_disease_details`](#available_disease_details) | details which can be used to specify additional information for `health_assessment` | dict               | :white_check_mark: | :x:                | :x:                | :x:                |\n\nDatetime objects are created by method `datetime.fromtimestamp(timestamp)`. This means that datetime objects are in\nlocal timezone.\n\n### Documentation\n\n#### available_details\n\nReturns details which can be used to specify additional information for `identify` method. `\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi()\n\navailable_details = api.available_details()\n```\n\n#### identify\n\nCreates a new identification. In one identification, you can include up to 5 images.\n\n```python\nimport base64\nfrom datetime import datetime\n\nfrom kindwise import PlantApi, PlantIdentification, ClassificationLevel\n\napi = PlantApi(api_key=\'your_api_key\')\n# this creates one identification composed of 5 images(not 5 different identifications)\n#\n# as input image is accepted path to an image(str / pathlib.Path), base64 encoded stream(bytes/string), stream(bytes/string),\n# or file object(supports read,seek and mode methods)\n# or PIL.Image.Image object\n# or list of images\nimages = [\'path/to/image1.jpg\', \'path/to/image2.jpg\', \'path/to/image3.jpg\', \'path/to/image4.jpg\', \'path/to/image5.jpg\']\n\n# details included in identification\ndetails = [\'common_names\', \'taxonomy\', \'image\']\n\n# disease details included in health identification(only used if health=True)\n# disease_details parameter is only available for plant.id\ndisease_details = [\'local_name\', \'description\', \'treatment\', \'cause\']\n\n# specify up to 3 languages\nlanguage = [\'en\', \'cs\']\n\n# default for similar_images is True\nsimilar_images = True\n\n# where was an image taken\nlatitude_longitude = (49.20340, 16.57318)\n\n# include health assessment in your identification by specifying health=\'all\',\n# also use health=\'only\' to get HealthAssessment(health assessment only)\n# health assessment is only available for plant.id\nhealth = \'all\'\n\n# custom id is used to identify identification in your system, but can be replaced with access_token\ncustom_id = 123\n\n# when was an image taken, datetime can be specified as a datetime object, timestamp, or string in ISO format\ndate_time = datetime.now()\n\n# default image size is 1500px, can be turned off by setting max_image_size to None\n# be aware that our API has limit 25Mpx(e.g. 5000px x 5000px)\nmax_image_size = 1500\n\n# specify into what depth should be the plant classified\n# choose from ClassificationLevel.SPECIES, ClassificationLevel.GENUS, ClassificationLevel.ALL\n# default is ClassificationLevel.SPECIES\nclassification_level = ClassificationLevel.SPECIES\n# in case of need to merge results for different taxon levels yourself, set classification_raw=True\n# be aware that the result will be in type kindwise.models.RawPlantIdentification\nclassification_raw = False\n# if our api will be ahead of this sdk and you do not want to wait for update,\n# specify extra_get_params or extra_post_params\nextra_get_params = None  # default\nextra_post_params = None  # default\n\nidentification: PlantIdentification = api.identify(\n    images,\n    details=details,\n    disease_details=disease_details,\n    language=language,\n    similar_images=similar_images,\n    latitude_longitude=latitude_longitude,\n    health=health,\n    custom_id=custom_id,\n    date_time=date_time,\n    max_image_size=max_image_size,\n    classification_level=classification_level,\n    classification_raw=classification_raw,\n    extra_get_params=extra_get_params,\n    extra_post_params=extra_post_params,\n)\n\n# identification created from stream\nwith open(\'path/to/image.jpg\', \'rb\') as image :\n    identification_from_stream: PlantIdentification = api.identify(image.read())\n\n# identification created from file object\nwith open(\'path/to/image.jpg\', \'rb\') as image :\n    identification_from_file: PlantIdentification = api.identify(image)\n\n# identification created from base64 encoded image\nwith open(\'path/to/image.jpg\', \'rb\') as image :\n    image_in_base64 = base64.b64encode(image.read())\n    identification_from_base64: PlantIdentification = api.identify(image)\n\n# identification created from PIL.Image.Image object\nfrom PIL import Image\nimage = Image.open(\'path/to/image.jpg\')\nidentification_from_pil: PlantIdentification = api.identify(image)\n\n# identification created from image url\nimage_url = \'https://api.gbif.org/v1/image/cache/fit-in/500x/occurrence/4596837568/media/33ff3ad210e56b73ade6f9fe622c650e\'\nidentification_from_url: PlantIdentification = api.identify(image_url)\n```\n\nWhen you don\'t want to wait until the identification is finished, you can specify `asynchronous=True` and\nget `access_token`  or `custom_id` if specified and retrieve the answer later.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification\n\napi = PlantApi(api_key=\'your_api_key\')\n\nimage = \'path/to/image.jpg\'\nidentification: PlantIdentification = api.identify(image, asynchronous=True)\n# now do something else\n# ...\n# and later get identification by access_token or custom_id\nidentification: PlantIdentification = api.get_identification(identification.access_token, details=[\'common_names\'])\n```\n\n#### get_identification\n\nGet identification by token. You can specify which details you want to get. We store your identifications for 6 months.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification\n\napi = PlantApi(api_key=\'your_api_key\')\n\naccess_token = \'identification_access_token\'\n# details included in identification, can be different from used in identification create\ndetails = [\'common_names\', \'taxonomy\', \'image\']\n# language can also differ from used in identification create\nlanguage = \'de\'\nidentification: PlantIdentification = api.get_identification(access_token, details=details, language=language)\n```\n\n#### delete_identification\n\nDeletes identification from our database. You can specify identification by access_token or custom_id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or Identification object\napi.delete_identification(custom_id)\n```\n\n#### usage_info\n\nGives you information about your api key usage.\n\n```python\nfrom kindwise import PlantApi, UsageInfo\n\napi = PlantApi(api_key=\'your_api_key\')\n\nusage_info: UsageInfo = api.usage_info()\n```\n\n#### feedback\n\nSend feedback for identification. You can specify a comment(string) or rating(int) in feedback. At least one of comment\nand rating must be specified. You can specify identification by access_token or custom_id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or Identification object\napi.feedback(custom_id, comment=\'comment\', rating=5)\n```\n\n#### available_disease_details\n\nReturns details which can be used to specify additional information for `health_assessment` method. Only available for\nplant.id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi()\n\navailable_disease_details = api.available_disease_details()\n```\n\n#### health_assessment\n\nReturns only health assessment for identification. Health assessment is only available for plant.id. `health_assessment`\nmethod is similar to `identify` method, but it returns only health assessment. Details differs for each system.\n\n```python\nfrom datetime import datetime\n\nfrom kindwise import PlantApi, HealthAssessment\n\napi = PlantApi(api_key="your_api_key")\n# the same as in identify method\nimages = [\n    "path/to/image1.jpg",\n    "path/to/image2.jpg",\n    "path/to/image3.jpg",\n    "path/to/image4.jpg",\n    "path/to/image5.jpg",\n]\n\n# details included in identification\ndetails = ["local_name", "description", "treatment", "cause", "image"]\n\n# specify up to 3 languages\nlanguage = ["en", "cs"]\n\n# default for similar_images is True\nsimilar_images = True\n\n# where was an image taken\nlatitude_longitude = (49.20340, 16.57318)\n\n# custom id is used to identify identification in your system, but can be replaced with access_token\ncustom_id = 123\n\n# list of suggested diseases also contains general diseases such as "Abiotic", default is False\nfull_disease_list = True\n\n# when was an image taken, datetime can be specified as a datetime object, timestamp, or string in ISO format\ndate_time = datetime.now()\n\n# default image size is 1500px, can be turned off by setting max_image_size to None\n# be aware that our API has limit 25Mpx(e.g. 5000px x 5000px)\nmax_image_size = 1500\n\n# if our api will be ahead of this sdk and you do not want to wait for update,\n# specify extra_get_params or extra_post_params\nextra_get_params = None  # default\nextra_post_params = None  # default\n\nidentification: HealthAssessment = api.health_assessment(\n    images,\n    details=details,\n    language=language,\n    similar_images=similar_images,\n    latitude_longitude=latitude_longitude,\n    custom_id=custom_id,\n    full_disease_list=full_disease_list,\n    date_time=date_time,\n    max_image_size=max_image_size,\n)\n\n```\n\nWhen you don\'t want to wait until the identification is finished, you can specify `asynchronous=True` similar\nto [`identify`](#identify) method.\n\n#### get_health_assessment\n\nGet a health assessment for identification. You can specify which details you want to get. We store your identifications\nfor 6 months.\n\n```python\nfrom kindwise import PlantApi, HealthAssessment\n\napi = PlantApi(api_key=\'your_api_key\')\n\naccess_token = \'identification_access_token\'\n\n# details included in identification can be different from those used in identification creation\ndetails = [\'classification\', \'local_name\']\n\n# language can also differ from what is used in identification creation\nlanguage = \'de\'\n\nfull_disease_list = False\n\nidentification: HealthAssessment = api.get_health_assessment(\n    access_token,\n    details=details,\n    language=language,\n    full_disease_list=full_disease_list\n)\n```\n\n#### delete_health_assessment\n\nDelete health assessment for identification.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or HealthAssessment object\napi.delete_health_assessment(custom_id)\n```\n',
+    'long_description': '# Kindwise sdk for python\n\nPython SDK toolkit for integrating Kindwise API into your application. This Python SDK provides a convenient way to\ninteract with the Kindwise API for plant, insect, and mushroom identification. The SDK is organized into different\nmodules, each corresponding to a specific domain ([plant](https://web.plant.id/plant-identification-api/),\n[insect](https://www.kindwise.com/insect-id), [mushroom](https://www.kindwise.com/mushroom-id)). You can always use our\nAPI without our SDK, the documentation can be found on the following links:\n\n- [plant.id](https://plant.id/docs)\n- [insect.id](https://insect.kindwise.com/docs)\n- [mushroom.id](https://mushroom.kindwise.com/docs)\n- [crop.health](https://crop.kindwise.com/docs)\n\n## Setup\n\n### Install\n\n```bash\npip install kindwise\n```\n\n### API key\n\nThe API key serves to identify your account and is required to make requests to the API. Get API key at\n[admin.kindwise.com](https://admin.kindwise.com).\n\n## Quick Start\n\nTo use Kindwise API, an active API key is needed. See the section [above](#api-key) on how to get an API key.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification, UsageInfo\n\n# initialize plant.id api\n# "PLANT_API_KEY" environment variable can be set instead of specifying api_key\napi = PlantApi(api_key=\'your_api_key\')\n\n# get usage information\nusage: UsageInfo = api.usage_info()\n\n# identify plant by image\nlatitude_longitude = (49.20340, 16.57318)\n# pass the image as a path\nimage_path = \'path/to/plant_image.jpg\'\n# make identification\nidentification: PlantIdentification = api.identify(image_path, latitude_longitude=latitude_longitude)\n\n# get identification by a token with changed views\n# this method can be used to modify additional information in identification or to get identification from database\n# also works with identification.custom_id\nidentification_with_different_views: PlantIdentification = api.get_identification(identification.access_token)\n\n# delete identification\napi.delete_identification(identification)  # also works with identification.access_token or identification.custom_id\n```\n\n## Structure\n\nSDK supports the following Kindwise systems:\n\n- [plant.id](https://web.plant.id/plant-identification-api/)\n- [insect.id](https://insect.kindwise.com)\n- [mushroom.id](https://mushroom.kindwise.com)\n- [crop.health](https://crop.kindwise.com)\n\nEach system has its class, which is used to make requests to the API. Each class has the following methods:\n\n| method                                                    | description                                                                         | return type        | plant.id           | insect.id          | mushroom.id        | crop.health        |\n|-----------------------------------------------------------|-------------------------------------------------------------------------------------|--------------------|--------------------|--------------------|--------------------|--------------------|\n| [`identify`](#identify)                                   | create new identification                                                           | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`get_identification`](#get_identification)               | get identification by token                                                         | `Identification`   | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`delete_identification`](#delete_identification)         | delete identification by token                                                      | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`usage_info`](#usage_info)                               | get api key usage information                                                       | `UsageInfo`        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`feedback`](#feedback)                                   | send feedback for identification                                                    | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`health_assessment`](#health_assessment)                 | create health assessment identification                                             | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |\n| [`get_health_assessment`](#get_health_assessment)         | get health assessment identification                                                | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |\n| [`delete_health_assessment`](#delete_health_assessment)   | delete health assessment                                                            | boolean            | :white_check_mark: | :x:                | :x:                | :x:                |\n| [`available_details`](#available_details)                 | details which can be used to specify additional information for `identify`          | dict               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |\n| [`available_disease_details`](#available_disease_details) | details which can be used to specify additional information for `health_assessment` | dict               | :white_check_mark: | :x:                | :x:                | :x:                |\n| [`search`](#search)                                       | search for entity by query param in our database                                    | `SearchRecord`     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :x:                |\n| [`get_kb_detail`](#get_kb_detail)                         | returns information about entity                                                    | `dict`             | :white_check_mark: | :white_check_mark: | :white_check_mark: | :x:                |\n\nDatetime objects are created by method `datetime.fromtimestamp(timestamp)`. This means that datetime objects are in\nlocal timezone.\n\n### Documentation\n\n#### available_details\n\nReturns details which can be used to specify additional information for `identify` method. `\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi()\n\navailable_details = api.available_details()\n```\n\n#### identify\n\nCreates a new identification. In one identification, you can include up to 5 images.\n\n```python\nimport base64\nfrom datetime import datetime\n\nfrom kindwise import PlantApi, PlantIdentification, ClassificationLevel\n\napi = PlantApi(api_key=\'your_api_key\')\n# this creates one identification composed of 5 images(not 5 different identifications)\n#\n# as input image is accepted path to an image(str / pathlib.Path), base64 encoded stream(bytes/string), stream(bytes/string),\n# or file object(supports read,seek and mode methods)\n# or PIL.Image.Image object\n# or list of images\nimages = [\'path/to/image1.jpg\', \'path/to/image2.jpg\', \'path/to/image3.jpg\', \'path/to/image4.jpg\', \'path/to/image5.jpg\']\n\n# details included in identification\ndetails = [\'common_names\', \'taxonomy\', \'image\']\n\n# disease details included in health identification(only used if health=True)\n# disease_details parameter is only available for plant.id\ndisease_details = [\'local_name\', \'description\', \'treatment\', \'cause\']\n\n# specify up to 3 languages\nlanguage = [\'en\', \'cs\']\n\n# default for similar_images is True\nsimilar_images = True\n\n# where was an image taken\nlatitude_longitude = (49.20340, 16.57318)\n\n# include health assessment in your identification by specifying health=\'all\',\n# also use health=\'only\' to get HealthAssessment(health assessment only)\n# health assessment is only available for plant.id\nhealth = \'all\'\n\n# custom id is used to identify identification in your system, but can be replaced with access_token\ncustom_id = 123\n\n# when was an image taken, datetime can be specified as a datetime object, timestamp, or string in ISO format\ndate_time = datetime.now()\n\n# default image size is 1500px, can be turned off by setting max_image_size to None\n# be aware that our API has limit 25Mpx(e.g. 5000px x 5000px)\nmax_image_size = 1500\n\n# specify into what depth should be the plant classified\n# choose from ClassificationLevel.SPECIES, ClassificationLevel.GENUS, ClassificationLevel.ALL\n# default is ClassificationLevel.SPECIES\nclassification_level = ClassificationLevel.SPECIES\n# in case of need to merge results for different taxon levels yourself, set classification_raw=True\n# be aware that the result will be in type kindwise.models.RawPlantIdentification\nclassification_raw = False\n# if our api will be ahead of this sdk and you do not want to wait for update,\n# specify extra_get_params or extra_post_params\nextra_get_params = None  # default\nextra_post_params = None  # default\n\nidentification: PlantIdentification = api.identify(\n    images,\n    details=details,\n    disease_details=disease_details,\n    language=language,\n    similar_images=similar_images,\n    latitude_longitude=latitude_longitude,\n    health=health,\n    custom_id=custom_id,\n    date_time=date_time,\n    max_image_size=max_image_size,\n    classification_level=classification_level,\n    classification_raw=classification_raw,\n    extra_get_params=extra_get_params,\n    extra_post_params=extra_post_params,\n)\n\n# identification created from stream\nwith open(\'path/to/image.jpg\', \'rb\') as image:\n    identification_from_stream: PlantIdentification = api.identify(image.read())\n\n# identification created from file object\nwith open(\'path/to/image.jpg\', \'rb\') as image:\n    identification_from_file: PlantIdentification = api.identify(image)\n\n# identification created from base64 encoded image\nwith open(\'path/to/image.jpg\', \'rb\') as image:\n    image_in_base64 = base64.b64encode(image.read())\n    identification_from_base64: PlantIdentification = api.identify(image)\n\n# identification created from PIL.Image.Image object\nfrom PIL import Image\n\nimage = Image.open(\'path/to/image.jpg\')\nidentification_from_pil: PlantIdentification = api.identify(image)\n\n# identification created from image url\nimage_url = \'https://api.gbif.org/v1/image/cache/fit-in/500x/occurrence/4596837568/media/33ff3ad210e56b73ade6f9fe622c650e\'\nidentification_from_url: PlantIdentification = api.identify(image_url)\n```\n\nWhen you don\'t want to wait until the identification is finished, you can specify `asynchronous=True` and\nget `access_token`  or `custom_id` if specified and retrieve the answer later.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification\n\napi = PlantApi(api_key=\'your_api_key\')\n\nimage = \'path/to/image.jpg\'\nidentification: PlantIdentification = api.identify(image, asynchronous=True)\n# now do something else\n# ...\n# and later get identification by access_token or custom_id\nidentification: PlantIdentification = api.get_identification(identification.access_token, details=[\'common_names\'])\n```\n\n#### get_identification\n\nGet identification by token. You can specify which details you want to get. We store your identifications for 6 months.\n\n```python\nfrom kindwise import PlantApi, PlantIdentification\n\napi = PlantApi(api_key=\'your_api_key\')\n\naccess_token = \'identification_access_token\'\n# details included in identification, can be different from used in identification create\ndetails = [\'common_names\', \'taxonomy\', \'image\']\n# language can also differ from used in identification create\nlanguage = \'de\'\nidentification: PlantIdentification = api.get_identification(access_token, details=details, language=language)\n```\n\n#### delete_identification\n\nDeletes identification from our database. You can specify identification by access_token or custom_id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or Identification object\napi.delete_identification(custom_id)\n```\n\n#### usage_info\n\nGives you information about your api key usage.\n\n```python\nfrom kindwise import PlantApi, UsageInfo\n\napi = PlantApi(api_key=\'your_api_key\')\n\nusage_info: UsageInfo = api.usage_info()\n```\n\n#### feedback\n\nSend feedback for identification. You can specify a comment(string) or rating(int) in feedback. At least one of comment\nand rating must be specified. You can specify identification by access_token or custom_id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or Identification object\napi.feedback(custom_id, comment=\'comment\', rating=5)\n```\n\n#### available_disease_details\n\nReturns details which can be used to specify additional information for `health_assessment` method. Only available for\nplant.id.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi()\n\navailable_disease_details = api.available_disease_details()\n```\n\n#### health_assessment\n\nReturns only health assessment for identification. Health assessment is only available for plant.id. `health_assessment`\nmethod is similar to `identify` method, but it returns only health assessment. Details differs for each system.\n\n```python\nfrom datetime import datetime\n\nfrom kindwise import PlantApi, HealthAssessment\n\napi = PlantApi(api_key="your_api_key")\n# the same as in identify method\nimages = [\n    "path/to/image1.jpg",\n    "path/to/image2.jpg",\n    "path/to/image3.jpg",\n    "path/to/image4.jpg",\n    "path/to/image5.jpg",\n]\n\n# details included in identification\ndetails = ["local_name", "description", "treatment", "cause", "image"]\n\n# specify up to 3 languages\nlanguage = ["en", "cs"]\n\n# default for similar_images is True\nsimilar_images = True\n\n# where was an image taken\nlatitude_longitude = (49.20340, 16.57318)\n\n# custom id is used to identify identification in your system, but can be replaced with access_token\ncustom_id = 123\n\n# list of suggested diseases also contains general diseases such as "Abiotic", default is False\nfull_disease_list = True\n\n# when was an image taken, datetime can be specified as a datetime object, timestamp, or string in ISO format\ndate_time = datetime.now()\n\n# default image size is 1500px, can be turned off by setting max_image_size to None\n# be aware that our API has limit 25Mpx(e.g. 5000px x 5000px)\nmax_image_size = 1500\n\n# if our api will be ahead of this sdk and you do not want to wait for update,\n# specify extra_get_params or extra_post_params\nextra_get_params = None  # default\nextra_post_params = None  # default\n\nidentification: HealthAssessment = api.health_assessment(\n    images,\n    details=details,\n    language=language,\n    similar_images=similar_images,\n    latitude_longitude=latitude_longitude,\n    custom_id=custom_id,\n    full_disease_list=full_disease_list,\n    date_time=date_time,\n    max_image_size=max_image_size,\n)\n\n```\n\nWhen you don\'t want to wait until the identification is finished, you can specify `asynchronous=True` similar\nto [`identify`](#identify) method.\n\n#### get_health_assessment\n\nGet a health assessment for identification. You can specify which details you want to get. We store your identifications\nfor 6 months.\n\n```python\nfrom kindwise import PlantApi, HealthAssessment\n\napi = PlantApi(api_key=\'your_api_key\')\n\naccess_token = \'identification_access_token\'\n\n# details included in identification can be different from those used in identification creation\ndetails = [\'classification\', \'local_name\']\n\n# language can also differ from what is used in identification creation\nlanguage = \'de\'\n\nfull_disease_list = False\n\nidentification: HealthAssessment = api.get_health_assessment(\n    access_token,\n    details=details,\n    language=language,\n    full_disease_list=full_disease_list\n)\n```\n\n#### delete_health_assessment\n\nDelete health assessment for identification.\n\n```python\nfrom kindwise import PlantApi\n\napi = PlantApi(api_key=\'your_api_key\')\n\ncustom_id = 123  # also works with access_token or HealthAssessment object\napi.delete_health_assessment(custom_id)\n```\n\n#### search\n\nSearch for entity(e.g. `Taraxacum`) by query param in our database. You can specify language, limit and database type.\n\n```python\nfrom kindwise import PlantApi, SearchResult, PlantKBType\n\napi = PlantApi(api_key=\'your_api_key\')\nkb_type = PlantKBType.PLANTS\nlimit = 10\nsearch_result: SearchResult = api.search(\'Taraxacum\', language=\'en\', kb_type=kb_type, limit=limit)\n```\n\n#### get_kb_detail\n\nReturns information about entity(e.g. `Taraxacum`) in our database. You can specify in what language you want the\nresult.\n\n```python\nfrom kindwise import PlantApi, SearchResult\n\napi = PlantApi(api_key=\'your_api_key\')\nsearch_result: SearchResult = api.search(\'Taraxacum\', language=\'en\', limit=1)\n\n# details can also be specified as a list of strings\ndetails = \'common_names,taxonomy\'\n\nentity_details = api.get_kb_detail(search_result.entities[0].access_token, details, language=\'de\')\n```\n',
     'author': 'Simon Plhak',
     'author_email': 'simon.plhak@flowerchecker.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/flowerchecker/kindwise',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `kindwise_api_client-0.4.1/PKG-INFO` & `kindwise_api_client-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kindwise-api-client
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python SDK toolkit for integrating Kindwise API
 Home-page: https://github.com/flowerchecker/kindwise
 License: MIT
 Author: Simon Plhak
 Author-email: simon.plhak@flowerchecker.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -92,14 +92,16 @@
 | [`usage_info`](#usage_info)                               | get api key usage information                                                       | `UsageInfo`        | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | [`feedback`](#feedback)                                   | send feedback for identification                                                    | boolean            | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | [`health_assessment`](#health_assessment)                 | create health assessment identification                                             | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |
 | [`get_health_assessment`](#get_health_assessment)         | get health assessment identification                                                | `HealthAssessment` | :white_check_mark: | :x:                | :x:                | :x:                |
 | [`delete_health_assessment`](#delete_health_assessment)   | delete health assessment                                                            | boolean            | :white_check_mark: | :x:                | :x:                | :x:                |
 | [`available_details`](#available_details)                 | details which can be used to specify additional information for `identify`          | dict               | :white_check_mark: | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | [`available_disease_details`](#available_disease_details) | details which can be used to specify additional information for `health_assessment` | dict               | :white_check_mark: | :x:                | :x:                | :x:                |
+| [`search`](#search)                                       | search for entity by query param in our database                                    | `SearchRecord`     | :white_check_mark: | :white_check_mark: | :white_check_mark: | :x:                |
+| [`get_kb_detail`](#get_kb_detail)                         | returns information about entity                                                    | `dict`             | :white_check_mark: | :white_check_mark: | :white_check_mark: | :x:                |
 
 Datetime objects are created by method `datetime.fromtimestamp(timestamp)`. This means that datetime objects are in
 local timezone.
 
 ### Documentation
 
 #### available_details
@@ -190,28 +192,29 @@
     classification_level=classification_level,
     classification_raw=classification_raw,
     extra_get_params=extra_get_params,
     extra_post_params=extra_post_params,
 )
 
 # identification created from stream
-with open('path/to/image.jpg', 'rb') as image :
+with open('path/to/image.jpg', 'rb') as image:
     identification_from_stream: PlantIdentification = api.identify(image.read())
 
 # identification created from file object
-with open('path/to/image.jpg', 'rb') as image :
+with open('path/to/image.jpg', 'rb') as image:
     identification_from_file: PlantIdentification = api.identify(image)
 
 # identification created from base64 encoded image
-with open('path/to/image.jpg', 'rb') as image :
+with open('path/to/image.jpg', 'rb') as image:
     image_in_base64 = base64.b64encode(image.read())
     identification_from_base64: PlantIdentification = api.identify(image)
 
 # identification created from PIL.Image.Image object
 from PIL import Image
+
 image = Image.open('path/to/image.jpg')
 identification_from_pil: PlantIdentification = api.identify(image)
 
 # identification created from image url
 image_url = 'https://api.gbif.org/v1/image/cache/fit-in/500x/occurrence/4596837568/media/33ff3ad210e56b73ade6f9fe622c650e'
 identification_from_url: PlantIdentification = api.identify(image_url)
 ```
@@ -405,7 +408,37 @@
 
 api = PlantApi(api_key='your_api_key')
 
 custom_id = 123  # also works with access_token or HealthAssessment object
 api.delete_health_assessment(custom_id)
 ```
 
+#### search
+
+Search for entity(e.g. `Taraxacum`) by query param in our database. You can specify language, limit and database type.
+
+```python
+from kindwise import PlantApi, SearchResult, PlantKBType
+
+api = PlantApi(api_key='your_api_key')
+kb_type = PlantKBType.PLANTS
+limit = 10
+search_result: SearchResult = api.search('Taraxacum', language='en', kb_type=kb_type, limit=limit)
+```
+
+#### get_kb_detail
+
+Returns information about entity(e.g. `Taraxacum`) in our database. You can specify in what language you want the
+result.
+
+```python
+from kindwise import PlantApi, SearchResult
+
+api = PlantApi(api_key='your_api_key')
+search_result: SearchResult = api.search('Taraxacum', language='en', limit=1)
+
+# details can also be specified as a list of strings
+details = 'common_names,taxonomy'
+
+entity_details = api.get_kb_detail(search_result.entities[0].access_token, details, language='de')
+```
+
```

