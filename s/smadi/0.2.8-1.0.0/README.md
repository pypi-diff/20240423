# Comparing `tmp/smadi-0.2.8.tar.gz` & `tmp/smadi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smadi-0.2.8.tar", last modified: Sun Apr  7 23:28:40 2024, max compression
+gzip compressed data, was "smadi-1.0.0.tar", last modified: Mon Apr 22 22:44:25 2024, max compression
```

## Comparing `smadi-0.2.8.tar` & `smadi-1.0.0.tar`

### file list

```diff
@@ -1,53 +1,61 @@
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.951335 smadi-0.2.8/
--rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-0.2.8/.coveragerc
--rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-0.2.8/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-0.2.8/.readthedocs.yml
--rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-0.2.8/AUTHORS.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-0.2.8/CHANGELOG.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-0.2.8/CONTRIBUTING.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-0.2.8/LICENSE.txt
--rw-r--r--   0 m294      (1000) m294      (1000)     6981 2024-04-07 23:28:40.951335 smadi-0.2.8/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)     5563 2024-04-07 23:28:23.000000 smadi-0.2.8/README.rst
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.947335 smadi-0.2.8/docs/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/Makefile
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.947335 smadi-0.2.8/docs/_static/
--rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/_static/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/authors.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/changelog.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     9748 2024-04-03 20:04:41.000000 smadi-0.2.8/docs/conf.py
--rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/contributing.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/index.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/license.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-0.2.8/docs/readme.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      231 2024-04-03 20:04:36.000000 smadi-0.2.8/docs/requirements.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-0.2.8/pyproject.toml
--rw-rw-r--   0 m294      (1000) m294      (1000)      301 2024-04-03 02:37:06.000000 smadi-0.2.8/requirements.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)     1492 2024-04-07 23:28:40.955335 smadi-0.2.8/setup.cfg
--rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-04-07 23:20:59.000000 smadi-0.2.8/setup.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.943334 smadi-0.2.8/src/
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.951335 smadi-0.2.8/src/smadi/
--rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-0.2.8/src/smadi/__init__.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    18006 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/anomaly_detectors.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    15636 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     3482 2024-04-02 14:59:26.000000 smadi-0.2.8/src/smadi/data_reader.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8809 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     5419 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/map.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2871 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/metadata.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     7809 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/plot.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8624 2024-04-03 14:16:38.000000 smadi-0.2.8/src/smadi/preprocess.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     4882 2024-04-03 14:50:02.000000 smadi-0.2.8/src/smadi/utils.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    18957 2024-04-07 23:20:39.000000 smadi-0.2.8/src/smadi/workflow.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.951335 smadi-0.2.8/src/smadi.egg-info/
--rw-r--r--   0 m294      (1000) m294      (1000)     6981 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)      915 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/SOURCES.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/dependency_links.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/entry_points.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/not-zip-safe
--rw-rw-r--   0 m294      (1000) m294      (1000)      327 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/requires.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-04-07 23:28:40.000000 smadi-0.2.8/src/smadi.egg-info/top_level.txt
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-07 23:28:40.951335 smadi-0.2.8/tests/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-0.2.8/tests/conftest.py
--rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-0.2.8/tests/data_sample.csv
--rw-rw-r--   0 m294      (1000) m294      (1000)    20031 2024-03-30 14:58:36.000000 smadi-0.2.8/tests/test_climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-0.2.8/tests/test_indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-0.2.8/tox.ini
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.770442 smadi-1.0.0/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-1.0.0/.coveragerc
+-rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-1.0.0/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-1.0.0/.readthedocs.yml
+-rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-1.0.0/AUTHORS.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-1.0.0/CHANGELOG.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-1.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-1.0.0/LICENSE.txt
+-rw-r--r--   0 m294      (1000) m294      (1000)     5297 2024-04-22 22:44:25.770442 smadi-1.0.0/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)     3848 2024-04-22 22:42:47.000000 smadi-1.0.0/README.rst
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.742442 smadi-1.0.0/docs/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/Makefile
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.758442 smadi-1.0.0/docs/_static/
+-rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/_static/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/authors.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/changelog.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9748 2024-04-03 20:04:41.000000 smadi-1.0.0/docs/conf.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/contributing.rst
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.758442 smadi-1.0.0/docs/examples/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2726 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/Installation.ipynb
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9238 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/Loading_data.ipynb
+-rw-rw-r--   0 m294      (1000) m294      (1000)    43432 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/compute_climatology.ipynb
+-rw-rw-r--   0 m294      (1000) m294      (1000)  1280907 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/detect_the_anomlies.ipynb
+-rw-rw-r--   0 m294      (1000) m294      (1000)   694911 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/plot_climatology.ipynb
+-rw-rw-r--   0 m294      (1000) m294      (1000)   819526 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/workflow.ipynb
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/index.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2642 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/introduction.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/license.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/readme.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      231 2024-04-03 20:04:36.000000 smadi-1.0.0/docs/requirements.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-1.0.0/pyproject.toml
+-rw-rw-r--   0 m294      (1000) m294      (1000)      301 2024-04-03 02:37:06.000000 smadi-1.0.0/requirements.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1509 2024-04-22 22:44:25.770442 smadi-1.0.0/setup.cfg
+-rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-04-22 22:43:11.000000 smadi-1.0.0/setup.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.686442 smadi-1.0.0/src/
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.762442 smadi-1.0.0/src/smadi/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-1.0.0/src/smadi/__init__.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    22743 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/anomaly_detectors.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    18044 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     7512 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/data_reader.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9168 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     4472 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/map.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2420 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/metadata.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     8206 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/plot.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9108 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/preprocess.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     4964 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/utils.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    19724 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/workflow.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.770442 smadi-1.0.0/src/smadi.egg-info/
+-rw-r--r--   0 m294      (1000) m294      (1000)     5297 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1149 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/SOURCES.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/dependency_links.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/entry_points.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/not-zip-safe
+-rw-rw-r--   0 m294      (1000) m294      (1000)      343 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/requires.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/top_level.txt
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.770442 smadi-1.0.0/tests/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-1.0.0/tests/conftest.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-1.0.0/tests/data_sample.csv
+-rw-rw-r--   0 m294      (1000) m294      (1000)    20040 2024-04-22 22:42:47.000000 smadi-1.0.0/tests/test_climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-1.0.0/tests/test_indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-1.0.0/tox.ini
```

### Comparing `smadi-0.2.8/.coveragerc` & `smadi-1.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/.gitignore` & `smadi-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/.readthedocs.yml` & `smadi-1.0.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/CONTRIBUTING.rst` & `smadi-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/LICENSE.txt` & `smadi-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/docs/Makefile` & `smadi-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/docs/conf.py` & `smadi-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/docs/index.rst` & `smadi-1.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/setup.cfg` & `smadi-1.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 	cmcrameri
 	fibgrid
 	datashader
 	pycountry
 	PyQt5
 	PySide2
 	mapclassify
