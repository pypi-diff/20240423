# Comparing `tmp/osdatahub-1.2.8.tar.gz` & `tmp/osdatahub-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osdatahub-1.2.8.tar", last modified: Wed Oct  4 09:02:43 2023, max compression
+gzip compressed data, was "osdatahub-1.2.9.tar", last modified: Thu Nov  2 15:57:41 2023, max compression
```

## Comparing `osdatahub-1.2.8.tar` & `osdatahub-1.2.9.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.875578 osdatahub-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-10-04 09:02:11.000000 osdatahub-1.2.8/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.847576 osdatahub-1.2.8/Examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/CRS pitfalls.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   231081 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/Converting API Results into Common Data Formats.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1837789 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/Defining Extents for API Queries.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12538 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/Filtering Attributes for API Queries.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10298 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/Interactive Plotting for API Results - Folium.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   945983 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    34430 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/Post Processing API Queries.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/Quick Start Guide.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/Setting up an API key.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    86367 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/Using the NGD Features API.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.855577 osdatahub-1.2.8/Examples/images/
--rw-r--r--   0 runner    (1001) docker     (127)  2124067 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/images/1_homescreen.PNG
--rw-r--r--   0 runner    (1001) docker     (127)   178174 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/images/2_sign_up.PNG
--rw-r--r--   0 runner    (1001) docker     (127)  1883255 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/images/3_datahub_homepage.PNG
--rw-r--r--   0 runner    (1001) docker     (127)   115385 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/images/4_new_project.PNG
--rw-r--r--   0 runner    (1001) docker     (127)   153664 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/images/5_add_api_to_project.PNG
--rw-r--r--   0 runner    (1001) docker     (127)   113078 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/images/6_view_api_key.PNG
--rw-r--r--   0 runner    (1001) docker     (127)  1790610 2023-10-04 09:02:11.000000 osdatahub-1.2.8/Examples/images/CRS.png
--rw-r--r--   0 runner    (1001) docker     (127)    33604 2023-10-04 09:02:11.000000 osdatahub-1.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-10-04 09:02:11.000000 osdatahub-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15737 2023-10-04 09:02:43.875578 osdatahub-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2023-10-04 09:02:11.000000 osdatahub-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.859577 osdatahub-1.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/DownloadsAPI.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/Extent.rst
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/FeaturesAPI.rst
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/LinkedIdentifiersAPI.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/NGD.rst
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/NamesAPI.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/PlacesAPI.rst
--rw-r--r--   0 runner    (1001) docker     (127)      798 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/Utilities.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.859577 osdatahub-1.2.8/docs/media/
--rw-r--r--   0 runner    (1001) docker     (127)    23309 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/media/os-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/readme_link.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-04 09:02:11.000000 osdatahub-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.859577 osdatahub-1.2.8/media/
--rw-r--r--   0 runner    (1001) docker     (127)    23309 2023-10-04 09:02:11.000000 osdatahub-1.2.8/media/os-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-04 09:02:11.000000 osdatahub-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-10-04 09:02:11.000000 osdatahub-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-10-04 09:02:43.875578 osdatahub-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-04 09:02:11.000000 osdatahub-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.839576 osdatahub-1.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.863577 osdatahub-1.2.8/src/osdatahub/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.863577 osdatahub-1.2.8/src/osdatahub/DownloadsAPI/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/DownloadsAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/DownloadsAPI/data_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     9380 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/DownloadsAPI/downloads_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/DownloadsAPI/opendata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.863577 osdatahub-1.2.8/src/osdatahub/FeaturesAPI/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/FeaturesAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/FeaturesAPI/feature_products.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/FeaturesAPI/features_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.863577 osdatahub-1.2.8/src/osdatahub/LinkedIdentifiersAPI/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/LinkedIdentifiersAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.867577 osdatahub-1.2.8/src/osdatahub/NGD/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/NGD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/NGD/crs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/NGD/ngd_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.867577 osdatahub-1.2.8/src/osdatahub/NamesAPI/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/NamesAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/NamesAPI/local_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/NamesAPI/names_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.867577 osdatahub-1.2.8/src/osdatahub/PlacesAPI/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/PlacesAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15066 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/PlacesAPI/places_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/extent.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/grow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/ons_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/requests_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/spatial_filter_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2023-10-04 09:02:11.000000 osdatahub-1.2.8/src/osdatahub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.863577 osdatahub-1.2.8/src/osdatahub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15737 2023-10-04 09:02:43.000000 osdatahub-1.2.8/src/osdatahub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2023-10-04 09:02:43.000000 osdatahub-1.2.8/src/osdatahub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 09:02:43.000000 osdatahub-1.2.8/src/osdatahub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-10-04 09:02:43.000000 osdatahub-1.2.8/src/osdatahub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-04 09:02:43.000000 osdatahub-1.2.8/src/osdatahub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.867577 osdatahub-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.871578 osdatahub-1.2.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.871578 osdatahub-1.2.8/tests/data/clean_polygon_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.871578 osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/
--rw-r--r--   0 runner    (1001) docker     (127)    29650 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    45345 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    32875 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    20201 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 09:02:43.871578 osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/
--rw-r--r--   0 runner    (1001) docker     (127)    37512 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    58496 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    33032 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson
--rw-r--r--   0 runner    (1001) docker     (127)    25361 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data/get_uncleaned_polygons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/clean_polygon_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/downloads_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/extent_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7737 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/features_api_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/filters_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/linked_identifiers_api_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/names_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/ngd_crs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    24199 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/ngd_merge_geojsons_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/ngd_query_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/places_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/data/utils_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/run_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_clean_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_downloads_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_extent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_features_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_grow_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_linked_identifiers_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_names_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_ngd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_places_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-10-04 09:02:11.000000 osdatahub-1.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.289072 osdatahub-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2023-11-02 15:57:06.000000 osdatahub-1.2.9/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.257072 osdatahub-1.2.9/Examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/CRS pitfalls.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   231081 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/Converting API Results into Common Data Formats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1837789 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/Defining Extents for API Queries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/Filtering Attributes for API Queries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10298 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/Interactive Plotting for API Results - Folium.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   945983 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    34430 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/Post Processing API Queries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/Quick Start Guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/Setting up an API key.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    86367 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/Using the NGD Features API.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.265072 osdatahub-1.2.9/Examples/images/
+-rw-r--r--   0 runner    (1001) docker     (127)  2124067 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/images/1_homescreen.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)   178174 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/images/2_sign_up.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)  1883255 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/images/3_datahub_homepage.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)   115385 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/images/4_new_project.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)   153664 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/images/5_add_api_to_project.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)   113078 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/images/6_view_api_key.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)  1790610 2023-11-02 15:57:06.000000 osdatahub-1.2.9/Examples/images/CRS.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33604 2023-11-02 15:57:06.000000 osdatahub-1.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-11-02 15:57:06.000000 osdatahub-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15737 2023-11-02 15:57:41.289072 osdatahub-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2023-11-02 15:57:06.000000 osdatahub-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.269072 osdatahub-1.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/DownloadsAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/Extent.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/FeaturesAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/LinkedIdentifiersAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/NGD.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/NamesAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/PlacesAPI.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/Utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.269072 osdatahub-1.2.9/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    23309 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/media/os-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/readme_link.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-11-02 15:57:06.000000 osdatahub-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.269072 osdatahub-1.2.9/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    23309 2023-11-02 15:57:06.000000 osdatahub-1.2.9/media/os-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2023-11-02 15:57:06.000000 osdatahub-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-02 15:57:06.000000 osdatahub-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2023-11-02 15:57:41.293072 osdatahub-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-02 15:57:06.000000 osdatahub-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.249072 osdatahub-1.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.273072 osdatahub-1.2.9/src/osdatahub/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.277072 osdatahub-1.2.9/src/osdatahub/DownloadsAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/DownloadsAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5023 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/DownloadsAPI/data_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9381 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/DownloadsAPI/downloads_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/DownloadsAPI/opendata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.277072 osdatahub-1.2.9/src/osdatahub/FeaturesAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/FeaturesAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/FeaturesAPI/feature_products.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/FeaturesAPI/features_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.277072 osdatahub-1.2.9/src/osdatahub/LinkedIdentifiersAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/LinkedIdentifiersAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.277072 osdatahub-1.2.9/src/osdatahub/NGD/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/NGD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/NGD/crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/NGD/ngd_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.281072 osdatahub-1.2.9/src/osdatahub/NamesAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/NamesAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/NamesAPI/local_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7409 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/NamesAPI/names_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.281072 osdatahub-1.2.9/src/osdatahub/PlacesAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/PlacesAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15066 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/PlacesAPI/places_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/grow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/ons_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/requests_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/spatial_filter_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2023-11-02 15:57:06.000000 osdatahub-1.2.9/src/osdatahub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.277072 osdatahub-1.2.9/src/osdatahub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15737 2023-11-02 15:57:41.000000 osdatahub-1.2.9/src/osdatahub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2023-11-02 15:57:41.000000 osdatahub-1.2.9/src/osdatahub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 15:57:41.000000 osdatahub-1.2.9/src/osdatahub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-02 15:57:41.000000 osdatahub-1.2.9/src/osdatahub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-02 15:57:41.000000 osdatahub-1.2.9/src/osdatahub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.285072 osdatahub-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.285072 osdatahub-1.2.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.285072 osdatahub-1.2.9/tests/data/clean_polygon_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.289072 osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/
+-rw-r--r--   0 runner    (1001) docker     (127)    29650 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    45345 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    32875 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    20201 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 15:57:41.289072 osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/
+-rw-r--r--   0 runner    (1001) docker     (127)    37512 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    58496 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    33032 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)    25361 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data/get_uncleaned_polygons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/clean_polygon_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/downloads_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/extent_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/features_api_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/filters_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/linked_identifiers_api_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/names_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/ngd_crs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24199 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/ngd_merge_geojsons_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/ngd_query_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/places_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/data/utils_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/run_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_clean_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_downloads_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_features_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_grow_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_linked_identifiers_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_names_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_ngd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_places_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2023-11-02 15:57:06.000000 osdatahub-1.2.9/tox.ini
```

### Comparing `osdatahub-1.2.8/.readthedocs.yaml` & `osdatahub-1.2.9/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/CRS pitfalls.ipynb` & `osdatahub-1.2.9/Examples/CRS pitfalls.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/Converting API Results into Common Data Formats.ipynb` & `osdatahub-1.2.9/Examples/Converting API Results into Common Data Formats.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/Defining Extents for API Queries.ipynb` & `osdatahub-1.2.9/Examples/Defining Extents for API Queries.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/Filtering Attributes for API Queries.ipynb` & `osdatahub-1.2.9/Examples/Filtering Attributes for API Queries.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/Interactive Plotting for API Results - Folium.ipynb` & `osdatahub-1.2.9/Examples/Interactive Plotting for API Results - Folium.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb` & `osdatahub-1.2.9/Examples/Plotting API Results - GeoPandas, Matplotlib and Contextily.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/Post Processing API Queries.ipynb` & `osdatahub-1.2.9/Examples/Post Processing API Queries.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/Quick Start Guide.ipynb` & `osdatahub-1.2.9/Examples/Quick Start Guide.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/Setting up an API key.ipynb` & `osdatahub-1.2.9/Examples/Setting up an API key.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/Using the NGD Features API.ipynb` & `osdatahub-1.2.9/Examples/Using the NGD Features API.ipynb`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/images/1_homescreen.PNG` & `osdatahub-1.2.9/Examples/images/1_homescreen.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/images/2_sign_up.PNG` & `osdatahub-1.2.9/Examples/images/2_sign_up.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/images/3_datahub_homepage.PNG` & `osdatahub-1.2.9/Examples/images/3_datahub_homepage.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/images/4_new_project.PNG` & `osdatahub-1.2.9/Examples/images/4_new_project.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/images/5_add_api_to_project.PNG` & `osdatahub-1.2.9/Examples/images/5_add_api_to_project.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/images/6_view_api_key.PNG` & `osdatahub-1.2.9/Examples/images/6_view_api_key.PNG`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/Examples/images/CRS.png` & `osdatahub-1.2.9/Examples/images/CRS.png`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/LICENSE.txt` & `osdatahub-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/PKG-INFO` & `osdatahub-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osdatahub
-Version: 1.2.8
+Version: 1.2.9
 Summary: osdatahub is Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS Data Hub APIs readily accessible to developers.
 Home-page: https://github.com/OrdnanceSurvey/osdatahub
 Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping
 Author-email: rapidprototyping@os.uk
 License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osdatahub Version: 1.2.8 Summary: osdatahub is
+Metadata-Version: 2.1 Name: osdatahub Version: 1.2.9 Summary: osdatahub is
 Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS
 Data Hub APIs readily accessible to developers. Home-page: https://github.com/
 OrdnanceSurvey/osdatahub Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping Author-email: rapidprototyping@os.uk License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub Project-URL:
 Documentation, https://osdatahub.readthedocs.io/en/latest/ Project-URL: Issues,
 https://github.com/OrdnanceSurvey/osdatahub/issues Keywords: Ordnance-
```

