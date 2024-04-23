# Comparing `tmp/danecode-0.2.8.tar.gz` & `tmp/danecode-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danecode-0.2.8.tar", last modified: Fri Mar  1 00:10:32 2024, max compression
+gzip compressed data, was "danecode-0.2.9.tar", last modified: Tue Mar 12 03:01:54 2024, max compression
```

## Comparing `danecode-0.2.8.tar` & `danecode-0.2.9.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 00:10:32.482244 danecode-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-01 00:10:28.000000 danecode-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-01 00:10:32.482244 danecode-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-01 00:10:28.000000 danecode-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 00:10:32.474244 danecode-0.2.8/danecode/
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54064 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/country_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 00:10:32.474244 danecode-0.2.8/danecode/files/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 00:10:32.482244 danecode-0.2.8/danecode/files/centros_poblados/
--rw-r--r--   0 runner    (1001) docker     (127)    41273 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/05.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/08.csv
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/11.csv
--rw-r--r--   0 runner    (1001) docker     (127)    27250 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/13.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/15.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/17.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/18.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20822 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/19.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/20.csv
--rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/23.csv
--rw-r--r--   0 runner    (1001) docker     (127)    27725 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/25.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18594 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/27.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9881 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/41.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/44.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/47.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/50.csv
--rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/52.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/54.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/63.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/66.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/68.csv
--rw-r--r--   0 runner    (1001) docker     (127)    19374 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/70.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/73.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33434 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/76.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/81.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/85.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/86.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/88.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/91.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/94.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/95.csv
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/97.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/centros_poblados/99.csv
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/files/departamentos.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 00:10:32.482244 danecode-0.2.8/danecode/services/
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-01 00:10:28.000000 danecode-0.2.8/danecode/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 00:10:32.482244 danecode-0.2.8/danecode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-01 00:10:32.000000 danecode-0.2.8/danecode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-03-01 00:10:32.000000 danecode-0.2.8/danecode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 00:10:32.000000 danecode-0.2.8/danecode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-01 00:10:32.000000 danecode-0.2.8/danecode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-01 00:10:32.000000 danecode-0.2.8/danecode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 00:10:32.482244 danecode-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-01 00:10:28.000000 danecode-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:01:54.323229 danecode-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-12 03:01:50.000000 danecode-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-12 03:01:54.323229 danecode-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-12 03:01:50.000000 danecode-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:01:54.315229 danecode-0.2.9/danecode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54064 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/country_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:01:54.315229 danecode-0.2.9/danecode/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:01:54.323229 danecode-0.2.9/danecode/files/centros_poblados/
+-rw-r--r--   0 runner    (1001) docker     (127)    41273 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/05.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/08.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/11.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    27250 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/13.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/15.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10092 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/17.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/18.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20822 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/19.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/20.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/23.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    27725 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/25.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18594 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/27.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9881 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/41.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/44.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/47.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/50.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/52.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/54.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/63.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/66.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18713 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/68.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    19374 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/70.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13436 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/73.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33434 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/76.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/81.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/85.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/86.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/88.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/91.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/94.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/95.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/97.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/99.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/centros_poblados/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/files/departamentos.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:01:54.323229 danecode-0.2.9/danecode/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-12 03:01:50.000000 danecode-0.2.9/danecode/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 03:01:54.323229 danecode-0.2.9/danecode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-12 03:01:54.000000 danecode-0.2.9/danecode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-12 03:01:54.000000 danecode-0.2.9/danecode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 03:01:54.000000 danecode-0.2.9/danecode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-12 03:01:54.000000 danecode-0.2.9/danecode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-12 03:01:54.000000 danecode-0.2.9/danecode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 03:01:54.323229 danecode-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-12 03:01:50.000000 danecode-0.2.9/setup.py
```

### Comparing `danecode-0.2.8/LICENSE` & `danecode-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/PKG-INFO` & `danecode-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danecode
-Version: 0.2.8
+Version: 0.2.9
 Summary: A simple util to get dane codes by department and municipality
 Author: santiagofep
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `danecode-0.2.8/danecode/__init__.py` & `danecode-0.2.9/danecode/__init__.py`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/country_data.py` & `danecode-0.2.9/danecode/country_data.py`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/05.csv` & `danecode-0.2.9/danecode/files/centros_poblados/05.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/08.csv` & `danecode-0.2.9/danecode/files/centros_poblados/08.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/11.csv` & `danecode-0.2.9/danecode/files/centros_poblados/11.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/13.csv` & `danecode-0.2.9/danecode/files/centros_poblados/13.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/15.csv` & `danecode-0.2.9/danecode/files/centros_poblados/15.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/17.csv` & `danecode-0.2.9/danecode/files/centros_poblados/17.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/18.csv` & `danecode-0.2.9/danecode/files/centros_poblados/18.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/19.csv` & `danecode-0.2.9/danecode/files/centros_poblados/19.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/20.csv` & `danecode-0.2.9/danecode/files/centros_poblados/20.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/23.csv` & `danecode-0.2.9/danecode/files/centros_poblados/23.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/25.csv` & `danecode-0.2.9/danecode/files/centros_poblados/25.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/27.csv` & `danecode-0.2.9/danecode/files/centros_poblados/27.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/41.csv` & `danecode-0.2.9/danecode/files/centros_poblados/41.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/44.csv` & `danecode-0.2.9/danecode/files/centros_poblados/44.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/47.csv` & `danecode-0.2.9/danecode/files/centros_poblados/47.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/50.csv` & `danecode-0.2.9/danecode/files/centros_poblados/50.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/52.csv` & `danecode-0.2.9/danecode/files/centros_poblados/52.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/54.csv` & `danecode-0.2.9/danecode/files/centros_poblados/54.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/63.csv` & `danecode-0.2.9/danecode/files/centros_poblados/63.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/66.csv` & `danecode-0.2.9/danecode/files/centros_poblados/66.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/68.csv` & `danecode-0.2.9/danecode/files/centros_poblados/68.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/70.csv` & `danecode-0.2.9/danecode/files/centros_poblados/70.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/73.csv` & `danecode-0.2.9/danecode/files/centros_poblados/73.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/76.csv` & `danecode-0.2.9/danecode/files/centros_poblados/76.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/81.csv` & `danecode-0.2.9/danecode/files/centros_poblados/81.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/85.csv` & `danecode-0.2.9/danecode/files/centros_poblados/85.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/86.csv` & `danecode-0.2.9/danecode/files/centros_poblados/86.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/88.csv` & `danecode-0.2.9/danecode/files/centros_poblados/88.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/91.csv` & `danecode-0.2.9/danecode/files/centros_poblados/91.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/94.csv` & `danecode-0.2.9/danecode/files/centros_poblados/94.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/95.csv` & `danecode-0.2.9/danecode/files/centros_poblados/95.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/97.csv` & `danecode-0.2.9/danecode/files/centros_poblados/97.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/centros_poblados/99.csv` & `danecode-0.2.9/danecode/files/centros_poblados/99.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/files/departamentos.csv` & `danecode-0.2.9/danecode/files/departamentos.csv`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode/services/__init__.py` & `danecode-0.2.9/danecode/services/__init__.py`

 * *Files identical despite different names*

### Comparing `danecode-0.2.8/danecode.egg-info/PKG-INFO` & `danecode-0.2.9/danecode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danecode
-Version: 0.2.8
+Version: 0.2.9
 Summary: A simple util to get dane codes by department and municipality
 Author: santiagofep
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `danecode-0.2.8/danecode.egg-info/SOURCES.txt` & `danecode-0.2.9/danecode.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 danecode/__init__.py
 danecode/country_data.py
 danecode.egg-info/PKG-INFO
 danecode.egg-info/SOURCES.txt
 danecode.egg-info/dependency_links.txt
 danecode.egg-info/requires.txt
 danecode.egg-info/top_level.txt
+danecode/files/__init__.py
 danecode/files/departamentos.csv
 danecode/files/centros_poblados/05.csv
 danecode/files/centros_poblados/08.csv
 danecode/files/centros_poblados/11.csv
 danecode/files/centros_poblados/13.csv
 danecode/files/centros_poblados/15.csv
 danecode/files/centros_poblados/17.csv
@@ -38,8 +39,9 @@
 danecode/files/centros_poblados/86.csv
 danecode/files/centros_poblados/88.csv
 danecode/files/centros_poblados/91.csv
 danecode/files/centros_poblados/94.csv
 danecode/files/centros_poblados/95.csv
 danecode/files/centros_poblados/97.csv
 danecode/files/centros_poblados/99.csv
+danecode/files/centros_poblados/__init__.py
 danecode/services/__init__.py
```

### Comparing `danecode-0.2.8/setup.py` & `danecode-0.2.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="danecode",
-    version="0.2.8",
+    version="0.2.9",
     author="santiagofep",
     description="A simple util to get dane codes by department and municipality",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

