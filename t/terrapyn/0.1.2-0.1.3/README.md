# Comparing `tmp/terrapyn-0.1.2.tar.gz` & `tmp/terrapyn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrapyn-0.1.2.tar", max compression
+gzip compressed data, was "terrapyn-0.1.3.tar", max compression
```

## Comparing `terrapyn-0.1.2.tar` & `terrapyn-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      126 2024-04-18 23:47:03.828582 terrapyn-0.1.2/AUTHORS.md
--rw-r--r--   0        0        0     1468 2024-04-18 23:47:03.828582 terrapyn-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     1958 2024-04-18 23:47:03.828582 terrapyn-0.1.2/README.md
--rw-r--r--   0        0        0     1197 2024-04-18 23:47:16.000667 terrapyn-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      522 2024-04-18 23:47:03.828582 terrapyn-0.1.2/terrapyn/__init__.py
--rw-r--r--   0        0        0       39 2024-04-18 23:47:03.828582 terrapyn-0.1.2/terrapyn/bq/__init__.py
--rw-r--r--   0        0        0    12530 2024-04-18 23:47:03.828582 terrapyn-0.1.2/terrapyn/bq/data.py
--rw-r--r--   0        0        0    24009 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/conversion.py
--rw-r--r--   0        0        0     2842 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/dask_utils.py
--rw-r--r--   0        0        0       81 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/ee/__init__.py
--rw-r--r--   0        0        0     8800 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/ee/data.py
--rw-r--r--   0        0        0     1484 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/ee/io.py
--rw-r--r--   0        0        0     8188 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/ee/stats.py
--rw-r--r--   0        0        0     5230 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/ee/utils.py
--rw-r--r--   0        0        0       99 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/indices/__init__.py
--rw-r--r--   0        0        0     1066 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/indices/_agro.py
--rw-r--r--   0        0        0    15286 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/indices/spi.py
--rw-r--r--   0        0        0     3982 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/io.py
--rw-r--r--   0        0        0      155 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/logger.py
--rw-r--r--   0        0        0       67 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/params/__init__.py
--rw-r--r--   0        0        0     9594 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/params/etp.py
--rw-r--r--   0        0        0     3920 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/params/soil.py
--rw-r--r--   0        0        0    23658 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/params/solar.py
--rw-r--r--   0        0        0        0 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/py.typed
--rw-r--r--   0        0        0    26042 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/space.py
--rw-r--r--   0        0        0    22088 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/stats.py
--rw-r--r--   0        0        0    47655 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/time.py
--rw-r--r--   0        0        0     7736 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/utils.py
--rw-r--r--   0        0        0     3387 2024-04-18 23:47:03.832582 terrapyn-0.1.2/terrapyn/validation.py
--rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 terrapyn-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      126 2024-04-23 16:14:35.488026 terrapyn-0.1.3/AUTHORS.md
+-rw-r--r--   0        0        0     1468 2024-04-23 16:14:35.488026 terrapyn-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     1958 2024-04-23 16:14:35.488026 terrapyn-0.1.3/README.md
+-rw-r--r--   0        0        0     1197 2024-04-23 16:14:43.579927 terrapyn-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      522 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/__init__.py
+-rw-r--r--   0        0        0       39 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/bq/__init__.py
+-rw-r--r--   0        0        0    13136 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/bq/data.py
+-rw-r--r--   0        0        0    24009 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/conversion.py
+-rw-r--r--   0        0        0     2842 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/dask_utils.py
+-rw-r--r--   0        0        0       81 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/ee/__init__.py
+-rw-r--r--   0        0        0     8800 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/ee/data.py
+-rw-r--r--   0        0        0     1484 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/ee/io.py
+-rw-r--r--   0        0        0     8188 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/ee/stats.py
+-rw-r--r--   0        0        0     5230 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/ee/utils.py
+-rw-r--r--   0        0        0       99 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/indices/__init__.py
+-rw-r--r--   0        0        0     1066 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/indices/_agro.py
+-rw-r--r--   0        0        0    15286 2024-04-23 16:14:35.492026 terrapyn-0.1.3/terrapyn/indices/spi.py
+-rw-r--r--   0        0        0     3982 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/io.py
+-rw-r--r--   0        0        0      155 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/logger.py
+-rw-r--r--   0        0        0       67 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/params/__init__.py
+-rw-r--r--   0        0        0     9594 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/params/etp.py
+-rw-r--r--   0        0        0     3920 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/params/soil.py
+-rw-r--r--   0        0        0    23658 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/params/solar.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/py.typed
+-rw-r--r--   0        0        0    26042 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/space.py
+-rw-r--r--   0        0        0    22088 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/stats.py
+-rw-r--r--   0        0        0    47655 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/time.py
+-rw-r--r--   0        0        0     7736 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/utils.py
+-rw-r--r--   0        0        0     3387 2024-04-23 16:14:35.496026 terrapyn-0.1.3/terrapyn/validation.py
+-rw-r--r--   0        0        0     3092 1970-01-01 00:00:00.000000 terrapyn-0.1.3/PKG-INFO
```

### Comparing `terrapyn-0.1.2/LICENSE.md` & `terrapyn-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/README.md` & `terrapyn-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/pyproject.toml` & `terrapyn-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "terrapyn"
-version = "0.1.2"
+version = "0.1.3"
 description="Toolkit to manipulate Earth observations and models."
 authors = ["colinahill <colinalastairhill@gmail.com>"]
 readme = "README.md"
 license="BSD-3-Clause"
 packages = [{include = "terrapyn"}]
 
 [tool.poetry.dependencies]