### Comparing `osdatahub-1.2.8/README.md` & `osdatahub-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/docs/Utilities.rst` & `osdatahub-1.2.9/docs/Utilities.rst`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/docs/conf.py` & `osdatahub-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/docs/index.rst` & `osdatahub-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/docs/media/os-logo.png` & `osdatahub-1.2.9/docs/media/os-logo.png`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/media/os-logo.png` & `osdatahub-1.2.9/media/os-logo.png`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/setup.cfg` & `osdatahub-1.2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osdatahub
-version = 1.2.8
+version = 1.2.9
 author = OS Rapid Prototyping
 author_email = rapidprototyping@os.uk
 classifiers = 
 	Natural Language :: English
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Programming Language :: Python :: 3.7
```

### Comparing `osdatahub-1.2.8/src/osdatahub/DownloadsAPI/data_package.py` & `osdatahub-1.2.9/src/osdatahub/DownloadsAPI/data_package.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/DownloadsAPI/downloads_api.py` & `osdatahub-1.2.9/src/osdatahub/DownloadsAPI/downloads_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                             )
                         pbar.write(
                             f"Finished downloading {self.file_name} to {output_path}")
                 break
 
             except HTTPError as exc:
                 if int(exc.response.status_code) == 429:
-                    time.sleep(1)
+                    time.sleep(20)
                     continue
                 raise
 
         return output_path
 
 
 def remove_key(url: str):
