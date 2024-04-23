# Comparing `tmp/py2nut-4.2.3.tar.gz` & `tmp/py2nut-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2nut-4.2.3.tar", last modified: Wed Feb 14 08:32:03 2024, max compression
+gzip compressed data, was "py2nut-4.2.4.tar", last modified: Tue Apr 23 12:21:49 2024, max compression
```

## Comparing `py2nut-4.2.3.tar` & `py2nut-4.2.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.557234 py2nut-4.2.3/
--rw-rw-rw-   0        0        0    35803 2023-07-05 07:28:17.000000 py2nut-4.2.3/LICENSE
--rw-rw-rw-   0        0        0       22 2023-07-05 07:28:17.000000 py2nut-4.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0    21808 2024-02-14 08:32:03.551818 py2nut-4.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    21290 2023-07-05 07:28:17.000000 py2nut-4.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.390275 py2nut-4.2.3/py2Nut/
--rw-rw-rw-   0        0        0       23 2024-02-14 08:18:57.000000 py2nut-4.2.3/py2Nut/__init__.py
--rw-rw-rw-   0        0        0        3 2023-07-05 07:28:17.000000 py2nut-4.2.3/py2Nut/_lib.py
--rw-rw-rw-   0        0        0       42 2023-07-05 07:28:17.000000 py2nut-4.2.3/py2Nut/nutApi.py
--rw-rw-rw-   0        0        0       52 2023-07-05 07:28:17.000000 py2nut-4.2.3/py2Nut/nutDataframe.py
--rw-rw-rw-   0        0        0       45 2023-07-05 07:28:17.000000 py2nut-4.2.3/py2Nut/nutDate.py
--rw-rw-rw-   0        0        0       37 2023-07-05 07:28:17.000000 py2nut-4.2.3/py2Nut/nutDb.py
--rw-rw-rw-   0        0        0       46 2023-07-05 07:28:17.000000 py2nut-4.2.3/py2Nut/nutEmail.py
--rw-rw-rw-   0        0        0       48 2023-07-05 07:28:17.000000 py2nut-4.2.3/py2Nut/nutFiles.py
--rw-rw-rw-   0        0        0       40 2023-07-05 07:28:17.000000 py2nut-4.2.3/py2Nut/nutFtp.py
--rw-rw-rw-   0        0        0       48 2023-07-05 07:28:17.000000 py2nut-4.2.3/py2Nut/nutOther.py
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.394275 py2nut-4.2.3/py2Nut/xlrd/
--rw-rw-rw-   0        0        0    34373 2023-07-05 07:28:17.000000 py2nut-4.2.3/py2Nut/xlrd/xlsx.py
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.548730 py2nut-4.2.3/py2nut.egg-info/
--rw-rw-rw-   0        0        0    21808 2024-02-14 08:32:03.000000 py2nut-4.2.3/py2nut.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1164 2024-02-14 08:32:03.000000 py2nut-4.2.3/py2nut.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-14 08:32:03.000000 py2nut-4.2.3/py2nut.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-02-14 08:32:03.000000 py2nut-4.2.3/py2nut.egg-info/requires.txt
--rw-rw-rw-   0        0        0       83 2024-02-14 08:32:03.000000 py2nut-4.2.3/py2nut.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.417141 py2nut-4.2.3/pynut_1tools/
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.441141 py2nut-4.2.3/pynut_1tools/pyNutTools/
--rw-rw-rw-   0        0        0       23 2023-09-26 08:50:35.000000 py2nut-4.2.3/pynut_1tools/pyNutTools/__init__.py
--rw-rw-rw-   0        0        0     2054 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_1tools/pyNutTools/_lib.py
--rw-rw-rw-   0        0        0    32469 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_1tools/pyNutTools/nutDataframe.py
--rw-rw-rw-   0        0        0    18046 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_1tools/pyNutTools/nutDate.py
--rw-rw-rw-   0        0        0     8732 2023-09-26 09:23:38.000000 py2nut-4.2.3/pynut_1tools/pyNutTools/nutOther.py
--rw-rw-rw-   0        0        0     1029 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_1tools/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.447144 py2nut-4.2.3/pynut_2api/
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.460303 py2nut-4.2.3/pynut_2api/pyNutApi/
--rw-rw-rw-   0        0        0       23 2023-09-26 08:50:28.000000 py2nut-4.2.3/pynut_2api/pyNutApi/__init__.py
--rw-rw-rw-   0        0        0     3607 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_2api/pyNutApi/_lib.py
--rw-rw-rw-   0        0        0    29117 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_2api/pyNutApi/nutApi.py
--rw-rw-rw-   0        0        0     1079 2023-10-04 11:50:27.000000 py2nut-4.2.3/pynut_2api/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.466308 py2nut-4.2.3/pynut_2files/
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.479305 py2nut-4.2.3/pynut_2files/pyNutFiles/
--rw-rw-rw-   0        0        0       21 2023-09-26 08:50:20.000000 py2nut-4.2.3/pynut_2files/pyNutFiles/__init__.py
--rw-rw-rw-   0        0        0     6710 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_2files/pyNutFiles/_lib.py
--rw-rw-rw-   0        0        0   132618 2023-10-10 08:56:21.000000 py2nut-4.2.3/pynut_2files/pyNutFiles/nutFiles.py
--rw-rw-rw-   0        0        0     1170 2023-10-04 11:50:16.000000 py2nut-4.2.3/pynut_2files/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.485306 py2nut-4.2.3/pynut_3db/
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.496460 py2nut-4.2.3/pynut_3db/pyNutDB/
--rw-rw-rw-   0        0        0       21 2023-09-26 08:50:12.000000 py2nut-4.2.3/pynut_3db/pyNutDB/__init__.py
--rw-rw-rw-   0        0        0     2591 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_3db/pyNutDB/_lib.py
--rw-rw-rw-   0        0        0    21550 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_3db/pyNutDB/nutDb.py
--rw-rw-rw-   0        0        0     1051 2023-10-04 11:50:05.000000 py2nut-4.2.3/pynut_3db/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.501462 py2nut-4.2.3/pynut_3email/
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.514463 py2nut-4.2.3/pynut_3email/pyNutEmail/
--rw-rw-rw-   0        0        0       21 2023-10-04 12:16:01.000000 py2nut-4.2.3/pynut_3email/pyNutEmail/__init__.py
--rw-rw-rw-   0        0        0     4303 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_3email/pyNutEmail/_lib.py
--rw-rw-rw-   0        0        0    37272 2023-10-25 02:36:26.000000 py2nut-4.2.3/pynut_3email/pyNutEmail/nutEmail.py
--rw-rw-rw-   0        0        0     1064 2023-10-04 11:49:55.000000 py2nut-4.2.3/pynut_3email/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.519463 py2nut-4.2.3/pynut_3ftp/
-drwxrwxrwx   0        0        0        0 2024-02-14 08:32:03.532730 py2nut-4.2.3/pynut_3ftp/pyNutFtp/
--rw-rw-rw-   0        0        0       23 2023-09-26 08:50:04.000000 py2nut-4.2.3/pynut_3ftp/pyNutFtp/__init__.py
--rw-rw-rw-   0        0        0     3476 2023-07-05 07:28:17.000000 py2nut-4.2.3/pynut_3ftp/pyNutFtp/_lib.py
--rw-rw-rw-   0        0        0    29668 2024-02-14 08:20:10.000000 py2nut-4.2.3/pynut_3ftp/pyNutFtp/nutFtp.py
--rw-rw-rw-   0        0        0     1072 2023-10-04 11:49:47.000000 py2nut-4.2.3/pynut_3ftp/setup.py
--rw-rw-rw-   0        0        0       42 2024-02-14 08:32:03.557234 py2nut-4.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1565 2023-07-05 07:28:17.000000 py2nut-4.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.129866 py2nut-4.2.4/
+-rw-rw-rw-   0        0        0    35803 2023-07-05 07:28:17.000000 py2nut-4.2.4/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-07-05 07:28:17.000000 py2nut-4.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    21808 2024-04-23 12:21:49.129866 py2nut-4.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    21290 2023-07-05 07:28:17.000000 py2nut-4.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:48.976120 py2nut-4.2.4/py2Nut/
+-rw-rw-rw-   0        0        0       21 2024-04-23 12:15:17.000000 py2nut-4.2.4/py2Nut/__init__.py
+-rw-rw-rw-   0        0        0        3 2023-07-05 07:28:17.000000 py2nut-4.2.4/py2Nut/_lib.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 07:28:17.000000 py2nut-4.2.4/py2Nut/nutApi.py
+-rw-rw-rw-   0        0        0       52 2023-07-05 07:28:17.000000 py2nut-4.2.4/py2Nut/nutDataframe.py
+-rw-rw-rw-   0        0        0       45 2023-07-05 07:28:17.000000 py2nut-4.2.4/py2Nut/nutDate.py
+-rw-rw-rw-   0        0        0       37 2023-07-05 07:28:17.000000 py2nut-4.2.4/py2Nut/nutDb.py
+-rw-rw-rw-   0        0        0       46 2023-07-05 07:28:17.000000 py2nut-4.2.4/py2Nut/nutEmail.py
+-rw-rw-rw-   0        0        0       48 2023-07-05 07:28:17.000000 py2nut-4.2.4/py2Nut/nutFiles.py
+-rw-rw-rw-   0        0        0       40 2023-07-05 07:28:17.000000 py2nut-4.2.4/py2Nut/nutFtp.py
+-rw-rw-rw-   0        0        0       48 2023-07-05 07:28:17.000000 py2nut-4.2.4/py2Nut/nutOther.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:48.991744 py2nut-4.2.4/py2Nut/xlrd/
+-rw-rw-rw-   0        0        0    34373 2023-07-05 07:28:17.000000 py2nut-4.2.4/py2Nut/xlrd/xlsx.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.129866 py2nut-4.2.4/py2nut.egg-info/
+-rw-rw-rw-   0        0        0    21808 2024-04-23 12:21:48.000000 py2nut-4.2.4/py2nut.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1164 2024-04-23 12:21:48.000000 py2nut-4.2.4/py2nut.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 12:21:48.000000 py2nut-4.2.4/py2nut.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-23 12:21:48.000000 py2nut-4.2.4/py2nut.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       83 2024-04-23 12:21:48.000000 py2nut-4.2.4/py2nut.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:48.998260 py2nut-4.2.4/pynut_1tools/
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.031539 py2nut-4.2.4/pynut_1tools/pyNutTools/
+-rw-rw-rw-   0        0        0       23 2024-04-23 12:15:08.000000 py2nut-4.2.4/pynut_1tools/pyNutTools/__init__.py
+-rw-rw-rw-   0        0        0     2054 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_1tools/pyNutTools/_lib.py
+-rw-rw-rw-   0        0        0    32469 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_1tools/pyNutTools/nutDataframe.py
+-rw-rw-rw-   0        0        0    18046 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_1tools/pyNutTools/nutDate.py
+-rw-rw-rw-   0        0        0     9915 2024-04-23 12:15:00.000000 py2nut-4.2.4/pynut_1tools/pyNutTools/nutOther.py
+-rw-rw-rw-   0        0        0     1029 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_1tools/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.031539 py2nut-4.2.4/pynut_2api/
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.047193 py2nut-4.2.4/pynut_2api/pyNutApi/
+-rw-rw-rw-   0        0        0       23 2023-09-26 08:50:28.000000 py2nut-4.2.4/pynut_2api/pyNutApi/__init__.py
+-rw-rw-rw-   0        0        0     3607 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_2api/pyNutApi/_lib.py
+-rw-rw-rw-   0        0        0    29117 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_2api/pyNutApi/nutApi.py
+-rw-rw-rw-   0        0        0     1079 2023-10-04 11:50:27.000000 py2nut-4.2.4/pynut_2api/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.047193 py2nut-4.2.4/pynut_2files/
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.062811 py2nut-4.2.4/pynut_2files/pyNutFiles/
+-rw-rw-rw-   0        0        0       21 2023-09-26 08:50:20.000000 py2nut-4.2.4/pynut_2files/pyNutFiles/__init__.py
+-rw-rw-rw-   0        0        0     6710 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_2files/pyNutFiles/_lib.py
+-rw-rw-rw-   0        0        0   132618 2023-10-10 08:56:21.000000 py2nut-4.2.4/pynut_2files/pyNutFiles/nutFiles.py
+-rw-rw-rw-   0        0        0     1170 2023-10-04 11:50:16.000000 py2nut-4.2.4/pynut_2files/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.078436 py2nut-4.2.4/pynut_3db/
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.078436 py2nut-4.2.4/pynut_3db/pyNutDB/
+-rw-rw-rw-   0        0        0       21 2023-09-26 08:50:12.000000 py2nut-4.2.4/pynut_3db/pyNutDB/__init__.py
+-rw-rw-rw-   0        0        0     2591 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_3db/pyNutDB/_lib.py
+-rw-rw-rw-   0        0        0    21550 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_3db/pyNutDB/nutDb.py
+-rw-rw-rw-   0        0        0     1051 2023-10-04 11:50:05.000000 py2nut-4.2.4/pynut_3db/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.098580 py2nut-4.2.4/pynut_3email/
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.098580 py2nut-4.2.4/pynut_3email/pyNutEmail/
+-rw-rw-rw-   0        0        0       21 2023-10-04 12:16:01.000000 py2nut-4.2.4/pynut_3email/pyNutEmail/__init__.py
+-rw-rw-rw-   0        0        0     4303 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_3email/pyNutEmail/_lib.py
+-rw-rw-rw-   0        0        0    37272 2023-10-25 02:36:26.000000 py2nut-4.2.4/pynut_3email/pyNutEmail/nutEmail.py
+-rw-rw-rw-   0        0        0     1064 2023-10-04 11:49:55.000000 py2nut-4.2.4/pynut_3email/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.114228 py2nut-4.2.4/pynut_3ftp/
+drwxrwxrwx   0        0        0        0 2024-04-23 12:21:49.129866 py2nut-4.2.4/pynut_3ftp/pyNutFtp/
+-rw-rw-rw-   0        0        0       23 2023-09-26 08:50:04.000000 py2nut-4.2.4/pynut_3ftp/pyNutFtp/__init__.py
+-rw-rw-rw-   0        0        0     3476 2023-07-05 07:28:17.000000 py2nut-4.2.4/pynut_3ftp/pyNutFtp/_lib.py
+-rw-rw-rw-   0        0        0    29668 2024-02-14 08:20:10.000000 py2nut-4.2.4/pynut_3ftp/pyNutFtp/nutFtp.py
+-rw-rw-rw-   0        0        0     1072 2023-10-04 11:49:47.000000 py2nut-4.2.4/pynut_3ftp/setup.py
+-rw-rw-rw-   0        0        0       42 2024-04-23 12:21:49.129866 py2nut-4.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1565 2023-07-05 07:28:17.000000 py2nut-4.2.4/setup.py
```

### Comparing `py2nut-4.2.3/LICENSE` & `py2nut-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/PKG-INFO` & `py2nut-4.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2nut
-Version: 4.2.3
+Version: 4.2.4
 Summary: This Library allows you to make Misc operations in various domain
 Home-page: https://github.com/Laurent-Tupin/py2nut
 Author: Laurent Tupin
 Author-email: laurent.tupinn@gmail.com
 License: Copyright 2022-2035
 Classifier: License :: Free For Home Use
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py2nut-4.2.3/README.md` & `py2nut-4.2.4/README.md`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/py2Nut/xlrd/xlsx.py` & `py2nut-4.2.4/py2Nut/xlrd/xlsx.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/py2nut.egg-info/PKG-INFO` & `py2nut-4.2.4/py2nut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2nut
-Version: 4.2.3
+Version: 4.2.4
 Summary: This Library allows you to make Misc operations in various domain
 Home-page: https://github.com/Laurent-Tupin/py2nut
 Author: Laurent Tupin
 Author-email: laurent.tupinn@gmail.com
 License: Copyright 2022-2035
 Classifier: License :: Free For Home Use
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py2nut-4.2.3/py2nut.egg-info/SOURCES.txt` & `py2nut-4.2.4/py2nut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_1tools/pyNutTools/_lib.py` & `py2nut-4.2.4/pynut_1tools/pyNutTools/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_1tools/pyNutTools/nutDataframe.py` & `py2nut-4.2.4/pynut_1tools/pyNutTools/nutDataframe.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_1tools/pyNutTools/nutDate.py` & `py2nut-4.2.4/pynut_1tools/pyNutTools/nutDate.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_1tools/pyNutTools/nutOther.py` & `py2nut-4.2.4/pynut_1tools/pyNutTools/nutOther.py`

 * *Files 12% similar despite different names*

