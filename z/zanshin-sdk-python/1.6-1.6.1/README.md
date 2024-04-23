# Comparing `tmp/zanshin_sdk_python-1.6.tar.gz` & `tmp/zanshin_sdk_python-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zanshin_sdk_python-1.6.tar", max compression
+gzip compressed data, was "zanshin_sdk_python-1.6.1.tar", max compression
```

## Comparing `zanshin_sdk_python-1.6.tar` & `zanshin_sdk_python-1.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-23 12:32:16.534726 zanshin_sdk_python-1.6/LICENSE
--rw-r--r--   0        0        0     5372 2024-04-23 12:32:16.534726 zanshin_sdk_python-1.6/README.md
--rw-r--r--   0        0        0     1501 2024-04-23 12:32:16.766728 zanshin_sdk_python-1.6/pyproject.toml
--rw-r--r--   0        0        0      757 2024-04-23 12:32:16.550726 zanshin_sdk_python-1.6/zanshinsdk/__init__.py
--rw-r--r--   0        0        0     1887 2024-04-23 12:32:16.550726 zanshin_sdk_python-1.6/zanshinsdk/alerts_history.py
--rw-r--r--   0        0        0   103665 2024-04-23 12:32:16.554726 zanshin_sdk_python-1.6/zanshinsdk/client.py
--rw-r--r--   0        0        0     4397 2024-04-23 12:32:16.554726 zanshin_sdk_python-1.6/zanshinsdk/docs/README.md
--rw-r--r--   0        0        0       60 2024-04-23 12:32:16.554726 zanshin_sdk_python-1.6/zanshinsdk/dummy_aws_credentials
--rw-r--r--   0        0        0     2038 2024-04-23 12:32:16.554726 zanshin_sdk_python-1.6/zanshinsdk/dummy_cloudformation_zanshin_service_role_template.json
--rw-r--r--   0        0        0     1782 2024-04-23 12:32:16.554726 zanshin_sdk_python-1.6/zanshinsdk/following_alerts_history.py
--rw-r--r--   0        0        0     5751 2024-04-23 12:32:16.554726 zanshin_sdk_python-1.6/zanshinsdk/iterator.py
--rw-r--r--   0        0        0     2471 2024-04-23 12:32:16.554726 zanshin_sdk_python-1.6/zanshinsdk/test_alerts_history.py
--rw-r--r--   0        0        0   113864 2024-04-23 12:32:16.554726 zanshin_sdk_python-1.6/zanshinsdk/test_client.py
--rw-r--r--   0        0        0     2542 2024-04-23 12:32:16.554726 zanshin_sdk_python-1.6/zanshinsdk/test_following_alerts_history.py
--rw-r--r--   0        0        0    10022 2024-04-23 12:32:16.554726 zanshin_sdk_python-1.6/zanshinsdk/test_iterator.py
--rw-r--r--   0        0        0       20 2024-04-23 12:32:16.762727 zanshin_sdk_python-1.6/zanshinsdk/version.py
--rw-r--r--   0        0        0     6638 1970-01-01 00:00:00.000000 zanshin_sdk_python-1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-23 16:56:39.716131 zanshin_sdk_python-1.6.1/LICENSE
+-rw-r--r--   0        0        0     5372 2024-04-23 16:56:39.716131 zanshin_sdk_python-1.6.1/README.md
+-rw-r--r--   0        0        0     1503 2024-04-23 16:56:39.956131 zanshin_sdk_python-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0      745 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/__init__.py
+-rw-r--r--   0        0        0     1887 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/alerts_history.py
+-rw-r--r--   0        0        0   103609 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/client.py
+-rw-r--r--   0        0        0     4397 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/docs/README.md
+-rw-r--r--   0        0        0       60 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/dummy_aws_credentials
+-rw-r--r--   0        0        0     2038 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/dummy_cloudformation_zanshin_service_role_template.json
+-rw-r--r--   0        0        0     1782 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/following_alerts_history.py
+-rw-r--r--   0        0        0     5751 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/iterator.py
+-rw-r--r--   0        0        0     2471 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/test_alerts_history.py
+-rw-r--r--   0        0        0   113840 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/test_client.py
+-rw-r--r--   0        0        0     2542 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/test_following_alerts_history.py
+-rw-r--r--   0        0        0    10022 2024-04-23 16:56:39.736131 zanshin_sdk_python-1.6.1/zanshinsdk/test_iterator.py
+-rw-r--r--   0        0        0       22 2024-04-23 16:56:39.952130 zanshin_sdk_python-1.6.1/zanshinsdk/version.py
+-rw-r--r--   0        0        0     6640 1970-01-01 00:00:00.000000 zanshin_sdk_python-1.6.1/PKG-INFO
```

### Comparing `zanshin_sdk_python-1.6/LICENSE` & `zanshin_sdk_python-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6/README.md` & `zanshin_sdk_python-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6/pyproject.toml` & `zanshin_sdk_python-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zanshin-sdk-python"
-version = "1.6"
+version = "1.6.1"
 description = "Python SDK to access the Tenchi Security Zanshin API v1"
 license = "Apache Software License"
 authors = ["Tenchi Security <contact@tenchisecurity.com>"]
 readme = "README.md"
 packages = [{include = "zanshinsdk"}]
 homepage = "https://github.com/tenchi-security/zanshin-sdk-python"
 classifiers=[
```

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/__init__.py` & `zanshin_sdk_python-1.6.1/zanshinsdk/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 
 from zanshinsdk.client import (
     DAILY,
-    HOURLY,
     WEEKLY,
     AlertSeverity,
     AlertsOrderOpts,
     AlertState,
     Client,
     Languages,
     Roles,
```

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/alerts_history.py` & `zanshin_sdk_python-1.6.1/zanshinsdk/alerts_history.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/client.py` & `zanshin_sdk_python-1.6.1/zanshinsdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from os.path import isfile
 from pathlib import Path
 from typing import Dict, Iterable, Iterator, Optional, Union
 from urllib.parse import urlparse
 from uuid import UUID
 
 import httpx
+from pydantic import BaseModel, Field
 
 from zanshinsdk.version import __version__ as sdk_version
 
 CONFIG_DIR = Path.home() / ".tenchi"
 CONFIG_FILE = CONFIG_DIR / "config"
 
 
@@ -62,19 +63,18 @@
 
 class SortOpts(str, Enum):
     ASC = "asc"
     DESC = "desc"
 
 
 class Frequency(Enum):
-    ONE_HOUR = "1h"
     SIX_HOURS = "6h"
-    TWELVE_HOURS = ("12h",)
-    DAILY = ("1d",)
-    WEEKLY = ("7d",)
+    TWELVE_HOURS = "12h"
+    DAILY = "1d"
+    WEEKLY = "7d"
 
 
 class TimeOfDay(Enum):
     MORNING = "MORNING"
     AFTERNOON = "AFTERNOON"
     EVENING = "EVENING"
     NIGHT = "NIGHT"
@@ -86,46 +86,41 @@
     TUESDAY = "TUESDAY"
     WEDNESDAY = "WEDNESDAY"
     THURSDAY = "THURSDAY"
     FRIDAY = "FRIDAY"
     SATURDAY = "SATURDAY"
 
 
-class ScanTargetSchedule:
-    def __init__(
-        self,
-        frequency: Frequency,
-        timeOfDay: TimeOfDay = TimeOfDay.NIGHT,
-        day: Day = Day.SUNDAY,
-    ):
-        self._frequency = frequency
-        self._timeOfDay = timeOfDay
-        self._day = day
+class ScanTargetSchedule(BaseModel):
+    frequency: Frequency
+    time_of_day: Optional[TimeOfDay] = Field(TimeOfDay.NIGHT, alias="timeOfDay")
+    day: Optional[Day] = Day.SUNDAY
 
     def value(self):
-        if self._frequency.value < Frequency.DAILY.value:
-            return {"frequency": self._frequency.name}
-        if self._frequency == Frequency.WEEKLY:
+        if self.frequency in (Frequency.SIX_HOURS, Frequency.TWELVE_HOURS):
+            return {"frequency": self.frequency.value}
+        if self.frequency == Frequency.WEEKLY:
             return {
-                "frequency": Frequency.WEEKLY.name,
-                "timeOfDay": self._timeOfDay.name,
-                "day": self._day.name,
+                "frequency": self.frequency.value,
+                "timeOfDay": self.time_of_day.value,
+                "day": self.day.value,
             }
         return {
-            "frequency": Frequency.DAILY.name,
-            "timeOfDay": self._timeOfDay.name,
+            "frequency": self.frequency.value,
+            "timeOfDay": self.time_of_day.value,
         }
 
     def json(self):
         return json.dumps(self.value())
 
 
-DAILY = ScanTargetSchedule(Frequency.DAILY, TimeOfDay.NIGHT)
-HOURLY = ScanTargetSchedule(Frequency.ONE_HOUR)
-WEEKLY = ScanTargetSchedule(Frequency.WEEKLY, TimeOfDay.NIGHT, Day.SUNDAY)
+DAILY = ScanTargetSchedule(frequency=Frequency.DAILY, time_of_day=TimeOfDay.NIGHT)
+WEEKLY = ScanTargetSchedule(
+    frequency=Frequency.WEEKLY, time_of_day=TimeOfDay.NIGHT, day=Day.SUNDAY
+)
 
 
 class ScanTargetAWS(dict):
     def __init__(self, account):
         dict.__init__(self, account=account)
```

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/docs/README.md` & `zanshin_sdk_python-1.6.1/zanshinsdk/docs/README.md`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/dummy_cloudformation_zanshin_service_role_template.json` & `zanshin_sdk_python-1.6.1/zanshinsdk/dummy_cloudformation_zanshin_service_role_template.json`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/following_alerts_history.py` & `zanshin_sdk_python-1.6.1/zanshinsdk/following_alerts_history.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/iterator.py` & `zanshin_sdk_python-1.6.1/zanshinsdk/iterator.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/test_alerts_history.py` & `zanshin_sdk_python-1.6.1/zanshinsdk/test_alerts_history.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/test_client.py` & `zanshin_sdk_python-1.6.1/zanshinsdk/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -858,15 +858,15 @@
         self.sdk._request.assert_called_once_with(
             "POST",
             f"/organizations/{organization_id}/scantargets",
             body={
                 "name": name,
                 "kind": kind,
                 "credential": credential,
-                "schedule": {"frequency": "DAILY", "timeOfDay": "NIGHT"},
+                "schedule": {"frequency": "1d", "timeOfDay": "NIGHT"},
             },
         )
 
     def test_create_organization_scan_target_AZURE(self):
         organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
         kind = zanshinsdk.ScanTargetKind.AZURE
         name = "ScanTargetTest"
@@ -882,15 +882,15 @@
         self.sdk._request.assert_called_once_with(
             "POST",
             f"/organizations/{organization_id}/scantargets",
             body={
                 "name": name,
                 "kind": kind,
                 "credential": credential,
-                "schedule": {"frequency": "DAILY", "timeOfDay": "NIGHT"},
+                "schedule": {"frequency": "1d", "timeOfDay": "NIGHT"},
             },
         )
 
     def test_create_organization_scan_target_GCP(self):
         organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
         kind = zanshinsdk.ScanTargetKind.GCP
         name = "ScanTargetTest"
@@ -904,15 +904,15 @@
         self.sdk._request.assert_called_once_with(
             "POST",
             f"/organizations/{organization_id}/scantargets",
             body={
                 "name": name,
                 "kind": kind,
                 "credential": credential,
-                "schedule": {"frequency": "DAILY", "timeOfDay": "NIGHT"},
+                "schedule": {"frequency": "1d", "timeOfDay": "NIGHT"},
             },
         )
 
     def test_create_organization_scan_target_HUAWEI(self):
         organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
         kind = zanshinsdk.ScanTargetKind.HUAWEI
         name = "ScanTargetTest"
@@ -926,15 +926,15 @@
         self.sdk._request.assert_called_once_with(
             "POST",
             f"/organizations/{organization_id}/scantargets",
             body={
                 "name": name,
                 "kind": kind,
                 "credential": credential,
-                "schedule": {"frequency": "DAILY", "timeOfDay": "NIGHT"},
+                "schedule": {"frequency": "1d", "timeOfDay": "NIGHT"},
             },
         )
 
     def test_create_organization_scan_target_DOMAIN(self):
         organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
         kind = zanshinsdk.ScanTargetKind.DOMAIN
         name = "ScanTargetTest"
@@ -948,15 +948,15 @@
         self.sdk._request.assert_called_once_with(
             "POST",
             f"/organizations/{organization_id}/scantargets",
             body={
                 "name": name,
                 "kind": kind,
                 "credential": credential,
-                "schedule": {"frequency": "DAILY", "timeOfDay": "NIGHT"},
+                "schedule": {"frequency": "1d", "timeOfDay": "NIGHT"},
             },
         )
 
     def test_get_organization_scan_target(self):
         organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
         scan_target_id = "e22f4225-43e9-4922-b6b8-8b0620bdb110"
 
@@ -977,15 +977,15 @@
         )
 
         self.sdk._request.assert_called_once_with(
             "PUT",
             f"/organizations/{organization_id}/scantargets/{scan_target_id}",
             body={
                 "name": name,
-                "schedule": {"frequency": "DAILY", "timeOfDay": "NIGHT"},
+                "schedule": {"frequency": "1d", "timeOfDay": "NIGHT"},
             },
         )
 
     def test_delete_organization_scan_target(self):
         organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
         scan_target_id = "e22f4225-43e9-4922-b6b8-8b0620bdb110"
 
@@ -3086,15 +3086,15 @@
         # Assert that Scan Target was called with correct parameters
         client._client.request.assert_any_call(
             "POST",
             f"/organizations/{organization_id}/scantargets",
             body={
                 "name": name,
                 "kind": kind,
-                "schedule": {"frequency": "DAILY", "timeOfDay": "NIGHT"},
+                "schedule": {"frequency": "1d", "timeOfDay": "NIGHT"},
                 "credential": {"account": aws_account_id},
             },
         )
         # Assert that we checked Scan Target to start scan
         client._client.request.assert_any_call(
             "POST",
             f"/organizations/{organization_id}/scantargets/{created_scan_target_id}/check",
@@ -3208,15 +3208,15 @@
         # Assert that Scan Target was called with correct parameters
         client._client.request.assert_any_call(
             "POST",
             f"/organizations/{organization_id}/scantargets",
             body={
                 "name": name,
                 "kind": kind,
-                "schedule": {"frequency": "DAILY", "timeOfDay": "NIGHT"},
+                "schedule": {"frequency": "1d", "timeOfDay": "NIGHT"},
                 "credential": {"account": aws_account_id},
             },
         )
         # Assert that we checked Scan Target to start scan
         client._client.request.assert_any_call(
             "POST",
             f"/organizations/{organization_id}/scantargets/{created_scan_target_id}/check",
```

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/test_following_alerts_history.py` & `zanshin_sdk_python-1.6.1/zanshinsdk/test_following_alerts_history.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6/zanshinsdk/test_iterator.py` & `zanshin_sdk_python-1.6.1/zanshinsdk/test_iterator.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6/PKG-INFO` & `zanshin_sdk_python-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zanshin-sdk-python
-Version: 1.6
+Version: 1.6.1
 Summary: Python SDK to access the Tenchi Security Zanshin API v1
 Home-page: https://github.com/tenchi-security/zanshin-sdk-python
 License: Apache Software License
 Author: Tenchi Security
 Author-email: contact@tenchisecurity.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

