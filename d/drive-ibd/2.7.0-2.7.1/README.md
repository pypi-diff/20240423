# Comparing `tmp/drive_ibd-2.7.0.tar.gz` & `tmp/drive_ibd-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drive_ibd-2.7.0.tar", max compression
+gzip compressed data, was "drive_ibd-2.7.1.tar", max compression
```

## Comparing `drive_ibd-2.7.0.tar` & `drive_ibd-2.7.1.tar`

### file list

```diff
@@ -1,40 +1,75 @@
--rw-r--r--   0        0        0    11357 2023-10-09 16:10:09.111536 drive_ibd-2.7.0/LICENSE
--rw-r--r--   0        0        0     1614 2023-12-15 15:41:34.755994 drive_ibd-2.7.0/README.md
--rw-r--r--   0        0        0        0 2023-07-03 15:02:02.235740 drive_ibd-2.7.0/drive/__init__.py
--rwxr-xr-x   0        0        0    12233 2024-04-05 15:53:53.695267 drive_ibd-2.7.0/drive/__main__.py
--rw-r--r--   0        0        0       45 2023-08-03 19:43:34.428381 drive_ibd-2.7.0/drive/cluster/__init__.py
--rw-r--r--   0        0        0    20260 2024-03-06 22:07:36.488162 drive_ibd-2.7.0/drive/cluster/cluster.py
--rw-r--r--   0        0        0      205 2023-08-03 19:43:34.456380 drive_ibd-2.7.0/drive/config.json
--rwxr-xr-x   0        0        0    12405 2024-04-05 15:53:53.699267 drive_ibd-2.7.0/drive/drive.py
--rw-r--r--   0        0        0      129 2023-08-03 19:43:34.456380 drive_ibd-2.7.0/drive/factory/__init__.py
--rw-r--r--   0        0        0     1529 2023-08-03 19:43:34.524379 drive_ibd-2.7.0/drive/factory/factory.py
--rw-r--r--   0        0        0      784 2023-08-03 19:43:34.616376 drive_ibd-2.7.0/drive/factory/loader.py
--rw-r--r--   0        0        0       30 2023-08-03 19:43:34.664375 drive_ibd-2.7.0/drive/filters/__init__.py
--rw-r--r--   0        0        0    18393 2024-04-05 15:53:55.759238 drive_ibd-2.7.0/drive/filters/filter.py
--rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.7.0/drive/log/.git
--rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.7.0/drive/log/.gitignore
--rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.7.0/drive/log/README.md
--rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.7.0/drive/log/__init__.py
--rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.7.0/drive/log/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.7.0/drive/log/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7199 2023-11-25 21:04:36.562604 drive_ibd-2.7.0/drive/log/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.7.0/drive/log/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     5031 2024-04-05 15:53:55.955235 drive_ibd-2.7.0/drive/log/logger.py
--rw-r--r--   0        0        0      189 2023-12-15 15:59:21.176736 drive_ibd-2.7.0/drive/models/__init__.py
--rw-r--r--   0        0        0      697 2024-03-19 14:02:55.531225 drive_ibd-2.7.0/drive/models/data_container.py
--rw-r--r--   0        0        0     4576 2024-03-06 22:07:36.492162 drive_ibd-2.7.0/drive/models/generate_indices.py
--rw-r--r--   0        0        0     2161 2023-08-03 19:43:34.884370 drive_ibd-2.7.0/drive/models/networks.py
--rw-r--r--   0        0        0      617 2023-08-03 19:43:34.908369 drive_ibd-2.7.0/drive/models/types.py
--rw-r--r--   0        0        0        0 2023-08-03 19:43:34.908369 drive_ibd-2.7.0/drive/plugins/__init__.py
--rw-r--r--   0        0        0     4475 2024-04-05 15:32:38.137080 drive_ibd-2.7.0/drive/plugins/network_writer.py
--rw-r--r--   0        0        0    13389 2024-04-05 15:32:28.593218 drive_ibd-2.7.0/drive/plugins/pvalues.py
--rw-r--r--   0        0        0        3 2024-03-06 22:07:36.516162 drive_ibd-2.7.0/drive/profile.json
--rw-r--r--   0        0        0       39 2023-12-15 15:59:21.224735 drive_ibd-2.7.0/drive/utilities/callbacks/__init__.py
--rw-r--r--   0        0        0     1821 2024-04-05 15:53:53.827265 drive_ibd-2.7.0/drive/utilities/callbacks/callbacks.py
--rw-r--r--   0        0        0     2263 2023-08-03 19:43:35.044366 drive_ibd-2.7.0/drive/utilities/load_phenotypes.py
--rw-r--r--   0        0        0      121 2023-08-03 19:43:35.076365 drive_ibd-2.7.0/drive/utilities/parser/__init__.py
--rw-r--r--   0        0        0     7764 2024-04-05 15:53:53.739266 drive_ibd-2.7.0/drive/utilities/parser/case_file_parser.py
--rw-r--r--   0        0        0      919 2023-08-03 19:43:35.156363 drive_ibd-2.7.0/drive/utilities/parser/phenotype_descriptions_parser.py
--rw-r--r--   0        0        0     2211 2024-04-05 15:55:23.838003 drive_ibd-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 drive_ibd-2.7.0/setup.py
--rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 drive_ibd-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-09 16:10:09.111536 drive_ibd-2.7.1/LICENSE
+-rw-r--r--   0        0        0     1614 2023-12-15 15:41:34.755994 drive_ibd-2.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 15:02:02.235740 drive_ibd-2.7.1/drive/__init__.py
+-rwxr-xr-x   0        0        0    12233 2024-04-05 15:53:53.695267 drive_ibd-2.7.1/drive/__main__.py
+-rw-r--r--   0        0        0       45 2023-08-03 19:43:34.428381 drive_ibd-2.7.1/drive/cluster/__init__.py
+-rw-r--r--   0        0        0      268 2023-08-03 19:43:45.404117 drive_ibd-2.7.1/drive/cluster/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      249 2023-04-14 16:19:48.390166 drive_ibd-2.7.1/drive/cluster/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    22026 2024-03-18 13:15:24.956654 drive_ibd-2.7.1/drive/cluster/__pycache__/cluster.cpython-311.pyc
+-rw-r--r--   0        0        0     9654 2023-04-14 17:05:43.254068 drive_ibd-2.7.1/drive/cluster/__pycache__/cluster.cpython-39.pyc
+-rw-r--r--   0        0        0    20260 2024-03-06 22:07:36.488162 drive_ibd-2.7.1/drive/cluster/cluster.py
+-rw-r--r--   0        0        0      205 2023-08-03 19:43:34.456380 drive_ibd-2.7.1/drive/config.json
+-rwxr-xr-x   0        0        0    12387 2024-04-05 18:01:42.273139 drive_ibd-2.7.1/drive/drive.py
+-rw-r--r--   0        0        0      129 2023-08-03 19:43:34.456380 drive_ibd-2.7.1/drive/factory/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-05 17:35:45.894718 drive_ibd-2.7.1/drive/factory/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      385 2023-08-03 19:43:45.400117 drive_ibd-2.7.1/drive/factory/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      300 2023-05-08 16:24:50.719069 drive_ibd-2.7.1/drive/factory/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2171 2023-05-05 17:35:45.926716 drive_ibd-2.7.1/drive/factory/__pycache__/factory.cpython-310.pyc
+-rw-r--r--   0        0        0     3085 2023-08-03 19:43:45.400117 drive_ibd-2.7.1/drive/factory/__pycache__/factory.cpython-311.pyc
+-rw-r--r--   0        0        0     2160 2023-05-08 16:24:50.747068 drive_ibd-2.7.1/drive/factory/__pycache__/factory.cpython-39.pyc
+-rw-r--r--   0        0        0     1285 2023-05-05 17:35:45.942716 drive_ibd-2.7.1/drive/factory/__pycache__/loader.cpython-310.pyc
+-rw-r--r--   0        0        0     1676 2023-08-03 19:43:45.404117 drive_ibd-2.7.1/drive/factory/__pycache__/loader.cpython-311.pyc
+-rw-r--r--   0        0        0     1261 2023-05-08 16:24:50.755067 drive_ibd-2.7.1/drive/factory/__pycache__/loader.cpython-39.pyc
+-rw-r--r--   0        0        0     1529 2023-08-03 19:43:34.524379 drive_ibd-2.7.1/drive/factory/factory.py
+-rw-r--r--   0        0        0      784 2023-08-03 19:43:34.616376 drive_ibd-2.7.1/drive/factory/loader.py
+-rw-r--r--   0        0        0       30 2023-08-03 19:43:34.664375 drive_ibd-2.7.1/drive/filters/__init__.py
+-rw-r--r--   0        0        0      247 2023-08-03 19:43:45.744109 drive_ibd-2.7.1/drive/filters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      215 2023-04-14 16:20:20.729270 drive_ibd-2.7.1/drive/filters/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    19840 2024-03-20 14:54:09.155239 drive_ibd-2.7.1/drive/filters/__pycache__/filter.cpython-311.pyc
+-rw-r--r--   0        0        0     8230 2023-04-14 16:20:20.805268 drive_ibd-2.7.1/drive/filters/__pycache__/filter.cpython-39.pyc
+-rw-r--r--   0        0        0    18393 2024-04-05 15:53:55.759238 drive_ibd-2.7.1/drive/filters/filter.py
+-rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.7.1/drive/log/.git
+-rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.7.1/drive/log/.gitignore
+-rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.7.1/drive/log/README.md
+-rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.7.1/drive/log/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.7.1/drive/log/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.7.1/drive/log/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7199 2023-11-25 21:04:36.562604 drive_ibd-2.7.1/drive/log/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.7.1/drive/log/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     5031 2024-04-05 15:53:55.955235 drive_ibd-2.7.1/drive/log/logger.py
+-rw-r--r--   0        0        0      189 2023-12-15 15:59:21.176736 drive_ibd-2.7.1/drive/models/__init__.py
+-rw-r--r--   0        0        0      543 2024-01-10 18:49:23.779927 drive_ibd-2.7.1/drive/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      365 2023-04-14 16:19:50.554106 drive_ibd-2.7.1/drive/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1337 2023-08-03 19:43:45.724110 drive_ibd-2.7.1/drive/models/__pycache__/choices.cpython-311.pyc
+-rw-r--r--   0        0        0      707 2023-04-14 16:19:50.610104 drive_ibd-2.7.1/drive/models/__pycache__/choices.cpython-39.pyc
+-rw-r--r--   0        0        0     1703 2024-03-19 14:31:34.691297 drive_ibd-2.7.1/drive/models/__pycache__/data_container.cpython-311.pyc
+-rw-r--r--   0        0        0     8018 2024-03-18 13:15:51.744268 drive_ibd-2.7.1/drive/models/__pycache__/generate_indices.cpython-311.pyc
+-rw-r--r--   0        0        0     5141 2023-04-14 16:19:50.670103 drive_ibd-2.7.1/drive/models/__pycache__/generate_indices.cpython-39.pyc
+-rw-r--r--   0        0        0     3526 2023-08-03 19:43:45.728109 drive_ibd-2.7.1/drive/models/__pycache__/networks.cpython-311.pyc
+-rw-r--r--   0        0        0      988 2023-08-03 19:43:45.736109 drive_ibd-2.7.1/drive/models/__pycache__/types.cpython-311.pyc
+-rw-r--r--   0        0        0      677 2023-04-14 16:20:20.069288 drive_ibd-2.7.1/drive/models/__pycache__/types.cpython-39.pyc
+-rw-r--r--   0        0        0      697 2024-03-19 14:02:55.531225 drive_ibd-2.7.1/drive/models/data_container.py
+-rw-r--r--   0        0        0     4576 2024-03-06 22:07:36.492162 drive_ibd-2.7.1/drive/models/generate_indices.py
+-rw-r--r--   0        0        0     2161 2023-08-03 19:43:34.884370 drive_ibd-2.7.1/drive/models/networks.py
+-rw-r--r--   0        0        0      617 2023-08-03 19:43:34.908369 drive_ibd-2.7.1/drive/models/types.py
+-rw-r--r--   0        0        0        0 2023-08-03 19:43:34.908369 drive_ibd-2.7.1/drive/plugins/__init__.py
+-rw-r--r--   0        0        0      193 2023-08-08 14:49:14.259845 drive_ibd-2.7.1/drive/plugins/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5669 2024-04-05 15:49:33.478880 drive_ibd-2.7.1/drive/plugins/__pycache__/network_writer.cpython-311.pyc
+-rw-r--r--   0        0        0    14030 2024-04-05 15:49:05.867259 drive_ibd-2.7.1/drive/plugins/__pycache__/pvalues.cpython-311.pyc
+-rw-r--r--   0        0        0     4475 2024-04-05 15:32:38.137080 drive_ibd-2.7.1/drive/plugins/network_writer.py
+-rw-r--r--   0        0        0    13389 2024-04-05 15:32:28.593218 drive_ibd-2.7.1/drive/plugins/pvalues.py
+-rw-r--r--   0        0        0        3 2024-03-06 22:07:36.516162 drive_ibd-2.7.1/drive/profile.json
+-rw-r--r--   0        0        0       39 2023-12-15 15:59:21.224735 drive_ibd-2.7.1/drive/utilities/callbacks/__init__.py
+-rw-r--r--   0        0        0      268 2024-01-10 18:49:24.035923 drive_ibd-2.7.1/drive/utilities/callbacks/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1820 2024-01-10 18:49:24.067922 drive_ibd-2.7.1/drive/utilities/callbacks/__pycache__/callbacks.cpython-311.pyc
+-rw-r--r--   0        0        0     1821 2024-04-05 15:53:53.827265 drive_ibd-2.7.1/drive/utilities/callbacks/callbacks.py
+-rw-r--r--   0        0        0     2263 2023-08-03 19:43:35.044366 drive_ibd-2.7.1/drive/utilities/load_phenotypes.py
+-rw-r--r--   0        0        0      121 2023-08-03 19:43:35.076365 drive_ibd-2.7.1/drive/utilities/parser/__init__.py
+-rw-r--r--   0        0        0      373 2023-08-03 19:43:45.756109 drive_ibd-2.7.1/drive/utilities/parser/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9907 2024-04-05 15:33:30.596319 drive_ibd-2.7.1/drive/utilities/parser/__pycache__/case_file_parser.cpython-311.pyc
+-rw-r--r--   0        0        0     1483 2023-08-03 19:43:45.764109 drive_ibd-2.7.1/drive/utilities/parser/__pycache__/phenotype_descriptions_parser.cpython-311.pyc
+-rw-r--r--   0        0        0     7764 2024-04-05 15:53:53.739266 drive_ibd-2.7.1/drive/utilities/parser/case_file_parser.py
+-rw-r--r--   0        0        0      919 2023-08-03 19:43:35.156363 drive_ibd-2.7.1/drive/utilities/parser/phenotype_descriptions_parser.py
+-rw-r--r--   0        0        0     2211 2024-04-23 13:58:32.594603 drive_ibd-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 drive_ibd-2.7.1/setup.py
+-rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 drive_ibd-2.7.1/PKG-INFO
```

### Comparing `drive_ibd-2.7.0/LICENSE` & `drive_ibd-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/README.md` & `drive_ibd-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/__main__.py` & `drive_ibd-2.7.1/drive/__main__.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/cluster/cluster.py` & `drive_ibd-2.7.1/drive/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/drive.py` & `drive_ibd-2.7.1/drive/drive.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,14 @@
 
     parser.add_argument(
         "--version", action="version", version=f"%(prog)s: {version('drive-ibd')}"
     )
 
     args = parser.parse_args()
 