+	standard-precip
 	importlib-metadata; python_version<"3.8"
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `smadi-0.2.8/setup.py` & `smadi-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
         setup(
-            version="0.2.8",
+            version="1.0.0",
             entry_points={
                 "console_scripts": [
                     "run = smadi.workflow:main",
                 ]
             },
         )
```

### Comparing `smadi-0.2.8/src/smadi/__init__.py` & `smadi-1.0.0/src/smadi/__init__.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/src/smadi/anomaly_detectors.py` & `smadi-1.0.0/src/smadi/anomaly_detectors.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,24 +10,30 @@
 7. SMCI: The Soil Moisture Condition Index method.
 8. SMCA: The Soil Moisture Content Anomaly method.
 9. ParaDis: The Parametric Distribution method.
 
 
 """
 
-__author__ = "Muhammed Abdelaal"
-__email__ = "muhammedaabdelaal@gmail.com"
-
 import warnings
 from typing import List
 import pandas as pd
+import matplotlib.pyplot as plt
 
 
 from smadi.climatology import Climatology
 from smadi.preprocess import filter_df, clim_groupping
+from smadi.plot import (
+    plot_figure,
+    plot_colmns,
+    draw_hbars,
+    plot_categories_count,
+    get_plot_options,
+    clss_counter,
+)
 from smadi.indicators import (
     zscore,
     smapi,
     smdi,
     smad,
     smca,
     smci,
@@ -54,14 +60,15 @@
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "month",
         normal_metrics: List[str] = ["mean"],
+        agg_metric: str = "mean",
     ):
         """
         Initialize the AnomalyDetector class.
 
         parameters:
         -----------
         df: pd.DataFrame
@@ -99,14 +106,15 @@
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
             time_step,
             normal_metrics,
+            agg_metric,
         )
         # self.clim_df = pd.DataFrame()
         # self.groupby_param = None
 
     @property
     def groupby_param(self):
 
@@ -137,14 +145,132 @@
             A dataframe containing the computed anomalies.
 
         """
         self.clim_df = self._preprocess().copy()
 
         return filter_df(self.clim_df, **kwargs)
 
+    def plot_anomaly(
+        self,
+        df=None,
+        x_axis=None,
+        colmns=None,
+        thresholds=None,
+        plot_hbars=True,
+        plot_categories=True,
+        plot_style="ggplot",
+        **kwargs,
+    ):
+        """
+        Plot the computed anomalies.
+
+        parameters:
+        -----------
+
+        df: pd.DataFrame
+            The dataframe containing the data to plot. if None, the computed anomalies will be used.
+
+        x_axis: list
+            The x-axis values for the plot. if None, the index of the dataframe will be used.
+
+        colmns: dict
+            A dictionary containing the columns to plot. The key is the column name and the value is the plot options.
+
+        thresholds: str
+            The name of the anomaly method to use its corresponding thresholds values.
+
+        plot_hbars: bool
+            Whether to plot the horizontal bars on the plot according to the thresholds of the anomaly method used.
+
+        plot_categories: bool
+            Whether to plot the number of values in each category of the anomaly method that fall within the thresholds.
+
+        plot_style: str
+            The plot style to use for the plot.
+
+        kwargs: dict
+            Additional parameters to be used for customizing the plot. It can be any of the following:
+
+            ['title', 'xlabel', 'ylabel', 'legend', 'figsize', 'grid']
+
+        """
+        plt.style.use(plot_style)
+        # Set values for kwargs based on provided values
+        plot_params = get_plot_options(**kwargs)
+
+        df = self.detect_anomaly() if df is None else df
+        x_axis = df.index if x_axis is None else x_axis
+        plt.figure(figsize=plot_params["figsize"])
+        plot_colmns(df, x_axis, colmns)
+
+        if plot_hbars:
+            draw_hbars(thresholds, x_axis)
+        if plot_categories:
+            results = clss_counter(df, colmns, thresholds)
+            plot_categories_count(x_axis, results, thresholds)
+
+        plot_figure(plot_params)
+
+    def plot_fill_bet(
+        self, df=None, x_axis=None, colmn=None, plot_style="ggplot", **kwargs
+    ):
+        """
+        Plot the computed anomalies using the fill_between method.
+
+        parameters:
+        -----------
+
+        df: pd.DataFrame
+            The dataframe containing the data to plot. if None, the computed anomalies will be used.
+
+        x_axis: list
+            The x-axis values for the plot. if None, the index of the dataframe will be used.
+
+        colmn: str
+            The column name to plot.
+
+        plot_style: str
+            The plot style to use for the plot.
+
+        kwargs: dict
+            Additional parameters to be used for customizing the plot. It can be any of the following:
+
+            ['title', 'xlabel', 'ylabel', 'legend', 'figsize', 'grid']
+
+        """
+
+        plt.style.use(plot_style)
+        plot_params = get_plot_options(**kwargs)
+        df = self.detect_anomaly() if df is None else df
+        x_axis = df.index if x_axis is None else x_axis
+        plt.figure(figsize=plot_params["figsize"])
+
+        plt.fill_between(
+            df.index,
+            df[colmn],
+            where=df[colmn].values >= 0,
+            color="blue",
+            label="Wet",
+        )
+
+        plt.fill_between(
+            df.index,
+            df[colmn],
+            where=df[colmn].values < 0,
+            color="red",
+            label="Dry",
+        )
+
+        # Add horizontal line at y=0
+        plt.axhline(y=0, color="black", linestyle="--", linewidth=1)
+
+        plt.legend(loc="upper right", fontsize=10)
+
+        plot_figure(plot_params)
+
 
 class ZScore(AnomalyDetector):
     """
     A class for detecting anomalies in time series data based on the Z-Score method.
 
     z_score = (x - μ) / σ
 
@@ -162,35 +288,37 @@
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "month",
+        agg_metric: str = "mean",
     ):
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
             time_step,
