# Comparing `tmp/gridengine_framework-0.8.1.tar.gz` & `tmp/gridengine_framework-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridengine_framework-0.8.1.tar", last modified: Mon Apr 22 06:10:57 2024, max compression
+gzip compressed data, was "gridengine_framework-0.8.2.tar", last modified: Tue Apr 23 10:45:40 2024, max compression
```

## Comparing `gridengine_framework-0.8.1.tar` & `gridengine_framework-0.8.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.912455 gridengine_framework-0.8.1/
--rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.8.1/LICENSE
--rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 06:10:57.912455 gridengine_framework-0.8.1/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     5278 2023-11-02 07:42:03.000000 gridengine_framework-0.8.1/README.md
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.909122 gridengine_framework-0.8.1/grid_engine/
--rw-r--r--   0 boss      (1000) boss      (1002)      135 2023-11-25 03:11:25.000000 gridengine_framework-0.8.1/grid_engine/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     1293 2023-11-28 08:03:58.000000 gridengine_framework-0.8.1/grid_engine/__log__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4931 2023-12-10 21:45:39.000000 gridengine_framework-0.8.1/grid_engine/__main__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.909122 gridengine_framework-0.8.1/grid_engine/_blueprint/
--rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.8.1/grid_engine/_blueprint/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3624 2024-04-22 04:56:11.000000 gridengine_framework-0.8.1/grid_engine/_blueprint/__main__.py
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2024-01-11 22:32:29.000000 gridengine_framework-0.8.1/grid_engine/_blueprint/_floorplan_classes.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5608 2024-02-11 03:43:12.000000 gridengine_framework-0.8.1/grid_engine/_blueprint/_floorplan_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)    17503 2024-04-22 05:11:05.000000 gridengine_framework-0.8.1/grid_engine/_blueprint/_grid_blueprint.py
--rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-02-12 03:03:41.000000 gridengine_framework-0.8.1/grid_engine/_blueprint/_grid_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)    10946 2024-04-22 05:08:00.000000 gridengine_framework-0.8.1/grid_engine/_blueprint/_terrain_processing.py
--rw-r--r--   0 boss      (1000) boss      (1002)      272 2024-04-22 02:43:45.000000 gridengine_framework-0.8.1/grid_engine/_blueprint/objects.json
--rw-r--r--   0 boss      (1000) boss      (1002)     1615 2024-04-22 04:53:36.000000 gridengine_framework-0.8.1/grid_engine/_blueprint/terrains.json
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.909122 gridengine_framework-0.8.1/grid_engine/_cell/
--rw-r--r--   0 boss      (1000) boss      (1002)       22 2024-04-22 05:54:10.000000 gridengine_framework-0.8.1/grid_engine/_cell/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    32374 2024-04-22 05:54:03.000000 gridengine_framework-0.8.1/grid_engine/_cell/cell.py
--rw-r--r--   0 boss      (1000) boss      (1002)     4756 2023-11-25 03:11:01.000000 gridengine_framework-0.8.1/grid_engine/_dungeon.py
--rw-r--r--   0 boss      (1000) boss      (1002)    54747 2024-04-22 06:08:51.000000 gridengine_framework-0.8.1/grid_engine/_grid.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.909122 gridengine_framework-0.8.1/grid_engine/_grid_feature/
--rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.8.1/grid_engine/_grid_feature/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2442 2023-10-31 05:21:50.000000 gridengine_framework-0.8.1/grid_engine/_grid_feature/grid_feature.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.909122 gridengine_framework-0.8.1/grid_engine/_grid_group/
--rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-22 06:07:32.000000 gridengine_framework-0.8.1/grid_engine/_grid_group/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     3642 2023-10-31 05:21:50.000000 gridengine_framework-0.8.1/grid_engine/_grid_group/grid_group.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.909122 gridengine_framework-0.8.1/grid_engine/_grid_object/
--rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.8.1/grid_engine/_grid_object/__init__.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.909122 gridengine_framework-0.8.1/grid_engine/_grid_object/grid_item/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.1/grid_engine/_grid_object/grid_item/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.8.1/grid_engine/_grid_object/grid_item/grid_item.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2283 2023-11-12 05:05:46.000000 gridengine_framework-0.8.1/grid_engine/_grid_object/grid_object.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.909122 gridengine_framework-0.8.1/grid_engine/_grid_object/grid_structure/
--rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.8.1/grid_engine/_grid_object/grid_structure/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.8.1/grid_engine/_grid_object/grid_structure/grid_structure.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.909122 gridengine_framework-0.8.1/grid_engine/_grid_object/grid_zone/
--rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.1/grid_engine/_grid_object/grid_zone/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.8.1/grid_engine/_grid_object/grid_zone/grid_zone.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.912455 gridengine_framework-0.8.1/grid_engine/_terraform/
--rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.8.1/grid_engine/_terraform/__init__.py
--rw-r--r--   0 boss      (1000) boss      (1002)    11795 2024-04-22 06:10:43.000000 gridengine_framework-0.8.1/grid_engine/_terraform/terraformer.py
--rw-r--r--   0 boss      (1000) boss      (1002)     5714 2024-02-24 16:00:59.000000 gridengine_framework-0.8.1/grid_engine/_utility.py
--rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-02-12 03:13:00.000000 gridengine_framework-0.8.1/grid_engine/layout_test.py
-drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-22 06:10:57.912455 gridengine_framework-0.8.1/gridengine_framework.egg-info/
--rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-22 06:10:57.000000 gridengine_framework-0.8.1/gridengine_framework.egg-info/PKG-INFO
--rw-r--r--   0 boss      (1000) boss      (1002)     1439 2024-04-22 06:10:57.000000 gridengine_framework-0.8.1/gridengine_framework.egg-info/SOURCES.txt
--rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-04-22 06:10:57.000000 gridengine_framework-0.8.1/gridengine_framework.egg-info/dependency_links.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-22 06:10:57.000000 gridengine_framework-0.8.1/gridengine_framework.egg-info/requires.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-04-22 06:10:57.000000 gridengine_framework-0.8.1/gridengine_framework.egg-info/top_level.txt
--rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-04-22 06:10:57.912455 gridengine_framework-0.8.1/setup.cfg
--rw-r--r--   0 boss      (1000) boss      (1002)      903 2024-04-22 06:10:48.000000 gridengine_framework-0.8.1/setup.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/
+-rw-r--r--   0 boss      (1000) boss      (1002)     1068 2023-10-14 02:22:20.000000 gridengine_framework-0.8.2/LICENSE
+-rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     5278 2023-11-02 07:42:03.000000 gridengine_framework-0.8.2/README.md
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.402058 gridengine_framework-0.8.2/grid_engine/
+-rw-r--r--   0 boss      (1000) boss      (1002)      135 2023-11-25 03:11:25.000000 gridengine_framework-0.8.2/grid_engine/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     1293 2023-11-28 08:03:58.000000 gridengine_framework-0.8.2/grid_engine/__log__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4931 2023-12-10 21:45:39.000000 gridengine_framework-0.8.2/grid_engine/__main__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/grid_engine/_blueprint/
+-rw-r--r--   0 boss      (1000) boss      (1002)      127 2023-11-10 05:29:28.000000 gridengine_framework-0.8.2/grid_engine/_blueprint/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3624 2024-04-22 04:56:11.000000 gridengine_framework-0.8.2/grid_engine/_blueprint/__main__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2024-01-11 22:32:29.000000 gridengine_framework-0.8.2/grid_engine/_blueprint/_floorplan_classes.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5608 2024-02-11 03:43:12.000000 gridengine_framework-0.8.2/grid_engine/_blueprint/_floorplan_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    17503 2024-04-22 05:11:05.000000 gridengine_framework-0.8.2/grid_engine/_blueprint/_grid_blueprint.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    18503 2024-02-12 03:03:41.000000 gridengine_framework-0.8.2/grid_engine/_blueprint/_grid_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    10946 2024-04-22 05:08:00.000000 gridengine_framework-0.8.2/grid_engine/_blueprint/_terrain_processing.py
+-rw-r--r--   0 boss      (1000) boss      (1002)      272 2024-04-22 02:43:45.000000 gridengine_framework-0.8.2/grid_engine/_blueprint/objects.json
+-rw-r--r--   0 boss      (1000) boss      (1002)     1615 2024-04-22 04:53:36.000000 gridengine_framework-0.8.2/grid_engine/_blueprint/terrains.json
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/grid_engine/_cell/
+-rw-r--r--   0 boss      (1000) boss      (1002)       22 2024-04-22 05:54:10.000000 gridengine_framework-0.8.2/grid_engine/_cell/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    32407 2024-04-23 10:41:35.000000 gridengine_framework-0.8.2/grid_engine/_cell/cell.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     4756 2023-11-25 03:11:01.000000 gridengine_framework-0.8.2/grid_engine/_dungeon.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    54746 2024-04-23 10:41:49.000000 gridengine_framework-0.8.2/grid_engine/_grid.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/grid_engine/_grid_feature/
+-rw-r--r--   0 boss      (1000) boss      (1002)        0 2023-10-31 05:21:50.000000 gridengine_framework-0.8.2/grid_engine/_grid_feature/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2442 2023-10-31 05:21:50.000000 gridengine_framework-0.8.2/grid_engine/_grid_feature/grid_feature.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/grid_engine/_grid_group/
+-rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-22 06:07:32.000000 gridengine_framework-0.8.2/grid_engine/_grid_group/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     3648 2024-04-23 10:20:01.000000 gridengine_framework-0.8.2/grid_engine/_grid_group/grid_group.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/grid_engine/_grid_object/
+-rw-r--r--   0 boss      (1000) boss      (1002)      106 2023-10-31 05:21:50.000000 gridengine_framework-0.8.2/grid_engine/_grid_object/__init__.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/grid_engine/_grid_object/grid_item/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.2/grid_engine/_grid_object/grid_item/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2335 2023-11-05 11:27:17.000000 gridengine_framework-0.8.2/grid_engine/_grid_object/grid_item/grid_item.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2283 2023-11-12 05:05:46.000000 gridengine_framework-0.8.2/grid_engine/_grid_object/grid_object.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/grid_engine/_grid_object/grid_structure/
+-rw-r--r--   0 boss      (1000) boss      (1002)       29 2023-10-31 05:21:50.000000 gridengine_framework-0.8.2/grid_engine/_grid_object/grid_structure/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2216 2023-10-31 05:21:50.000000 gridengine_framework-0.8.2/grid_engine/_grid_object/grid_structure/grid_structure.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/grid_engine/_grid_object/grid_zone/
+-rw-r--r--   0 boss      (1000) boss      (1002)       24 2023-10-31 05:21:50.000000 gridengine_framework-0.8.2/grid_engine/_grid_object/grid_zone/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5023 2023-11-05 11:55:55.000000 gridengine_framework-0.8.2/grid_engine/_grid_object/grid_zone/grid_zone.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/grid_engine/_terraform/
+-rw-r--r--   0 boss      (1000) boss      (1002)       36 2023-10-31 05:21:50.000000 gridengine_framework-0.8.2/grid_engine/_terraform/__init__.py
+-rw-r--r--   0 boss      (1000) boss      (1002)    13290 2024-04-23 10:43:30.000000 gridengine_framework-0.8.2/grid_engine/_terraform/terraformer.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     5714 2024-02-24 16:00:59.000000 gridengine_framework-0.8.2/grid_engine/_utility.py
+-rw-r--r--   0 boss      (1000) boss      (1002)     2925 2024-02-12 03:13:00.000000 gridengine_framework-0.8.2/grid_engine/layout_test.py
+drwxr-xr-x   0 boss      (1000) boss      (1002)        0 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/gridengine_framework.egg-info/
+-rw-r--r--   0 boss      (1000) boss      (1002)     5810 2024-04-23 10:45:40.000000 gridengine_framework-0.8.2/gridengine_framework.egg-info/PKG-INFO
+-rw-r--r--   0 boss      (1000) boss      (1002)     1439 2024-04-23 10:45:40.000000 gridengine_framework-0.8.2/gridengine_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)        1 2024-04-23 10:45:40.000000 gridengine_framework-0.8.2/gridengine_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       33 2024-04-23 10:45:40.000000 gridengine_framework-0.8.2/gridengine_framework.egg-info/requires.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       12 2024-04-23 10:45:40.000000 gridengine_framework-0.8.2/gridengine_framework.egg-info/top_level.txt
+-rw-r--r--   0 boss      (1000) boss      (1002)       38 2024-04-23 10:45:40.405391 gridengine_framework-0.8.2/setup.cfg
+-rw-r--r--   0 boss      (1000) boss      (1002)      903 2024-04-23 10:45:30.000000 gridengine_framework-0.8.2/setup.py
```

### Comparing `gridengine_framework-0.8.1/LICENSE` & `gridengine_framework-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/PKG-INFO` & `gridengine_framework-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridengine_framework
-Version: 0.8.1
+Version: 0.8.2
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gridengine_framework-0.8.1/README.md` & `gridengine_framework-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/__log__.py` & `gridengine_framework-0.8.2/grid_engine/__log__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/__main__.py` & `gridengine_framework-0.8.2/grid_engine/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_blueprint/__main__.py` & `gridengine_framework-0.8.2/grid_engine/_blueprint/__main__.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_blueprint/_floorplan_processing.py` & `gridengine_framework-0.8.2/grid_engine/_blueprint/_floorplan_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_blueprint/_grid_blueprint.py` & `gridengine_framework-0.8.2/grid_engine/_blueprint/_grid_blueprint.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_blueprint/_grid_processing.py` & `gridengine_framework-0.8.2/grid_engine/_blueprint/_grid_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_blueprint/_terrain_processing.py` & `gridengine_framework-0.8.2/grid_engine/_blueprint/_terrain_processing.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_blueprint/terrains.json` & `gridengine_framework-0.8.2/grid_engine/_blueprint/terrains.json`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_cell/cell.py` & `gridengine_framework-0.8.2/grid_engine/_cell/cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     @property
     def down_left(self):
         """Returns the cell adjacent in the down-left direction"""
         if self.row == self.parentgrid.last_row or self.col == self.parentgrid.first_col:
             self._down_left = None
         else:
             self._down_left = self.parentgrid[self.adjacent[6]]
-            self._down_left = self.parentgrid.get_cell_by_position(self.x - self.size, self.y - self.size)
+            # self._down_left = self.parentgrid.get_cell_by_position(self.x - self.size, self.y - self.size)
         return self._down_left
 
     @property
     def clearance_down(self):
         """Returns the number of cells in the down direction that are passable"""
         if self.row == self.parentgrid.last_row:
             self._clearance_down = 0
@@ -653,25 +653,28 @@
             xaxis (int): -1 for left, 1 for right
             yaxis (int): -1 for down, 1 for up
             distance (int): The distance in cells of the diagonal
             
         Returns:
             GridGroup: The diagonal of the cell
         """
-        diagonal = GridGroup(self.parentgrid, f'{self.designation}_diagonal', [])
+        diagonal = []
         queue = deque([self])
         ys = [None, 'up', 'down']
         xs = [None, 'right', 'left']
         y = ys[yaxis]
         x = xs[xaxis]
         for _ in range(distance):
             current_cell = queue.popleft()
             cell = getattr(current_cell, f'{y}_{x}')
-            diagonal.add_cell(cell)
-            queue.append(cell)
+            if cell is not None:
+                diagonal.append(cell.designation)
+                queue.append(cell)
+            else:
+                break
         return diagonal
     
     def recv_occupant(self, occupant):
         """
         Receives an occupant signal from a GridEntity. 
         Triggers the dispatcher for the 'on_vacate' event if the cell is occupied 
         and the value of occupant is the same as the value of self.occupant.
```

