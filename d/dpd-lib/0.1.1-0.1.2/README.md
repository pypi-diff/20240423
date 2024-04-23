# Comparing `tmp/dpd_lib-0.1.1.tar.gz` & `tmp/dpd_lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpd_lib-0.1.1.tar", last modified: Thu Apr 11 22:27:09 2024, max compression
+gzip compressed data, was "dpd_lib-0.1.2.tar", last modified: Tue Apr 23 18:44:20 2024, max compression
```

## Comparing `dpd_lib-0.1.1.tar` & `dpd_lib-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 22:27:09.240592 dpd_lib-0.1.1/
--rw-r--r--   0 root         (0) root         (0)     2101 2024-04-11 22:27:09.240592 dpd_lib-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-11 22:22:00.000000 dpd_lib-0.1.1/PYPI.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 22:27:09.236592 dpd_lib-0.1.1/dpd_lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 22:27:00.000000 dpd_lib-0.1.1/dpd_lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 22:27:09.240592 dpd_lib-0.1.1/dpd_lib/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 22:27:00.000000 dpd_lib-0.1.1/dpd_lib/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-11 22:22:00.000000 dpd_lib-0.1.1/dpd_lib/client/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8426 2024-04-11 22:22:00.000000 dpd_lib-0.1.1/dpd_lib/client/influx.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2024-04-11 22:22:00.000000 dpd_lib-0.1.1/dpd_lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-11 22:22:00.000000 dpd_lib-0.1.1/dpd_lib/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 22:27:09.240592 dpd_lib-0.1.1/dpd_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2101 2024-04-11 22:27:09.000000 dpd_lib-0.1.1/dpd_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      313 2024-04-11 22:27:09.000000 dpd_lib-0.1.1/dpd_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 22:27:09.000000 dpd_lib-0.1.1/dpd_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2024-04-11 22:27:09.000000 dpd_lib-0.1.1/dpd_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 22:27:09.000000 dpd_lib-0.1.1/dpd_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-11 22:27:00.000000 dpd_lib-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 22:27:09.240592 dpd_lib-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:44:20.753496 dpd_lib-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-23 18:44:20.753496 dpd_lib-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/PYPI.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:44:20.749496 dpd_lib-0.1.2/dpd_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:44:11.000000 dpd_lib-0.1.2/dpd_lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:44:20.749496 dpd_lib-0.1.2/dpd_lib/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-23 18:44:11.000000 dpd_lib-0.1.2/dpd_lib/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/dpd_lib/client/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11597 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/dpd_lib/client/influx.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/dpd_lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      690 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/dpd_lib/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 18:44:20.753496 dpd_lib-0.1.2/dpd_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-23 18:44:20.000000 dpd_lib-0.1.2/dpd_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      313 2024-04-23 18:44:20.000000 dpd_lib-0.1.2/dpd_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 18:44:20.000000 dpd_lib-0.1.2/dpd_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-23 18:44:20.000000 dpd_lib-0.1.2/dpd_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-23 18:44:20.000000 dpd_lib-0.1.2/dpd_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-23 18:41:44.000000 dpd_lib-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 18:44:20.753496 dpd_lib-0.1.2/setup.cfg
```

### Comparing `dpd_lib-0.1.1/PKG-INFO` & `dpd_lib-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.1.1/PYPI.md` & `dpd_lib-0.1.2/PYPI.md`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.1.1/dpd_lib/client/exceptions.py` & `dpd_lib-0.1.2/dpd_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.1.1/dpd_lib/client/influx.py` & `dpd_lib-0.1.2/dpd_lib/client/influx.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,36 +26,37 @@
 from typing import Any, List
 
 from dpd_lib.client.exceptions import (
     BadQueryException,
     BucketNotFoundException,
     InfluxNotAvailableException,
 )
-from dpd_lib.models import InfluxInfrasoundRecord
+from dpd_lib.models import InfluxRecord
 from influxdb_client import InfluxDBClient, Point
 from influxdb_client.client.write_api import SYNCHRONOUS
 from influxdb_client.rest import ApiException
 from loguru import logger
 from pydantic import SecretStr
 from urllib3.exceptions import NewConnectionError
 
+INFRASOUND_TYPES = ["", "mccm", "velocity", "rsam", "pressure", "azimuth"]
+SEISMIC_YPES = ["", "rsam"]
+
 
 class InfluxClient:
     """
     A restricted client which implements an interface
     to query data from the influx database.
 
     Attributes:
         bucket (str): InfluxDB Bucket to query.
         _client (InfluxDBClient): The instantiated
             InfluxDB client.
     """
 
-    MEASUREMENT_NAME: str = "infrasound"
-
     def __init__(
         self, bucket: str, token: SecretStr, org: str, url: str
     ) -> None:
         """
         Initializes the InfluxDB Client based-off bucket, org, and url.
         Also requires an API token.
 
@@ -66,14 +67,99 @@
             url (str): InfluxDB url.
         """
         self.bucket = bucket
         self._client = InfluxDBClient(
             url=url, token=token.get_secret_value(), org=org
         )
 
+    async def record_seismic(
+        self, type: str, value: float, station: str, timestamp: datetime
+    ) -> None:
+        """
+        Records new seismic record for a given timestamp
+
+        Arguments:
+            type (str): The type of seismic record
+            value (float): The value of the record
+            station (str): The associated station
+            timestamp (datetime): The timestamp
+
+        Returns:
+            None
+
+        Raises:
+            InfluxNotAvailableException: An error occurred
+                while contacting the InfluxDB.
+            BadQueryException: There is an issue with the
+                influx query.
+            BucketNotFoundException: The requested bucket
+            is not present in the DB.
+        """
+        if type not in SEISMIC_YPES:
+            raise BadQueryException(
+                f"Seismic type not accepted. Accepted types: {SEISMIC_YPES}."
+            )
+        p = (
+            Point(type)
+            .tag("station", station)
+            .field(type, value)
+            .time(timestamp)
+        )
+        await self._insert(p)
+
+    async def read_seismic(
+        self,
+        type: str = "",
+        stations: List[str] = [],
+        t0: datetime = datetime.now(timezone.utc) - timedelta(seconds=15),
+        t1: datetime = datetime.now(timezone.utc),
+    ) -> List[InfluxRecord]:
+        """
+        Reads seismic records for a given type, station list, and timestamp
+
+        Arguments:
+            type (str): The type of seismic record
+            station (List(str)): The station of seismic record
+            t0 (datetime): the beginning of the timerange
+            t1 (datetime): The end of the timerange
+
+        Returns:
+            List[InfluxRecord]: All records of a
+            certain type for a given range.
+
+        Raises:
+            InfluxNotAvailableException: An error occurred
+                while contacting the InfluxDB.
+            BadQueryException: There is an issue with the
+                influx query.
+            BucketNotFoundException: The requested bucket
+            is not present in the DB.
+        """
+        if type not in SEISMIC_YPES:
+            raise BadQueryException(
+                f"Seismic type not accepted. Accepted types: {SEISMIC_YPES}."
+            )
+        query = """from(bucket:"{0}")
+        |> range(start: {1}, stop: {2})""".format(
+            self.bucket,
+            t0.strftime("%Y-%m-%dT%H:%M:%SZ"),
+            t1.strftime("%Y-%m-%dT%H:%M:%SZ"),
+        )
+        if type != "":
+            query += '|> filter(fn:(r) => r._measurement == "{0}")'.format(
+                type
+            )
+        if len(stations) != 0:
+            query += """
+            |> filter(fn:(r) => contains(value: r.station, set: {0}))
+            """.format(
+                json.dumps(stations)
+            )
+        return await self._query(query)
+
     async def record_infrasound(
         self, type: str, value: float, station: str, timestamp: datetime
     ) -> None:
         """
         Records new infrasound record for a given timestamp
 
         Arguments:
@@ -89,51 +175,58 @@
             InfluxNotAvailableException: An error occurred
                 while contacting the InfluxDB.
             BadQueryException: There is an issue with the
                 influx query.
             BucketNotFoundException: The requested bucket
             is not present in the DB.
         """
-
+        if type not in INFRASOUND_TYPES:
+            raise BadQueryException(
+                f"Type not accepted. Accepted types: {INFRASOUND_TYPES}."
+            )
         p = (
             Point(type)
             .tag("station", station)
             .field(type, value)
             .time(timestamp)
         )
         await self._insert(p)
 
     async def read_infrasound(
         self,
         type: str = "",
         stations: List[str] = [],
         t0: datetime = datetime.now(timezone.utc) - timedelta(seconds=15),
         t1: datetime = datetime.now(timezone.utc),
-    ) -> List[InfluxInfrasoundRecord]:
+    ) -> List[InfluxRecord]:
         """
         Reads infrasound records for a given type, station list, and timestamp
 
         Arguments:
             type (str): The type of infrasound record
             station (List(str)): The station of infrasound record
             t0 (datetime): the beginning of the timerange
             t1 (datetime): The end of the timerange
 
         Returns:
-            List[InfluxInfrasoundRecord]: All records of a
+            List[InfluxRecord]: All records of a
             certain type for a given range.
 
         Raises:
             InfluxNotAvailableException: An error occurred
                 while contacting the InfluxDB.
             BadQueryException: There is an issue with the
                 influx query.
             BucketNotFoundException: The requested bucket
             is not present in the DB.
         """
+        if type not in INFRASOUND_TYPES:
+            raise BadQueryException(
+                f"Type not accepted. Accepted types: {INFRASOUND_TYPES}."
+            )
         query = """from(bucket:"{0}")
         |> range(start: {1}, stop: {2})""".format(
             self.bucket,
             t0.strftime("%Y-%m-%dT%H:%M:%SZ"),
             t1.strftime("%Y-%m-%dT%H:%M:%SZ"),
         )
         if type != "":
@@ -144,40 +237,45 @@
             query += """
             |> filter(fn:(r) => contains(value: r.station, set: {0}))
             """.format(
                 json.dumps(stations)
             )
         return await self._query(query)
 
-    async def list_infrasound(
+    async def list_records(
         self,
         t0: datetime = datetime.now(timezone.utc) - timedelta(seconds=15),
         t1: datetime = datetime.now(timezone.utc),
-    ) -> List[InfluxInfrasoundRecord]:
+    ) -> List[InfluxRecord]:
         """
         Lists all records for given time range.
 
         Arguments:
             t0 (datetime): the beginning of the timerange
             t1 (datetime): The end of the timerange
 
         Returns:
-            List[InfluxInfrasoundRecord]:
+            List[InfluxRecord]:
                 All records for given time range.
 
         Raises:
             InfluxNotAvailableException: An error occurred
                 while contacting the InfluxDB.
             BadQueryException: There is an issue with the
                 influx query.
             BucketNotFoundException: The requested bucket
             is not present in the DB.
         """
-
-        return await self.read_infrasound(type="", stations=[], t0=t0, t1=t1)
+        query = """from(bucket:"{0}")
+        |> range(start: {1}, stop: {2})""".format(
+            self.bucket,
+            t0.strftime("%Y-%m-%dT%H:%M:%SZ"),
+            t1.strftime("%Y-%m-%dT%H:%M:%SZ"),
+        )
+        return await self._query(query)
 
     async def _insert(self, p: Point) -> Any:
         """
         Inserts a point into the database via InfluxDB write_api
 
         Arguments:
             p (Point): The data point to insert into the database
@@ -203,23 +301,23 @@
                 raise BadQueryException()
             if e.status and e.status == 404:
                 raise BucketNotFoundException()
             raise InfluxNotAvailableException()
         logger.info(f"{res=}")
         return res
 
-    async def _query(self, query: str = "") -> List[InfluxInfrasoundRecord]:
+    async def _query(self, query: str = "") -> List[InfluxRecord]:
         """
         Queries the InfluxDB with the proivded query string
 
         Arguments:
             query (str): The raw query string to pass to InfluxDB
 
         Returns:
-            List[InfluxInfrasoundRecord]:
+            List[InfluxRecord]:
                 A list of records that match the query
 
         Raises:
             InfluxNotAvailableException: An error occurred
                 while contacting the InfluxDB.
             BadQueryException: There is an issue with the
                 influx query.
@@ -237,19 +335,15 @@
                 raise BadQueryException()
             if e.status and e.status == 404:
                 raise BucketNotFoundException()
             raise InfluxNotAvailableException()
         res = []
         for table in result:
             for record in table.records:
-                logger.debug(record)
-                logger.debug(record.get_measurement())
-                logger.debug(record.values.get("station"))
-                logger.debug(record.get_time())
-                r = InfluxInfrasoundRecord(
+                r = InfluxRecord(
                     type=record.get_measurement(),
                     station=record.values.get("station"),
                     timestamp=record.get_time(),
                     value=record.get_value(),
                 )
                 res.append(r)
         logger.debug(f"Query returned {len(res)} records.")
```

### Comparing `dpd_lib-0.1.1/dpd_lib/config.py` & `dpd_lib-0.1.2/dpd_lib/config.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.1.1/dpd_lib/models.py` & `dpd_lib-0.1.2/dpd_lib/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 
 from pydantic import BaseModel, Field
 
 
-class InfluxInfrasoundRecord(BaseModel):
+class InfluxRecord(BaseModel):
     """
-    A pydantic model to structure infrasound records stored
+    A pydantic model to structure influx records stored
     in the InfluxDB.
 
     Attributes:
         type (str): Type of metric.
         value (float): Value of metric.
         station (str): Station metric was originally recorded.
         timestamp (datetime): Center of time window of processed metric.
```

### Comparing `dpd_lib-0.1.1/dpd_lib.egg-info/PKG-INFO` & `dpd_lib-0.1.2/dpd_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.1.1
+Version: 0.1.2
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.1.1/pyproject.toml` & `dpd_lib-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=66.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpd_lib"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Noah Harper", email="nharper@usgs.gov" },
 ]
 description = "A package for interacting with the USGS influx db"
 readme = "PYPI.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