-    print("test")
     # getting the programs start time
     start_time = datetime.now()
 
     # We need to make sure that there is a configuration file
     json_config = args.json_config if args.json_config else find_json_file()
 
     # creating and configuring the logger and then recording user inputs
```

### Comparing `drive_ibd-2.7.0/drive/factory/factory.py` & `drive_ibd-2.7.1/drive/factory/factory.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/factory/loader.py` & `drive_ibd-2.7.1/drive/factory/loader.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/filters/filter.py` & `drive_ibd-2.7.1/drive/filters/filter.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/log/README.md` & `drive_ibd-2.7.1/drive/log/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/log/__pycache__/logger.cpython-311.pyc` & `drive_ibd-2.7.1/drive/log/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/log/__pycache__/logger.cpython-39.pyc` & `drive_ibd-2.7.1/drive/log/__pycache__/logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/log/logger.py` & `drive_ibd-2.7.1/drive/log/logger.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/models/data_container.py` & `drive_ibd-2.7.1/drive/models/data_container.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/models/generate_indices.py` & `drive_ibd-2.7.1/drive/models/generate_indices.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/models/networks.py` & `drive_ibd-2.7.1/drive/models/networks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/models/types.py` & `drive_ibd-2.7.1/drive/models/types.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/plugins/network_writer.py` & `drive_ibd-2.7.1/drive/plugins/network_writer.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/plugins/pvalues.py` & `drive_ibd-2.7.1/drive/plugins/pvalues.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/utilities/callbacks/callbacks.py` & `drive_ibd-2.7.1/drive/utilities/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/utilities/load_phenotypes.py` & `drive_ibd-2.7.1/drive/utilities/load_phenotypes.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/utilities/parser/case_file_parser.py` & `drive_ibd-2.7.1/drive/utilities/parser/case_file_parser.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/drive/utilities/parser/phenotype_descriptions_parser.py` & `drive_ibd-2.7.1/drive/utilities/parser/phenotype_descriptions_parser.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.7.0/pyproject.toml` & `drive_ibd-2.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "drive-ibd"
 
