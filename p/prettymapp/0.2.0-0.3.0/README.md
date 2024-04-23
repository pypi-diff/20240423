# Comparing `tmp/prettymapp-0.2.0.tar.gz` & `tmp/prettymapp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettymapp-0.2.0.tar", last modified: Fri Aug 25 13:49:21 2023, max compression
+gzip compressed data, was "prettymapp-0.3.0.tar", last modified: Tue Apr 23 20:00:31 2024, max compression
```

## Comparing `prettymapp-0.2.0.tar` & `prettymapp-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-08-25 13:49:21.523222 prettymapp-0.2.0/
--rw-r--r--   0 chris      (501) staff       (20)     1072 2023-08-25 12:19:47.000000 prettymapp-0.2.0/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     2834 2023-08-25 13:49:21.523115 prettymapp-0.2.0/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     2333 2023-08-25 13:22:27.000000 prettymapp-0.2.0/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-08-25 13:49:21.521056 prettymapp-0.2.0/prettymapp/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-02-27 22:38:48.000000 prettymapp-0.2.0/prettymapp/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-08-25 13:49:21.522045 prettymapp-0.2.0/prettymapp/fonts/
--rw-r--r--   0 chris      (501) staff       (20)    73620 2023-02-27 22:38:48.000000 prettymapp-0.2.0/prettymapp/fonts/PermanentMarker-Regular.ttf
--rw-r--r--   0 chris      (501) staff       (20)     2679 2023-02-27 22:38:48.000000 prettymapp-0.2.0/prettymapp/geo.py
--rw-r--r--   0 chris      (501) staff       (20)     1811 2023-08-25 13:26:40.000000 prettymapp-0.2.0/prettymapp/osm.py
--rw-r--r--   0 chris      (501) staff       (20)     8728 2023-02-27 22:38:48.000000 prettymapp-0.2.0/prettymapp/plotting.py
--rw-r--r--   0 chris      (501) staff       (20)     4280 2023-02-27 22:38:48.000000 prettymapp-0.2.0/prettymapp/settings.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-08-25 13:49:21.522848 prettymapp-0.2.0/prettymapp/tests/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-02-27 22:38:48.000000 prettymapp-0.2.0/prettymapp/tests/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     2993 2023-02-27 22:38:48.000000 prettymapp-0.2.0/prettymapp/tests/test_geo.py
--rw-r--r--   0 chris      (501) staff       (20)     1165 2023-02-27 22:38:48.000000 prettymapp-0.2.0/prettymapp/tests/test_main.py
--rw-r--r--   0 chris      (501) staff       (20)      249 2023-02-27 22:38:48.000000 prettymapp-0.2.0/prettymapp/tests/test_plotting.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-08-25 13:49:21.521939 prettymapp-0.2.0/prettymapp.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     2834 2023-08-25 13:49:21.000000 prettymapp-0.2.0/prettymapp.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      517 2023-08-25 13:49:21.000000 prettymapp-0.2.0/prettymapp.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-08-25 13:49:21.000000 prettymapp-0.2.0/prettymapp.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-08-10 00:45:34.000000 prettymapp-0.2.0/prettymapp.egg-info/not-zip-safe
--rw-r--r--   0 chris      (501) staff       (20)       59 2023-08-25 13:49:21.000000 prettymapp-0.2.0/prettymapp.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       11 2023-08-25 13:49:21.000000 prettymapp-0.2.0/prettymapp.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)      103 2023-08-25 13:26:40.000000 prettymapp-0.2.0/requirements.txt
--rw-r--r--   0 chris      (501) staff       (20)       38 2023-08-25 13:49:21.523252 prettymapp-0.2.0/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     1142 2023-08-25 13:48:49.000000 prettymapp-0.2.0/setup.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-23 20:00:31.594824 prettymapp-0.3.0/
+-rw-r--r--   0 chris      (501) staff       (20)     1072 2023-08-25 12:19:47.000000 prettymapp-0.3.0/LICENSE
+-rw-r--r--   0 chris      (501) staff       (20)     3206 2024-04-23 20:00:31.594559 prettymapp-0.3.0/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)     2585 2024-04-23 19:09:03.000000 prettymapp-0.3.0/README.md
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-23 20:00:31.590722 prettymapp-0.3.0/prettymapp/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-02-27 22:38:48.000000 prettymapp-0.3.0/prettymapp/__init__.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-23 20:00:31.592256 prettymapp-0.3.0/prettymapp/fonts/
+-rw-r--r--   0 chris      (501) staff       (20)    73620 2023-02-27 22:38:48.000000 prettymapp-0.3.0/prettymapp/fonts/PermanentMarker-Regular.ttf
+-rw-r--r--   0 chris      (501) staff       (20)     2714 2024-04-20 18:36:05.000000 prettymapp-0.3.0/prettymapp/geo.py
+-rw-r--r--   0 chris      (501) staff       (20)     2842 2024-04-23 19:09:03.000000 prettymapp-0.3.0/prettymapp/osm.py
+-rw-r--r--   0 chris      (501) staff       (20)     8728 2023-02-27 22:38:48.000000 prettymapp-0.3.0/prettymapp/plotting.py
+-rw-r--r--   0 chris      (501) staff       (20)     4280 2023-09-05 19:39:57.000000 prettymapp-0.3.0/prettymapp/settings.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-23 20:00:31.593981 prettymapp-0.3.0/prettymapp/tests/
+-rw-r--r--   0 chris      (501) staff       (20)        0 2023-02-27 22:38:48.000000 prettymapp-0.3.0/prettymapp/tests/__init__.py
+-rw-r--r--   0 chris      (501) staff       (20)     2990 2024-04-23 19:18:41.000000 prettymapp-0.3.0/prettymapp/tests/test_geo.py
+-rw-r--r--   0 chris      (501) staff       (20)     1165 2023-02-27 22:38:48.000000 prettymapp-0.3.0/prettymapp/tests/test_main.py
+-rw-r--r--   0 chris      (501) staff       (20)     1125 2024-04-23 19:09:03.000000 prettymapp-0.3.0/prettymapp/tests/test_osm.py
+-rw-r--r--   0 chris      (501) staff       (20)      249 2023-02-27 22:38:48.000000 prettymapp-0.3.0/prettymapp/tests/test_plotting.py
+drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-04-23 20:00:31.594279 prettymapp-0.3.0/prettymapp.egg-info/
+-rw-r--r--   0 chris      (501) staff       (20)     3206 2024-04-23 20:00:31.000000 prettymapp-0.3.0/prettymapp.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (501) staff       (20)      546 2024-04-23 20:00:31.000000 prettymapp-0.3.0/prettymapp.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-04-23 20:00:31.000000 prettymapp-0.3.0/prettymapp.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (501) staff       (20)        1 2024-04-23 19:21:21.000000 prettymapp-0.3.0/prettymapp.egg-info/not-zip-safe
+-rw-r--r--   0 chris      (501) staff       (20)       60 2024-04-23 20:00:31.000000 prettymapp-0.3.0/prettymapp.egg-info/requires.txt
+-rw-r--r--   0 chris      (501) staff       (20)       11 2024-04-23 20:00:31.000000 prettymapp-0.3.0/prettymapp.egg-info/top_level.txt
+-rw-r--r--   0 chris      (501) staff       (20)      104 2024-04-23 19:11:07.000000 prettymapp-0.3.0/requirements.txt
+-rw-r--r--   0 chris      (501) staff       (20)       38 2024-04-23 20:00:31.594873 prettymapp-0.3.0/setup.cfg
+-rw-r--r--   0 chris      (501) staff       (20)     1142 2024-04-23 19:56:57.000000 prettymapp-0.3.0/setup.py
```

### Comparing `prettymapp-0.2.0/LICENSE` & `prettymapp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prettymapp-0.2.0/PKG-INFO` & `prettymapp-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: prettymapp
-Version: 0.2.0
-Home-page: https://github.com/chrieke/prettymapp
-Author: Christoph Rieke
-Author-email: christoph.k.rieke@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # prettymapp 🖼️
 
 **Prettymapp is a webapp and Python package to create beautiful maps from OpenStreetMap data**
 
 ---
 <h3 align="center">
     🎈 Try it out here: <a href="https://prettymapp.streamlit.app/">prettymapp on streamlit 🎈 </a>