```diff
@@ -187,14 +187,35 @@
 #-----------------------------------------------------------------
 # List
 #-----------------------------------------------------------------
 def fL_GetFlatList_fromListOfList(ll_input):
     l_list = [x for l_subList in ll_input for x in l_subList]
     return l_list
 
+def fL_sortListOfDictionary(l_dico, key = None, bl_reverse = False) -> list:
+    if key is None:
+        lDic_soted = fL_sortListOfDictionary(l_dico, key = l_dico[0].keys()[0], bl_reverse = bl_reverse)
+    elif type(key) is list:
+        int_len  = len(key)
+        if int_len == 0:
+            pass
+        elif int_len == 1:
+            lDic_soted = sorted(l_dico, key = lambda d: d[ key[0] ], reverse = bl_reverse )
+        elif int_len == 2:
+            lDic_soted = sorted(l_dico, key = lambda d: ( d[ key[0]], d[ key[1]] ), reverse = bl_reverse )
+        elif int_len == 3:
+            lDic_soted = sorted(l_dico, key = lambda d: ( d[ key[0]], d[ key[1]], d[ key[2]] ), reverse = bl_reverse )
+        elif int_len == 4:
+            lDic_soted = sorted(l_dico, key = lambda d: ( d[ key[0]], d[ key[1]], d[ key[2]], d[ key[3]] ), reverse = bl_reverse )
+        elif int_len >= 5:
+            lDic_soted = sorted(l_dico, key = lambda d: ( d[ key[0]], d[ key[1]], d[ key[2]], d[ key[3]], d[ key[4]] ), reverse = bl_reverse )
+    elif type(key) is str:
+        lDic_soted = sorted(l_dico, key = lambda d: d[ key ], reverse = bl_reverse )
+    return lDic_soted
+
 
 
 #-----------------------------------------------------------------
 # Dictionary
 #-----------------------------------------------------------------
 def fDic_comprehension(original_dict):
     new_dict = {num: num*num for num in range(1, 11)}
```