```

### Comparing `terrapyn-0.1.2/terrapyn/__init__.py` & `terrapyn-0.1.3/terrapyn/__init__.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/bq/data.py` & `terrapyn-0.1.3/terrapyn/bq/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,16 +77,16 @@
             " - precip: Precipitation (mm)\n"
             " - windspeed: Windspeed (m/s)"
         )
         return string
 
     def stations(
         self,
-        start_date: dt.datetime = dt.date(1750, 1, 1),
-        end_date: dt.datetime = dt.date.today(),
+        start_date: dt.date = dt.date(1750, 1, 1),
+        end_date: dt.date = dt.date.today(),
         geom: shapely.Geometry = None,
     ):
         """
         Get weather stations from the NOAA GSOD dataset that are within a given geometry and date range.
 
         Args:
             start_date: The start date for the station data.
@@ -95,29 +95,34 @@
 
         Returns:
             A Pandas DataFrame with the station metadata.
         """
         if geom is None:
             geom = shapely.geometry.box(-180, -90, 180, 90)
 
+        if isinstance(start_date, dt.datetime):
+            start_date = start_date.date()
+        if isinstance(end_date, dt.datetime):
+            end_date = end_date.date()
+
         geometry_string = _shapely_geometry_to_string_for_bigquery(geom)
 
         query = """
             with stations as (
                 select
                     concat(usaf, wban) as id,
                     st_geogpoint(lon, lat) as geom,
                     parse_numeric(elev) as elevation,
                     parse_date('%Y%m%d', `begin`) as start_date,
                     parse_date('%Y%m%d', `end`) as end_date,
                 from `bigquery-public-data.noaa_gsod.stations`
                 where lat != 0 and lon != 0
             )
             select * from stations
-            where ((start_date between @start and @end) or (end_date between @start and @end))
+            where start_date <= @end and end_date >= @start
             and st_intersects(geom, st_geogfromgeojson(@geometry_string, make_valid => True))
             """
 
         job_config = bigquery.QueryJobConfig(
             query_parameters=[
                 bigquery.ScalarQueryParameter("start", "DATE", start_date),
                 bigquery.ScalarQueryParameter("end", "DATE", end_date),
@@ -132,30 +137,35 @@
         df.loc[df["elevation"].isna() | df["elevation"].eq(-999), "elevation"] = 0.0
         df["elevation"] = df["elevation"].astype(float)
         return df
 
     def data(
         self,
         station_ids: T.Union[str, T.List[str]],
-        start_date: dt.datetime = dt.date(1750, 1, 1),
-        end_date: dt.datetime = dt.date.today(),
+        start_date: dt.date = dt.date(1750, 1, 1),
+        end_date: dt.date = dt.date.today(),
     ):
         """
         Get weather data from the NOAA GSOD dataset for the given stations and date range.
 
         Args:
             station_ids: The station ID(s).
             start_date: The start date for the station data.
             end_date: The end date for the station data.
 
         Returns:
             A Pandas DataFrame with the station data.
         """
         station_ids = tp.utils.ensure_list(station_ids)
 
+        if isinstance(start_date, dt.datetime):
+            start_date = start_date.date()
+        if isinstance(end_date, dt.datetime):
+            end_date = end_date.date()
+
         query = """
             with raw as (
                 select
                     concat(stn, wban) as id,
                     parse_date('%Y%m%d', concat(year, mo, da)) date,
                     if(`temp` = 9999.9, null, (`temp` - 32.0) * (5.0/9.0)) as tavg,
                     if(`max` = 9999.9, null, (`max` - 32.0) * (5.0/9.0)) as tmax,
@@ -210,16 +220,16 @@
             " - precip: Precipitation (mm)\n"
             " - snow: Snowfall (mm)\n"
         )
         return string
 
     def stations(
         self,
-        start_date: dt.datetime = dt.date(1750, 1, 1),
-        end_date: dt.datetime = dt.date.today(),
+        start_date: dt.date = dt.date(1750, 1, 1),
+        end_date: dt.date = dt.date.today(),
         geom: shapely.Geometry = None,
     ):
         """
         Get weather stations from the NOAA GHCN dataset that are within a given geometry and date range.
 
         Args:
             start_date: The start date for the station data.
@@ -228,14 +238,19 @@
 
         Returns:
             A Pandas DataFrame with the station metadata.
         """
         if geom is None:
             geom = shapely.geometry.box(-180, -90, 180, 90)
 
+        if isinstance(start_date, dt.datetime):
+            start_date = start_date.date()
+        if isinstance(end_date, dt.datetime):
+            end_date = end_date.date()
+
         geometry_string = _shapely_geometry_to_string_for_bigquery(geom)
 
         query = """
             with stations as (
                 select
                     a.id,
                     st_geogpoint(a.longitude, a.latitude) as geom,
@@ -250,15 +265,15 @@
                         max(lastyear) as end_year
                     from `bigquery-public-data.ghcn_d.ghcnd_inventory`
                     group by id
                     ) b
                 using(id)
             )
             select * from stations
-            where ((start_date between @start and @end) or (end_date between @start and @end))
+            where start_date <= @end and end_date >= @start
             and st_intersects(geom, st_geogfromgeojson(@geometry_string, make_valid => True))
             """
 
         job_config = bigquery.QueryJobConfig(
             query_parameters=[
                 bigquery.ScalarQueryParameter("start", "DATE", start_date),
                 bigquery.ScalarQueryParameter("end", "DATE", end_date),
@@ -273,30 +288,35 @@
         df.loc[df["elevation"].isna() | df["elevation"].eq(-999.9), "elevation"] = 0.0
         df["elevation"] = df["elevation"].astype(float)
         return df
 
     def data(
         self,
         station_ids: T.Union[str, T.List[str]],
-        start_date: dt.datetime = dt.date(1750, 1, 1),
-        end_date: dt.datetime = dt.date.today(),
+        start_date: dt.date = dt.date(1750, 1, 1),
+        end_date: dt.date = dt.date.today(),
     ):
         """
         Get weather data from the NOAA GHCN dataset for the given stations and date range.
 
         Args:
             station_ids: The station ID(s).
             start_date: The start date for the station data.
             end_date: The end date for the station data.
 
         Returns:
             A Pandas DataFrame with the station data.
         """
         station_ids = tp.utils.ensure_list(station_ids)
 
+        if isinstance(start_date, dt.datetime):
+            start_date = start_date.date()
+        if isinstance(end_date, dt.datetime):
+            end_date = end_date.date()
+
         query = """
             with raw as (
                 select
                     id,
                     `date`,
                     if(element = 'TMAX', value/10, null) as tmax,
                     if(element = 'TMIN', value/10, null) as tmin,
```

### Comparing `terrapyn-0.1.2/terrapyn/conversion.py` & `terrapyn-0.1.3/terrapyn/conversion.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/dask_utils.py` & `terrapyn-0.1.3/terrapyn/dask_utils.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/ee/data.py` & `terrapyn-0.1.3/terrapyn/ee/data.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/ee/io.py` & `terrapyn-0.1.3/terrapyn/ee/io.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/ee/stats.py` & `terrapyn-0.1.3/terrapyn/ee/stats.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/ee/utils.py` & `terrapyn-0.1.3/terrapyn/ee/utils.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/indices/_agro.py` & `terrapyn-0.1.3/terrapyn/indices/_agro.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/indices/spi.py` & `terrapyn-0.1.3/terrapyn/indices/spi.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/io.py` & `terrapyn-0.1.3/terrapyn/io.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/params/etp.py` & `terrapyn-0.1.3/terrapyn/params/etp.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/params/soil.py` & `terrapyn-0.1.3/terrapyn/params/soil.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/params/solar.py` & `terrapyn-0.1.3/terrapyn/params/solar.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/space.py` & `terrapyn-0.1.3/terrapyn/space.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/stats.py` & `terrapyn-0.1.3/terrapyn/stats.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/time.py` & `terrapyn-0.1.3/terrapyn/time.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/utils.py` & `terrapyn-0.1.3/terrapyn/utils.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/terrapyn/validation.py` & `terrapyn-0.1.3/terrapyn/validation.py`

 * *Files identical despite different names*

### Comparing `terrapyn-0.1.2/PKG-INFO` & `terrapyn-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrapyn
-Version: 0.1.2
+Version: 0.1.3
 Summary: Toolkit to manipulate Earth observations and models.
 License: BSD-3-Clause
 Author: colinahill
 Author-email: colinalastairhill@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

