# Comparing `tmp/ffats-1.3.8.tar.gz` & `tmp/ffats-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffats-1.3.8.tar", last modified: Wed Apr 10 17:28:56 2024, max compression
+gzip compressed data, was "ffats-1.3.9.tar", last modified: Fri Apr 12 09:17:45 2024, max compression
```

## Comparing `ffats-1.3.8.tar` & `ffats-1.3.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-10 17:28:56.784040 ffats-1.3.8/
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      347 2024-04-06 21:16:24.000000 ffats-1.3.8/CMakeLists.txt
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-10 17:28:56.784040 ffats-1.3.8/FFATS/
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      166 2024-04-04 07:15:17.000000 ffats-1.3.8/FFATS/Base.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     7007 2024-04-04 07:31:13.000000 ffats-1.3.8/FFATS/Feature.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)    36484 2024-04-10 17:13:13.000000 ffats-1.3.8/FFATS/FeatureFunctionLib.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      785 2024-04-04 07:15:55.000000 ffats-1.3.8/FFATS/PreprocessLC.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      221 2024-04-04 07:01:49.000000 ffats-1.3.8/FFATS/__init__.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1945 2024-04-04 08:05:18.000000 ffats-1.3.8/FFATS/alignLC.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      157 2024-04-04 07:30:52.000000 ffats-1.3.8/FFATS/featureFunction.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      706 2024-04-04 07:15:38.000000 ffats-1.3.8/FFATS/import_lc_cluster.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      724 2024-04-04 07:15:42.000000 ffats-1.3.8/FFATS/import_lightcurve.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     6572 2024-04-04 07:37:28.000000 ffats-1.3.8/FFATS/lomb.py
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-10 17:28:56.784040 ffats-1.3.8/FFATS/pybind11_CAR/
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1975 2024-04-06 19:52:30.000000 ffats-1.3.8/FFATS/pybind11_CAR/fast_CAR.cpp
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)    10756 2024-04-10 17:17:51.000000 ffats-1.3.8/FFATS/test_library.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1079 2024-04-04 06:18:41.000000 ffats-1.3.8/LICENSE
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       64 2024-04-06 21:21:16.000000 ffats-1.3.8/MANIFEST.in
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-10 17:28:56.784040 ffats-1.3.8/PKG-INFO
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      581 2024-04-06 18:30:47.000000 ffats-1.3.8/README.rst
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-10 17:28:56.784040 ffats-1.3.8/ffats.egg-info/
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-10 17:28:56.000000 ffats-1.3.8/ffats.egg-info/PKG-INFO
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      521 2024-04-10 17:28:56.000000 ffats-1.3.8/ffats.egg-info/SOURCES.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-10 17:28:56.000000 ffats-1.3.8/ffats.egg-info/dependency_links.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-06 20:10:00.000000 ffats-1.3.8/ffats.egg-info/not-zip-safe
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-10 17:28:56.000000 ffats-1.3.8/ffats.egg-info/requires.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       15 2024-04-10 17:28:56.000000 ffats-1.3.8/ffats.egg-info/top_level.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      143 2024-04-06 21:50:16.000000 ffats-1.3.8/pyproject.toml
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-06 18:19:27.000000 ffats-1.3.8/requirements.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       38 2024-04-10 17:28:56.784040 ffats-1.3.8/setup.cfg
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     9421 2024-04-10 17:28:42.000000 ffats-1.3.8/setup.py
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-12 09:17:45.204993 ffats-1.3.9/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      347 2024-04-06 21:16:24.000000 ffats-1.3.9/CMakeLists.txt
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-12 09:17:45.201660 ffats-1.3.9/FFATS/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      166 2024-04-04 07:15:17.000000 ffats-1.3.9/FFATS/Base.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     7010 2024-04-12 09:15:28.000000 ffats-1.3.9/FFATS/Feature.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)    36484 2024-04-10 17:13:13.000000 ffats-1.3.9/FFATS/FeatureFunctionLib.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      784 2024-04-12 09:13:56.000000 ffats-1.3.9/FFATS/PreprocessLC.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      221 2024-04-04 07:01:49.000000 ffats-1.3.9/FFATS/__init__.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1945 2024-04-04 08:05:18.000000 ffats-1.3.9/FFATS/alignLC.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      157 2024-04-04 07:30:52.000000 ffats-1.3.9/FFATS/featureFunction.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      705 2024-04-12 09:13:48.000000 ffats-1.3.9/FFATS/import_lc_cluster.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      724 2024-04-04 07:15:42.000000 ffats-1.3.9/FFATS/import_lightcurve.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     6572 2024-04-04 07:37:28.000000 ffats-1.3.9/FFATS/lomb.py
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-12 09:17:45.204993 ffats-1.3.9/FFATS/pybind11_CAR/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1975 2024-04-06 19:52:30.000000 ffats-1.3.9/FFATS/pybind11_CAR/fast_CAR.cpp
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)    10756 2024-04-10 17:17:51.000000 ffats-1.3.9/FFATS/test_library.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1079 2024-04-04 06:18:41.000000 ffats-1.3.9/LICENSE
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       64 2024-04-06 21:21:16.000000 ffats-1.3.9/MANIFEST.in
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-12 09:17:45.204993 ffats-1.3.9/PKG-INFO
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      581 2024-04-06 18:30:47.000000 ffats-1.3.9/README.rst
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-12 09:17:45.204993 ffats-1.3.9/ffats.egg-info/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-12 09:17:45.000000 ffats-1.3.9/ffats.egg-info/PKG-INFO
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      521 2024-04-12 09:17:45.000000 ffats-1.3.9/ffats.egg-info/SOURCES.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-12 09:17:45.000000 ffats-1.3.9/ffats.egg-info/dependency_links.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-06 20:10:00.000000 ffats-1.3.9/ffats.egg-info/not-zip-safe
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-12 09:17:45.000000 ffats-1.3.9/ffats.egg-info/requires.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       15 2024-04-12 09:17:45.000000 ffats-1.3.9/ffats.egg-info/top_level.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      143 2024-04-06 21:50:16.000000 ffats-1.3.9/pyproject.toml
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-06 18:19:27.000000 ffats-1.3.9/requirements.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       38 2024-04-12 09:17:45.204993 ffats-1.3.9/setup.cfg
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     9421 2024-04-12 09:14:33.000000 ffats-1.3.9/setup.py
```

### Comparing `ffats-1.3.8/FFATS/Feature.py` & `ffats-1.3.9/FFATS/Feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,18 @@
     Additional parameters are used for individual features.
     Format is featurename = [parameters]
 
     usage:
     data = np.random.randint(0,10000, 100000000)
     # automean is the featurename and [0,0] is the parameter for the feature
     a = FeatureSpace(category='all', automean=[0,0])