```

### Comparing `osdatahub-1.2.8/src/osdatahub/DownloadsAPI/opendata.py` & `osdatahub-1.2.9/src/osdatahub/DownloadsAPI/opendata.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/FeaturesAPI/feature_products.py` & `osdatahub-1.2.9/src/osdatahub/FeaturesAPI/feature_products.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/FeaturesAPI/features_api.py` & `osdatahub-1.2.9/src/osdatahub/FeaturesAPI/features_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py` & `osdatahub-1.2.9/src/osdatahub/LinkedIdentifiersAPI/linked_identifier_options.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py` & `osdatahub-1.2.9/src/osdatahub/LinkedIdentifiersAPI/linked_identifiers_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/NGD/crs.py` & `osdatahub-1.2.9/src/osdatahub/NGD/crs.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/NGD/ngd_api.py` & `osdatahub-1.2.9/src/osdatahub/NGD/ngd_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/NamesAPI/local_types.py` & `osdatahub-1.2.9/src/osdatahub/NamesAPI/local_types.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/NamesAPI/names_api.py` & `osdatahub-1.2.9/src/osdatahub/NamesAPI/names_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/PlacesAPI/places_api.py` & `osdatahub-1.2.9/src/osdatahub/PlacesAPI/places_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/__init__.py` & `osdatahub-1.2.9/src/osdatahub/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def set_proxies(proxies):
     os.environ["_OSDATAHUB_PROXIES"] = json.dumps(proxies)
 
 def get_proxies():
     return json.loads(os.environ["_OSDATAHUB_PROXIES"])
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 
 from osdatahub.extent import Extent
 from osdatahub.FeaturesAPI import FeaturesAPI
 from osdatahub.PlacesAPI import PlacesAPI
 from osdatahub.NamesAPI import NamesAPI
 from osdatahub.LinkedIdentifiersAPI import LinkedIdentifiersAPI
 from osdatahub.DownloadsAPI import OpenDataDownload, DataPackageDownload