+            agg_metric=agg_metric,
         )
 
     def _preprocess(self, **kwargs) -> pd.DataFrame:
         super()._preprocess(**kwargs)
         return self.clim_df
 
     def detect_anomaly(self, **kwargs) -> pd.DataFrame:
         super().detect_anomaly(**kwargs)
 
         self.clim_df["zscore"] = self.clim_df.groupby(self.groupby_param)[
-            f"{self.var}-avg"
+            f"{self.var}-{self.agg_metric}"
         ].transform(zscore)
 
         return filter_df(self.clim_df, **kwargs)
 
 
 class SMAPI(AnomalyDetector):
     """
@@ -211,40 +339,46 @@
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "month",
+        agg_metric: str = "mean",
         normal_metrics: str = ["mean"],
     ):
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
             time_step,
             normal_metrics,
+            agg_metric=agg_metric,
         )
 
     def _preprocess(self, **kwargs) -> pd.DataFrame:
         super()._preprocess(**kwargs)
         return self.clim_df
 
     def detect_anomaly(self, **kwargs) -> pd.DataFrame:
         super().detect_anomaly(**kwargs)
 
         for metric in self.normal_metrics:
             self.clim_df[f"smapi-{metric}"] = self.clim_df.groupby(self.groupby_param)[
-                f"{self.var}-avg"
+                f"{self.var}-{self.agg_metric}"
             ].transform(smapi, metric=metric)
 
+            self.clim_df[f"smapi-{metric}"] = self.clim_df[f"smapi-{metric}"].clip(
+                lower=-100, upper=100
+            )
+
         return filter_df(self.clim_df, **kwargs)
 
 
 class SMDI(AnomalyDetector):
     """
     A class for detecting anomalies in time series data based on the Soil Moisture Deficit Index(SMDI) method.
 
@@ -270,35 +404,37 @@
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "week",
+        agg_metric: str = "mean",
     ):
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
             time_step,
+            agg_metric=agg_metric,
         )
 
     def _preprocess(self, **kwargs) -> pd.DataFrame:
         super()._preprocess(**kwargs)
         return self.clim_df
 
     def detect_anomaly(self, **kwargs) -> pd.DataFrame:
         super().detect_anomaly(**kwargs)
 
         self.clim_df["sd"] = self.clim_df.groupby(self.groupby_param)[
-            f"{self.var}-avg"
+            f"{self.var}-{self.agg_metric}"
         ].transform(smd)
         self.clim_df["smdi"] = smdi(self.clim_df["sd"])
 
         return filter_df(self.clim_df, **kwargs)
 
 
 class SMCA(AnomalyDetector):
@@ -324,33 +460,35 @@
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "month",
         normal_metrics: List[str] = ["mean"],
+        agg_metric: str = "mean",
     ):
 
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
             time_step,
             normal_metrics,
+            agg_metric=agg_metric,
         )
 
     def detect_anomaly(self, **kwargs) -> pd.DataFrame:
         super().detect_anomaly(**kwargs)
         for metric in self.normal_metrics:
             self.clim_df[f"smca-{metric}"] = self.clim_df.groupby(self.groupby_param)[
-                f"{self.var}-avg"
+                f"{self.var}-{self.agg_metric}"
             ].transform(smca, metric=metric)
 
         return filter_df(self.clim_df, **kwargs)
 
 
 class SMAD(AnomalyDetector):
     """
@@ -372,35 +510,37 @@
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "month",
+        agg_metric: str = "mean",
     ):
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
             time_step,
             ["median"],
+            agg_metric=agg_metric,
         )
 
     def _preprocess(self, **kwargs) -> pd.DataFrame:
         super()._preprocess(**kwargs)
         return self.clim_df
 
     def detect_anomaly(self, **kwargs) -> pd.DataFrame:
         super().detect_anomaly(**kwargs)
         self.clim_df["smad"] = self.clim_df.groupby(self.groupby_param)[
-            f"{self.var}-avg"
+            f"{self.var}-{self.agg_metric}"
         ].transform(smad)
 
         return filter_df(self.clim_df, **kwargs)
 
 
 class SMCI(AnomalyDetector):
     """
@@ -422,33 +562,35 @@
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "month",
+        agg_metric: str = "mean",
     ):
 
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
             time_step,
             ["min", "max"],
+            agg_metric=agg_metric,
         )
 
     def detect_anomaly(self, **kwargs) -> pd.DataFrame:
         super().detect_anomaly(**kwargs)
 
         self.clim_df["smci"] = self.clim_df.groupby(self.groupby_param)[
-            f"{self.var}-avg"
+            f"{self.var}-{self.agg_metric}"
         ].transform(smci)
 
         return filter_df(self.clim_df, **kwargs)
 
 
 class SMDS(AnomalyDetector):
     """
@@ -472,34 +614,36 @@
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "month",
+        agg_metric: str = "mean",
     ):
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
             time_step,
+            agg_metric=agg_metric,
         )
 
     def _preprocess(self, **kwargs) -> pd.DataFrame:
         super()._preprocess(**kwargs)
         return self.clim_df
 
     def detect_anomaly(self, **kwargs) -> pd.DataFrame:
         super().detect_anomaly(**kwargs)
         self.clim_df["smds"] = self.clim_df.groupby(self.groupby_param)[
-            f"{self.var}-avg"
+            f"{self.var}-{self.agg_metric}"
         ].transform(smds)
         return filter_df(self.clim_df, **kwargs)
 
 
 class ESSMI(AnomalyDetector):
     """
     A class for detecting anomalies in time series data based on the Empirical Standardized Soil
@@ -538,35 +682,37 @@
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "month",
+        agg_metric: str = "mean",
     ):
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
             time_step,
             ["mean"],
