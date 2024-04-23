# Comparing `tmp/SplatStats-4.2.1.tar.gz` & `tmp/SplatStats-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-4.2.1.tar", last modified: Thu Apr 18 16:39:18 2024, max compression
+gzip compressed data, was "SplatStats-4.2.2.tar", last modified: Tue Apr 23 02:52:40 2024, max compression
```

## Comparing `SplatStats-4.2.1.tar` & `SplatStats-4.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-04-18 16:39:18.706938 SplatStats-4.2.1/
--rw-r--r--   0 chipdelmal   (501) staff       (20)    35149 2024-02-19 02:43:58.000000 SplatStats-4.2.1/LICENSE
--rw-r--r--   0 chipdelmal   (501) staff       (20)     7221 2024-04-18 16:39:18.706619 SplatStats-4.2.1/PKG-INFO
--rw-r--r--   0 chipdelmal   (501) staff       (20)     6370 2024-02-19 02:43:58.000000 SplatStats-4.2.1/README.md
-drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-04-18 16:39:18.705056 SplatStats-4.2.1/SplatStats/
--rw-r--r--   0 chipdelmal   (501) staff       (20)    10828 2024-02-19 02:43:58.000000 SplatStats-4.2.1/SplatStats/Battle.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    11409 2024-02-28 02:56:43.000000 SplatStats-4.2.1/SplatStats/Player.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     3107 2024-02-28 03:12:16.000000 SplatStats-4.2.1/SplatStats/StatInk.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     2477 2024-02-19 02:43:58.000000 SplatStats-4.2.1/SplatStats/Team.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)      896 2024-02-19 02:43:58.000000 SplatStats-4.2.1/SplatStats/__init__.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)       21 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats/_version.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     6148 2024-02-19 02:43:58.000000 SplatStats-4.2.1/SplatStats/auxiliary.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    14521 2024-02-21 04:08:00.000000 SplatStats-4.2.1/SplatStats/colors.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     6156 2024-03-01 03:27:11.000000 SplatStats-4.2.1/SplatStats/constants.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     4137 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/files.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    11074 2024-03-25 03:13:54.000000 SplatStats-4.2.1/SplatStats/parsers.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    59659 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/plots.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1428 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/plotsAux.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1707 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/plotsTeam.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    13586 2024-03-07 23:48:07.000000 SplatStats-4.2.1/SplatStats/statInkConstants.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    10922 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/statInkPlots.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)     8511 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/statInkStats.py
--rw-r--r--   0 chipdelmal   (501) staff       (20)    15022 2024-02-19 02:43:59.000000 SplatStats-4.2.1/SplatStats/stats.py
-drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-04-18 16:39:18.705894 SplatStats-4.2.1/SplatStats.egg-info/
--rw-r--r--   0 chipdelmal   (501) staff       (20)     7221 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats.egg-info/PKG-INFO
--rw-r--r--   0 chipdelmal   (501) staff       (20)      607 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats.egg-info/SOURCES.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)        1 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats.egg-info/dependency_links.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)      159 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats.egg-info/requires.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)       11 2024-04-18 16:39:18.000000 SplatStats-4.2.1/SplatStats.egg-info/top_level.txt
--rw-r--r--   0 chipdelmal   (501) staff       (20)       38 2024-04-18 16:39:18.707007 SplatStats-4.2.1/setup.cfg
--rw-r--r--   0 chipdelmal   (501) staff       (20)     1251 2024-02-19 02:43:59.000000 SplatStats-4.2.1/setup.py
+drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-04-23 02:52:40.456974 SplatStats-4.2.2/
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    35149 2024-02-19 02:43:58.000000 SplatStats-4.2.2/LICENSE
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     7221 2024-04-23 02:52:40.456686 SplatStats-4.2.2/PKG-INFO
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     6370 2024-02-19 02:43:58.000000 SplatStats-4.2.2/README.md
+drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-04-23 02:52:40.454873 SplatStats-4.2.2/SplatStats/
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    10828 2024-02-19 02:43:58.000000 SplatStats-4.2.2/SplatStats/Battle.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    11409 2024-02-28 02:56:43.000000 SplatStats-4.2.2/SplatStats/Player.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     3107 2024-02-28 03:12:16.000000 SplatStats-4.2.2/SplatStats/StatInk.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     2477 2024-02-19 02:43:58.000000 SplatStats-4.2.2/SplatStats/Team.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)      896 2024-02-19 02:43:58.000000 SplatStats-4.2.2/SplatStats/__init__.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)       21 2024-04-23 02:52:40.000000 SplatStats-4.2.2/SplatStats/_version.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     6148 2024-02-19 02:43:58.000000 SplatStats-4.2.2/SplatStats/auxiliary.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    14521 2024-02-21 04:08:00.000000 SplatStats-4.2.2/SplatStats/colors.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     6156 2024-03-01 03:27:11.000000 SplatStats-4.2.2/SplatStats/constants.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     4137 2024-02-19 02:43:59.000000 SplatStats-4.2.2/SplatStats/files.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    11074 2024-03-25 03:13:54.000000 SplatStats-4.2.2/SplatStats/parsers.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    59659 2024-02-19 02:43:59.000000 SplatStats-4.2.2/SplatStats/plots.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1428 2024-02-19 02:43:59.000000 SplatStats-4.2.2/SplatStats/plotsAux.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1707 2024-02-19 02:43:59.000000 SplatStats-4.2.2/SplatStats/plotsTeam.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    13585 2024-04-21 15:57:47.000000 SplatStats-4.2.2/SplatStats/statInkConstants.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    10922 2024-02-19 02:43:59.000000 SplatStats-4.2.2/SplatStats/statInkPlots.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     8511 2024-02-19 02:43:59.000000 SplatStats-4.2.2/SplatStats/statInkStats.py
+-rw-r--r--   0 chipdelmal   (501) staff       (20)    15022 2024-02-19 02:43:59.000000 SplatStats-4.2.2/SplatStats/stats.py
+drwxr-xr-x   0 chipdelmal   (501) staff       (20)        0 2024-04-23 02:52:40.455891 SplatStats-4.2.2/SplatStats.egg-info/
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     7221 2024-04-23 02:52:40.000000 SplatStats-4.2.2/SplatStats.egg-info/PKG-INFO
+-rw-r--r--   0 chipdelmal   (501) staff       (20)      607 2024-04-23 02:52:40.000000 SplatStats-4.2.2/SplatStats.egg-info/SOURCES.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)        1 2024-04-23 02:52:40.000000 SplatStats-4.2.2/SplatStats.egg-info/dependency_links.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)      159 2024-04-23 02:52:40.000000 SplatStats-4.2.2/SplatStats.egg-info/requires.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)       11 2024-04-23 02:52:40.000000 SplatStats-4.2.2/SplatStats.egg-info/top_level.txt
+-rw-r--r--   0 chipdelmal   (501) staff       (20)       38 2024-04-23 02:52:40.457027 SplatStats-4.2.2/setup.cfg
+-rw-r--r--   0 chipdelmal   (501) staff       (20)     1251 2024-02-19 02:43:59.000000 SplatStats-4.2.2/setup.py
```

### Comparing `SplatStats-4.2.1/LICENSE` & `SplatStats-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/PKG-INFO` & `SplatStats-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 4.2.1
+Version: 4.2.2
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-4.2.1/README.md` & `SplatStats-4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/Battle.py` & `SplatStats-4.2.2/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/Player.py` & `SplatStats-4.2.2/SplatStats/Player.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/StatInk.py` & `SplatStats-4.2.2/SplatStats/StatInk.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/Team.py` & `SplatStats-4.2.2/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/__init__.py` & `SplatStats-4.2.2/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/auxiliary.py` & `SplatStats-4.2.2/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/colors.py` & `SplatStats-4.2.2/SplatStats/colors.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/constants.py` & `SplatStats-4.2.2/SplatStats/constants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/files.py` & `SplatStats-4.2.2/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/parsers.py` & `SplatStats-4.2.2/SplatStats/parsers.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/plots.py` & `SplatStats-4.2.2/SplatStats/plots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/plotsAux.py` & `SplatStats-4.2.2/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/plotsTeam.py` & `SplatStats-4.2.2/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/statInkConstants.py` & `SplatStats-4.2.2/SplatStats/statInkConstants.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
   'lact450_deco': 'REEF-LUX 450 Deco',
   'order_stringer_replica': 'Order Stringer Replica',
   'tristringer': 'Tri-Stringer',
   'tristringer_collabo': 'Inkline Tri-Stringer'
 }
 WPNS_REPLICAS = (
   ('Hero Shot Replica', 'Splattershot'),
-  ('Octo Shot Replica', 'Tenktatek Splattershot'),
+  ('Octo Shot Replica', 'Tentatek Splattershot'),
   ('Order Shot Replica', 'Splattershot'),
   ('Order Blaster Replica', 'Luna Blaster'),
   ('Order Dualie Replicas', 'Splat Dualies'),
   ('Order Roller Replica', 'Splat Roller'),
   ('Orderbrush Replica', 'Octobrush'),
   ('Order Splatana Replica', 'Splatana Stamper'),
   ('Order Charger Replica', 'Splat Charger'),
```

### Comparing `SplatStats-4.2.1/SplatStats/statInkPlots.py` & `SplatStats-4.2.2/SplatStats/statInkPlots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/statInkStats.py` & `SplatStats-4.2.2/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats/stats.py` & `SplatStats-4.2.2/SplatStats/stats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/SplatStats.egg-info/PKG-INFO` & `SplatStats-4.2.2/SplatStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 4.2.1
+Version: 4.2.2
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-4.2.1/SplatStats.egg-info/SOURCES.txt` & `SplatStats-4.2.2/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-4.2.1/setup.py` & `SplatStats-4.2.2/setup.py`

 * *Files identical despite different names*