```

### Comparing `osdatahub-1.2.8/src/osdatahub/bbox.py` & `osdatahub-1.2.9/src/osdatahub/bbox.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/codes.py` & `osdatahub-1.2.9/src/osdatahub/codes.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/errors.py` & `osdatahub-1.2.9/src/osdatahub/errors.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/extent.py` & `osdatahub-1.2.9/src/osdatahub/extent.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/filters.py` & `osdatahub-1.2.9/src/osdatahub/filters.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/grow_list.py` & `osdatahub-1.2.9/src/osdatahub/grow_list.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/ons_api.py` & `osdatahub-1.2.9/src/osdatahub/ons_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/requests_wrapper.py` & `osdatahub-1.2.9/src/osdatahub/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/spatial_filter_types.py` & `osdatahub-1.2.9/src/osdatahub/spatial_filter_types.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub/utils.py` & `osdatahub-1.2.9/src/osdatahub/utils.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/src/osdatahub.egg-info/PKG-INFO` & `osdatahub-1.2.9/src/osdatahub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osdatahub
-Version: 1.2.8
+Version: 1.2.9
 Summary: osdatahub is Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS Data Hub APIs readily accessible to developers.
 Home-page: https://github.com/OrdnanceSurvey/osdatahub
 Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping
 Author-email: rapidprototyping@os.uk
 License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osdatahub Version: 1.2.8 Summary: osdatahub is
