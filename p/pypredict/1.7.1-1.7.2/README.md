# Comparing `tmp/pypredict-1.7.1.tar.gz` & `tmp/pypredict-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypredict-1.7.1.tar", last modified: Fri Aug 11 00:02:21 2023, max compression
+gzip compressed data, was "pypredict-1.7.2.tar", last modified: Tue Apr 23 19:40:03 2024, max compression
```

## Comparing `pypredict-1.7.1.tar` & `pypredict-1.7.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 spire     (1000) spire     (1000)        0 2023-08-11 00:02:21.363198 pypredict-1.7.1/
--rw-rw-r--   0 spire     (1000) spire     (1000)    11237 2023-08-11 00:02:21.363198 pypredict-1.7.1/PKG-INFO
--rw-rw-r--   0 spire     (1000) spire     (1000)     8818 2023-04-11 09:47:19.000000 pypredict-1.7.1/README.md
--rw-rw-r--   0 spire     (1000) spire     (1000)    95417 2021-05-17 23:55:16.000000 pypredict-1.7.1/predict.c
--rw-rw-r--   0 spire     (1000) spire     (1000)    12429 2022-08-19 12:33:35.000000 pypredict-1.7.1/predict.py
-drwxrwxr-x   0 spire     (1000) spire     (1000)        0 2023-08-11 00:02:21.363198 pypredict-1.7.1/pypredict.egg-info/
--rw-rw-r--   0 spire     (1000) spire     (1000)    11237 2023-08-11 00:02:21.000000 pypredict-1.7.1/pypredict.egg-info/PKG-INFO
--rw-rw-r--   0 spire     (1000) spire     (1000)      171 2023-08-11 00:02:21.000000 pypredict-1.7.1/pypredict.egg-info/SOURCES.txt
--rw-rw-r--   0 spire     (1000) spire     (1000)        1 2023-08-11 00:02:21.000000 pypredict-1.7.1/pypredict.egg-info/dependency_links.txt
--rw-rw-r--   0 spire     (1000) spire     (1000)       17 2023-08-11 00:02:21.000000 pypredict-1.7.1/pypredict.egg-info/top_level.txt
--rw-rw-r--   0 spire     (1000) spire     (1000)       38 2023-08-11 00:02:21.363198 pypredict-1.7.1/setup.cfg
--rwxrwxr-x   0 spire     (1000) spire     (1000)     1048 2023-08-10 23:43:27.000000 pypredict-1.7.1/setup.py
+drwxrwxr-x   0 spire     (1000) spire     (1000)        0 2024-04-23 19:40:03.649304 pypredict-1.7.2/
+-rw-rw-r--   0 spire     (1000) spire     (1000)    17990 2024-03-24 22:41:53.000000 pypredict-1.7.2/COPYING
+-rw-rw-r--   0 spire     (1000) spire     (1000)     9608 2024-04-23 19:40:03.649304 pypredict-1.7.2/PKG-INFO
+-rw-rw-r--   0 spire     (1000) spire     (1000)     8818 2024-03-24 22:41:53.000000 pypredict-1.7.2/README.md
+-rw-rw-r--   0 spire     (1000) spire     (1000)    94024 2024-04-23 19:36:46.000000 pypredict-1.7.2/predict.c
+-rw-rw-r--   0 spire     (1000) spire     (1000)    12429 2024-03-24 22:41:53.000000 pypredict-1.7.2/predict.py
+drwxrwxr-x   0 spire     (1000) spire     (1000)        0 2024-04-23 19:40:03.649304 pypredict-1.7.2/pypredict.egg-info/
+-rw-rw-r--   0 spire     (1000) spire     (1000)     9608 2024-04-23 19:40:03.000000 pypredict-1.7.2/pypredict.egg-info/PKG-INFO
+-rw-rw-r--   0 spire     (1000) spire     (1000)      179 2024-04-23 19:40:03.000000 pypredict-1.7.2/pypredict.egg-info/SOURCES.txt
+-rw-rw-r--   0 spire     (1000) spire     (1000)        1 2024-04-23 19:40:03.000000 pypredict-1.7.2/pypredict.egg-info/dependency_links.txt
+-rw-rw-r--   0 spire     (1000) spire     (1000)       17 2024-04-23 19:40:03.000000 pypredict-1.7.2/pypredict.egg-info/top_level.txt
+-rw-rw-r--   0 spire     (1000) spire     (1000)       38 2024-04-23 19:40:03.649304 pypredict-1.7.2/setup.cfg
+-rwxrwxr-x   0 spire     (1000) spire     (1000)     1048 2024-04-23 19:36:46.000000 pypredict-1.7.2/setup.py
```

### Comparing `pypredict-1.7.1/PKG-INFO` & `pypredict-1.7.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,225 +1,228 @@
 Metadata-Version: 2.1
 Name: pypredict
-Version: 1.7.1
+Version: 1.7.2
 Summary: Interface to the Predict satellite tracking and orbital prediction library
 Home-page: https://github.com/nsat/pypredict
 Author: Jesse Trutna
 Author-email: jesse@spire.com
 Maintainer: Spire Global Inc
 Maintainer-email: opensource@spire.com
 License: UNKNOWN
