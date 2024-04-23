# Comparing `tmp/tiegcmpy-1.2.6.tar.gz` & `tmp/tiegcmpy-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiegcmpy-1.2.6.tar", last modified: Thu Apr  4 15:16:39 2024, max compression
+gzip compressed data, was "tiegcmpy-1.2.7.tar", last modified: Tue Apr 23 17:14:56 2024, max compression
```

## Comparing `tiegcmpy-1.2.6.tar` & `tiegcmpy-1.2.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-04 15:16:39.242557 tiegcmpy-1.2.6/
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16517 2024-04-04 15:16:39.241600 tiegcmpy-1.2.6/PKG-INFO
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16164 2023-12-19 19:29:40.000000 tiegcmpy-1.2.6/README.md
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)       38 2024-04-04 15:16:39.242705 tiegcmpy-1.2.6/setup.cfg
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      810 2024-04-04 15:12:35.000000 tiegcmpy-1.2.6/setup.py
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-04 15:16:39.165096 tiegcmpy-1.2.6/src/
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-04 15:16:39.233253 tiegcmpy-1.2.6/src/tiegcmpy/
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      280 2023-12-19 18:21:34.000000 tiegcmpy-1.2.6/src/tiegcmpy/__init__.py
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)     1984 2023-10-18 21:02:51.000000 tiegcmpy-1.2.6/src/tiegcmpy/convert_units.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    42106 2023-12-06 02:37:57.000000 tiegcmpy-1.2.6/src/tiegcmpy/data_parse copy.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    50121 2024-03-22 14:36:32.000000 tiegcmpy-1.2.6/src/tiegcmpy/data_parse.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    43845 2023-12-04 20:38:48.000000 tiegcmpy-1.2.6/src/tiegcmpy/data_parse_old.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    16097 2023-12-19 20:29:36.000000 tiegcmpy-1.2.6/src/tiegcmpy/getoptions.py
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      683 2023-12-19 18:20:02.000000 tiegcmpy-1.2.6/src/tiegcmpy/io.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)     7391 2023-12-19 20:00:08.000000 tiegcmpy-1.2.6/src/tiegcmpy/main.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    35239 2023-12-05 15:26:08.000000 tiegcmpy-1.2.6/src/tiegcmpy/plot_gen copy.py
--rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    41531 2024-04-01 19:34:33.000000 tiegcmpy-1.2.6/src/tiegcmpy/plot_gen.py
-drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-04 15:16:39.240961 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16517 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/PKG-INFO
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)      503 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)        1 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)       86 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/entry_points.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)       32 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/requires.txt
--rw-r--r--   0 nikhilr  (42271) ncar      (1000)        9 2024-04-04 15:16:38.000000 tiegcmpy-1.2.6/src/tiegcmpy.egg-info/top_level.txt
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-23 17:14:56.166971 tiegcmpy-1.2.7/
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16517 2024-04-23 17:14:56.166030 tiegcmpy-1.2.7/PKG-INFO
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16164 2023-12-19 19:29:40.000000 tiegcmpy-1.2.7/README.md
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)       38 2024-04-23 17:14:56.167057 tiegcmpy-1.2.7/setup.cfg
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      810 2024-04-23 17:13:28.000000 tiegcmpy-1.2.7/setup.py
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-23 17:14:54.035626 tiegcmpy-1.2.7/src/
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-23 17:14:56.097859 tiegcmpy-1.2.7/src/tiegcmpy/
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      280 2023-12-19 18:21:34.000000 tiegcmpy-1.2.7/src/tiegcmpy/__init__.py
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)     1984 2023-10-18 21:02:51.000000 tiegcmpy-1.2.7/src/tiegcmpy/convert_units.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    42106 2023-12-06 02:37:57.000000 tiegcmpy-1.2.7/src/tiegcmpy/data_parse copy.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    51281 2024-04-21 22:58:17.000000 tiegcmpy-1.2.7/src/tiegcmpy/data_parse.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    43845 2023-12-04 20:38:48.000000 tiegcmpy-1.2.7/src/tiegcmpy/data_parse_old.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    16097 2023-12-19 20:29:36.000000 tiegcmpy-1.2.7/src/tiegcmpy/getoptions.py
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      683 2023-12-19 18:20:02.000000 tiegcmpy-1.2.7/src/tiegcmpy/io.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)     7391 2023-12-19 20:00:08.000000 tiegcmpy-1.2.7/src/tiegcmpy/main.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    35239 2023-12-05 15:26:08.000000 tiegcmpy-1.2.7/src/tiegcmpy/plot_gen copy.py
+-rwxr-xr-x   0 nikhilr  (42271) ncar      (1000)    45099 2024-04-23 13:59:20.000000 tiegcmpy-1.2.7/src/tiegcmpy/plot_gen.py
+drwxr-xr-x   0 nikhilr  (42271) ncar      (1000)        0 2024-04-23 17:14:56.165511 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)    16517 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)      503 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)        1 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)       86 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/entry_points.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)       32 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/requires.txt
+-rw-r--r--   0 nikhilr  (42271) ncar      (1000)        9 2024-04-23 17:14:52.000000 tiegcmpy-1.2.7/src/tiegcmpy.egg-info/top_level.txt
```

### Comparing `tiegcmpy-1.2.6/PKG-INFO` & `tiegcmpy-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiegcmpy
-Version: 1.2.6
+Version: 1.2.7
 Summary: A Python3 post processing tool for TIE-GCM
 Home-page: https://github.com/NCAR/tiegcm
 Author: Nikhil Rao
 Author-email: nikhilr@ucar.edu
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: cartopy
```

### Comparing `tiegcmpy-1.2.6/README.md` & `tiegcmpy-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.6/setup.py` & `tiegcmpy-1.2.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='tiegcmpy',
-    version='1.2.6',
+    version='1.2.7',
     author = "Nikhil Rao",
     author_email = "nikhilr@ucar.edu",
     description='A Python3 post processing tool for TIE-GCM',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/NCAR/tiegcm', 
     python_requires='>=3.8',