+Metadata-Version: 2.1 Name: osdatahub Version: 1.2.9 Summary: osdatahub is
 Ordnance Survey's (OS) Python API wrapper, designed to make data from the OS
 Data Hub APIs readily accessible to developers. Home-page: https://github.com/
 OrdnanceSurvey/osdatahub Download-URL: https://pypi.org/project/osdatahub/
 Author: OS Rapid Prototyping Author-email: rapidprototyping@os.uk License: OGL
 Project-URL: Code, https://github.com/OrdnanceSurvey/osdatahub Project-URL:
 Documentation, https://osdatahub.readthedocs.io/en/latest/ Project-URL: Issues,
 https://github.com/OrdnanceSurvey/osdatahub/issues Keywords: Ordnance-
```

### Comparing `osdatahub-1.2.8/src/osdatahub.egg-info/SOURCES.txt` & `osdatahub-1.2.9/src/osdatahub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson` & `osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson` & `osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon2.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson` & `osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/sites_multipolygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson` & `osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson` & `osdatahub-1.2.9/tests/data/clean_polygon_data/API (uncleaned)/sites_polygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson` & `osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/sites_multipolygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson` & `osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/sites_multipolygon2.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson` & `osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/sites_multipolygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson` & `osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/sites_polygon.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson` & `osdatahub-1.2.9/tests/data/clean_polygon_data/QGIS/sites_polygon_with_hole.geojson`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data/get_uncleaned_polygons.py` & `osdatahub-1.2.9/tests/data/clean_polygon_data/get_uncleaned_polygons.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/clean_polygon_data.py` & `osdatahub-1.2.9/tests/data/clean_polygon_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/downloads_data.py` & `osdatahub-1.2.9/tests/data/downloads_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/extent_data.py` & `osdatahub-1.2.9/tests/data/extent_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/features_api_data.py` & `osdatahub-1.2.9/tests/data/features_api_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/filters_data.py` & `osdatahub-1.2.9/tests/data/filters_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/linked_identifiers_api_data.py` & `osdatahub-1.2.9/tests/data/linked_identifiers_api_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/names_data.py` & `osdatahub-1.2.9/tests/data/names_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/ngd_crs_data.py` & `osdatahub-1.2.9/tests/data/ngd_crs_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/ngd_merge_geojsons_data.py` & `osdatahub-1.2.9/tests/data/ngd_merge_geojsons_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/ngd_query_data.py` & `osdatahub-1.2.9/tests/data/ngd_query_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/places_data.py` & `osdatahub-1.2.9/tests/data/places_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/data/utils_data.py` & `osdatahub-1.2.9/tests/data/utils_data.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/run_functions.py` & `osdatahub-1.2.9/tests/run_functions.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/test_downloads_api.py` & `osdatahub-1.2.9/tests/test_downloads_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,23 +73,22 @@
     def data_package(self):
         data_package = DataPackageDownload(key="test_key", product_id="test_id")
         yield data_package
 
     @pytest.mark.skipif(API_KEY is None, reason="Test API key not available")
     def test_download_pass(self):
         # Arrange
-        product_package = DataPackageDownload(API_KEY, "98")
-        files_to_download = product_package.product_list("156")
+        product_package = DataPackageDownload(API_KEY, "97")
 
         # Act
         with tempfile.TemporaryDirectory() as tmpdirname:
-            downloaded = product_package.download("156", tmpdirname)
+            downloaded = product_package.download("17094", tmpdirname, "bld_fts_buildingpart_orderSummary.json")
 
         # Assert
-        assert len(downloaded) == len(files_to_download["downloads"])
+        assert len(downloaded) == 1
 
     def test_download_list_pass(self):
         # TODO: implement download_list_pass
         pass
 
     def test_download_list_fail(self):
         # TODO: implement download_list_fail
```

### Comparing `osdatahub-1.2.8/tests/test_extent.py` & `osdatahub-1.2.9/tests/test_extent.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/test_features_api.py` & `osdatahub-1.2.9/tests/test_features_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/test_filters.py` & `osdatahub-1.2.9/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/test_grow_list.py` & `osdatahub-1.2.9/tests/test_grow_list.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/test_linked_identifiers_api.py` & `osdatahub-1.2.9/tests/test_linked_identifiers_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/test_names_api.py` & `osdatahub-1.2.9/tests/test_names_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/test_ngd.py` & `osdatahub-1.2.9/tests/test_ngd.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/test_places_api.py` & `osdatahub-1.2.9/tests/test_places_api.py`

 * *Files identical despite different names*

### Comparing `osdatahub-1.2.8/tests/test_utils.py` & `osdatahub-1.2.9/tests/test_utils.py`

 * *Files identical despite different names*