+            agg_metric=agg_metric,
         )
 
     def _preprocess(self, **kwargs) -> pd.DataFrame:
         super()._preprocess(**kwargs)
         return self.clim_df
 
     def detect_anomaly(self, **kwargs) -> pd.DataFrame:
         super().detect_anomaly(**kwargs)
         self.clim_df["essmi"] = self.clim_df.groupby(self.groupby_param)[
-            f"{self.var}-avg"
+            f"{self.var}-{self.agg_metric}"
         ].transform(essmi)
 
         return filter_df(self.clim_df, **kwargs)
 
 
 class ParaDis(AnomalyDetector):
     """
@@ -580,45 +726,51 @@
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "month",
+        agg_metric: str = "mean",
         dist: List[str] = ["beta"],
     ):
 
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
             time_step,
+            agg_metric=agg_metric,
         )
         self.dist = dist
 
     def _preprocess(self, **kwargs) -> pd.DataFrame:
         super()._preprocess(**kwargs)
         return self.clim_df
 
     def detect_anomaly(self, **kwargs) -> pd.DataFrame:
         super().detect_anomaly(**kwargs)
         for dist in self.dist:
             self.clim_df[f"{dist}"] = self.clim_df.groupby(self.groupby_param)[
-                f"{self.var}-avg"
+                f"{self.var}-{self.agg_metric}"
             ].transform(para_dis, dist=dist)
 
+            self.clim_df[f"{dist}"] = self.clim_df[f"{dist}"].clip(lower=-3, upper=3)
+
         return filter_df(self.clim_df, **kwargs)
 
 
 if __name__ == "__main__":
 
-    from pathlib import Path
-    from smadi.data_reader import extract_obs_ts
+    # from pathlib import Path
+    # from smadi.data_reader import extract_obs_ts
+
+    # ascat_path = Path("/home/m294/VSA/Code/datasets")
 
-    ascat_path = Path("/home/m294/VSA/Code/datasets")
+    # po = 4854801
+    # sm_ts = extract_obs_ts(po, ascat_path, obs_type="sm", read_bulk=False)
 
-    po = 4854801
-    sm_ts = extract_obs_ts(po, ascat_path, obs_type="sm", read_bulk=False)
+    pass
```

### Comparing `smadi-0.2.8/src/smadi/climatology.py` & `smadi-1.0.0/src/smadi/climatology.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 A module for calculating climatology (climate normal) for different time steps (month, dekad, week) based on time series data.
 """
 
-__author__ = "Muhammed Abdelaal"
-__email__ = "muhammedaabdelaal@gmail.com"
-
 from typing import List
 import pandas as pd
+import matplotlib.pyplot as plt
 
-
+from smadi.plot import get_plot_options, plot_colmns, plot_figure
 from smadi.preprocess import (
     fillna,
     smooth,
     filter_df,
     monthly_agg,
     dekadal_agg,
     weekly_agg,
@@ -44,14 +42,17 @@
 
     smooth_window_size : int
         The size of the moving window for smoothing(n-days). It is recommended to be an odd number.
 
     timespan : list[str, str] optional
         The start and end dates for a timespan to be aggregated. Format: ['YYYY-MM-DD', 'YYYY-MM-DD']
 
+    agg_metric : str
+        The aggregation metric to be used. Supported values: 'mean', 'median', 'min', 'max', 'std', etc.
+
     resulted_df : pd.DataFrame
         The resulting DataFrame after aggregation.
 
     Methods:
     --------
 
     _fillna:
@@ -85,26 +86,28 @@
         df: pd.DataFrame,
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
+        agg_metric: str = "mean",
     ):
         """
         Initializes the Aggregation class.
 
         """
         self.original_df = df
         self.var = variable
         self.fillna = fillna
         self.fillna_window_size = fillna_window_size
         self.smoothing = smoothing
         self.smooth_window_size = smooth_window_size
         self.timespan = timespan
+        self.agg_metric = agg_metric
         self._validate_input()
         self.resulted_df = pd.DataFrame()
 
     @property
     def df(self):
         """
         Prepares the DataFrame for aggregation.
@@ -229,28 +232,32 @@
         df: pd.DataFrame,
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = 3,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
+        agg_metric: str = "mean",
     ):
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
+            agg_metric,
         )
 
     def aggregate(self, **kwargs):
 
-        self.resulted_df[f"{self.var}-avg"] = monthly_agg(self.df, self.var)
+        self.resulted_df[f"{self.var}-{self.agg_metric}"] = monthly_agg(
+            self.df, self.var, self.agg_metric
+        )
 
         return filter_df(self.resulted_df, **kwargs)
 
 
 class DekadalAggregator(Aggregator):
     """
     Aggregates the data based on dekad-based time step.
@@ -261,29 +268,33 @@
         df: pd.DataFrame,
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
+        agg_metric: str = "mean",
     ):
 
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
+            agg_metric,
         )
 
     def aggregate(self, **kwargs):
 
-        self.resulted_df[f"{self.var}-avg"] = dekadal_agg(self.df, self.var)
+        self.resulted_df[f"{self.var}-{self.agg_metric}"] = dekadal_agg(
+            self.df, self.var
+        )
 
         return filter_df(self.resulted_df, **kwargs)
 
 
 class WeeklyAggregator(Aggregator):
     """
     Aggregates the time series data based on week-based time step.
@@ -294,28 +305,32 @@
         df: pd.DataFrame,
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
+        agg_metric: str = "mean",
     ):
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
+            agg_metric,
         )
 
     def aggregate(self, **kwargs):
 
-        self.resulted_df[f"{self.var}-avg"] = weekly_agg(self.df, self.var)
+        self.resulted_df[f"{self.var}-{self.agg_metric}"] = weekly_agg(
+            self.df, self.var
+        )
 
         return filter_df(self.resulted_df, **kwargs)
 
 
 class BimonthlyAggregator(Aggregator):
     """
     Aggregates the time series data based on bimonthly (twice a month) time step.
@@ -326,28 +341,32 @@
         df: pd.DataFrame,
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
+        agg_metric: str = "mean",
     ):
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
+            agg_metric,
         )
 
     def aggregate(self, **kwargs):
 
-        self.resulted_df[f"{self.var}-avg"] = bimonthly_agg(self.df, self.var)
+        self.resulted_df[f"{self.var}-{self.agg_metric}"] = bimonthly_agg(
+            self.df, self.var
+        )
 
         return filter_df(self.resulted_df, **kwargs)
 
 
 class DailyAggregator(Aggregator):
     """
     Aggregates the time series data based on daily time step.
@@ -358,28 +377,30 @@
         df: pd.DataFrame,
         variable: str,
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
+        agg_metric: str = "mean",
     ):
 
         super().__init__(
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
+            agg_metric,
         )
 
     def aggregate(self, **kwargs):
-        self.resulted_df[f"{self.var}-avg"] = self.df[self.var]
+        self.resulted_df[f"{self.var}-{self.agg_metric}"] = self.df[self.var]
         return filter_df(self.resulted_df.drop_duplicates(), **kwargs)
 
 
 class Climatology(Aggregator):
     """
     A class for calculating climatology(climate normal) for time series data.
 