```

### Comparing `tiegcmpy-1.2.6/src/tiegcmpy/convert_units.py` & `tiegcmpy-1.2.7/src/tiegcmpy/convert_units.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.6/src/tiegcmpy/data_parse copy.py` & `tiegcmpy-1.2.7/src/tiegcmpy/data_parse copy.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.6/src/tiegcmpy/data_parse.py` & `tiegcmpy-1.2.7/src/tiegcmpy/data_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,16 @@
         - selected_mtime (array): Model time array corresponding to the specified time.
         - filename (str): The name of the dataset file from which data is extracted.
     """
     for ds, filenames in datasets:
         if time in ds['time'].values:
             # Extract variable attributes
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
             selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
             selected_mtime = get_mtime(ds,time)
             filename = filenames
             data = ds[variable_name].sel(time=time)
 
             not_all_nan_indices = ~np.isnan(data.values).all(axis=1)
@@ -164,14 +166,16 @@
         time = np.datetime64(time, 'ns')
 
     # Iterate over datasets to find the matching time and extract relevant data
     for ds, filenames in datasets:
         if time in ds['time'].values:
             # Extracting variable attributes and time information
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
             selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
             selected_mtime = get_mtime(ds,time)
             filename = filenames
             # Data selection based on latitude
             if selected_lat == "mean":
                 # Averaging over all latitudes
@@ -245,14 +249,16 @@
             if time in ds['time'].values:
                 if 'lev' not in ds[variable_name].dims:
                     raise ValueError("The variable "+variable_name+" doesn't use the dimensions 'lat', 'lon', 'lev'")
                     return 0
 
                 # Extract variable attributes
                 variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+                if variable_unit == 'cm/s' and selected_unit == None:
+                    selected_unit = 'm/s'
                 variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
                 selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
                 selected_mtime = get_mtime(ds,time)
                 filename = filenames
 
 
                 if selected_lev_ilev == "mean":
@@ -323,14 +329,16 @@
             if time in ds['time'].values:
                 if 'ilev' not in ds[variable_name].dims:
                     raise ValueError("The variable "+variable_name+" doesn't use the dimensions 'lat', 'lon', 'ilev'")
                     return 0
                             
                 # Extract variable attributes
                 variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+                if variable_unit == 'cm/s' and selected_unit == None:
+                    selected_unit = 'm/s'
                 variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
                 selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
                 selected_mtime=get_mtime(ds,time)
                 filename = filenames
 
                 if selected_lev_ilev == "mean":
                     # if selected_lon is "mean", then we calculate the mean over all longitudes.
@@ -400,14 +408,16 @@
         elif lev_ilev == None:
             first_pass == False
             selected_lev_ilev = None
             if time in ds['time'].values:
 
                 # Extract variable attributes
                 variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+                if variable_unit == 'cm/s' and selected_unit == None:
+                    selected_unit = 'm/s'
                 variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
                 selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
                 selected_mtime = get_mtime(ds,time)
                 filename = filenames
 
                 # Extract the data for the given time and lev
                 data = ds[variable_name].sel(time=time)
@@ -463,14 +473,16 @@
             elif selected_lat == "mean":
                 data = ds[variable_name].sel(time=time, lon=selected_lon).mean(dim='lat')
             else:
                 data = ds[variable_name].sel(time=time, lat=selected_lat, lon=selected_lon, method="nearest")
 
 
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
             selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
             selected_mtime=get_mtime(ds,time)
             filename = filenames
             valid_indices = ~np.isnan(data.values)
             variable_values = data.values[valid_indices]
             if selected_unit != None:
@@ -516,14 +528,16 @@
     """
     if isinstance(time, str):
         time = np.datetime64(time, 'ns')
     for ds, filenames in datasets:
         if time in ds['time'].values:
             # Extract variable attributes
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
             selected_ut = ds['ut'].sel(time=time).values.item() / (1e9 * 3600)
             selected_mtime = get_mtime(ds,time)
             filename = filenames
             if selected_lon == "mean":
                 # if selected_lon is "mean", then we calculate the mean over all longitudes.
                 data = ds[variable_name].sel(time=time).mean(dim='lon')