-Description: [![ci](https://github.com/nsat/pypredict/actions/workflows/python-app.yml/badge.svg)](https://github.com/nsat/pypredict/actions/workflows/python-app.yml)
-        
-        PyPredict
-        =======
-        
-        ><b>NOTE</b>: To preserve compatibility with `predict`, pypredict uses __north__ latitude and __west__ longitude for terrestrial coordinates.
-        
-        Do you want accurate and time-tested satellite tracking and pass prediction in a convenient python wrapper?
-        You're in the right place.
-        
-        PyPredict is a C Python extension directly adapted from the ubiquitous [predict](http://www.qsl.net/kd2bd/predict.html) satellite tracking command line application.
-        Originally written for the commodore 64, predict has a proven pedigree; We just aim to provide a convenient API.
-        PyPredict is a port of the predict codebase and should yield identical results.
-        
-        If you think you've found an error in `pypredict`, please include output from `predict` on same inputs to the bug report.  
-        If you think you've found a bug in predict, please report and we'll coordinate with upstream.
-        
-        ### Installation
-        
-        ```bash
-        sudo apt-get install python-dev
-        sudo python setup.py install
-        ```
-        
-        ## Usage
-        
-        #### Observe a satellite (relative to a position on earth)
-        
-        ```python
-        import predict
-        tle = """0 LEMUR 1
-        1 40044U 14033AL  15013.74135905  .00002013  00000-0  31503-3 0  6119
-        2 40044 097.9584 269.2923 0059425 258.2447 101.2095 14.72707190 30443"""
-        qth = (37.771034, 122.413815, 7)  # lat (N), long (W), alt (meters)
-        predict.observe(tle, qth) # optional time argument defaults to time.time()
-        # => {'altitude': 676.8782276657903,
-        #     'azimuth': 96.04762045174824,
-        #     'beta_angle': -27.92735429908726,
-        #     'decayed': 0,
-        #     'doppler': 1259.6041017128405,
-        #     'eci_obs_x': -2438.227652191655,
-        #     'eci_obs_y': -4420.154476060397,
-        #     'eci_obs_z': 3885.390601342013,
-        #     'eci_sun_x': 148633398.020844,
-        #     'eci_sun_y': -7451536.44122029,
-        #     'eci_sun_z': -3229999.50056359,
-        #     'eci_vx': 0.20076213530665032,
-        #     'eci_vy': -1.3282146055077213,
-        #     'eci_vz': 7.377067234096598,
-        #     'eci_x': 6045.827328897242,
-        #     'eci_y': -3540.5885778261277,
-        #     'eci_z': -825.4065096776636,
-        #     'eclipse_depth': -87.61858291647795,
-        #     'elevation': -43.711904591801726,
-        #     'epoch': 1521290038.347793,
-        #     'footprint': 5633.548906707907,
-        #     'geostationary': 0,
-        #     'has_aos': 1,
-        #     'latitude': -6.759563817939698,
-        #     'longitude': 326.1137007912563,
-        #     'name': '0 LEMUR 1',
-        #     'norad_id': 40044,
-        #     'orbit': 20532,
-        #     'orbital_model': 'SGP4',
-        #     'orbital_phase': 145.3256815318047,
-        #     'orbital_velocity': 26994.138671706416,
-        #     'slant_range': 9743.943478523843,
-        #     'sunlit': 1,
-        #     'visibility': 'D'
-        #    }
-        ```
-        
-        #### Show upcoming transits of satellite over ground station
-        
-        ```python
-        # start and stop transit times as UNIX timestamp
-        transit_start = 1680775200
-        transit_stop = 1681034400
-        
-        p = predict.transits(tle, qth, transit_start, transit_stop)
-        
-        print("Start of Transit\tTransit Duration (s)\tPeak Elevation")
-        for transit in p:
-            print(f"{transit.start}\t{transit.duration()}\t{transit.peak()['elevation']}")
-        ```
-        
-        
-        #### Modeling an entire constellation
-        
-        Generating transits for a lot of satellites over a lot of ground stations can be slow.
-        Luckily, generating transits for each satellite-groundstation pair can be parallelized for a big speed-up.
-        
-        ```python
-        import itertools
-        from multiprocessing.pool import Pool
-        import time
-        
-        import predict
-        import requests
-        
-        # Define a function that returns arguments for all the transits() calls you want to make
-        def _transits_call_arguments():
-            now = time.time()
-            tle = requests.get('http://tle.spire.com/25544').text.rstrip()
-            for latitude in range(-90, 91, 15):
-                for longitude in range(-180, 181, 15):
-                    qth = (latitude, longitude, 0)
-                    yield {'tle': tle, 'qth': qth, 'ending_before': now+60*60*24*7}
-        
-        # Define a function that calls the transit function on a set of arguments and does per-transit processing
-        def _transits_call_fx(kwargs):
-            try:
-                transits = list(predict.transits(**kwargs))
-                return [t.above(10) for t in transits]
-            except predict.PredictException:
-                pass
-        
-        # Map the transit() caller across all the arguments you want, then flatten results into a single list
-        pool = Pool(processes=10)
-        array_of_results = pool.map(_transits_call_fx, _transits_call_arguments())
-        flattened_results = list(itertools.chain.from_iterable(filter(None, array_of_results)))
-        transits = flattened_results
-        ```
-        
-        NOTE: If precise accuracy isn't necessary (for modeling purposes, for example) setting the tolerance argument
-              to the `above` call to a larger value, say 1 degree, can provide a significant performance boost.
-        
-        #### Call predict analogs directly
-        
-        ```python
-        predict.quick_find(tle.split('\n'), time.time(), (37.7727, 122.407, 25))
-        predict.quick_predict(tle.split('\n'), time.time(), (37.7727, 122.407, 25))
-        ```
-        
-        ## API
-        <pre>
-        <b>observe</b>(<i>tle, qth[, at=None]</i>)  
-            Return an observation of a satellite relative to a groundstation.
-            <i>qth</i> groundstation coordinates as (lat(N),long(W),alt(m))
-            If <i>at</i> is not defined, defaults to current time (time.time())
-            Returns an "observation" or dictionary containing:  
-                <i>altitude</i> _ altitude of satellite in kilometers
-                <i>azimuth</i> - azimuth of satellite in degrees from perspective of groundstation.
-                <i>beta_angle</i>
-                <i>decayed</i> - 1 if satellite has decayed out of orbit, 0 otherwise.
-                <i>doppler</i> - doppler shift between groundstation and satellite.
-                <i>eci_obs_x</i>
-                <i>eci_obs_y</i>
-                <i>eci_obs_z</i>
-                <i>eci_sun_x</i>
-                <i>eci_sun_y</i>
-                <i>eci_sun_z</i>
-                <i>eci_vx</i>
-                <i>eci_vy</i>
-                <i>eci_vz</i>
-                <i>eci_x</i>
-                <i>eci_y</i>
-                <i>eci_z</i>
-                <i>eclipse_depth</i>
-                <i>elevation</i> - elevation of satellite in degrees from perspective of groundstation.
-                <i>epoch</i> - time of observation in seconds (unix epoch)
-                <i>footprint</i>
-                <i>geostationary</i> - 1 if satellite is determined to be geostationary, 0 otherwise.
-                <i>has_aos</i> - 1 if the satellite will eventually be visible from the groundstation
-                <i>latitude</i> - north latitude of point on earth directly under satellite.
-                <i>longitude</i> - west longitude of point on earth directly under satellite.
-                <i>name</i> - name of satellite from first line of TLE.
-                <i>norad_id</i> - NORAD id of satellite.
-                <i>orbit</i>
-                <i>orbital_phase</i>
-                <i>orbital_model</i>
-                <i>orbital_velocity</i>
-                <i>slant_range</i> - distance to satellite from groundstation in meters.
-                <i>sunlit</i> - 1 if satellite is in sunlight, 0 otherwise.
-                <i>visibility</i>
-        <b>transits</b>(<i>tle, qth[, ending_after=None][, ending_before=None]</i>)  
-            Returns iterator of <b>Transit</b> objects representing passes of tle over qth.  
-            If <i>ending_after</i> is not defined, defaults to current time  
-            If <i>ending_before</i> is not defined, the iterator will yield until calculation failure.
-        </pre>
-        ><b>NOTE</b>: We yield passes based on their end time.  This means we'll yield currently active passes in the two-argument invocation form, but their start times will be in the past.
-        
-        <pre>
-        <b>Transit</b>(<i>tle, qth, start, end</i>)  
-            Utility class representing a pass of a satellite over a groundstation.
-            Instantiation parameters are parsed and made available as fields.
-            <b>duration</b>()  
-                Returns length of transit in seconds
-            <b>peak</b>(<i>epsilon=0.1</i>)  
-                Returns epoch time where transit reaches maximum elevation (within ~<i>epsilon</i>)
-            <b>at</b>(<i>timestamp</i>)  
-                Returns observation during transit via <b>quick_find</b>(<i>tle, timestamp, qth</i>)
-            <b>above</b>b(<i>elevation</i>, <i>tolerance</i>)
-                Returns portion of transit above elevation. If the entire transit is below the target elevation, both
-                endpoints will be set to the peak and the duration will be zero. If a portion of the transit is above
-                the elevation target, the endpoints will be between elevation and elevation + tolerance (unless
-                endpoint is already above elevation, in which case it will be unchanged)
-        <b>quick_find</b>(<i>tle[, time[, (lat, long, alt)]]</i>)  
-            <i>time</i> defaults to current time   
-            <i>(lat, long, alt)</i> defaults to values in ~/.predict/predict.qth  
-            Returns observation dictionary equivalent to observe(tle, time, (lat, long, alt))
-        <b>quick_predict</b>(<i>tle[, time[, (lat, long, alt)]]</i>)  
-                Returns an array of observations for the next pass as calculated by predict.
-                Each observation is identical to that returned by <b>quick_find</b>.
-        </pre>
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: COPYING
+
+[![ci](https://github.com/nsat/pypredict/actions/workflows/python-app.yml/badge.svg)](https://github.com/nsat/pypredict/actions/workflows/python-app.yml)
+
+PyPredict
+=======
+
+><b>NOTE</b>: To preserve compatibility with `predict`, pypredict uses __north__ latitude and __west__ longitude for terrestrial coordinates.
+
+Do you want accurate and time-tested satellite tracking and pass prediction in a convenient python wrapper?
+You're in the right place.
+
+PyPredict is a C Python extension directly adapted from the ubiquitous [predict](http://www.qsl.net/kd2bd/predict.html) satellite tracking command line application.
+Originally written for the commodore 64, predict has a proven pedigree; We just aim to provide a convenient API.
+PyPredict is a port of the predict codebase and should yield identical results.
+
+If you think you've found an error in `pypredict`, please include output from `predict` on same inputs to the bug report.  
+If you think you've found a bug in predict, please report and we'll coordinate with upstream.
+
+### Installation
+
+```bash
+sudo apt-get install python-dev
+sudo python setup.py install
+```
+
+## Usage
+
+#### Observe a satellite (relative to a position on earth)
+
+```python
+import predict
+tle = """0 LEMUR 1
+1 40044U 14033AL  15013.74135905  .00002013  00000-0  31503-3 0  6119
+2 40044 097.9584 269.2923 0059425 258.2447 101.2095 14.72707190 30443"""
+qth = (37.771034, 122.413815, 7)  # lat (N), long (W), alt (meters)
+predict.observe(tle, qth) # optional time argument defaults to time.time()
+# => {'altitude': 676.8782276657903,
+#     'azimuth': 96.04762045174824,
+#     'beta_angle': -27.92735429908726,
+#     'decayed': 0,
+#     'doppler': 1259.6041017128405,
+#     'eci_obs_x': -2438.227652191655,
+#     'eci_obs_y': -4420.154476060397,
+#     'eci_obs_z': 3885.390601342013,
+#     'eci_sun_x': 148633398.020844,
+#     'eci_sun_y': -7451536.44122029,
+#     'eci_sun_z': -3229999.50056359,
+#     'eci_vx': 0.20076213530665032,
+#     'eci_vy': -1.3282146055077213,
+#     'eci_vz': 7.377067234096598,
+#     'eci_x': 6045.827328897242,
+#     'eci_y': -3540.5885778261277,
+#     'eci_z': -825.4065096776636,
+#     'eclipse_depth': -87.61858291647795,
+#     'elevation': -43.711904591801726,
+#     'epoch': 1521290038.347793,
+#     'footprint': 5633.548906707907,
+#     'geostationary': 0,
+#     'has_aos': 1,
+#     'latitude': -6.759563817939698,
+#     'longitude': 326.1137007912563,
+#     'name': '0 LEMUR 1',
+#     'norad_id': 40044,
+#     'orbit': 20532,
+#     'orbital_model': 'SGP4',
+#     'orbital_phase': 145.3256815318047,
+#     'orbital_velocity': 26994.138671706416,
+#     'slant_range': 9743.943478523843,
+#     'sunlit': 1,
+#     'visibility': 'D'
+#    }
+```
+
+#### Show upcoming transits of satellite over ground station
+
+```python
+# start and stop transit times as UNIX timestamp
+transit_start = 1680775200
+transit_stop = 1681034400
+
+p = predict.transits(tle, qth, transit_start, transit_stop)
+
+print("Start of Transit\tTransit Duration (s)\tPeak Elevation")
+for transit in p:
+    print(f"{transit.start}\t{transit.duration()}\t{transit.peak()['elevation']}")
+```
+
+
+#### Modeling an entire constellation
+
+Generating transits for a lot of satellites over a lot of ground stations can be slow.
+Luckily, generating transits for each satellite-groundstation pair can be parallelized for a big speed-up.
+
+```python
+import itertools
+from multiprocessing.pool import Pool
+import time
+
+import predict
+import requests
+
+# Define a function that returns arguments for all the transits() calls you want to make
+def _transits_call_arguments():
+    now = time.time()
+    tle = requests.get('http://tle.spire.com/25544').text.rstrip()
+    for latitude in range(-90, 91, 15):
+        for longitude in range(-180, 181, 15):
+            qth = (latitude, longitude, 0)
+            yield {'tle': tle, 'qth': qth, 'ending_before': now+60*60*24*7}
+
+# Define a function that calls the transit function on a set of arguments and does per-transit processing
+def _transits_call_fx(kwargs):
+    try:
+        transits = list(predict.transits(**kwargs))
+        return [t.above(10) for t in transits]
+    except predict.PredictException:
+        pass
+
+# Map the transit() caller across all the arguments you want, then flatten results into a single list
+pool = Pool(processes=10)
+array_of_results = pool.map(_transits_call_fx, _transits_call_arguments())
+flattened_results = list(itertools.chain.from_iterable(filter(None, array_of_results)))
+transits = flattened_results
+```
+
+NOTE: If precise accuracy isn't necessary (for modeling purposes, for example) setting the tolerance argument
+      to the `above` call to a larger value, say 1 degree, can provide a significant performance boost.
+
+#### Call predict analogs directly
+
+```python
+predict.quick_find(tle.split('\n'), time.time(), (37.7727, 122.407, 25))
+predict.quick_predict(tle.split('\n'), time.time(), (37.7727, 122.407, 25))
+```
+
+## API
+<pre>
+<b>observe</b>(<i>tle, qth[, at=None]</i>)  
+    Return an observation of a satellite relative to a groundstation.
+    <i>qth</i> groundstation coordinates as (lat(N),long(W),alt(m))
+    If <i>at</i> is not defined, defaults to current time (time.time())
+    Returns an "observation" or dictionary containing:  
+        <i>altitude</i> _ altitude of satellite in kilometers
+        <i>azimuth</i> - azimuth of satellite in degrees from perspective of groundstation.
+        <i>beta_angle</i>
+        <i>decayed</i> - 1 if satellite has decayed out of orbit, 0 otherwise.
+        <i>doppler</i> - doppler shift between groundstation and satellite.
+        <i>eci_obs_x</i>
+        <i>eci_obs_y</i>
+        <i>eci_obs_z</i>
+        <i>eci_sun_x</i>
+        <i>eci_sun_y</i>
+        <i>eci_sun_z</i>
+        <i>eci_vx</i>
+        <i>eci_vy</i>
+        <i>eci_vz</i>
+        <i>eci_x</i>
+        <i>eci_y</i>
+        <i>eci_z</i>
+        <i>eclipse_depth</i>
+        <i>elevation</i> - elevation of satellite in degrees from perspective of groundstation.
+        <i>epoch</i> - time of observation in seconds (unix epoch)
+        <i>footprint</i>
+        <i>geostationary</i> - 1 if satellite is determined to be geostationary, 0 otherwise.
+        <i>has_aos</i> - 1 if the satellite will eventually be visible from the groundstation
+        <i>latitude</i> - north latitude of point on earth directly under satellite.
+        <i>longitude</i> - west longitude of point on earth directly under satellite.
+        <i>name</i> - name of satellite from first line of TLE.
+        <i>norad_id</i> - NORAD id of satellite.
+        <i>orbit</i>
+        <i>orbital_phase</i>
+        <i>orbital_model</i>
+        <i>orbital_velocity</i>
+        <i>slant_range</i> - distance to satellite from groundstation in meters.
+        <i>sunlit</i> - 1 if satellite is in sunlight, 0 otherwise.
+        <i>visibility</i>
+<b>transits</b>(<i>tle, qth[, ending_after=None][, ending_before=None]</i>)  
+    Returns iterator of <b>Transit</b> objects representing passes of tle over qth.  
+    If <i>ending_after</i> is not defined, defaults to current time  
+    If <i>ending_before</i> is not defined, the iterator will yield until calculation failure.
+</pre>
+><b>NOTE</b>: We yield passes based on their end time.  This means we'll yield currently active passes in the two-argument invocation form, but their start times will be in the past.
+
+<pre>
+<b>Transit</b>(<i>tle, qth, start, end</i>)  
+    Utility class representing a pass of a satellite over a groundstation.
+    Instantiation parameters are parsed and made available as fields.
+    <b>duration</b>()  
+        Returns length of transit in seconds
+    <b>peak</b>(<i>epsilon=0.1</i>)  
+        Returns epoch time where transit reaches maximum elevation (within ~<i>epsilon</i>)
+    <b>at</b>(<i>timestamp</i>)  
+        Returns observation during transit via <b>quick_find</b>(<i>tle, timestamp, qth</i>)
+    <b>above</b>b(<i>elevation</i>, <i>tolerance</i>)
+        Returns portion of transit above elevation. If the entire transit is below the target elevation, both
+        endpoints will be set to the peak and the duration will be zero. If a portion of the transit is above
+        the elevation target, the endpoints will be between elevation and elevation + tolerance (unless
+        endpoint is already above elevation, in which case it will be unchanged)
+<b>quick_find</b>(<i>tle[, time[, (lat, long, alt)]]</i>)  
+    <i>time</i> defaults to current time   
+    <i>(lat, long, alt)</i> defaults to values in ~/.predict/predict.qth  
+    Returns observation dictionary equivalent to observe(tle, time, (lat, long, alt))
+<b>quick_predict</b>(<i>tle[, time[, (lat, long, alt)]]</i>)  
+        Returns an array of observations for the next pass as calculated by predict.
+        Each observation is identical to that returned by <b>quick_find</b>.
+</pre>
+
+
```

### Comparing `pypredict-1.7.1/README.md` & `pypredict-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pypredict-1.7.1/predict.c` & `pypredict-1.7.2/predict.c`

 * *Files 2% similar despite different names*

```diff
@@ -115,22 +115,14 @@
 #define VISIBLE_FLAG           0x002000
 #define SAT_ECLIPSED_FLAG      0x004000
 
 // Python Extension Globals
 static PyObject *PredictException;
 static PyObject *NoTransitException;
 
-/*
-  TODO: This is a refactoring hack to ensure we get consistent before/after
-        tests.  Freezes the clock to a specified time, making calculations
-        deterministic. (remove when finished along with (2) call sites)
-*/
-char debug_freeze_time = 0;
-struct tm debug_frozen_tm = { tm_year: 114, tm_mon: 10, tm_mday: 2 };
-
 // This struct represents an observation of a particular satellite
 // from a particular reference point (on earth) at a particular time
 // and is used primarily in the PyPredict code.
 typedef struct observation {
 	double epoch;
 	char orbital_model[5];
 	long norad_id;
@@ -171,16 +163,16 @@
 struct	{
 	   char line1[70];       // First line of TLE
 	   char line2[70];       // Second line of TLE
 	   char name[25];        // Spacecraft Name
  	   long catnum;          // Catalog Number (a.k.a NORAD id)
 	   long setnum;          // Element Set No.
 	   char designator[10];  // Designator
- 	   int year;             // Reference Epoch (year?) (?)
-	   double refepoch;      // Reference Epoch (?)
+	   int year;             // Reference Epoch from TLE (2-digit year)
+	   double refepoch;      // Reference Epoch from TLE (day of the year and fractional portion of the day)
 	   double incl;          // Inclination
 	   double raan;          // RAAN
 	   double eccn;          // Eccentricity
 	   double argper;        // Arg of Perigee
 	   double meanan;        // Mean Anomaly
 	   double meanmo;        // Mean Motion
 	   double drag;          // Decay Rate
@@ -2079,21 +2071,14 @@
 	obs_set->x=FMod2p(obs_set->x);
 }
 
 /* .... SGP4/SDP4 functions end .... */
 
 time_t CurrentTime()
 {
-	//TODO: Refactoring Hack (remove)
-	if (debug_freeze_time)
-	{
-		time_t debug_frozen_time = mktime(&debug_frozen_tm);
-		return debug_frozen_time;
-	}
-
 	return time(NULL);
 }
 
 double FixAngle(double x)
 {
 	/* This function reduces angles greater than
 	   two pi by subtracting two pi from the angle */
@@ -2606,72 +2591,26 @@
 	return dn;
 }
 
 double CurrentDaynum()
 {
 	/* Read the system clock and return the number
 	   of days since 31Dec79 00:00:00 UTC (daynum 0) */
-
-	//TODO: Refactoring Hack (remove)
-	if (debug_freeze_time)
-	{
-		time_t debug_frozen_time = mktime(&debug_frozen_tm);
-		return ((((double)debug_frozen_time)/86400.0) - 3651.0);
-	}
-
 	int x;
 	struct timeval tptr;
 	double usecs, seconds;
 
 	x=gettimeofday(&tptr,NULL);
 
 	usecs=0.000001*(double)tptr.tv_usec;
 	seconds=usecs+(double)tptr.tv_sec;
 
 	return ((seconds/86400.0)-3651.0);
 }
 
-char *Daynum2String(daynum)
-double daynum;
-{
-	/* This function takes the given epoch as a fractional number of
-	   days since 31Dec79 00:00:00 UTC and returns the corresponding
-	   date as a string of the form "Tue 12Oct99 17:22:37". */
-
-	char timestr[26];
-	time_t t;
-	int x;
-
-	/* Convert daynum to Unix time (seconds since 01-Jan-70) */
-	t=(time_t)(86400.0*(daynum+3651.0));
-
-	sprintf(timestr,"%s",asctime(gmtime(&t)));
-
-	if (timestr[8]==' ')
-	{
-		timestr[8]='0';
-	}
-
-	for (x=0; x<=3; output[x]=timestr[x], x++);
-
-	output[4]=timestr[8];
-	output[5]=timestr[9];
-	output[6]=timestr[4];
-	output[7]=timestr[5];
-	output[8]=timestr[6];
-	output[9]=timestr[22];
-	output[10]=timestr[23];
-	output[11]=' ';
-
-	for (x=12; x<=19; output[x]=timestr[x-1], x++);
-
-	output[20]=0;
-	return output;
-}
-
 void FindMoon(double daynum)
 {
 	/* This function determines the position of the moon, including
 	   the azimuth and elevation headings, relative to the latitude
 	   and longitude of the tracking station.  This code was derived
 	   from a Javascript implementation of the Meeus method for
 	   determining the exact position of the Moon found at:
@@ -3539,37 +3478,35 @@
 }
 
 static char quick_find_docs[] =
     "quick_find((tle_line0, tle_line1, tle_line2), time, (gs_lat, gs_lon, gs_alt))\n";
 
 static PyObject* quick_predict(PyObject* self, PyObject *args)
 {
-	double now;
+	double tle_epoch;
 	int lastel=0;
 	char errbuff[100];
 	observation obs = { 0 };
 
 	PyObject* transit = PyList_New(0);
 	if (transit == NULL)
 	{
 		goto cleanup_and_raise_exception;
 	}
 
-	now=CurrentDaynum();
-
 	if (load(args) != 0)
 	{
 		// load will set the appropriate exception string if it fails.
 		goto cleanup_and_raise_exception;
 	}
 
-	//TODO: Seems like this should be based on the freshness of the TLE, not wall clock.
-	if ((daynum<now-365.0) || (daynum>now+365.0))
+	tle_epoch=(double)DayNum(1,0,sat.year)+sat.refepoch;
+	if ((daynum<tle_epoch-365.0) || (daynum>tle_epoch+365.0))
 	{
-		sprintf(errbuff, "time %s too far from present\n", Daynum2String(daynum));
+		sprintf(errbuff, "day number %.0f too far from tle epoch day %.0f\n", daynum, tle_epoch);
 		PyErr_SetString(PredictException, errbuff);
 		goto cleanup_and_raise_exception;
 	}
 
 	PreCalc(0);
 	Calc();
 	if (MakeObservation(daynum, &obs) != 0)
```

### Comparing `pypredict-1.7.1/predict.py` & `pypredict-1.7.2/predict.py`

 * *Files identical despite different names*

### Comparing `pypredict-1.7.1/pypredict.egg-info/PKG-INFO` & `pypredict-1.7.2/pypredict.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,225 +1,228 @@
 Metadata-Version: 2.1
 Name: pypredict
-Version: 1.7.1
+Version: 1.7.2
 Summary: Interface to the Predict satellite tracking and orbital prediction library
 Home-page: https://github.com/nsat/pypredict
 Author: Jesse Trutna
 Author-email: jesse@spire.com
 Maintainer: Spire Global Inc
 Maintainer-email: opensource@spire.com
 License: UNKNOWN
-Description: [![ci](https://github.com/nsat/pypredict/actions/workflows/python-app.yml/badge.svg)](https://github.com/nsat/pypredict/actions/workflows/python-app.yml)
-        
-        PyPredict
-        =======
-        
-        ><b>NOTE</b>: To preserve compatibility with `predict`, pypredict uses __north__ latitude and __west__ longitude for terrestrial coordinates.
-        
-        Do you want accurate and time-tested satellite tracking and pass prediction in a convenient python wrapper?
-        You're in the right place.
-        
-        PyPredict is a C Python extension directly adapted from the ubiquitous [predict](http://www.qsl.net/kd2bd/predict.html) satellite tracking command line application.
-        Originally written for the commodore 64, predict has a proven pedigree; We just aim to provide a convenient API.
-        PyPredict is a port of the predict codebase and should yield identical results.
-        
-        If you think you've found an error in `pypredict`, please include output from `predict` on same inputs to the bug report.  
-        If you think you've found a bug in predict, please report and we'll coordinate with upstream.
-        
-        ### Installation
-        
-        ```bash
-        sudo apt-get install python-dev
-        sudo python setup.py install
-        ```
-        
-        ## Usage
-        
-        #### Observe a satellite (relative to a position on earth)
-        
-        ```python
-        import predict
-        tle = """0 LEMUR 1
-        1 40044U 14033AL  15013.74135905  .00002013  00000-0  31503-3 0  6119
-        2 40044 097.9584 269.2923 0059425 258.2447 101.2095 14.72707190 30443"""
-        qth = (37.771034, 122.413815, 7)  # lat (N), long (W), alt (meters)
-        predict.observe(tle, qth) # optional time argument defaults to time.time()
-        # => {'altitude': 676.8782276657903,
-        #     'azimuth': 96.04762045174824,
-        #     'beta_angle': -27.92735429908726,
-        #     'decayed': 0,
-        #     'doppler': 1259.6041017128405,
-        #     'eci_obs_x': -2438.227652191655,
-        #     'eci_obs_y': -4420.154476060397,
-        #     'eci_obs_z': 3885.390601342013,
-        #     'eci_sun_x': 148633398.020844,
-        #     'eci_sun_y': -7451536.44122029,
-        #     'eci_sun_z': -3229999.50056359,
-        #     'eci_vx': 0.20076213530665032,
-        #     'eci_vy': -1.3282146055077213,
-        #     'eci_vz': 7.377067234096598,
-        #     'eci_x': 6045.827328897242,
-        #     'eci_y': -3540.5885778261277,
-        #     'eci_z': -825.4065096776636,
-        #     'eclipse_depth': -87.61858291647795,
-        #     'elevation': -43.711904591801726,
-        #     'epoch': 1521290038.347793,
-        #     'footprint': 5633.548906707907,
-        #     'geostationary': 0,
-        #     'has_aos': 1,
-        #     'latitude': -6.759563817939698,
-        #     'longitude': 326.1137007912563,
-        #     'name': '0 LEMUR 1',
-        #     'norad_id': 40044,
-        #     'orbit': 20532,
-        #     'orbital_model': 'SGP4',
-        #     'orbital_phase': 145.3256815318047,
-        #     'orbital_velocity': 26994.138671706416,
-        #     'slant_range': 9743.943478523843,
-        #     'sunlit': 1,
-        #     'visibility': 'D'
-        #    }
-        ```
-        
-        #### Show upcoming transits of satellite over ground station
-        
-        ```python
-        # start and stop transit times as UNIX timestamp
-        transit_start = 1680775200
-        transit_stop = 1681034400
-        
-        p = predict.transits(tle, qth, transit_start, transit_stop)
-        
-        print("Start of Transit\tTransit Duration (s)\tPeak Elevation")
-        for transit in p:
-            print(f"{transit.start}\t{transit.duration()}\t{transit.peak()['elevation']}")
-        ```
-        
-        
-        #### Modeling an entire constellation
-        
-        Generating transits for a lot of satellites over a lot of ground stations can be slow.
-        Luckily, generating transits for each satellite-groundstation pair can be parallelized for a big speed-up.
-        
-        ```python
-        import itertools
-        from multiprocessing.pool import Pool
-        import time
-        
-        import predict
-        import requests
-        
-        # Define a function that returns arguments for all the transits() calls you want to make
-        def _transits_call_arguments():
-            now = time.time()
-            tle = requests.get('http://tle.spire.com/25544').text.rstrip()
-            for latitude in range(-90, 91, 15):
-                for longitude in range(-180, 181, 15):
-                    qth = (latitude, longitude, 0)
-                    yield {'tle': tle, 'qth': qth, 'ending_before': now+60*60*24*7}
-        
-        # Define a function that calls the transit function on a set of arguments and does per-transit processing
-        def _transits_call_fx(kwargs):
-            try:
-                transits = list(predict.transits(**kwargs))
-                return [t.above(10) for t in transits]
-            except predict.PredictException:
-                pass
-        
-        # Map the transit() caller across all the arguments you want, then flatten results into a single list
-        pool = Pool(processes=10)
-        array_of_results = pool.map(_transits_call_fx, _transits_call_arguments())
-        flattened_results = list(itertools.chain.from_iterable(filter(None, array_of_results)))
-        transits = flattened_results
-        ```
-        
-        NOTE: If precise accuracy isn't necessary (for modeling purposes, for example) setting the tolerance argument
-              to the `above` call to a larger value, say 1 degree, can provide a significant performance boost.
-        
-        #### Call predict analogs directly
-        
-        ```python
-        predict.quick_find(tle.split('\n'), time.time(), (37.7727, 122.407, 25))
-        predict.quick_predict(tle.split('\n'), time.time(), (37.7727, 122.407, 25))
-        ```
-        
-        ## API
-        <pre>
-        <b>observe</b>(<i>tle, qth[, at=None]</i>)  
-            Return an observation of a satellite relative to a groundstation.
-            <i>qth</i> groundstation coordinates as (lat(N),long(W),alt(m))
-            If <i>at</i> is not defined, defaults to current time (time.time())
-            Returns an "observation" or dictionary containing:  
-                <i>altitude</i> _ altitude of satellite in kilometers
-                <i>azimuth</i> - azimuth of satellite in degrees from perspective of groundstation.
-                <i>beta_angle</i>
-                <i>decayed</i> - 1 if satellite has decayed out of orbit, 0 otherwise.
-                <i>doppler</i> - doppler shift between groundstation and satellite.
-                <i>eci_obs_x</i>
-                <i>eci_obs_y</i>
-                <i>eci_obs_z</i>
-                <i>eci_sun_x</i>
-                <i>eci_sun_y</i>
-                <i>eci_sun_z</i>
-                <i>eci_vx</i>
-                <i>eci_vy</i>
-                <i>eci_vz</i>
-                <i>eci_x</i>
-                <i>eci_y</i>
-                <i>eci_z</i>
-                <i>eclipse_depth</i>
-                <i>elevation</i> - elevation of satellite in degrees from perspective of groundstation.
-                <i>epoch</i> - time of observation in seconds (unix epoch)
-                <i>footprint</i>
-                <i>geostationary</i> - 1 if satellite is determined to be geostationary, 0 otherwise.
-                <i>has_aos</i> - 1 if the satellite will eventually be visible from the groundstation
-                <i>latitude</i> - north latitude of point on earth directly under satellite.
-                <i>longitude</i> - west longitude of point on earth directly under satellite.
-                <i>name</i> - name of satellite from first line of TLE.
-                <i>norad_id</i> - NORAD id of satellite.
-                <i>orbit</i>
-                <i>orbital_phase</i>
-                <i>orbital_model</i>
-                <i>orbital_velocity</i>
-                <i>slant_range</i> - distance to satellite from groundstation in meters.
-                <i>sunlit</i> - 1 if satellite is in sunlight, 0 otherwise.
-                <i>visibility</i>
-        <b>transits</b>(<i>tle, qth[, ending_after=None][, ending_before=None]</i>)  
-            Returns iterator of <b>Transit</b> objects representing passes of tle over qth.  
-            If <i>ending_after</i> is not defined, defaults to current time  
-            If <i>ending_before</i> is not defined, the iterator will yield until calculation failure.
-        </pre>
-        ><b>NOTE</b>: We yield passes based on their end time.  This means we'll yield currently active passes in the two-argument invocation form, but their start times will be in the past.
-        
-        <pre>
-        <b>Transit</b>(<i>tle, qth, start, end</i>)  
-            Utility class representing a pass of a satellite over a groundstation.
-            Instantiation parameters are parsed and made available as fields.
-            <b>duration</b>()  
-                Returns length of transit in seconds
-            <b>peak</b>(<i>epsilon=0.1</i>)  
-                Returns epoch time where transit reaches maximum elevation (within ~<i>epsilon</i>)
-            <b>at</b>(<i>timestamp</i>)  
-                Returns observation during transit via <b>quick_find</b>(<i>tle, timestamp, qth</i>)
-            <b>above</b>b(<i>elevation</i>, <i>tolerance</i>)
-                Returns portion of transit above elevation. If the entire transit is below the target elevation, both
-                endpoints will be set to the peak and the duration will be zero. If a portion of the transit is above
-                the elevation target, the endpoints will be between elevation and elevation + tolerance (unless
-                endpoint is already above elevation, in which case it will be unchanged)
-        <b>quick_find</b>(<i>tle[, time[, (lat, long, alt)]]</i>)  
-            <i>time</i> defaults to current time   
-            <i>(lat, long, alt)</i> defaults to values in ~/.predict/predict.qth  
-            Returns observation dictionary equivalent to observe(tle, time, (lat, long, alt))
-        <b>quick_predict</b>(<i>tle[, time[, (lat, long, alt)]]</i>)  
-                Returns an array of observations for the next pass as calculated by predict.
-                Each observation is identical to that returned by <b>quick_find</b>.
-        </pre>
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: COPYING
+
+[![ci](https://github.com/nsat/pypredict/actions/workflows/python-app.yml/badge.svg)](https://github.com/nsat/pypredict/actions/workflows/python-app.yml)
+
+PyPredict
+=======
+
+><b>NOTE</b>: To preserve compatibility with `predict`, pypredict uses __north__ latitude and __west__ longitude for terrestrial coordinates.
+
+Do you want accurate and time-tested satellite tracking and pass prediction in a convenient python wrapper?
+You're in the right place.
+
+PyPredict is a C Python extension directly adapted from the ubiquitous [predict](http://www.qsl.net/kd2bd/predict.html) satellite tracking command line application.
+Originally written for the commodore 64, predict has a proven pedigree; We just aim to provide a convenient API.
+PyPredict is a port of the predict codebase and should yield identical results.
+
+If you think you've found an error in `pypredict`, please include output from `predict` on same inputs to the bug report.  
+If you think you've found a bug in predict, please report and we'll coordinate with upstream.
+
+### Installation
+
+```bash
+sudo apt-get install python-dev
+sudo python setup.py install
+```
+
+## Usage
+
+#### Observe a satellite (relative to a position on earth)
+
+```python
+import predict
+tle = """0 LEMUR 1
+1 40044U 14033AL  15013.74135905  .00002013  00000-0  31503-3 0  6119
+2 40044 097.9584 269.2923 0059425 258.2447 101.2095 14.72707190 30443"""
+qth = (37.771034, 122.413815, 7)  # lat (N), long (W), alt (meters)
+predict.observe(tle, qth) # optional time argument defaults to time.time()
+# => {'altitude': 676.8782276657903,
+#     'azimuth': 96.04762045174824,
+#     'beta_angle': -27.92735429908726,
+#     'decayed': 0,
+#     'doppler': 1259.6041017128405,
+#     'eci_obs_x': -2438.227652191655,
+#     'eci_obs_y': -4420.154476060397,
+#     'eci_obs_z': 3885.390601342013,
+#     'eci_sun_x': 148633398.020844,
+#     'eci_sun_y': -7451536.44122029,
+#     'eci_sun_z': -3229999.50056359,
+#     'eci_vx': 0.20076213530665032,
+#     'eci_vy': -1.3282146055077213,
+#     'eci_vz': 7.377067234096598,
+#     'eci_x': 6045.827328897242,
+#     'eci_y': -3540.5885778261277,
+#     'eci_z': -825.4065096776636,
+#     'eclipse_depth': -87.61858291647795,
+#     'elevation': -43.711904591801726,
+#     'epoch': 1521290038.347793,
+#     'footprint': 5633.548906707907,
+#     'geostationary': 0,
+#     'has_aos': 1,
+#     'latitude': -6.759563817939698,
+#     'longitude': 326.1137007912563,
+#     'name': '0 LEMUR 1',
+#     'norad_id': 40044,
+#     'orbit': 20532,
+#     'orbital_model': 'SGP4',
+#     'orbital_phase': 145.3256815318047,
+#     'orbital_velocity': 26994.138671706416,
+#     'slant_range': 9743.943478523843,
+#     'sunlit': 1,
+#     'visibility': 'D'
+#    }
+```
+
+#### Show upcoming transits of satellite over ground station
+
+```python
+# start and stop transit times as UNIX timestamp
+transit_start = 1680775200
+transit_stop = 1681034400
+
+p = predict.transits(tle, qth, transit_start, transit_stop)
+
+print("Start of Transit\tTransit Duration (s)\tPeak Elevation")
+for transit in p:
+    print(f"{transit.start}\t{transit.duration()}\t{transit.peak()['elevation']}")
+```
+
+
+#### Modeling an entire constellation
+
+Generating transits for a lot of satellites over a lot of ground stations can be slow.
+Luckily, generating transits for each satellite-groundstation pair can be parallelized for a big speed-up.
+
+```python
+import itertools
+from multiprocessing.pool import Pool
+import time
+
+import predict
+import requests
+
+# Define a function that returns arguments for all the transits() calls you want to make
+def _transits_call_arguments():
+    now = time.time()
+    tle = requests.get('http://tle.spire.com/25544').text.rstrip()
+    for latitude in range(-90, 91, 15):
+        for longitude in range(-180, 181, 15):
+            qth = (latitude, longitude, 0)
+            yield {'tle': tle, 'qth': qth, 'ending_before': now+60*60*24*7}
+
+# Define a function that calls the transit function on a set of arguments and does per-transit processing
+def _transits_call_fx(kwargs):
+    try:
+        transits = list(predict.transits(**kwargs))
+        return [t.above(10) for t in transits]
+    except predict.PredictException:
+        pass
+
+# Map the transit() caller across all the arguments you want, then flatten results into a single list
+pool = Pool(processes=10)
+array_of_results = pool.map(_transits_call_fx, _transits_call_arguments())
+flattened_results = list(itertools.chain.from_iterable(filter(None, array_of_results)))
+transits = flattened_results
+```
+
+NOTE: If precise accuracy isn't necessary (for modeling purposes, for example) setting the tolerance argument
+      to the `above` call to a larger value, say 1 degree, can provide a significant performance boost.
+
+#### Call predict analogs directly
+
+```python
+predict.quick_find(tle.split('\n'), time.time(), (37.7727, 122.407, 25))
+predict.quick_predict(tle.split('\n'), time.time(), (37.7727, 122.407, 25))
+```
+
+## API
+<pre>
+<b>observe</b>(<i>tle, qth[, at=None]</i>)  
+    Return an observation of a satellite relative to a groundstation.
+    <i>qth</i> groundstation coordinates as (lat(N),long(W),alt(m))
+    If <i>at</i> is not defined, defaults to current time (time.time())
+    Returns an "observation" or dictionary containing:  
+        <i>altitude</i> _ altitude of satellite in kilometers
+        <i>azimuth</i> - azimuth of satellite in degrees from perspective of groundstation.
+        <i>beta_angle</i>
+        <i>decayed</i> - 1 if satellite has decayed out of orbit, 0 otherwise.
+        <i>doppler</i> - doppler shift between groundstation and satellite.
+        <i>eci_obs_x</i>
+        <i>eci_obs_y</i>
+        <i>eci_obs_z</i>
+        <i>eci_sun_x</i>
+        <i>eci_sun_y</i>
+        <i>eci_sun_z</i>
+        <i>eci_vx</i>
+        <i>eci_vy</i>
+        <i>eci_vz</i>
+        <i>eci_x</i>
+        <i>eci_y</i>
+        <i>eci_z</i>
+        <i>eclipse_depth</i>
+        <i>elevation</i> - elevation of satellite in degrees from perspective of groundstation.
+        <i>epoch</i> - time of observation in seconds (unix epoch)
+        <i>footprint</i>
+        <i>geostationary</i> - 1 if satellite is determined to be geostationary, 0 otherwise.
+        <i>has_aos</i> - 1 if the satellite will eventually be visible from the groundstation
+        <i>latitude</i> - north latitude of point on earth directly under satellite.
+        <i>longitude</i> - west longitude of point on earth directly under satellite.
+        <i>name</i> - name of satellite from first line of TLE.
+        <i>norad_id</i> - NORAD id of satellite.
+        <i>orbit</i>
+        <i>orbital_phase</i>
+        <i>orbital_model</i>
+        <i>orbital_velocity</i>
+        <i>slant_range</i> - distance to satellite from groundstation in meters.
+        <i>sunlit</i> - 1 if satellite is in sunlight, 0 otherwise.
+        <i>visibility</i>
+<b>transits</b>(<i>tle, qth[, ending_after=None][, ending_before=None]</i>)  
+    Returns iterator of <b>Transit</b> objects representing passes of tle over qth.  
+    If <i>ending_after</i> is not defined, defaults to current time  
+    If <i>ending_before</i> is not defined, the iterator will yield until calculation failure.
+</pre>
+><b>NOTE</b>: We yield passes based on their end time.  This means we'll yield currently active passes in the two-argument invocation form, but their start times will be in the past.
+
+<pre>
+<b>Transit</b>(<i>tle, qth, start, end</i>)  
+    Utility class representing a pass of a satellite over a groundstation.
+    Instantiation parameters are parsed and made available as fields.
+    <b>duration</b>()  
+        Returns length of transit in seconds
+    <b>peak</b>(<i>epsilon=0.1</i>)  
+        Returns epoch time where transit reaches maximum elevation (within ~<i>epsilon</i>)
+    <b>at</b>(<i>timestamp</i>)  
+        Returns observation during transit via <b>quick_find</b>(<i>tle, timestamp, qth</i>)
+    <b>above</b>b(<i>elevation</i>, <i>tolerance</i>)
+        Returns portion of transit above elevation. If the entire transit is below the target elevation, both
+        endpoints will be set to the peak and the duration will be zero. If a portion of the transit is above
+        the elevation target, the endpoints will be between elevation and elevation + tolerance (unless
+        endpoint is already above elevation, in which case it will be unchanged)
+<b>quick_find</b>(<i>tle[, time[, (lat, long, alt)]]</i>)  
+    <i>time</i> defaults to current time   
+    <i>(lat, long, alt)</i> defaults to values in ~/.predict/predict.qth  
+    Returns observation dictionary equivalent to observe(tle, time, (lat, long, alt))
+<b>quick_predict</b>(<i>tle[, time[, (lat, long, alt)]]</i>)  
+        Returns an array of observations for the next pass as calculated by predict.
+        Each observation is identical to that returned by <b>quick_find</b>.
+</pre>
+
+
```

### Comparing `pypredict-1.7.1/setup.py` & `pypredict-1.7.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, Extension
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pypredict",
-    version="1.7.1",
+    version="1.7.2",
     author="Jesse Trutna",
     author_email="jesse@spire.com",
     maintainer="Spire Global Inc",
     maintainer_email="opensource@spire.com",
     description="Interface to the Predict satellite tracking and orbital prediction library",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