-    print a.featureList
+    print(a.featureList)
     a=a.calculateFeature(data)
-    print a.result(method='array')
-    print a.result(method='dict')
+    print(a.result(method='array'))
+    print(a.result(method='dict'))
 
     """
 
     def __init__(self, Data=None, featureList=None, excludeList=[], **kwargs):
         self.featureFunc = []
         self.featureList = []
         self.featureOrder = []
```

### Comparing `ffats-1.3.8/FFATS/FeatureFunctionLib.py` & `ffats-1.3.9/FFATS/FeatureFunctionLib.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.8/FFATS/PreprocessLC.py` & `ffats-1.3.9/FFATS/PreprocessLC.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def Preprocess(self):
 
         mjd_out = []
         data_out = []
         error_out = []
 
-        for i in xrange(len(self.data)):
+        for i in range(len(self.data)):
 
             if self.error[i] < (3 * self.m) and (np.absolute(self.data[i] - np.mean(self.data)) / np.std(self.data)) < 5:
 
                 mjd_out.append(self.mjd[i])
                 data_out.append(self.data[i])
                 error_out.append(self.error[i])
```

### Comparing `ffats-1.3.8/FFATS/alignLC.py` & `ffats-1.3.9/FFATS/alignLC.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.8/FFATS/import_lc_cluster.py` & `ffats-1.3.9/FFATS/import_lc_cluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         mjd = []
         error = []
         # Opening the blue band
         # fid = open(self.id,'r')
 
         self.content1 = self.content1[3:]
 
-        for i in xrange(len(self.content1)):
+        for i in range(len(self.content1)):
             if not self.content1[i]:
                 break
             else:
                 content = self.content1[i].split(' ')
                 mjd.append(float(content[0]))
                 data.append(float(content[1]))
                 error.append(float(content[2]))
```

### Comparing `ffats-1.3.8/FFATS/import_lightcurve.py` & `ffats-1.3.9/FFATS/import_lightcurve.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.8/FFATS/lomb.py` & `ffats-1.3.9/FFATS/lomb.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.8/FFATS/pybind11_CAR/fast_CAR.cpp` & `ffats-1.3.9/FFATS/pybind11_CAR/fast_CAR.cpp`

 * *Files identical despite different names*

### Comparing `ffats-1.3.8/FFATS/test_library.py` & `ffats-1.3.9/FFATS/test_library.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.8/LICENSE` & `ffats-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ffats-1.3.8/PKG-INFO` & `ffats-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffats
-Version: 1.3.8
+Version: 1.3.9
 Summary: Library with compilation of features for time series
 Home-page: https://github.com/vBazilevich/FFATS
 Download-URL: https://github.com/vBazilevich/FFATS
 Author: Vladimir Bazilevich
 Author-email: bazilevichvl@gmail.com
 License: MIT licence
 Keywords: times series features,light curves
```

### Comparing `ffats-1.3.8/README.rst` & `ffats-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `ffats-1.3.8/ffats.egg-info/PKG-INFO` & `ffats-1.3.9/ffats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffats
-Version: 1.3.8
+Version: 1.3.9
 Summary: Library with compilation of features for time series
 Home-page: https://github.com/vBazilevich/FFATS
 Download-URL: https://github.com/vBazilevich/FFATS
 Author: Vladimir Bazilevich
 Author-email: bazilevichvl@gmail.com
 License: MIT licence
 Keywords: times series features,light curves
```

### Comparing `ffats-1.3.8/ffats.egg-info/SOURCES.txt` & `ffats-1.3.9/ffats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ffats-1.3.8/setup.py` & `ffats-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
 setup(
     name='ffats',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/development.html#single-sourcing-the-version
-    version='1.3.8',
+    version='1.3.9',
 
     description='Library with compilation of features for time series',
     long_description=readme(),
     # The project's main homepage.
     url='https://github.com/vBazilevich/FFATS',
 
     download_url = 'https://github.com/vBazilevich/FFATS',
```