@@ -45,17 +29,17 @@
 It drops more complex configuration options in favour of improved speed, reduced code complexity and 
 simplified configuration interfaces. It is partially tested and adds a [streamlit](https://streamlit.io/) webapp component.
 
 ## Running the app locally
 
 ```bash
 git clone https://github.com/chrieke/prettymapp.git
-cd prettymapp/streamlit-prettymapp
-pip install -r requirements.txt
-streamlit run app.py
+cd prettymapp
+pip install -r streamlit-prettymapp/requirements.txt
+streamlit run streamlit-prettymapp/app.py
 ```
 
 ## Python package
 
 You can also use prettymapp without the webapp, directly in Python. This lets you customize the functionality or 
 build your own application.
 
@@ -81,10 +65,20 @@
     aoi_bounds=aoi.bounds,
     draw_settings=STYLES["Peach"]
 ).plot_all()
 
 fig.savefig("map.jpg")
 ```
 
+You can also plot exported OSM XML files e.g. from openstreetmap.org:
+
+```python
+from prettymapp.osm import get_osm_geometries_from_xml
+
+df = get_osm_geometries_from_xml(filepath="Berlin.osm")
+aoi_bounds = df.total_bounds
+...
+```
+
 To customize the map appearance, use the additional arguments of the [`Plot`](plotting.py#L36) class (e.g. `shape`, 
 `contour_width` etc.). Check the preconfigured [styles](prettymapp/settings.py#L35) and 
 webapp [examples](streamlit-prettymapp/examples.json) for inspiration.
```