@@ -408,14 +429,17 @@
 
     timespan: list[str, str] optional
         The start and end dates for a timespan to be aggregated. Format: ['YYYY-MM-DD ]
 
     time_step: str
         The time step for aggregation. Supported values: 'day', 'week', 'dekad', 'bimonth', 'month'.
 
+    agg_metric: str
+        The aggregation metric to be used. Supported values: 'mean', 'median', 'min', 'max', 'std', etc.
+
     normal_metrics: List[str]
         The metrics to be used in the climatology computation. Supported values: 'mean', 'median', 'min', 'max', etc.
 
     clima_df: pd.DataFrame
         The DataFrame containing climatology information.
 
     Methods:
@@ -440,14 +464,15 @@
         fillna: bool = False,
         fillna_window_size: int = None,
         smoothing=False,
         smooth_window_size=None,
         timespan: List[str] = None,
         time_step: str = "month",
         normal_metrics: List[str] = ["mean"],
+        agg_metric: str = "mean",
     ):
         """
         Initializes the Climatology class.
         """
         self.time_step = time_step
         self.normal_metrics = normal_metrics
         self.valid_time_steps = ["month", "dekad", "week", "day", "bimonth"]
@@ -456,14 +481,15 @@
             df,
             variable,
             fillna,
             fillna_window_size,
             smoothing,
             smooth_window_size,
             timespan,
+            agg_metric,
         )
         self.clim_df = pd.DataFrame()
 
     def _validate_time_step(
         self,
     ) -> None:
         """
@@ -501,68 +527,38 @@
         self._validate_metrics()
 
     def aggregate(self):
         """
         Aggregates the data based on the time step and metrics provided.
 
         """
+        params = {
+            "df": self.df,
+            "variable": self.var,
+            "fillna": self.fillna,
+            "fillna_window_size": self.fillna_window_size,
+            "smoothing": self.smoothing,
+            "smooth_window_size": self.smooth_window_size,
+            "timespan": self.timespan,
+            "agg_metric": self.agg_metric,
+        }
         if self.time_step == "month":
-            return MonthlyAggregator(
-                self.df,
-                self.var,
-                self.fillna,
-                self.fillna_window_size,
-                self.smoothing,
-                self.smooth_window_size,
-                self.timespan,
-            ).aggregate()
+            return MonthlyAggregator(**params).aggregate()
 
         elif self.time_step == "week":
-            return WeeklyAggregator(
-                self.df,
-                self.var,
-                self.fillna,
-                self.fillna_window_size,
-                self.smoothing,
-                self.smooth_window_size,
-                self.timespan,
-            ).aggregate()
+            return WeeklyAggregator(**params).aggregate()
 
         elif self.time_step == "dekad":
-            return DekadalAggregator(
-                self.df,
-                self.var,
-                self.fillna,
-                self.fillna_window_size,
-                self.smoothing,
-                self.smooth_window_size,
-                self.timespan,
-            ).aggregate()
+            return DekadalAggregator(**params).aggregate()
 
         elif self.time_step == "bimonth":
-            return BimonthlyAggregator(
-                self.df,
-                self.var,
-                self.fillna,
-                self.fillna_window_size,
-                self.smoothing,
-                self.smooth_window_size,
-                self.timespan,
-            ).aggregate()
+            return BimonthlyAggregator(**params).aggregate()
 
         elif self.time_step == "day":
-            return DailyAggregator(
-                self.df,
-                self.var,
-                self.fillna,
-                self.fillna_window_size,
-                self.smoothing,
-                self.smooth_window_size,
-                self.timespan,
-            ).aggregate()
+            return DailyAggregator(**params).aggregate()
 
     def compute_normals(self, **kwargs) -> pd.DataFrame:
         """
         Calculates climatology based on the aggregated data.
 
         Parameters:
         -----------
@@ -570,12 +566,87 @@
             Additional time/date filtering parameters.
 
         Returns:
         --------
         pd.DataFrame
             The DataFrame containing climatology information.
         """
+
         self.clim_df = compute_clim(
-            self.aggregate(), self.time_step, f"{self.var}-avg", self.normal_metrics
+            self.aggregate(),
+            self.time_step,
+            f"{self.var}-{self.agg_metric}",
+            self.normal_metrics,
         )
 
         return filter_df(self.clim_df, **kwargs)
+
+    def plot_ts(
+        self,
+        df=None,
+        x_axis=None,
+        colmns_kwargs=None,
+        plot_raw=False,
+        raw_resample="D",
+        raw_kwargs=None,
+        plot_style="ggplot",
+        **kwargs,
+    ):
+        """
+        Plot the time series data for the provided dataframe.
+
+        parameters:
+        -----------
+
+        df: pd.DataFrame
+            The dataframe containing the data to plot. or None if the climatology object is used.
+
+        x_axis: list
+            The x-axis values for the plot. or None if the climatology object is used.
+
+        colmns_kwargs: dict
+            The dictionary containing the column names and their respective matplotlib plot options.
+
+        plot_raw: bool
+            Whether to plot the raw data on the plot as background.
+
+        raw_resample: str
+            The resample frequency for the raw data. Supported values: 'D', 'W', 'M', etc.
+
+        raw_kwargs: dict
+            The dictionary containing the matplotlib plot options for the raw data.
+
+        kwargs: dict
+            The keyword arguments for the matplotlib plot for the figure such as title, xlabel, ylabel, legend, figsize, and grid.
+
+        """
+        # Set values for kwargs based on provided values
+        plt.style.use(plot_style)
+        df = self.compute_normals() if df is None else df
+        x_axis = df.index if x_axis is None else x_axis
+        colmns_kwargs = (
+            {
+                f"{self.var}-{self.agg_metric}": {
+                    "label": f"{self.var}-{self.agg_metric}"
+                }
+            }
+            if colmns_kwargs is None
+            else colmns_kwargs
+        )
+        plot_params = get_plot_options(**kwargs)
+        if plot_params["figsize"] is not None:
+            plt.figure(figsize=plot_params["figsize"])
+
+        if plot_raw:
+            raw_df = (
+                self.original_df.resample(raw_resample).mean()
+                if raw_resample
+                else self.original_df
+            )
+            plt.plot(
+                raw_df.index,
+                raw_df[f"{self.var}"],
+                **raw_kwargs if raw_kwargs else {"alpha": 0.5, "label": "Raw Data"},
+            )
+
+        plot_colmns(df, x_axis, colmns_kwargs)
+        plot_figure(plot_params)
```

### Comparing `smadi-0.2.8/src/smadi/indicators.py` & `smadi-1.0.0/src/smadi/indicators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 from scipy.stats import gaussian_kde
 from scipy.stats import norm, beta, gamma
 from scipy.stats import percentileofscore
+from standard_precip.spi import SPI
 
 
 def zscore(obs, mean=None, std=None):
     """
     Computes the standardized z-score of the time series data.
 
     Parameters:
