# Comparing `tmp/weather_rp5-1.0.1.tar.gz` & `tmp/weather_rp5-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_rp5-1.0.1.tar", last modified: Mon Apr 22 19:08:59 2024, max compression
+gzip compressed data, was "weather_rp5-1.0.2.tar", last modified: Tue Apr 23 19:47:49 2024, max compression
```

## Comparing `weather_rp5-1.0.1.tar` & `weather_rp5-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 19:08:59.833860 weather_rp5-1.0.1/
--rw-rw-rw-   0        0        0     1526 2024-04-22 19:08:59.830641 weather_rp5-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1097 2024-04-21 18:50:26.000000 weather_rp5-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 19:08:59.834978 weather_rp5-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-04-22 19:07:42.000000 weather_rp5-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:08:59.805709 weather_rp5-1.0.1/weather_rp5/
--rw-rw-rw-   0        0        0       50 2024-04-22 18:54:46.000000 weather_rp5-1.0.1/weather_rp5/__init__.py
--rw-rw-rw-   0        0        0     1975 2024-04-21 19:03:54.000000 weather_rp5-1.0.1/weather_rp5/cleanup.py
--rw-rw-rw-   0        0        0     3915 2024-04-22 19:06:26.000000 weather_rp5-1.0.1/weather_rp5/downloader.py
--rw-rw-rw-   0        0        0     7544 2024-04-20 18:39:08.000000 weather_rp5-1.0.1/weather_rp5/headers.py
--rw-rw-rw-   0        0        0     4035 2024-04-22 19:06:46.000000 weather_rp5-1.0.1/weather_rp5/main.py
--rw-rw-rw-   0        0        0     3016 2024-04-21 19:12:08.000000 weather_rp5-1.0.1/weather_rp5/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 19:08:59.827643 weather_rp5-1.0.1/weather_rp5.egg-info/
--rw-rw-rw-   0        0        0     1526 2024-04-22 19:08:59.000000 weather_rp5-1.0.1/weather_rp5.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2024-04-22 19:08:59.000000 weather_rp5-1.0.1/weather_rp5.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 19:08:59.000000 weather_rp5-1.0.1/weather_rp5.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-22 19:08:59.000000 weather_rp5-1.0.1/weather_rp5.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 19:47:49.492070 weather_rp5-1.0.2/
+-rw-rw-rw-   0        0        0     1526 2024-04-23 19:47:49.490070 weather_rp5-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1097 2024-04-21 18:50:26.000000 weather_rp5-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 19:47:49.492070 weather_rp5-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-04-23 19:47:37.000000 weather_rp5-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:47:49.426317 weather_rp5-1.0.2/weather_rp5/
+-rw-rw-rw-   0        0        0       50 2024-04-22 18:54:46.000000 weather_rp5-1.0.2/weather_rp5/__init__.py
+-rw-rw-rw-   0        0        0     1975 2024-04-21 19:03:54.000000 weather_rp5-1.0.2/weather_rp5/cleanup.py
+-rw-rw-rw-   0        0        0     3915 2024-04-22 19:06:26.000000 weather_rp5-1.0.2/weather_rp5/downloader.py
+-rw-rw-rw-   0        0        0     7544 2024-04-20 18:39:08.000000 weather_rp5-1.0.2/weather_rp5/headers.py
+-rw-rw-rw-   0        0        0     4027 2024-04-23 19:44:52.000000 weather_rp5-1.0.2/weather_rp5/main.py
+-rw-rw-rw-   0        0        0     2989 2024-04-23 19:45:28.000000 weather_rp5-1.0.2/weather_rp5/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:47:49.488068 weather_rp5-1.0.2/weather_rp5.egg-info/
+-rw-rw-rw-   0        0        0     1526 2024-04-23 19:47:48.000000 weather_rp5-1.0.2/weather_rp5.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2024-04-23 19:47:49.000000 weather_rp5-1.0.2/weather_rp5.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 19:47:48.000000 weather_rp5-1.0.2/weather_rp5.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-23 19:47:49.000000 weather_rp5-1.0.2/weather_rp5.egg-info/top_level.txt
```

### Comparing `weather_rp5-1.0.1/PKG-INFO` & `weather_rp5-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather_rp5
-Version: 1.0.1
+Version: 1.0.2
 Summary: Functions for retrieving weather data from rp5.ru
 Home-page: https://github.com/jakmuell/weather_rp5/
 Author: Jakob Müller
 Author-email: jakob.mueller1004@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `weather_rp5-1.0.1/README.md` & `weather_rp5-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `weather_rp5-1.0.1/setup.py` & `weather_rp5-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='weather_rp5',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     author='Jakob Müller',
     author_email='jakob.mueller1004@gmail.com',
     description='Functions for retrieving weather data from rp5.ru',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jakmuell/weather_rp5/',
```

### Comparing `weather_rp5-1.0.1/weather_rp5/cleanup.py` & `weather_rp5-1.0.2/weather_rp5/cleanup.py`

 * *Files identical despite different names*

### Comparing `weather_rp5-1.0.1/weather_rp5/downloader.py` & `weather_rp5-1.0.2/weather_rp5/downloader.py`

 * *Files identical despite different names*

### Comparing `weather_rp5-1.0.1/weather_rp5/headers.py` & `weather_rp5-1.0.2/weather_rp5/headers.py`

 * *Files identical despite different names*

### Comparing `weather_rp5-1.0.1/weather_rp5/main.py` & `weather_rp5-1.0.2/weather_rp5/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         raise ValueError('End date must be after start date.')
     total_days = (end-start).days
     if total_days <= 180:
         return _get_weather_data_for_short_range(
             station_id, start, end, is_metar)
     num_partial_downloads = ceil(total_days/180)
     start_dates, end_dates = split_time_period(
-        start_date, end_date, num_intervals=num_partial_downloads)
+        start, end, num_intervals=num_partial_downloads)
     df = pd.DataFrame()
     for start_partial, end_partial in zip(start_dates, end_dates):
         df_partial = _get_weather_data_for_short_range(
             station_id, start=start_partial, end=end_partial, is_metar=is_metar
         )
         df = pd.concat([df, df_partial], axis='index')
     return df
@@ -106,7 +106,8 @@
         'https://rp5.ru/Weather_archive_in_Sao_Paulo'
     )
     # wmo_id = 10384
     start_date = date(2024,2,1)
     end_date = date(2024,2,10)
     df = get_weather_data(wmo_id, start_date, end_date, False)
     print(df)
+
```

### Comparing `weather_rp5-1.0.1/weather_rp5/utils.py` & `weather_rp5-1.0.2/weather_rp5/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,10 +85,9 @@
         start = start_date + timedelta(days=interval_days * i)
         start_dates.append(start)
         if i == num_intervals - 1:
             end = end_date
         else:
             end = start_date + timedelta(days=interval_days * (i + 1) - 1)
         end_dates.append(end)
-        print(start, end)
 
     return start_dates, end_dates
```

### Comparing `weather_rp5-1.0.1/weather_rp5.egg-info/PKG-INFO` & `weather_rp5-1.0.2/weather_rp5.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather_rp5
-Version: 1.0.1
+Version: 1.0.2
 Summary: Functions for retrieving weather data from rp5.ru
 Home-page: https://github.com/jakmuell/weather_rp5/
 Author: Jakob Müller
 Author-email: jakob.mueller1004@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