#### html2text {}

```diff
@@ -1,16 +1,9 @@
-Metadata-Version: 2.1 Name: prettymapp Version: 0.2.0 Home-page: https://
-github.com/chrieke/prettymapp Author: Christoph Rieke Author-email:
-christoph.k.rieke@gmail.com License: MIT Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE # prettymapp ð¼ï¸
-**Prettymapp is a webapp and Python package to create beautiful maps from
-OpenStreetMap data** ---
+# prettymapp ð¼ï¸ **Prettymapp is a webapp and Python package to create
+beautiful maps from OpenStreetMap data** ---
          ******** ?ð??? TTrryy iitt oouutt hheerree:: _pp_rr_ee_tt_tt_yy_mm_aa_pp_pp_ _oo_nn_ _ss_tt_rr_ee_aa_mm_ll_ii_tt_ _?ð_?_?_? ********
 ---
                _[_._/_s_t_r_e_a_m_l_i_t_-_p_r_e_t_t_y_m_a_p_p_/_e_x_a_m_p_l_e___p_r_i_n_t_s_/_d_e_m_o_._g_i_f_]
 
 [./streamlit-prettymapp/example_prints/ [./streamlit-prettymapp/example_prints/
 macau.png]                              barcelona.png]
 ## Based on the prettymaps project Prettymapp is based on a rewrite of the
@@ -18,21 +11,25 @@
 [@marceloprates](https://github.com/marceloprates). All credit for the original
 idea, designs and implementation go to him. The prettymapp rewrite focuses on
 speed and adapted configuration to interface with the webapp. It drops more
 complex configuration options in favour of improved speed, reduced code
 complexity and simplified configuration interfaces. It is partially tested and
 adds a [streamlit](https://streamlit.io/) webapp component. ## Running the app
 locally ```bash git clone https://github.com/chrieke/prettymapp.git cd