@@ -266,23 +267,35 @@
     parameters:
     -----------
 
     obs: pd.Series or np.ndarray or sequence-like object
         The observed time series data.
 
     dist: str, optional
-        The distribution to fit the observed data to. Supported values: 'beta', 'gamma'
+        The distribution to fit the observed data to. Supported values: 'beta','gamma', 'gam', 'exp', 'pe3'
+        gam: Gamma
+        exp: Exponential
+        pe3: Pearson III
+
+
     """
 
     obs = np.asarray(obs)
 
     if dist == "beta":
         a, b, loc, scale = beta.fit(obs)
         fitted = beta(a, b, loc, scale)
+        cdf = fitted.cdf(obs)
+
+        return norm.ppf(cdf)
 
     elif dist == "gamma":
         shape, loc, scale = gamma.fit(obs)
         fitted = gamma(shape, loc, scale)
+        cdf = fitted.cdf(obs)
+        return norm.ppf(cdf)
 
-    cdf = fitted.cdf(obs)
+    else:
+        param_dis = SPI()
+        params, p_zero = param_dis.fit_distribution(obs, dist, "lmom")
 
-    return norm.ppf(cdf)
+        return param_dis.cdf_to_ppf(obs, params, p_zero)
```

### Comparing `smadi-0.2.8/src/smadi/plot.py` & `smadi-1.0.0/src/smadi/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 import matplotlib
 import matplotlib.pyplot as plt
 
 
-from smadi.anomaly_detectors import *
 from smadi.metadata import indicators_thresholds
-from smadi.map import set_thresholds
+
+
+def set_thresholds(method):
+    """
+    Set the thresholds for the specified method based on the method name.
+
+    parameters:
+    -----------
+
+    method: str
+        The method name for which the thresholds are to be set. Supported methods are:
+        'zscore', 'smapi', 'smdi', 'smca', 'smad', 'smci', 'smds', 'essmi', 'beta', 'gamma'
+    """
+
+    if method in indicators_thresholds.keys():
+        return indicators_thresholds[method]
+    else:
+        return None
 
 
 def get_plot_options(**kwargs):
     """
     Set the basic plot options based on the provided kwargs for the plot.
 
     parameters:
```

### Comparing `smadi-0.2.8/src/smadi/preprocess.py` & `smadi-1.0.0/src/smadi/preprocess.py`

 * *Files 8% similar despite different names*

```diff
@@ -141,109 +141,117 @@
 
     if day:
         df = df[df.index.day == day]
 
     return df
 
 
-def monthly_agg(df: pd.DataFrame, variable: str) -> pd.DataFrame:
+def monthly_agg(df: pd.DataFrame, variable: str, agg_metric="mean") -> pd.DataFrame:
     """
     Aggregates the time series data based on month-based time step.
 
     Parameters:
     -----------
     df: pd.DataFrame
         The DataFrame containing the time series data to be aggregated indexed by datetime index.
 
     variable: str
         The variable/column in the DataFrame to be aggregated.
 
+    agg_metric: str
+        The aggregation metric to be used. Supported values: 'mean', 'median', 'min', 'max', etc.
+
     Returns:
     --------
     pd.DataFrame
         The DataFrame containing the aggregated data.
     """
-    return (
-        df.groupby([df.index.year, df.index.month])[variable]
-        .transform("mean")
-        .drop_duplicates()
-    )
+    return df.resample("ME")[variable].agg(agg_metric)
 
 
-def dekadal_agg(df: pd.DataFrame, variable: str) -> pd.DataFrame:
+def dekadal_agg(df: pd.DataFrame, variable: str, agg_metric="mean") -> pd.DataFrame:
     """
     Aggregates the time series data based on dekad-based time step.
 
     Parameters:
     -----------
     df: pd.DataFrame
         The DataFrame containing the time series data to be aggregated indexed by datetime index.
 
     variable: str
         The variable/column in the DataFrame to be aggregated.
 
+    agg_metric: str
+        The aggregation metric to be used. Supported values: 'mean', 'median', 'min', 'max', etc.
+
     Returns:
     --------
     pd.DataFrame
         The DataFrame containing the aggregated data.
     """
     df["dekad"] = df.index.map(lambda x: 1 if x.day <= 10 else 2 if x.day <= 20 else 3)
     return (
         df.groupby([df.index.year, df.index.month, "dekad"])[variable]
-        .transform("mean")
+        .transform(agg_metric)
         .drop_duplicates()
     )
 
 
-def weekly_agg(df: pd.DataFrame, variable: str) -> pd.DataFrame:
+def weekly_agg(df: pd.DataFrame, variable: str, agg_metric="mean") -> pd.DataFrame:
     """
     Aggregates the time series data based on week-based time step.
 
     Parameters:
     -----------
     df: pd.DataFrame
         The DataFrame containing the time series data to be aggregated indexed by datetime index.
 
     variable: str
         The variable/column in the DataFrame to be aggregated.
 
+    agg_metric: str
+        The aggregation metric to be used. Supported values: 'mean', 'median', 'min', 'max', etc.
+
     Returns:
     --------
     pd.DataFrame
         The DataFrame containing the aggregated data.
     """
     return (
         df.groupby([df.index.year, df.index.isocalendar().week])[variable]
-        .transform("mean")
+        .transform(agg_metric)
         .drop_duplicates()
     )
 
 
-def bimonthly_agg(df: pd.DataFrame, variable: str) -> pd.DataFrame:
+def bimonthly_agg(df: pd.DataFrame, variable: str, agg_metric="mean") -> pd.DataFrame:
     """
     Aggregates the time series data based on bimonth-based time step.
 
     Parameters:
     -----------
     df: pd.DataFrame
         The DataFrame containing the time series data to be aggregated indexed by datetime index.
 
     variable: str
         The variable/column in the DataFrame to be aggregated.
 
+    agg_metric: str
+        The aggregation metric to be used. Supported values: 'mean', 'median', 'min', 'max', etc.
+
     Returns:
     --------
     pd.DataFrame
         The DataFrame containing the aggregated data.
     """
     if "bimonth" not in df.columns:
         df["bimonth"] = df.index.map(lambda x: 1 if x.day <= 15 else 2)
     return (
         df.groupby([df.index.year, df.index.month, df["bimonth"]])[variable]
-        .transform("mean")
+        .transform(agg_metric)
         .drop_duplicates()
     )
 
 
 def clim_groupping(df: pd.DataFrame, time_step: str) -> list:
     """
     Groups the DataFrame based on the provided time step for climatology computation.
```

### Comparing `smadi-0.2.8/src/smadi/utils.py` & `smadi-1.0.0/src/smadi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import logging
 import requests
 from functools import wraps
 from time import time
 from io import StringIO
 import pycountry
 import pandas as pd
+import matplotlib.pyplot as plt
 
 from fibgrid.realization import FibLandGrid
 
+from smadi.metadata import indicators_thresholds
+
 
 def create_logger(name, level=logging.DEBUG):
     """
     Create a logger with the given name and level
 
     parameters:
     -----------