@@ -582,14 +596,16 @@
             selected_lon = -180
     variable_values_all = []
     combined_mtime = []
     levs_ilevs_all = []
     avg_info_print = 0
     for ds, filenames in datasets:
         variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+        if variable_unit == 'cm/s' and selected_unit == None:
+            selected_unit = 'm/s'
         variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
         mtime_values = ds['mtime'].values
         if selected_lon == "mean" and selected_lat == "mean":
             # if selected_lon is "mean", then we calculate the mean over all longitudes. This doesn't work fix
             data = ds[variable_name].mean(dim=['lon', 'lat'])
             variable_values = data.T 
         elif selected_lon == "mean":
@@ -699,14 +715,16 @@
             lev_ilev = check_var_dims(ds, variable_name)
         if lev_ilev == 'lev':
             first_pass == False            
             if 'lev' not in ds[variable_name].dims:
                 raise ValueError("The variable "+variable_name+" doesn't use the dimensions 'lat', 'lon', 'lev'")
                 return 0
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
             mtime_values = ds['mtime'].values
             filename = filenames
             if selected_lon == 'mean' and selected_lev_ilev == 'mean':
                 data = ds[variable_name].sel(method='nearest').mean(dim=['lev', 'lon'])
                 variable_values = data.T 
                 lats = data.lat.values    
@@ -765,14 +783,16 @@
         elif lev_ilev == 'ilev':
             first_pass == False
             avg_info_print = 0
             if 'ilev' not in ds[variable_name].dims:
                 raise ValueError("The variable "+variable_name+" doesn't use the dimensions 'lat', 'lon', 'ilev'")
                 return 0
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
             mtime_values = ds['mtime'].values
             filename = filenames
             
             if selected_lon == 'mean' and selected_lev_ilev == 'mean':
                 data = ds[variable_name].sel(method='nearest').mean(dim=['ilev', 'lon'])
                 variable_values = data.T 
@@ -833,14 +853,16 @@
 
         elif lev_ilev == None:
             first_pass == False
             selected_lev_ilev = None
 
             avg_info_print = 0
             variable_unit = ds[variable_name].attrs.get('units', 'N/A')
+            if variable_unit == 'cm/s' and selected_unit == None:
+                selected_unit = 'm/s'
             variable_long_name = ds[variable_name].attrs.get('long_name', 'N/A')
             mtime_values = ds['mtime'].values
             filename = filenames
 
             if selected_lon =='mean':
                 data = ds[variable_name].sel(method='nearest').mean(dim='lon')
                 variable_values = data.T