### Comparing `py2nut-4.2.3/pynut_1tools/setup.py` & `py2nut-4.2.4/pynut_1tools/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_2api/pyNutApi/_lib.py` & `py2nut-4.2.4/pynut_2api/pyNutApi/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_2api/pyNutApi/nutApi.py` & `py2nut-4.2.4/pynut_2api/pyNutApi/nutApi.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_2api/setup.py` & `py2nut-4.2.4/pynut_2api/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_2files/pyNutFiles/_lib.py` & `py2nut-4.2.4/pynut_2files/pyNutFiles/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_2files/pyNutFiles/nutFiles.py` & `py2nut-4.2.4/pynut_2files/pyNutFiles/nutFiles.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_2files/setup.py` & `py2nut-4.2.4/pynut_2files/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_3db/pyNutDB/_lib.py` & `py2nut-4.2.4/pynut_3db/pyNutDB/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_3db/pyNutDB/nutDb.py` & `py2nut-4.2.4/pynut_3db/pyNutDB/nutDb.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_3db/setup.py` & `py2nut-4.2.4/pynut_3db/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_3email/pyNutEmail/_lib.py` & `py2nut-4.2.4/pynut_3email/pyNutEmail/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_3email/pyNutEmail/nutEmail.py` & `py2nut-4.2.4/pynut_3email/pyNutEmail/nutEmail.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_3email/setup.py` & `py2nut-4.2.4/pynut_3email/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_3ftp/pyNutFtp/_lib.py` & `py2nut-4.2.4/pynut_3ftp/pyNutFtp/_lib.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_3ftp/pyNutFtp/nutFtp.py` & `py2nut-4.2.4/pynut_3ftp/pyNutFtp/nutFtp.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/pynut_3ftp/setup.py` & `py2nut-4.2.4/pynut_3ftp/setup.py`

 * *Files identical despite different names*

### Comparing `py2nut-4.2.3/setup.py` & `py2nut-4.2.4/setup.py`

 * *Files identical despite different names*