### Comparing `gridengine_framework-0.8.1/grid_engine/_dungeon.py` & `gridengine_framework-0.8.2/grid_engine/_dungeon.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_grid.py` & `gridengine_framework-0.8.2/grid_engine/_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -492,15 +492,15 @@
             self.lake_count = len(self.lakes)
             self._set_water_cells()
             self.river_count = 0
             self.rivers: list[list[_Cell,]] = []
             self._terraformer = Terraformer(self)
             self.terraformer.set_rivers(2)
             self._fix_minute_water_bodies()
-            self.terraformer.set_forests()
+            self.terraformer.set_forest()
 
         # self.town = GridZone(self, 'Town', 'town', self.random_cell(attr=('passable', True)), (45, 45, 45), 2)
 
     def _size_warning(self, cell_count):
         import colorama
         quit = input(
             f'{colorama.Fore.RED}WARNING{colorama.Fore.RESET}: The provided parameters will generate a grid composed '
```

### Comparing `gridengine_framework-0.8.1/grid_engine/_grid_feature/grid_feature.py` & `gridengine_framework-0.8.2/grid_engine/_grid_feature/grid_feature.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_grid_group/grid_group.py` & `gridengine_framework-0.8.2/grid_engine/_grid_group/grid_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.initiate_group()
 
     def initiate_group(self):
         """Adds the group to the cells in the group."""
         for cell in self.cells:
             cell.join_group(self.title, self)
 
-    def add_cell(self, cell):
+    def add_cell(self, cell: Cell):
         """Adds a cell to the group and adds the group to the cell."""
 
         self.cells.append(cell)
         cell.join_group(self.title, self)
 
     def in_group(self, cell: _Union[str, Cell]):
         """Checks if a cell is in the group"""
```

### Comparing `gridengine_framework-0.8.1/grid_engine/_grid_object/grid_item/grid_item.py` & `gridengine_framework-0.8.2/grid_engine/_grid_object/grid_item/grid_item.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_grid_object/grid_object.py` & `gridengine_framework-0.8.2/grid_engine/_grid_object/grid_object.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_grid_object/grid_structure/grid_structure.py` & `gridengine_framework-0.8.2/grid_engine/_grid_object/grid_structure/grid_structure.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_grid_object/grid_zone/grid_zone.py` & `gridengine_framework-0.8.2/grid_engine/_grid_object/grid_zone/grid_zone.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/_terraform/terraformer.py` & `gridengine_framework-0.8.2/grid_engine/_terraform/terraformer.py`

 * *Files 16% similar despite different names*

```diff
@@ -241,30 +241,63 @@
             print(f'Start cell: {start}, End cell: {end}')
             print('Building river ...')
             self.generate_realistic_river(start.designation, end.designation)
         riverbanks = self.get_river_banks()
         self.expand_riverbanks(riverbanks)
         print('done')            
  
-    def set_forests(self, forest_count=1):
-        for forest in range(forest_count):
-            center = self.grid.random_cell(('passable', True))
-            while center.clearance_y < 5 or center.clearance_x < 5:
-                center = self.grid.random_cell(('passable', True))
-            area = self.grid.get_area(center, 4)
-            for cell in area:
-                cell.terrain_str = 'FOREST'
-                cell.terrain_char = '^'
-                cell.terrain_raw = 0.0
-                cell.terrain_int = None
-                cell.terrain_color = 'GRASS_GREEN'
-                cell._cost_in = 2
-                cell._cost_out = 2
-                self.dictTerrain[cell.designation] = {
-                    'str': cell.terrain_str, 
-                    'raw': cell.terrain_raw, 
-                    'int': cell.terrain_int, 
-                    'color': cell.terrain_color, 
-                    'cost_in': cell.cost_in, 
-                    'cost_out': cell.cost_out
-                    }
-                
+    def seed_forest(self):
+        start_cell = self.grid.random_cell()
+        while start_cell.clearance_x < 10 or start_cell.clearance_y < 10:
+            start_cell = self.grid.random_cell()
+        return start_cell
+ 
+    def get_forest_borders(self, start_cells: Union[Cell, List[Cell]]):
+        forest_border_start = start_cells.get_diagonal(-1, -1, random.randint(1, 5))[-1]
+        forest_border_step2 = start_cells.get_diagonal(-1, 1, random.randint(1, 5))[-1]
+        forest_border_step3 = start_cells.get_diagonal(1, 1, random.randint(1, 5))[-1]
+        forest_border_step4 = start_cells.get_diagonal(1, -1, random.randint(1, 5))[-1]
+        forest_border = []
+        step1 = self.grid.get_walk(forest_border_start, forest_border_step2)
+        forest_border.extend(step1)
+        step2 = self.grid.get_walk(forest_border_step2, forest_border_step3)
+        forest_border.extend(step2)
+        step3 = self.grid.get_walk(forest_border_step3, forest_border_step4)
+        forest_border.extend(step3)
+        step4 = self.grid.get_walk(forest_border_step4, forest_border_start)
+        forest_border.extend(step4)
+        return forest_border
+        
+    def get_inner_forest_cells(self, start_cell, forest_border):
+        for cell in forest_border:
+            self.grid[cell].passable = False
+        inner_forest_cells = start_cell.get_clearance_zone()
+        inner_forest_cells = inner_forest_cells.cells
+        for cell in forest_border:
+            self.grid[cell].passable = True
+        forest_cells = []
+        forest_cells.extend(forest_border)
+        for cell in inner_forest_cells:
+            forest_cells.append(cell.designation)
+        return forest_cells
+    
+    def set_forest(self):
+        start_cells = self.seed_forest()
+        forest_borders = self.get_forest_borders(start_cells)
+        forest_cells = self.get_inner_forest_cells(start_cells, forest_borders)
+        for cell in forest_cells:
+            cell = self.grid[cell]
+            cell.terrain_str = 'FOREST'
+            cell.terrain_raw = 0.0
+            cell.terrain_int = 4
+            cell.terrain_color = 'GRASS_GREEN'
+            cell.terrain_char = '^'
+            self.dictTerrain[cell.designation] = {
+                'str': cell.terrain_str, 
+                'raw': cell.terrain_raw, 
+                'int': cell.terrain_int, 
+                'color': cell.terrain_color, 
+                'cost_in': 2, 
+                'cost_out': 2,
+                'char': '^'
+                }
+
```

### Comparing `gridengine_framework-0.8.1/grid_engine/_utility.py` & `gridengine_framework-0.8.2/grid_engine/_utility.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/grid_engine/layout_test.py` & `gridengine_framework-0.8.2/grid_engine/layout_test.py`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/gridengine_framework.egg-info/PKG-INFO` & `gridengine_framework-0.8.2/gridengine_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridengine-framework
-Version: 0.8.1
+Version: 0.8.2
 Summary: A framework for generating and manipulating grid-based game worlds
 Home-page: https://github.com/primal-coder/grid-engine
 Author: James Evans
 Author-email: joesaysahoy@gmail.com
 Keywords: game development 2d grid world generation procedural generation cell numpy pillow pyglet pymunk cli
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gridengine_framework-0.8.1/gridengine_framework.egg-info/SOURCES.txt` & `gridengine_framework-0.8.2/gridengine_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gridengine_framework-0.8.1/setup.py` & `gridengine_framework-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
     
 setup(
     name='gridengine_framework',
-    version='0.8.1',
+    version='0.8.2',
     description='A framework for generating and manipulating grid-based game worlds',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='James Evans',
     author_email='joesaysahoy@gmail.com',
     url='https://github.com/primal-coder/grid-engine',
     packages=find_packages(),
```

