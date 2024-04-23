# Comparing `tmp/myria3d-3.8.2.tar.gz` & `tmp/myria3d-3.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myria3d-3.8.2.tar", last modified: Thu Apr 18 13:05:20 2024, max compression
+gzip compressed data, was "myria3d-3.8.3.tar", last modified: Tue Apr 23 15:07:32 2024, max compression
```

## Comparing `myria3d-3.8.2.tar` & `myria3d-3.8.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2024-04-18 13:05:20.222821 myria3d-3.8.2/
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     1571 2022-12-07 10:34:45.000000 myria3d-3.8.2/LICENSE
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     5839 2024-04-18 13:05:20.222821 myria3d-3.8.2/PKG-INFO
--rwxr-xr-x   0 LVauchier (24820) usernis  (10000)     3396 2023-04-04 08:22:07.000000 myria3d-3.8.2/README.md
-drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2024-04-18 13:05:20.218821 myria3d-3.8.2/myria3d/
--rwxr-xr-x   0 LVauchier (24820) usernis  (10000)      266 2022-12-07 10:34:45.000000 myria3d-3.8.2/myria3d/__init__.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)       74 2024-04-18 13:00:25.000000 myria3d-3.8.2/myria3d/_version.py
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     2713 2024-03-13 09:13:29.000000 myria3d-3.8.2/myria3d/predict.py
--rwxr-xr-x   0 LVauchier (24820) usernis  (10000)     6751 2024-03-13 09:13:29.000000 myria3d-3.8.2/myria3d/train.py
-drwxr-xr-x   0 LVauchier (24820) usernis  (10000)        0 2024-04-18 13:05:20.222821 myria3d-3.8.2/myria3d.egg-info/
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     5839 2024-04-18 13:05:20.000000 myria3d-3.8.2/myria3d.egg-info/PKG-INFO
--rw-r--r--   0 LVauchier (24820) usernis  (10000)      232 2024-04-18 13:05:20.000000 myria3d-3.8.2/myria3d.egg-info/SOURCES.txt
--rw-r--r--   0 LVauchier (24820) usernis  (10000)        1 2024-04-18 13:05:20.000000 myria3d-3.8.2/myria3d.egg-info/dependency_links.txt
--rw-r--r--   0 LVauchier (24820) usernis  (10000)        8 2024-04-18 13:05:20.000000 myria3d-3.8.2/myria3d.egg-info/top_level.txt
--rw-r--r--   0 LVauchier (24820) usernis  (10000)     1958 2024-04-18 12:55:41.000000 myria3d-3.8.2/pyproject.toml
--rw-r--r--   0 LVauchier (24820) usernis  (10000)       38 2024-04-18 13:05:20.222821 myria3d-3.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:32.162069 myria3d-3.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-23 15:04:02.000000 myria3d-3.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-23 15:07:32.162069 myria3d-3.8.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3396 2024-04-23 15:04:02.000000 myria3d-3.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:32.158069 myria3d-3.8.3/myria3d/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      266 2024-04-23 15:04:02.000000 myria3d-3.8.3/myria3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-23 15:04:02.000000 myria3d-3.8.3/myria3d/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-23 15:04:02.000000 myria3d-3.8.3/myria3d/predict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6751 2024-04-23 15:04:02.000000 myria3d-3.8.3/myria3d/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 15:07:32.162069 myria3d-3.8.3/myria3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-23 15:07:32.000000 myria3d-3.8.3/myria3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-23 15:07:32.000000 myria3d-3.8.3/myria3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 15:07:32.000000 myria3d-3.8.3/myria3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 15:07:32.000000 myria3d-3.8.3/myria3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-23 15:04:02.000000 myria3d-3.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 15:07:32.162069 myria3d-3.8.3/setup.cfg
```

### Comparing `myria3d-3.8.2/LICENSE` & `myria3d-3.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `myria3d-3.8.2/PKG-INFO` & `myria3d-3.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myria3d
-Version: 3.8.2
+Version: 3.8.3
 Summary: Deep Learning for the Semantic Segmentation of Aerial Lidar Point Clouds
 Author-email: Charles GAYDON <charles.gaydon@gmail.com>
 Maintainer: Michel DAAB
 Maintainer-email: Charles GAYDON <charles.gaydon@gmail.com>, Léa VAUCHIER <lea.vauchier@ign.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Institut National de l'Information Géographique et Forestière
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: myria3d Version: 3.8.2 Summary: Deep Learning for
+Metadata-Version: 2.1 Name: myria3d Version: 3.8.3 Summary: Deep Learning for
 the Semantic Segmentation of Aerial Lidar Point Clouds Author-email: Charles
 GAYDON
 gmail.com> Maintainer: Michel DAAB Maintainer-email: Charles GAYDON
 gmail.com>, LÃ©a VAUCHIER
 ign.fr> License: BSD 3-Clause License Copyright (c) 2021, Institut National de
 l'Information GÃ©ographique et ForestiÃ¨re All rights reserved. Redistribution
 and use in source and binary forms, with or without modification, are permitted
```

### Comparing `myria3d-3.8.2/README.md` & `myria3d-3.8.3/README.md`

 * *Files identical despite different names*

### Comparing `myria3d-3.8.2/myria3d/predict.py` & `myria3d-3.8.3/myria3d/predict.py`

 * *Files identical despite different names*

### Comparing `myria3d-3.8.2/myria3d/train.py` & `myria3d-3.8.3/myria3d/train.py`

 * *Files identical despite different names*

### Comparing `myria3d-3.8.2/myria3d.egg-info/PKG-INFO` & `myria3d-3.8.3/myria3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myria3d
-Version: 3.8.2
+Version: 3.8.3
 Summary: Deep Learning for the Semantic Segmentation of Aerial Lidar Point Clouds
 Author-email: Charles GAYDON <charles.gaydon@gmail.com>
 Maintainer: Michel DAAB
 Maintainer-email: Charles GAYDON <charles.gaydon@gmail.com>, Léa VAUCHIER <lea.vauchier@ign.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Institut National de l'Information Géographique et Forestière
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: myria3d Version: 3.8.2 Summary: Deep Learning for
+Metadata-Version: 2.1 Name: myria3d Version: 3.8.3 Summary: Deep Learning for
 the Semantic Segmentation of Aerial Lidar Point Clouds Author-email: Charles
 GAYDON
 gmail.com> Maintainer: Michel DAAB Maintainer-email: Charles GAYDON
 gmail.com>, LÃ©a VAUCHIER
 ign.fr> License: BSD 3-Clause License Copyright (c) 2021, Institut National de
 l'Information GÃ©ographique et ForestiÃ¨re All rights reserved. Redistribution
 and use in source and binary forms, with or without modification, are permitted
```

### Comparing `myria3d-3.8.2/pyproject.toml` & `myria3d-3.8.3/pyproject.toml`

 * *Files identical despite different names*

