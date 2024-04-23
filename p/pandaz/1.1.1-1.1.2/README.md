# Comparing `tmp/pandaz-1.1.1.tar.gz` & `tmp/pandaz-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandaz-1.1.1.tar", last modified: Tue Apr 23 11:42:31 2024, max compression
+gzip compressed data, was "pandaz-1.1.2.tar", last modified: Tue Apr 23 16:41:11 2024, max compression
```

## Comparing `pandaz-1.1.1.tar` & `pandaz-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 11:42:31.048807 pandaz-1.1.1/
--rw-rw-rw-   0        0        0     1088 2024-04-22 12:14:20.000000 pandaz-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      562 2024-04-23 11:42:31.047809 pandaz-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 11:42:31.026906 pandaz-1.1.1/pandaj/
--rw-rw-rw-   0        0        0      876 2024-04-22 16:16:57.000000 pandaz-1.1.1/pandaj/1_descriptive_stats.py
--rw-rw-rw-   0        0        0     1404 2024-04-22 16:16:57.000000 pandaz-1.1.1/pandaj/2_data_imputation.py
--rw-rw-rw-   0        0        0     1035 2024-04-22 16:16:57.000000 pandaz-1.1.1/pandaj/3_data_visualisation.py
--rw-rw-rw-   0        0        0     2963 2024-04-22 16:16:57.000000 pandaz-1.1.1/pandaj/4_supervised_learning.py
--rw-rw-rw-   0        0        0     1380 2024-04-22 16:16:57.000000 pandaz-1.1.1/pandaj/5_unsupervised_learning.py
--rw-rw-rw-   0        0        0     2235 2024-04-23 11:42:28.000000 pandaz-1.1.1/pandaj/6_timeseriesforecasting.py
--rw-rw-rw-   0        0        0      710 2024-04-22 16:16:57.000000 pandaz-1.1.1/pandaj/7_outlier_detection.py
--rw-rw-rw-   0        0        0     1422 2024-04-22 16:16:57.000000 pandaz-1.1.1/pandaj/8_SMOTE.py
--rw-rw-rw-   0        0        0     1031 2024-04-22 16:16:57.000000 pandaz-1.1.1/pandaj/9_inferential_stats.py
--rw-rw-rw-   0        0        0        0 2024-04-22 12:21:04.000000 pandaz-1.1.1/pandaj/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:42:31.046812 pandaz-1.1.1/pandaz.egg-info/
--rw-rw-rw-   0        0        0      562 2024-04-23 11:42:30.000000 pandaz-1.1.1/pandaz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      422 2024-04-23 11:42:30.000000 pandaz-1.1.1/pandaz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 11:42:30.000000 pandaz-1.1.1/pandaz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 11:42:30.000000 pandaz-1.1.1/pandaz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 11:42:31.048807 pandaz-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      865 2024-04-23 11:40:00.000000 pandaz-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:41:11.190553 pandaz-1.1.2/
+-rw-rw-rw-   0        0        0     1088 2024-04-22 12:14:20.000000 pandaz-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      562 2024-04-23 16:41:11.188555 pandaz-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 16:41:11.158982 pandaz-1.1.2/pandaz/
+-rw-rw-rw-   0        0        0     4510 2024-04-23 16:39:33.000000 pandaz-1.1.2/pandaz/1_descriptive_stats.py
+-rw-rw-rw-   0        0        0     1404 2024-04-22 16:16:57.000000 pandaz-1.1.2/pandaz/2_data_imputation.py
+-rw-rw-rw-   0        0        0     1035 2024-04-22 16:16:57.000000 pandaz-1.1.2/pandaz/3_data_visualisation.py
+-rw-rw-rw-   0        0        0     2963 2024-04-22 16:16:57.000000 pandaz-1.1.2/pandaz/4_supervised_learning.py
+-rw-rw-rw-   0        0        0     1380 2024-04-22 16:16:57.000000 pandaz-1.1.2/pandaz/5_unsupervised_learning.py
+-rw-rw-rw-   0        0        0     2235 2024-04-23 11:42:28.000000 pandaz-1.1.2/pandaz/6_timeseriesforecasting.py
+-rw-rw-rw-   0        0        0      710 2024-04-22 16:16:57.000000 pandaz-1.1.2/pandaz/7_outlier_detection.py
+-rw-rw-rw-   0        0        0     1422 2024-04-22 16:16:57.000000 pandaz-1.1.2/pandaz/8_SMOTE.py
+-rw-rw-rw-   0        0        0     1031 2024-04-22 16:16:57.000000 pandaz-1.1.2/pandaz/9_inferential_stats.py
+-rw-rw-rw-   0        0        0        0 2024-04-22 12:21:04.000000 pandaz-1.1.2/pandaz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:41:11.186544 pandaz-1.1.2/pandaz.egg-info/
+-rw-rw-rw-   0        0        0      562 2024-04-23 16:41:10.000000 pandaz-1.1.2/pandaz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-04-23 16:41:10.000000 pandaz-1.1.2/pandaz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 16:41:10.000000 pandaz-1.1.2/pandaz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 16:41:10.000000 pandaz-1.1.2/pandaz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 16:41:11.191062 pandaz-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      865 2024-04-23 16:41:08.000000 pandaz-1.1.2/setup.py
```

### Comparing `pandaz-1.1.1/LICENSE` & `pandaz-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandaz-1.1.1/PKG-INFO` & `pandaz-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandaz
-Version: 1.1.1
+Version: 1.1.2
 Summary: Helps users code efficently
 Author: Tom Hanks
 Author-email: <tomhanks02@gmail.com>
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pandaz-1.1.1/pandaj/2_data_imputation.py` & `pandaz-1.1.2/pandaz/2_data_imputation.py`

 * *Files identical despite different names*

### Comparing `pandaz-1.1.1/pandaj/3_data_visualisation.py` & `pandaz-1.1.2/pandaz/3_data_visualisation.py`

 * *Files identical despite different names*

### Comparing `pandaz-1.1.1/pandaj/4_supervised_learning.py` & `pandaz-1.1.2/pandaz/4_supervised_learning.py`

 * *Files identical despite different names*

### Comparing `pandaz-1.1.1/pandaj/5_unsupervised_learning.py` & `pandaz-1.1.2/pandaz/5_unsupervised_learning.py`

 * *Files identical despite different names*

### Comparing `pandaz-1.1.1/pandaj/6_timeseriesforecasting.py` & `pandaz-1.1.2/pandaz/6_timeseriesforecasting.py`

 * *Files identical despite different names*

### Comparing `pandaz-1.1.1/pandaj/7_outlier_detection.py` & `pandaz-1.1.2/pandaz/7_outlier_detection.py`

 * *Files identical despite different names*

### Comparing `pandaz-1.1.1/pandaj/8_SMOTE.py` & `pandaz-1.1.2/pandaz/8_SMOTE.py`

 * *Files identical despite different names*

### Comparing `pandaz-1.1.1/pandaj/9_inferential_stats.py` & `pandaz-1.1.2/pandaz/9_inferential_stats.py`

 * *Files identical despite different names*

### Comparing `pandaz-1.1.1/pandaz.egg-info/PKG-INFO` & `pandaz-1.1.2/pandaz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandaz
-Version: 1.1.1
+Version: 1.1.2
 Summary: Helps users code efficently
 Author: Tom Hanks
 Author-email: <tomhanks02@gmail.com>
 Keywords: python,video,stream,video stream,camera stream,sockets
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pandaz-1.1.1/setup.py` & `pandaz-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.1'
+VERSION = '1.1.2'
 DESCRIPTION = 'Helps users code efficently'
 LONG_DESCRIPTION = 'A package that allows to build simple codes in a well defined and efficient manner.'
 
 # Setting up
 setup(
     name="pandaz",
     version=VERSION,
```