-version = "2.7.0"
+version = "2.7.1"
 description = "cli tool to identify networks of individuals who share IBD segments overlapping loci of interest"
 authors = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>", "Jennifer E. Below <jennifer.e.below@vumc.org>"]
 maintainers = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>"]
 repository = "https://github.com/belowlab/drive"
 homepage = "https://drive-ibd.readthedocs.io/en/latest/"
 readme = "README.md"
 keywords = ["python", "genetics", "identity by descent", "relatedness"]
```

### Comparing `drive_ibd-2.7.0/setup.py` & `drive_ibd-2.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'scipy>=1.10.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['drive = drive.drive:main']}
 
 setup_kwargs = {
     'name': 'drive-ibd',
-    'version': '2.7.0',
+    'version': '2.7.1',
     'description': 'cli tool to identify networks of individuals who share IBD segments overlapping loci of interest',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/drive-ibd/badge/?version=latest)](https://drive-ibd.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI version](https://badge.fury.io/py/drive-ibd.svg)](https://badge.fury.io/py/drive-ibd)\n\n# DRIVE:\n\nThis repository contains the source code for the tool DRIVE (Distant Relatedness for Identification and Variant Evaluation) is a novel approach to IBD-based genotype inference used to identify shared chromosomal segments in dense genetic arrays. DRIVE implements a random walk algorithm that identifies clusters of individuals who pairwise share an IBD segment overlapping a locus of interest. This tool was developed in python by the Below Lab at Vanderbilt University. The documentation for how to use this tool can be found here [DRIVE documentation](https://drive-ibd.readthedocs.io/en/latest/)\n\n## Installing DRIVE:\nDRIVE is available on PYPI and can easily be installed using the following command:\n\n```bash\npip install drive-ibd\n```\nIt is recommended to install DRIVE within a virtual environment such as venv, or conda. More information about this process can be found within the documentation.\n\nIf the user wishes to develop DRIVE or install the program from source then they can clone the repository. This process is described under the section called "Github Installation" in the documentation.\n\n### Reporting issues:\nIf you wish to report a bug or propose a feature you can find templates under the .github/ISSUE_TEMPLATE directory.\n\n',
     'author': 'James Baker',
     'author_email': 'james.baker@vanderbilt.edu',
     'maintainer': 'James Baker',
     'maintainer_email': 'james.baker@vanderbilt.edu',
     'url': 'https://drive-ibd.readthedocs.io/en/latest/',
```

### Comparing `drive_ibd-2.7.0/PKG-INFO` & `drive_ibd-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drive-ibd
-Version: 2.7.0
+Version: 2.7.1
 Summary: cli tool to identify networks of individuals who share IBD segments overlapping loci of interest
 Home-page: https://drive-ibd.readthedocs.io/en/latest/
 Keywords: python,genetics,identity by descent,relatedness
 Author: James Baker
 Author-email: james.baker@vanderbilt.edu
 Maintainer: James Baker
 Maintainer-email: james.baker@vanderbilt.edu
```

