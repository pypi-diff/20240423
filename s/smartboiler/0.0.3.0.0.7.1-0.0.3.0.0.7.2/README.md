# Comparing `tmp/smartboiler-0.0.3.0.0.7.1.tar.gz` & `tmp/smartboiler-0.0.3.0.0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.0.3.0.0.7.1.tar", last modified: Tue Apr 23 15:58:26 2024, max compression
+gzip compressed data, was "smartboiler-0.0.3.0.0.7.2.tar", last modified: Tue Apr 23 19:24:11 2024, max compression
```

## Comparing `smartboiler-0.0.3.0.0.7.1.tar` & `smartboiler-0.0.3.0.0.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:58:26.621552 smartboiler-0.0.3.0.0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-23 15:58:26.621552 smartboiler-0.0.3.0.0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:58:26.621552 smartboiler-0.0.3.0.0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-23 15:58:26.000000 smartboiler-0.0.3.0.0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:58:26.621552 smartboiler-0.0.3.0.0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:58:26.621552 smartboiler-0.0.3.0.0.7.1/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/retrieve_hass.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/time_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-23 15:58:24.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler/week_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:58:26.621552 smartboiler-0.0.3.0.0.7.1/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-23 15:58:26.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 15:58:26.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:58:26.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 15:58:26.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 15:58:26.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 15:58:26.000000 smartboiler-0.0.3.0.0.7.1/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:24:11.660982 smartboiler-0.0.3.0.0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-23 19:24:11.660982 smartboiler-0.0.3.0.0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:24:11.660982 smartboiler-0.0.3.0.0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-23 19:24:09.000000 smartboiler-0.0.3.0.0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:24:11.656982 smartboiler-0.0.3.0.0.7.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:24:11.660982 smartboiler-0.0.3.0.0.7.2/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13097 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/retrieve_hass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/time_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-23 19:24:08.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler/week_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:24:11.660982 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:24:11.000000 smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.0.3.0.0.7.1/PKG-INFO` & `smartboiler-0.0.3.0.0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.7.1
+Version: 0.0.3.0.0.7.2
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.7.1/README.md` & `smartboiler-0.0.3.0.0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.1/setup.py` & `smartboiler-0.0.3.0.0.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='smartboiler',  # Required
-    version='0.0.3.0.0.7.1',  # Required
+    version='0.0.3.0.0.7.2',  # Required
     description='Smart boiling of household',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/grinwi/smartboiler',  # Optional
     author='Adam GRUNWALD',  # Optional
     author_email='grunwald.adam24@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler/boiler.py` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler/controller.py` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,28 +23,21 @@
 
 from datetime import datetime, timedelta
 import pandas as pd
 import calendar
 from influxdb import DataFrameClient
 from influxdb import InfluxDBClient
 import os.path
-import signal
-import sys
+
 import argparse
 import logging
 import time
 import os
 
 import json
-import requests
-
-
-from distutils.util import strtobool
-from scipy.misc import electrocardiogram
-import numpy as np
 
 
 from smartboiler.data_handler import DataHandler
 from smartboiler.fotovoltaics import Fotovoltaics
 from smartboiler.forecast import Forecast
 from smartboiler.boiler import Boiler
 
@@ -216,32 +209,15 @@
                 return
         # TODO event checker for holidays
 
 
 if __name__ == "__main__":
     logging.info("Starting SmartBoiler Controller")
 
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "--url",
-        type=str,
-        help="The URL to your Home Assistant instance, ex the external_url in your hass configuration",
-    )
-    parser.add_argument(
-        "--key",
-        type=str,
-        help="Your access key. If using EMHASS in standalone this should be a Long-Lived Access Token",
-    )
-    parser.add_argument(
-        "--addon",
-        type=strtobool,
-        default="False",
-        help="Define if we are usinng EMHASS with the add-on or in standalone mode",
-    )
-    args = parser.parse_args()
+
 
     OPTIONS_PATH = os.getenv("OPTIONS_PATH", default="/app/options.json")
     options_json = Path(OPTIONS_PATH)
 
     # Read options info
     if options_json.exists():
         with options_json.open("r") as data:
```

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler/data_handler.py` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler/event_checker.py` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler/forecast.py` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler/fotovoltaics.py` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler/retrieve_hass.py` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler/retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler/switch.py` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler/time_handler.py` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler/week_planner.py` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler/week_planner.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.7.1
+Version: 0.0.3.0.0.7.2
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `smartboiler-0.0.3.0.0.7.1/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.0.3.0.0.7.2/src/smartboiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