```

### Comparing `smadi-0.2.8/src/smadi/workflow.py` & `smadi-1.0.0/src/smadi/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,55 @@
 """
 run_workflow.py - SMADI Workflow Execution
 
 """
 
-__author__ = "Muhammed Abdelaal"
-__email__ = "muhammedaabdelaal@gmail.com"
-
 from argparse import ArgumentParser, Namespace, ArgumentError
 from typing import List, Tuple, Union, Dict
 from concurrent.futures import ProcessPoolExecutor
 from functools import partial
 import pandas as pd
 import numpy as np
 
 
-from smadi.metadata import _Detectors
-from smadi.data_reader import AscatData
+from smadi.data_reader import AscatData, read_era5
 from smadi.utils import (
     create_logger,
     log_exception,
     log_time,
     load_gpis_by_country,
     get_gpis_from_bbox,
 )
+from smadi.anomaly_detectors import (
+    ZScore,
+    SMAPI,
+    SMDI,
+    SMCA,
+    SMAD,
+    SMCI,
+    SMDS,
+    ESSMI,
+    ParaDis,
+)
+
+# Supported anomaly detection methods
+_Detectors = {
+    "zscore": ZScore,
+    "smapi-mean": SMAPI,
+    "smapi-median": SMAPI,
+    "smdi": SMDI,
+    "smca-mean": SMCA,
+    "smca-median": SMCA,
+    "smad": SMAD,
+    "smci": SMCI,
+    "smds": SMDS,
+    "essmi": ESSMI,
+    "beta": ParaDis,
+    "gamma": ParaDis,
+}
 
 
 def setup_argument_parser() -> ArgumentParser:
     """
     Setup argument parser for SMADI workflow execution.
     """
     parser = ArgumentParser(
@@ -387,44 +410,47 @@
 
 def addi_retrival(
     addi_retrive: list = ["var", "norm", "abs"],
     results: pd.DataFrame = None,
     anomaly: pd.DataFrame = None,
     variable: str = None,
     date_str: str = None,
+    agg_metric: str = "mean",
 ):
     """
     Validate and retrieve additional parameters from the anomaly dataframe.
     """
 
     if addi_retrive is not None:
 
         # if not all(value in ["var", "norm"] for value in addi_retrive):
         #     raise ValueError(
         #         "The additional retrieval parameters must be one of the following: 'var', 'norm'"
         #     )
 
         if "var" in addi_retrive:
-            results[f"{variable}-avg" + f"({date_str})"] = anomaly[
-                f"{variable}-avg"
+            results[f"{variable}-{agg_metric}" + f"({date_str})"] = anomaly[
+                f"{variable}-{agg_metric}"
             ].values
         if "norm" in addi_retrive:
             if "norm-mean" in anomaly.columns:
                 results["norm-mean" + f"({date_str})"] = anomaly["norm-mean"].values
             if "norm-median" in anomaly.columns:
                 results["norm-median" + f"({date_str})"] = anomaly["norm-median"].values
 
         if "abs" in addi_retrive:
             if "norm-mean" in anomaly.columns:
                 results["abs-mean" + f"({date_str})"] = (
-                    anomaly[f"{variable}-avg"].values - anomaly["norm-mean"].values
+                    anomaly[f"{variable}-{agg_metric}"].values
+                    - anomaly["norm-mean"].values
                 )
             if "norm-median" in anomaly.columns:
                 results["abs-median" + f"({date_str})"] = (
-                    anomaly[f"{variable}-avg"].values - anomaly["norm-median"].values
+                    anomaly[f"{variable}-{agg_metric}"].values
+                    - anomaly["norm-median"].values
                 )
 
     return results
 
 
 @log_exception(logger)
 def single_po_run(
@@ -440,14 +466,17 @@
     month: Union[int, List[int]] = None,
     dekad: Union[int, List[int]] = None,
     week: Union[int, List[int]] = None,
     bimonth: Union[int, List[int]] = None,
     day: Union[int, List[int]] = None,
     timespan: List[str] = None,
     addi_retrive: list = ["var", "norm"],
+    agg_metric: list = "mean",
+    mode: str = "anomaly",
+    era5_path: str = None,
 ) -> Tuple[int, Dict[str, float]]:
     """
     Run the anomaly detection workflow for a single grid point index.
     """
 
     # Load the time series for the given gpi
     global ascat_obj
@@ -471,38 +500,44 @@
             "variable": variable,
             "time_step": time_step,
             "fillna": fillna,
             "fillna_window_size": fillna_window_size,
             "smoothing": smoothing,
             "smooth_window_size": smooth_window_size,
             "timespan": timespan,
+            "agg_metric": agg_metric,
         }
 
         # If the method has a metric parameter (e.g. smapi-mean, smapi-median), set the metric parameter
         if "-" in method:
             anomaly_params["normal_metrics"] = [method.split("-")[1]]
 
         elif method in ["beta", "gamma"]:
             anomaly_params["dist"] = [method]
 
         try:
             for date_param in date_params:
                 anomaly = _Detectors[method](**anomaly_params).detect_anomaly(
                     **date_param
                 )
+
+                # if mode == "anomaly":
                 date_str = f"-".join(str(value) for value in date_param.values())
                 results[method + f"({date_str})"] = anomaly[method].values
 
                 results = addi_retrival(
                     addi_retrive=addi_retrive,
                     results=results,
                     anomaly=anomaly,
                     variable=variable,
                     date_str=date_str,
+                    agg_metric=agg_metric,
                 )
+                # elif mode == "spi":
+                #     era5_df = read_era5(era5_path, loc=(lon, lat))
 
         except AttributeError as e:
             return None
 
     return (gpi, results)
```

### Comparing `smadi-0.2.8/src/smadi.egg-info/SOURCES.txt` & `smadi-1.0.0/src/smadi.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -13,18 +13,25 @@
 tox.ini
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
+docs/introduction.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
+docs/examples/Installation.ipynb
+docs/examples/Loading_data.ipynb
+docs/examples/compute_climatology.ipynb
+docs/examples/detect_the_anomlies.ipynb
+docs/examples/plot_climatology.ipynb
+docs/examples/workflow.ipynb
 src/smadi/__init__.py
 src/smadi/anomaly_detectors.py
 src/smadi/climatology.py
 src/smadi/data_reader.py
 src/smadi/indicators.py
 src/smadi/map.py
 src/smadi/metadata.py
```

### Comparing `smadi-0.2.8/tests/conftest.py` & `smadi-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/tests/data_sample.csv` & `smadi-1.0.0/tests/data_sample.csv`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/tests/test_climatology.py` & `smadi-1.0.0/tests/test_climatology.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         """
 
         assert aggregator.aggregate() is not None
         # Perform aggregation
         df = aggregator.aggregate()
         # Check if aggregation result is a DataFrame
         assert isinstance(df, pd.DataFrame)
-        assert f"{variable}-avg" in df.columns
+        assert f"{variable}-mean" in df.columns
 
     @pytest.mark.skip(reason="Test implemented only for child classes.")
     def test_drop_duplicates(self, aggregator):
         """
         Test the drop_duplicates of Aggregator class.
         """
         # Perform aggregation
@@ -130,15 +130,15 @@
 
         daily_obs = Aggregator(data_sample, variable).aggregate(year=2022, month=2)
         month_avg = MonthlyAggregator(data_sample, variable).aggregate(
             year=2022, month=2
         )
 
         assert daily_obs[variable].mean() == pytest.approx(
-            month_avg[f"{variable}-avg"].iloc[0]
+            month_avg[f"{variable}-mean"].iloc[0]
         )
 
     def test_drop_duplicates(self, aggregator):
         """
         Test the drop_duplicates of MonthlyAggregator class.
         """
         super().test_drop_duplicates(aggregator)
@@ -187,15 +187,15 @@
             year=2019, month=1, dekad=3
         )
         dekadal_avg = DekadalAggregator(data_sample, variable).aggregate(
             year=2019, month=1, dekad=3
         )
 
         assert daily_obs[variable].mean() == pytest.approx(
-            dekadal_avg[f"{variable}-avg"].iloc[0]
+            dekadal_avg[f"{variable}-mean"].iloc[0]
         )
 
     def test_drop_duplicates(self, aggregator):
         """
         Test the drop_duplicates of DekadalAggregator class.
         """
         super().test_drop_duplicates(aggregator)
@@ -242,15 +242,15 @@
 
         daily_obs = Aggregator(data_sample, variable).aggregate(year=2015, week=15)
         weekly_obs = WeeklyAggregator(data_sample, variable).aggregate(
             year=2015, week=15
         )
 
         assert daily_obs[variable].mean() == pytest.approx(
-            weekly_obs[f"{variable}-avg"].iloc[0]
+            weekly_obs[f"{variable}-mean"].iloc[0]
         )
 
     def test_drop_duplicates(self, aggregator):
         """
         Test the drop_duplicates of WeeklyAggregator class.
         """
         super().test_drop_duplicates(aggregator)
@@ -299,15 +299,15 @@
             year=2015, month=5, bimonth=1
         )
         bimonthly_obs = BimonthlyAggregator(data_sample, variable).aggregate(
             year=2015, month=5, bimonth=1
         )
 
         assert daily_obs[variable].mean() == pytest.approx(
-            bimonthly_obs[f"{variable}-avg"].iloc[0]
+            bimonthly_obs[f"{variable}-mean"].iloc[0]
         )
 
     def test_drop_duplicates(self, aggregator, variable="sm"):
         """
         Test the drop_duplicates of BimonthlyAggregator class.
         """
         super().test_drop_duplicates(aggregator)
@@ -356,15 +356,15 @@
             year=2015, month=5, day=1
         )
         daily_avg = DailyAggregator(data_sample, variable).aggregate(
             year=2015, month=5, day=1
         )
 
         assert daily_obs[variable].mean() == pytest.approx(
-            daily_avg[f"{variable}-avg"].iloc[0]
+            daily_avg[f"{variable}-mean"].iloc[0]
         )
 
     def test_aggregate_filter_df(data_sample, aggregator):
         """
         Test the aggregation method of DailyAggregator class with filtering.
         """
 
@@ -463,15 +463,15 @@
         """
         Test the aggregation method of Climatology class.
         """
 
         climatology.time_step = time_steps
         df = climatology.aggregate()
         assert isinstance(df, pd.DataFrame)
-        assert f"{climatology.var}-avg" in df.columns
+        assert f"{climatology.var}-mean" in df.columns
         assert (
             (df == _class(climatology.original_df, climatology.var).aggregate())
             .all()
             .all()
         )
 
     @pytest.mark.parametrize(
@@ -507,15 +507,15 @@
               months, dekads, weeks, bimonths, and days with different metrics.
         """
         clim_metrics_all.time_step = time_step
         df = clim_metrics_all.compute_normals(
             month=month, dekad=dekad, week=week, bimonth=bimonth, day=day
         )
 
-        expected_normal = df[f"{clim_metrics_all.var}-avg"].agg(metric)
+        expected_normal = df[f"{clim_metrics_all.var}-mean"].agg(metric)
         computed_normal = random.choice(df[f"norm-{metric}"])
         assert computed_normal == pytest.approx(expected_normal, rel=1e-4)
 
     @pytest.mark.parametrize(
         "time_step, metric, month, dekad, week, bimonth, day , window_size",
         [
             ("month", "mean", 2, None, None, None, None, 5),
@@ -559,14 +559,14 @@
         clim_metrics_all.time_step = time_step
         clim_metrics_all.smoothing = True
         clim_metrics_all.smooth_window_size = window_size
         df = clim_metrics_all.compute_normals(
             month=month, dekad=dekad, week=week, bimonth=bimonth, day=day
         )
 
-        expected_normal = df[f"{clim_metrics_all.var}-avg"].agg(metric)
+        expected_normal = df[f"{clim_metrics_all.var}-mean"].agg(metric)
         computed_normal = random.choice(df[f"norm-{metric}"])
         assert computed_normal == pytest.approx(expected_normal, rel=1e-4)
 
 
 if __name__ == "__main__":
     pytest.main([__file__])
```

### Comparing `smadi-0.2.8/tests/test_indicators.py` & `smadi-1.0.0/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `smadi-0.2.8/tox.ini` & `smadi-1.0.0/tox.ini`

 * *Files identical despite different names*