```

### Comparing `tiegcmpy-1.2.6/src/tiegcmpy/data_parse_old.py` & `tiegcmpy-1.2.7/src/tiegcmpy/data_parse_old.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.6/src/tiegcmpy/getoptions.py` & `tiegcmpy-1.2.7/src/tiegcmpy/getoptions.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.6/src/tiegcmpy/io.py` & `tiegcmpy-1.2.7/src/tiegcmpy/io.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.6/src/tiegcmpy/main.py` & `tiegcmpy-1.2.7/src/tiegcmpy/main.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.6/src/tiegcmpy/plot_gen copy.py` & `tiegcmpy-1.2.7/src/tiegcmpy/plot_gen copy.py`

 * *Files identical despite different names*

### Comparing `tiegcmpy-1.2.6/src/tiegcmpy/plot_gen.py` & `tiegcmpy-1.2.7/src/tiegcmpy/plot_gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import matplotlib.pyplot as plt
 from .data_parse import arr_lat_lon,arr_lev_var,arr_lev_lon, arr_lev_lat,arr_lev_time,arr_lat_time, calc_avg_ht, min_max, get_time
 import cartopy.crs as ccrs
 import cartopy.feature as cfeature
 from cartopy.feature.nightshade import Nightshade
 from datetime import datetime, timezone
 import matplotlib.ticker as mticker
-
+import math
 
 def longitude_to_local_time(longitude):
     """
     Convert longitude to local time.
     
     Parameters:
         - longitude (float): Longitude value.
@@ -119,15 +119,15 @@
     ax.set_xticks([value for value in unique_lons if value % 30 == 0], crs=ccrs.PlateCarree())  # Adjust the range and step as per your data
     ax.set_yticks(range(-90, 91, 30), crs=ccrs.PlateCarree())   # Adjust the range and step as per your data
 
     plt.show()
 
     return fig
 
-def plt_lat_lon(datasets, variable_name, time= None, mtime=None, level = None,  variable_unit = None, contour_intervals = None, contour_value = None, cmap_color = None, line_color = 'white', coastlines=False, nightshade=False, gm_equator=False, latitude_minimum = None, latitude_maximum = None, longitude_minimum = None, longitude_maximum = None, localtime_minimum = None, localtime_maximum = None ):
+def plt_lat_lon(datasets, variable_name, time= None, mtime=None, level = None,  variable_unit = None, contour_intervals = None, contour_value = None,symmetric_interval= False, cmap_color = None, line_color = 'white', coastlines=False, nightshade=False, gm_equator=False, latitude_minimum = None, latitude_maximum = None, longitude_minimum = None, longitude_maximum = None, localtime_minimum = None, localtime_maximum = None ):
 
     """
     Generates a Latitude vs Longitude contour plot for a variable.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
         variable_name (str): The name of the variable with latitude, longitude, ilev dimensions.