-prettymapp/streamlit-prettymapp pip install -r requirements.txt streamlit run
-app.py ``` ## Python package You can also use prettymapp without the webapp,
-directly in Python. This lets you customize the functionality or build your own
-application. **Installation:** ```bash pip install prettymapp ``` **Define the
-area, download and plot the OSM data:** ```python from prettymapp.geo import
-get_aoi from prettymapp.osm import get_osm_geometries from prettymapp.plotting
-import Plot from prettymapp.settings import STYLES aoi = get_aoi
-(address="PraÃ§a Ferreira do Amaral, Macau", radius=1100, rectangular=False) df
-= get_osm_geometries(aoi=aoi) fig = Plot( df=df, aoi_bounds=aoi.bounds,
-draw_settings=STYLES["Peach"] ).plot_all() fig.savefig("map.jpg") ``` To
-customize the map appearance, use the additional arguments of the [`Plot`]
-(plotting.py#L36) class (e.g. `shape`, `contour_width` etc.). Check the
-preconfigured [styles](prettymapp/settings.py#L35) and webapp [examples]
-(streamlit-prettymapp/examples.json) for inspiration.
+prettymapp pip install -r streamlit-prettymapp/requirements.txt streamlit run
+streamlit-prettymapp/app.py ``` ## Python package You can also use prettymapp
+without the webapp, directly in Python. This lets you customize the
+functionality or build your own application. **Installation:** ```bash pip
+install prettymapp ``` **Define the area, download and plot the OSM data:**
+```python from prettymapp.geo import get_aoi from prettymapp.osm import
+get_osm_geometries from prettymapp.plotting import Plot from
+prettymapp.settings import STYLES aoi = get_aoi(address="PraÃ§a Ferreira do
+Amaral, Macau", radius=1100, rectangular=False) df = get_osm_geometries
+(aoi=aoi) fig = Plot( df=df, aoi_bounds=aoi.bounds, draw_settings=STYLES
+["Peach"] ).plot_all() fig.savefig("map.jpg") ``` You can also plot exported
+OSM XML files e.g. from openstreetmap.org: ```python from prettymapp.osm import
+get_osm_geometries_from_xml df = get_osm_geometries_from_xml
+(filepath="Berlin.osm") aoi_bounds = df.total_bounds ... ``` To customize the
+map appearance, use the additional arguments of the [`Plot`](plotting.py#L36)
+class (e.g. `shape`, `contour_width` etc.). Check the preconfigured [styles]
+(prettymapp/settings.py#L35) and webapp [examples](streamlit-prettymapp/
+examples.json) for inspiration.
```

### Comparing `prettymapp-0.2.0/prettymapp/fonts/PermanentMarker-Regular.ttf` & `prettymapp-0.3.0/prettymapp/fonts/PermanentMarker-Regular.ttf`

 * *Files identical despite different names*

### Comparing `prettymapp-0.2.0/prettymapp/geo.py` & `prettymapp-0.3.0/prettymapp/geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,17 @@
         df: Input GeoDataFrame
     """
     mask = df.geom_type.isin(["MultiPolygon", "MultiLineString", "MultiPoint"])
     outdf = df[~mask]
     df_multi = df[mask]
     for _, row in df_multi.iterrows():
         df_temp = GeoDataFrame(
-            pd.DataFrame.from_records([row.to_dict()] * len(row.geometry.geoms)), crs="EPSG:4326"
+            pd.DataFrame.from_records([row.to_dict()] * len(row.geometry.geoms)),
+            crs="EPSG:4326",
         )
         df_temp.geometry = list(row.geometry.geoms)
-        outdf = GeoDataFrame(pd.concat([outdf, df_temp], ignore_index=True), crs="EPSG:4326")
+        outdf = GeoDataFrame(
+            pd.concat([outdf, df_temp], ignore_index=True), crs="EPSG:4326"
+        )
 
     outdf = outdf.reset_index(drop=True)
     return outdf
```

### Comparing `prettymapp-0.2.0/prettymapp/plotting.py` & `prettymapp-0.3.0/prettymapp/plotting.py`

 * *Files identical despite different names*

### Comparing `prettymapp-0.2.0/prettymapp/settings.py` & `prettymapp-0.3.0/prettymapp/settings.py`

 * *Files identical despite different names*

### Comparing `prettymapp-0.2.0/prettymapp/tests/test_geo.py` & `prettymapp-0.3.0/prettymapp/tests/test_geo.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,48 +26,48 @@
 def test_get_aoi_from_user_input_address(ox_geocode):
     ox_geocode.return_value = 52.52, 13.4
 
     poly = get_aoi("Unter den Linden 37, 10117 Berlin")
     assert isinstance(poly, Polygon)
     assert poly.bounds == (
         13.373621926483281,
-        52.507705884952586,
-        13.403083847278062,
-        52.52567909987013,
+        52.50770588495259,
+        13.40308384727806,
+        52.525679099870146,
     )
-    assert poly.area == 0.00041542753985753124
+    assert poly.area == 0.000415427539857519
 
 
 @patch.object(ox, "geocode")
 def test_get_aoi_from_user_input_coordinates(ox_geocode):
     ox_geocode.return_value = 52.52, 13.4
 
     poly = get_aoi(coordinates=(52.52, 13.4))
     assert isinstance(poly, Polygon)
     assert poly.bounds == (
         13.38526793559592,
-        52.51101333875345,
+        52.511013338753465,
         13.414732236942758,
-        52.52898664609028,
+        52.52898664609029,
     )
 
 
 @patch.object(ox, "geocode")
 def test_get_aoi_from_user_input_rectangle(ox_geocode):
     ox_geocode.return_value = 52.52, 13.4
 
     poly = get_aoi("Unter den Linden 37, 10117 Berlin", rectangular=True)
     assert isinstance(poly, Polygon)
     assert poly.bounds == (
         13.373621926483281,
-        52.507705884952586,
-        13.403083847278062,
-        52.52567909987013,
+        52.50770588495259,
+        13.40308384727806,
+        52.525679099870146,
     )
-    assert poly.area == 0.0005295254343283185
+    assert poly.area == 0.0005295254343284959
 
 
 @pytest.mark.live
 def test_get_aoi_from_user_input_address_live():
     poly = get_aoi("Unter den Linden 37, 10117 Berlin")
     assert isinstance(poly, Polygon)
     assert poly.bounds == (
```

### Comparing `prettymapp-0.2.0/prettymapp/tests/test_main.py` & `prettymapp-0.3.0/prettymapp/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `prettymapp-0.2.0/prettymapp.egg-info/PKG-INFO` & `prettymapp-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: prettymapp
-Version: 0.2.0
+Version: 0.3.0
 Home-page: https://github.com/chrieke/prettymapp
 Author: Christoph Rieke
 Author-email: christoph.k.rieke@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas==2.2.2
+Requires-Dist: osmnx==1.9.2
+Requires-Dist: pyogrio==0.7.2
+Requires-Dist: matplotlib==3.8.4
 
 # prettymapp 🖼️
 
 **Prettymapp is a webapp and Python package to create beautiful maps from OpenStreetMap data**
 
 ---
 <h3 align="center">
@@ -45,17 +49,17 @@
 It drops more complex configuration options in favour of improved speed, reduced code complexity and 
 simplified configuration interfaces. It is partially tested and adds a [streamlit](https://streamlit.io/) webapp component.
 
 ## Running the app locally
 
 ```bash
 git clone https://github.com/chrieke/prettymapp.git
-cd prettymapp/streamlit-prettymapp
-pip install -r requirements.txt
-streamlit run app.py
+cd prettymapp
+pip install -r streamlit-prettymapp/requirements.txt
+streamlit run streamlit-prettymapp/app.py
 ```
 
 ## Python package
 
 You can also use prettymapp without the webapp, directly in Python. This lets you customize the functionality or 
 build your own application.
 
@@ -81,10 +85,20 @@
     aoi_bounds=aoi.bounds,
     draw_settings=STYLES["Peach"]
 ).plot_all()
 
 fig.savefig("map.jpg")
 ```
 
+You can also plot exported OSM XML files e.g. from openstreetmap.org:
+
+```python
+from prettymapp.osm import get_osm_geometries_from_xml
+
+df = get_osm_geometries_from_xml(filepath="Berlin.osm")
+aoi_bounds = df.total_bounds
+...
+```
+
 To customize the map appearance, use the additional arguments of the [`Plot`](plotting.py#L36) class (e.g. `shape`, 
 `contour_width` etc.). Check the preconfigured [styles](prettymapp/settings.py#L35) and 
 webapp [examples](streamlit-prettymapp/examples.json) for inspiration.
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: prettymapp Version: 0.2.0 Home-page: https://
+Metadata-Version: 2.1 Name: prettymapp Version: 0.3.0 Home-page: https://
 github.com/chrieke/prettymapp Author: Christoph Rieke Author-email:
 christoph.k.rieke@gmail.com License: MIT Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Requires-Python: >=3.6 Description-
-Content-Type: text/markdown License-File: LICENSE # prettymapp ð¼ï¸
-**Prettymapp is a webapp and Python package to create beautiful maps from
-OpenStreetMap data** ---
+Content-Type: text/markdown License-File: LICENSE Requires-Dist: pandas==2.2.2
+Requires-Dist: osmnx==1.9.2 Requires-Dist: pyogrio==0.7.2 Requires-Dist:
+matplotlib==3.8.4 # prettymapp ð¼ï¸ **Prettymapp is a webapp and Python
+package to create beautiful maps from OpenStreetMap data** ---
          ******** ?ð??? TTrryy iitt oouutt hheerree:: _pp_rr_ee_tt_tt_yy_mm_aa_pp_pp_ _oo_nn_ _ss_tt_rr_ee_aa_mm_ll_ii_tt_ _?ð_?_?_? ********
 ---
                _[_._/_s_t_r_e_a_m_l_i_t_-_p_r_e_t_t_y_m_a_p_p_/_e_x_a_m_p_l_e___p_r_i_n_t_s_/_d_e_m_o_._g_i_f_]
 
 [./streamlit-prettymapp/example_prints/ [./streamlit-prettymapp/example_prints/
 macau.png]                              barcelona.png]
 ## Based on the prettymaps project Prettymapp is based on a rewrite of the
@@ -18,21 +19,25 @@
 [@marceloprates](https://github.com/marceloprates). All credit for the original
 idea, designs and implementation go to him. The prettymapp rewrite focuses on
 speed and adapted configuration to interface with the webapp. It drops more
 complex configuration options in favour of improved speed, reduced code
 complexity and simplified configuration interfaces. It is partially tested and
 adds a [streamlit](https://streamlit.io/) webapp component. ## Running the app
 locally ```bash git clone https://github.com/chrieke/prettymapp.git cd
-prettymapp/streamlit-prettymapp pip install -r requirements.txt streamlit run
-app.py ``` ## Python package You can also use prettymapp without the webapp,
-directly in Python. This lets you customize the functionality or build your own
-application. **Installation:** ```bash pip install prettymapp ``` **Define the
-area, download and plot the OSM data:** ```python from prettymapp.geo import
-get_aoi from prettymapp.osm import get_osm_geometries from prettymapp.plotting
-import Plot from prettymapp.settings import STYLES aoi = get_aoi
-(address="PraÃ§a Ferreira do Amaral, Macau", radius=1100, rectangular=False) df
-= get_osm_geometries(aoi=aoi) fig = Plot( df=df, aoi_bounds=aoi.bounds,
-draw_settings=STYLES["Peach"] ).plot_all() fig.savefig("map.jpg") ``` To
-customize the map appearance, use the additional arguments of the [`Plot`]
-(plotting.py#L36) class (e.g. `shape`, `contour_width` etc.). Check the
-preconfigured [styles](prettymapp/settings.py#L35) and webapp [examples]
-(streamlit-prettymapp/examples.json) for inspiration.
+prettymapp pip install -r streamlit-prettymapp/requirements.txt streamlit run
+streamlit-prettymapp/app.py ``` ## Python package You can also use prettymapp
+without the webapp, directly in Python. This lets you customize the
+functionality or build your own application. **Installation:** ```bash pip
+install prettymapp ``` **Define the area, download and plot the OSM data:**
+```python from prettymapp.geo import get_aoi from prettymapp.osm import
+get_osm_geometries from prettymapp.plotting import Plot from
+prettymapp.settings import STYLES aoi = get_aoi(address="PraÃ§a Ferreira do
+Amaral, Macau", radius=1100, rectangular=False) df = get_osm_geometries
+(aoi=aoi) fig = Plot( df=df, aoi_bounds=aoi.bounds, draw_settings=STYLES
+["Peach"] ).plot_all() fig.savefig("map.jpg") ``` You can also plot exported
+OSM XML files e.g. from openstreetmap.org: ```python from prettymapp.osm import
+get_osm_geometries_from_xml df = get_osm_geometries_from_xml
+(filepath="Berlin.osm") aoi_bounds = df.total_bounds ... ``` To customize the
+map appearance, use the additional arguments of the [`Plot`](plotting.py#L36)
+class (e.g. `shape`, `contour_width` etc.). Check the preconfigured [styles]
+(prettymapp/settings.py#L35) and webapp [examples](streamlit-prettymapp/
+examples.json) for inspiration.
```

### Comparing `prettymapp-0.2.0/prettymapp.egg-info/SOURCES.txt` & `prettymapp-0.3.0/prettymapp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,8 +13,9 @@
 prettymapp.egg-info/not-zip-safe
 prettymapp.egg-info/requires.txt
 prettymapp.egg-info/top_level.txt
 prettymapp/fonts/PermanentMarker-Regular.ttf
 prettymapp/tests/__init__.py
 prettymapp/tests/test_geo.py
 prettymapp/tests/test_main.py
+prettymapp/tests/test_osm.py
 prettymapp/tests/test_plotting.py
```

### Comparing `prettymapp-0.2.0/setup.py` & `prettymapp-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import setup, find_packages
 
 parent_dir = Path(__file__).resolve().parent
 
 setup(
     name="prettymapp",
-    version="0.2.0",
+    version="0.3.0",
     author="Christoph Rieke",
     author_email="christoph.k.rieke@gmail.com",
     description="",
     long_description=parent_dir.joinpath("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/chrieke/prettymapp",
     license="MIT",
```