@@ -173,38 +173,51 @@
             avg_ht=calc_avg_ht(datasets, time,level)
     else:
         data, unique_lats, unique_lons, variable_unit, variable_long_name, selected_ut, selected_mtime, filename =lat_lon(datasets, variable_name, time)
     '''
     if isinstance(time, str):
         time = np.datetime64(time, 'ns')
 
-    data, level,  unique_lats, unique_lons, variable_unit, variable_long_name, selected_ut, selected_mtime, filename =arr_lat_lon(datasets, variable_name, time, selected_lev_ilev = level, selected_unit = variable_unit, plot_mode = True)
+    variable_values, level,  unique_lats, unique_lons, variable_unit, variable_long_name, selected_ut, selected_mtime, filename =arr_lat_lon(datasets, variable_name, time, selected_lev_ilev = level, selected_unit = variable_unit, plot_mode = True)
     if level != 'mean' and level != None:
             avg_ht=calc_avg_ht(datasets, time,level)
     if latitude_minimum == None:
         latitude_minimum = np.nanmin(unique_lats)
     if latitude_maximum == None:
         latitude_maximum = np.nanmax(unique_lats)
     if longitude_minimum == None:
         longitude_minimum = np.nanmin(unique_lons)
     if longitude_maximum == None:   
         longitude_maximum = np.nanmax(unique_lons)
 
-    min_val, max_val = min_max(data)
+    min_val, max_val = min_max(variable_values)
     selected_day=selected_mtime[0]
     selected_hour=selected_mtime[1]
     selected_min=selected_mtime[2]
 
     if cmap_color == None:
         cmap_color, line_color = color_scheme(variable_name)
     # Extract values, latitudes, and longitudes from the array
     if contour_value is not None:
         contour_levels = np.arange(min_val, max_val + contour_value, contour_value)
-    else:
+        interval_value = contour_value
+    elif symmetric_interval == False:
         contour_levels = np.linspace(min_val, max_val, contour_intervals)
+        interval_value = (max_val - min_val) / (contour_intervals - 1)
+    elif symmetric_interval == True:
+        range_half = math.ceil(max(abs(min_val), abs(max_val))/10)*10
+        interval_value = range_half / (contour_intervals // 2)  # Divide by 2 to get intervals for one side
+        positive_levels = np.arange(interval_value, range_half + interval_value, interval_value)
+        negative_levels = -np.flip(positive_levels)  # Generate negative levels symmetrically
+        contour_levels = np.concatenate((negative_levels, [0], positive_levels))
+    if -180 in unique_lons:
+        lon_idx = np.where(unique_lons == -180)[0][-1]  # Get the index of the last occurrence of -180
+        unique_lons = np.append(unique_lons, 180)
+        variable_values = np.insert(variable_values, -1, variable_values[:, lon_idx], axis=1)
+
     # Generate contour plot
     
     interval_value = contour_value if contour_value else (max_val - min_val) / (contour_intervals - 1)
 
     # Generate contour plot
     plot = plt.figure(figsize=(20, 9))
 
@@ -219,16 +232,16 @@
         ax.add_feature(cfeature.COASTLINE, edgecolor=line_color, linewidth=3)
     if nightshade:
         ax.add_feature(Nightshade(datetime.fromtimestamp(time.astype('O')/1e9, tz=timezone.utc), alpha=0.4))
     if gm_equator:
         ax.plot(unique_lons, [0]*len(unique_lons), color=line_color, linestyle='--', transform=ccrs.Geodetic())
     
     
-    contour_filled = plt.contourf(unique_lons, unique_lats, data, cmap=cmap_color, levels=contour_levels)
-    contour_lines = plt.contour(unique_lons, unique_lats, data, colors=line_color, linewidths=0.5, levels=contour_levels)
+    contour_filled = plt.contourf(unique_lons, unique_lats, variable_values, cmap=cmap_color, levels=contour_levels)
+    contour_lines = plt.contour(unique_lons, unique_lats, variable_values, colors=line_color, linewidths=0.5, levels=contour_levels)
     plt.clabel(contour_lines, inline=True, fontsize=16, colors=line_color)
     cbar = plt.colorbar(contour_filled, label=variable_name + " [" + variable_unit + "]",fraction=0.046, pad=0.04)
     cbar.set_label(variable_name + " [" + variable_unit + "]", size=28, labelpad=15)
     cbar.ax.tick_params(labelsize=18)
     
     
     plt.xlabel('Longitude (Deg)', fontsize=28)
@@ -326,29 +339,29 @@
     plt.title(variable_long_name+' '+variable_name+' ('+variable_unit+') '+'\n\n',fontsize=36 )   
 
     plt.ylim(level_minimum, level_maximum)
 
 
 
     if longitude == 'mean' and latitude == 'mean':
-        plt.text(0.5, 1.08,'UT='+str(selected_ut) +"  LAT= Mean SLT= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'UT='+str(selected_ut) +"  LAT= Mean LON= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     elif longitude == 'mean':
-        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT='+str(latitude)+" SLT= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT='+str(latitude)+" LON= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     elif latitude == 'mean':
-        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT= Mean'+" SLT="+str(longitude_to_local_time(longitude))+"Hrs", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT= Mean'+" LON="+str(longitude), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     else:
-        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT='+str(latitude)+" SLT="+str(longitude_to_local_time(longitude))+"Hrs", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'UT='+str(selected_ut) +'  LAT='+str(latitude)+" LON="+str(longitude), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     plt.text(0.5, -0.2, "Min, Max = "+str("{:.2e}".format(min_val))+", "+str("{:.2e}".format(max_val)), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     plt.text(0.5, -0.25, "Day, Hour, Min = "+str(selected_day)+","+str(selected_hour)+","+str(selected_min), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
     plt.text(0.5, -0.3, str(filename), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
 
     return(plot)
 
 
-def plt_lev_lon(datasets, variable_name, latitude, time= None, mtime=None, variable_unit = None, contour_intervals = 20, contour_value = None, cmap_color = None, line_color = 'white',  level_minimum = None, level_maximum = None, longitude_minimum = None, longitude_maximum = None, localtime_minimum = None, localtime_maximum = None):
+def plt_lev_lon(datasets, variable_name, latitude, time= None, mtime=None, variable_unit = None, contour_intervals = 20, contour_value = None,symmetric_interval= False, cmap_color = None, line_color = 'white',  level_minimum = None, level_maximum = None, longitude_minimum = None, longitude_maximum = None, localtime_minimum = None, localtime_maximum = None):
     """
     Generates a Level vs Longitude contour plot for a given latitude.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
         variable_name (str): The name of the variable with latitude, longitude, and ilev dimensions.
         latitude (float): The specific latitude value for the plot.
@@ -397,21 +410,30 @@
     selected_min=selected_mtime[2]
 
     if cmap_color == None:
         cmap_color, line_color = color_scheme(variable_name)
 
     if contour_value is not None:
         contour_levels = np.arange(min_val, max_val + contour_value, contour_value)
-    else:
+        interval_value = contour_value
+    elif symmetric_interval == False:
         contour_levels = np.linspace(min_val, max_val, contour_intervals)
-    # Generate contour plot
-    
-    interval_value = contour_value if contour_value else (max_val - min_val) / (contour_intervals - 1)
-
+        interval_value = (max_val - min_val) / (contour_intervals - 1)
+    elif symmetric_interval == True:
+        range_half = math.ceil(max(abs(min_val), abs(max_val))/10)*10
+        interval_value = range_half / (contour_intervals // 2)  # Divide by 2 to get intervals for one side
+        positive_levels = np.arange(interval_value, range_half + interval_value, interval_value)
+        negative_levels = -np.flip(positive_levels)  # Generate negative levels symmetrically
+        contour_levels = np.concatenate((negative_levels, [0], positive_levels))
+    if -180 in unique_lons:
+        lon_idx = np.where(unique_lons == -180)[0][-1]  # Get the index of the last occurrence of -180
+        unique_lons = np.append(unique_lons, 180)
+        variable_values = np.insert(variable_values, -1, variable_values[:, lon_idx], axis=1)
 
+    # Generate contour plot   
     plot=plt.figure(figsize=(24, 12))
     contour_filled = plt.contourf(unique_lons, unique_levs, variable_values, cmap= cmap_color, levels=contour_levels)
     contour_lines = plt.contour(unique_lons, unique_levs, variable_values, colors=line_color, linewidths=0.5, levels=contour_levels)
     plt.clabel(contour_lines, inline=True, fontsize=16, colors=line_color)
     cbar = plt.colorbar(contour_filled, label=variable_name+" ["+variable_unit+"]")
     cbar.set_label(variable_name+" ["+variable_unit+"]", size=28, labelpad=15)
     cbar.ax.tick_params(labelsize=18)
@@ -446,15 +468,15 @@
     #plot, ax = plt.subplots()
 
     
     
     return(plot)
 
 
-def plt_lev_lat(datasets, variable_name, time= None, mtime=None, longitude = None, localtime = None, variable_unit = None, contour_intervals = 20, contour_value = None, cmap_color = None, line_color = 'white', level_minimum = None, level_maximum = None, latitude_minimum = None,latitude_maximum = None):
+def plt_lev_lat(datasets, variable_name, time= None, mtime=None, longitude = None, localtime = None, variable_unit = None, contour_intervals = 20, contour_value = None,symmetric_interval= False, cmap_color = None, line_color = 'white', level_minimum = None, level_maximum = None, latitude_minimum = None,latitude_maximum = None):
     """
     Generates a Level vs Latitude contour plot for a specified time and/or longitude.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
         variable_name (str): The name of the variable with latitude, longitude, and ilev dimensions.
         time (np.datetime64, optional): The selected time, e.g., '2022-01-01T12:00:00'.
@@ -500,16 +522,25 @@
     selected_min=selected_mtime[2]
 
     if cmap_color == None:
         cmap_color, line_color = color_scheme(variable_name)
 
     if contour_value is not None:
         contour_levels = np.arange(min_val, max_val + contour_value, contour_value)
-    else:
+        interval_value = contour_value
+    elif symmetric_interval == False:
         contour_levels = np.linspace(min_val, max_val, contour_intervals)
+        interval_value = (max_val - min_val) / (contour_intervals - 1)
+    elif symmetric_interval == True:
+        range_half = math.ceil(max(abs(min_val), abs(max_val))/10)*10
+        interval_value = range_half / (contour_intervals // 2)  # Divide by 2 to get intervals for one side
+        positive_levels = np.arange(interval_value, range_half + interval_value, interval_value)
+        negative_levels = -np.flip(positive_levels)  # Generate negative levels symmetrically
+        contour_levels = np.concatenate((negative_levels, [0], positive_levels))
+
     
     
     interval_value = contour_value if contour_value else (max_val - min_val) / (contour_intervals - 1)
     
     # Generate contour plot
     plot=plt.figure(figsize=(24, 12))
     contour_filled = plt.contourf(unique_lats, unique_levs, variable_values, cmap= cmap_color, levels=contour_levels)
@@ -542,15 +573,15 @@
     
     
     return(plot)
 
 
 
 
-def plt_lev_time(datasets, variable_name, latitude, longitude = None, localtime = None, variable_unit = None, contour_intervals = 10, contour_value = None, cmap_color = None, line_color = 'white',  level_minimum = None, level_maximum = None, mtime_minimum=None, mtime_maximum=None):
+def plt_lev_time(datasets, variable_name, latitude, longitude = None, localtime = None, variable_unit = None, contour_intervals = 10, contour_value = None,symmetric_interval= False, cmap_color = None, line_color = 'white',  level_minimum = None, level_maximum = None, mtime_minimum=None, mtime_maximum=None):
     """
     Generates a Level vs Time contour plot for a specified latitude and/or longitude.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
         variable_name (str): The name of the variable with latitude, longitude, time, and ilev dimensions.
         latitude (float): The specific latitude value for the plot.
@@ -606,16 +637,25 @@
     min_val, max_val = np.nanmin(variable_values_all), np.nanmax(variable_values_all)
 
     if cmap_color == None:
         cmap_color, line_color = color_scheme(variable_name)
 
     if contour_value is not None:
         contour_levels = np.arange(min_val, max_val + contour_value, contour_value)
-    else:
+        interval_value = contour_value
+    elif symmetric_interval == False:
         contour_levels = np.linspace(min_val, max_val, contour_intervals)
+        interval_value = (max_val - min_val) / (contour_intervals - 1)
+    elif symmetric_interval == True:
+        range_half = math.ceil(max(abs(min_val), abs(max_val))/10)*10
+        interval_value = range_half / (contour_intervals // 2)  # Divide by 2 to get intervals for one side
+        positive_levels = np.arange(interval_value, range_half + interval_value, interval_value)
+        negative_levels = -np.flip(positive_levels)  # Generate negative levels symmetrically
+        contour_levels = np.concatenate((negative_levels, [0], positive_levels))
+
     
     
     interval_value = contour_value if contour_value else (max_val - min_val) / (contour_intervals - 1)
     mtime_tuples = [tuple(entry) for entry in mtime_values]
     try:    # Modify this part to show both day and hour
         unique_times = sorted(list(set([(day, hour) for day, hour, _, _ in mtime_values])))
         time_indices = [i for i, (day, hour, _, _) in enumerate(mtime_tuples) if i == 0 or mtime_tuples[i-1][:2] != (day, hour)]
@@ -648,29 +688,29 @@
     plt.xticks(fontsize=18)  
     plt.yticks(fontsize=18) 
     plt.ylim(level_minimum,level_maximum)
 
 
     # Add subtext to the plot
     if longitude == 'mean' and latitude == 'mean':
-        plt.text(0.5, 1.08,'  LAT= Mean SLT= Mean', ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'  LAT= Mean LON= Mean', ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     elif longitude == 'mean':
-        plt.text(0.5, 1.08,'  LAT='+str(latitude)+" SLT= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'  LAT='+str(latitude)+" LON= Mean", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     elif latitude == 'mean':
-        plt.text(0.5, 1.08,'  LAT= Mean'+" SLT="+str(longitude_to_local_time(longitude))+"Hrs", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'  LAT= Mean'+" LON="+str(longitude), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     else:
-        plt.text(0.5, 1.08,'  LAT='+str(latitude)+" SLT="+str(longitude_to_local_time(longitude))+"Hrs", ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
+        plt.text(0.5, 1.08,'  LAT='+str(latitude)+" LON="+str(longitude), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes) 
     plt.text(0.5, -0.2, "Min, Max = "+str("{:.2e}".format(min_val))+", "+str("{:.2e}".format(max_val)), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
     plt.text(0.5, -0.25, "Contour Interval = "+str("{:.2e}".format(interval_value)), ha='center', va='center',fontsize=28, transform=plt.gca().transAxes)
 
     return(plot)
 
 
 
-def plt_lat_time(datasets, variable_name, level = None, longitude = None, localtime = None,  variable_unit = None, contour_intervals = 10, contour_value = None, cmap_color = None, line_color = 'white', latitude_minimum = None,latitude_maximum = None, mtime_minimum=None, mtime_maximum=None):
+def plt_lat_time(datasets, variable_name, level = None, longitude = None, localtime = None,  variable_unit = None, contour_intervals = 10, contour_value = None,symmetric_interval= False, cmap_color = None, line_color = 'white', latitude_minimum = None,latitude_maximum = None, mtime_minimum=None, mtime_maximum=None):
     """
     Generates a Latitude vs Time contour plot for a specified level and/or longitude.
     
     Parameters:
         datasets (xarray): The loaded dataset/s using xarray.
         variable_name (str): The name of the variable with latitude, longitude, time, and ilev dimensions.
         level (float): The specific level value for the plot.
@@ -727,16 +767,25 @@
     min_val, max_val = np.nanmin(variable_values_all), np.nanmax(variable_values_all)
     
     if cmap_color == None:
         cmap_color, line_color = color_scheme(variable_name)
 
     if contour_value is not None:
         contour_levels = np.arange(min_val, max_val + contour_value, contour_value)
-    else:
+        interval_value = contour_value
+    elif symmetric_interval == False:
         contour_levels = np.linspace(min_val, max_val, contour_intervals)
+        interval_value = (max_val - min_val) / (contour_intervals - 1)
+    elif symmetric_interval == True:
+        range_half = math.ceil(max(abs(min_val), abs(max_val))/10)*10
+        interval_value = range_half / (contour_intervals // 2)  # Divide by 2 to get intervals for one side
+        positive_levels = np.arange(interval_value, range_half + interval_value, interval_value)
+        negative_levels = -np.flip(positive_levels)  # Generate negative levels symmetrically
+        contour_levels = np.concatenate((negative_levels, [0], positive_levels))
+
     
     interval_value = contour_value if contour_value else (max_val - min_val) / (contour_intervals - 1)
 
     mtime_tuples = [tuple(entry) for entry in mtime_values]
     try:    # Modify this part to show both day and hour
         unique_times = sorted(list(set([(day, hour) for day, hour, _, _ in mtime_values])))
         time_indices = [i for i, (day, hour, _, _) in enumerate(mtime_tuples) if i == 0 or mtime_tuples[i-1][:2] != (day, hour)]
@@ -769,18 +818,18 @@
     plt.tight_layout()
     plt.xticks(fontsize=18)
     plt.yticks(fontsize=18)
     plt.ylim(latitude_minimum, latitude_maximum)
 
     # Add subtext to the plot
     if level == 'mean' and longitude == 'mean':
-        plt.text(0.5, 1.08, '  ZP= Mean SLT= Mean', ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
+        plt.text(0.5, 1.08, '  ZP= Mean LON= Mean', ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     elif longitude == 'mean':
-        plt.text(0.5, 1.08, '  ZP=' + str(level) + " SLT= Mean", ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
+        plt.text(0.5, 1.08, '  ZP=' + str(level) + " LON= Mean", ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     elif level == 'mean':
-        plt.text(0.5, 1.08, '  ZP= Mean' + " SLT=" + str(longitude_to_local_time(longitude)) + "Hrs", ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
+        plt.text(0.5, 1.08, '  ZP= Mean' + " LON=" + str(longitude), ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     else:
-        plt.text(0.5, 1.08, '  ZP=' + str(level) + " SLT=" + str(longitude_to_local_time(longitude)) + "Hrs", ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
+        plt.text(0.5, 1.08, '  ZP=' + str(level) + " LON=" + str(longitude), ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     plt.text(0.5, -0.2, "Min, Max = " + str("{:.2e}".format(min_val)) + ", " + str("{:.2e}".format(max_val)), ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     plt.text(0.5, -0.25, "Contour Interval = " + str("{:.2e}".format(interval_value)), ha='center', va='center', fontsize=28, transform=plt.gca().transAxes)
     plt.close(plot)
     return plot
```

### Comparing `tiegcmpy-1.2.6/src/tiegcmpy.egg-info/PKG-INFO` & `tiegcmpy-1.2.7/src/tiegcmpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiegcmpy
-Version: 1.2.6
+Version: 1.2.7
 Summary: A Python3 post processing tool for TIE-GCM
 Home-page: https://github.com/NCAR/tiegcm
 Author: Nikhil Rao
 Author-email: nikhilr@ucar.edu
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: cartopy
```

