# Comparing `tmp/ratecurve-0.0.1.tar.gz` & `tmp/ratecurve-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratecurve-0.0.1.tar", last modified: Mon Apr 22 15:35:10 2024, max compression
+gzip compressed data, was "ratecurve-0.0.2.tar", last modified: Mon Apr 22 16:02:10 2024, max compression
```

## Comparing `ratecurve-0.0.1.tar` & `ratecurve-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 15:35:10.819145 ratecurve-0.0.1/
--rw-r--r--   0 disent    (1000) disent    (1000)    11357 2024-04-11 17:03:55.000000 ratecurve-0.0.1/LICENSE
--rw-r--r--   0 disent    (1000) disent    (1000)       49 2024-04-17 21:48:00.000000 ratecurve-0.0.1/MANIFEST.in
--rw-r--r--   0 disent    (1000) disent    (1000)     1104 2024-04-22 15:35:10.819145 ratecurve-0.0.1/PKG-INFO
--rw-r--r--   0 disent    (1000) disent    (1000)      188 2024-04-17 21:52:01.000000 ratecurve-0.0.1/README.md
-drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 15:35:10.819145 ratecurve-0.0.1/ratecurve/
--rw-r--r--   0 disent    (1000) disent    (1000)      404 2024-04-20 00:38:44.000000 ratecurve-0.0.1/ratecurve/__init__.py
--rw-r--r--   0 disent    (1000) disent    (1000)        0 2024-04-17 21:10:09.000000 ratecurve-0.0.1/ratecurve/__main__.py
--rw-r--r--   0 disent    (1000) disent    (1000)     1401 2024-04-22 15:25:49.000000 ratecurve-0.0.1/ratecurve/equations.py
--rw-r--r--   0 disent    (1000) disent    (1000)     8812 2024-04-22 15:22:22.000000 ratecurve-0.0.1/ratecurve/ratecurve.py
--rw-r--r--   0 disent    (1000) disent    (1000)     3140 2024-04-20 00:40:20.000000 ratecurve-0.0.1/ratecurve/utils.py
-drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 15:35:10.819145 ratecurve-0.0.1/ratecurve.egg-info/
--rw-r--r--   0 disent    (1000) disent    (1000)     1104 2024-04-22 15:35:10.000000 ratecurve-0.0.1/ratecurve.egg-info/PKG-INFO
--rw-r--r--   0 disent    (1000) disent    (1000)      427 2024-04-22 15:35:10.000000 ratecurve-0.0.1/ratecurve.egg-info/SOURCES.txt
--rw-r--r--   0 disent    (1000) disent    (1000)        1 2024-04-22 15:35:10.000000 ratecurve-0.0.1/ratecurve.egg-info/dependency_links.txt
--rw-r--r--   0 disent    (1000) disent    (1000)        1 2024-04-18 15:56:39.000000 ratecurve-0.0.1/ratecurve.egg-info/not-zip-safe
--rw-r--r--   0 disent    (1000) disent    (1000)        9 2024-04-22 15:35:10.000000 ratecurve-0.0.1/ratecurve.egg-info/requires.txt
--rw-r--r--   0 disent    (1000) disent    (1000)       10 2024-04-22 15:35:10.000000 ratecurve-0.0.1/ratecurve.egg-info/top_level.txt
--rw-r--r--   0 disent    (1000) disent    (1000)       38 2024-04-22 15:35:10.819145 ratecurve-0.0.1/setup.cfg
--rw-r--r--   0 disent    (1000) disent    (1000)     1294 2024-04-22 15:34:34.000000 ratecurve-0.0.1/setup.py
-drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 15:35:10.819145 ratecurve-0.0.1/tests/
--rw-r--r--   0 disent    (1000) disent    (1000)     4174 2024-04-22 15:31:54.000000 ratecurve-0.0.1/tests/test_curve.py
--rw-r--r--   0 disent    (1000) disent    (1000)     2482 2024-04-22 15:31:54.000000 ratecurve-0.0.1/tests/test_equations.py
--rw-r--r--   0 disent    (1000) disent    (1000)      606 2024-04-22 15:31:54.000000 ratecurve-0.0.1/tests/test_suite.py
--rw-r--r--   0 disent    (1000) disent    (1000)     3071 2024-04-22 15:31:54.000000 ratecurve-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 16:02:10.568941 ratecurve-0.0.2/
+-rw-r--r--   0 disent    (1000) disent    (1000)    11357 2024-04-11 17:03:55.000000 ratecurve-0.0.2/LICENSE
+-rw-r--r--   0 disent    (1000) disent    (1000)       49 2024-04-17 21:48:00.000000 ratecurve-0.0.2/MANIFEST.in
+-rw-r--r--   0 disent    (1000) disent    (1000)     1169 2024-04-22 16:02:10.568941 ratecurve-0.0.2/PKG-INFO
+-rw-r--r--   0 disent    (1000) disent    (1000)      188 2024-04-17 21:52:01.000000 ratecurve-0.0.2/README.md
+drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 16:02:10.558941 ratecurve-0.0.2/ratecurve/
+-rw-r--r--   0 disent    (1000) disent    (1000)      404 2024-04-20 00:38:44.000000 ratecurve-0.0.2/ratecurve/__init__.py
+-rw-r--r--   0 disent    (1000) disent    (1000)        0 2024-04-17 21:10:09.000000 ratecurve-0.0.2/ratecurve/__main__.py
+-rw-r--r--   0 disent    (1000) disent    (1000)     1401 2024-04-22 15:25:49.000000 ratecurve-0.0.2/ratecurve/equations.py
+-rw-r--r--   0 disent    (1000) disent    (1000)     8812 2024-04-22 15:22:22.000000 ratecurve-0.0.2/ratecurve/ratecurve.py
+-rw-r--r--   0 disent    (1000) disent    (1000)     3140 2024-04-20 00:40:20.000000 ratecurve-0.0.2/ratecurve/utils.py
+drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 16:02:10.558941 ratecurve-0.0.2/ratecurve.egg-info/
+-rw-r--r--   0 disent    (1000) disent    (1000)     1169 2024-04-22 16:02:10.000000 ratecurve-0.0.2/ratecurve.egg-info/PKG-INFO
+-rw-r--r--   0 disent    (1000) disent    (1000)      427 2024-04-22 16:02:10.000000 ratecurve-0.0.2/ratecurve.egg-info/SOURCES.txt
+-rw-r--r--   0 disent    (1000) disent    (1000)        1 2024-04-22 16:02:10.000000 ratecurve-0.0.2/ratecurve.egg-info/dependency_links.txt
+-rw-r--r--   0 disent    (1000) disent    (1000)        1 2024-04-18 15:56:39.000000 ratecurve-0.0.2/ratecurve.egg-info/not-zip-safe
+-rw-r--r--   0 disent    (1000) disent    (1000)       28 2024-04-22 16:02:10.000000 ratecurve-0.0.2/ratecurve.egg-info/requires.txt
+-rw-r--r--   0 disent    (1000) disent    (1000)       10 2024-04-22 16:02:10.000000 ratecurve-0.0.2/ratecurve.egg-info/top_level.txt
+-rw-r--r--   0 disent    (1000) disent    (1000)       38 2024-04-22 16:02:10.568941 ratecurve-0.0.2/setup.cfg
+-rw-r--r--   0 disent    (1000) disent    (1000)     1320 2024-04-22 16:00:45.000000 ratecurve-0.0.2/setup.py
+drwxr-xr-x   0 disent    (1000) disent    (1000)        0 2024-04-22 16:02:10.558941 ratecurve-0.0.2/tests/
+-rw-r--r--   0 disent    (1000) disent    (1000)     4174 2024-04-22 15:31:54.000000 ratecurve-0.0.2/tests/test_curve.py
+-rw-r--r--   0 disent    (1000) disent    (1000)     2482 2024-04-22 15:31:54.000000 ratecurve-0.0.2/tests/test_equations.py
+-rw-r--r--   0 disent    (1000) disent    (1000)      606 2024-04-22 15:31:54.000000 ratecurve-0.0.2/tests/test_suite.py
+-rw-r--r--   0 disent    (1000) disent    (1000)     3071 2024-04-22 15:31:54.000000 ratecurve-0.0.2/tests/test_utils.py
```

### Comparing `ratecurve-0.0.1/LICENSE` & `ratecurve-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ratecurve-0.0.1/PKG-INFO` & `ratecurve-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ratecurve
-Version: 0.0.1
+Version: 0.0.2
 Summary: simple utility for curve interpolation
-Home-page: https://github.com/disentcorp/dateroll
+Home-page: https://github.com/disentcorp/ratecurve
 Author: Disent
 Author-email: chris@disent.com
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -21,8 +21,11 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Utilities
 Classifier: Operating System :: Unix
 Requires-Python: >=3.7
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
 Requires-Dist: dateroll
```

### Comparing `ratecurve-0.0.1/ratecurve/equations.py` & `ratecurve-0.0.2/ratecurve/equations.py`

 * *Files identical despite different names*

### Comparing `ratecurve-0.0.1/ratecurve/ratecurve.py` & `ratecurve-0.0.2/ratecurve/ratecurve.py`

 * *Files identical despite different names*

### Comparing `ratecurve-0.0.1/ratecurve/utils.py` & `ratecurve-0.0.2/ratecurve/utils.py`

 * *Files identical despite different names*

### Comparing `ratecurve-0.0.1/ratecurve.egg-info/PKG-INFO` & `ratecurve-0.0.2/ratecurve.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ratecurve
-Version: 0.0.1
+Version: 0.0.2
 Summary: simple utility for curve interpolation
-Home-page: https://github.com/disentcorp/dateroll
+Home-page: https://github.com/disentcorp/ratecurve
 Author: Disent
 Author-email: chris@disent.com
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -21,8 +21,11 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Utilities
 Classifier: Operating System :: Unix
 Requires-Python: >=3.7
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: scipy
 Requires-Dist: dateroll
```

### Comparing `ratecurve-0.0.1/setup.py` & `ratecurve-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 setup(
     name="ratecurve",
-    version="0.0.1",
+    version="0.0.2",
     description="""simple utility for curve interpolation""",
     author="Disent",
     author_email="chris@disent.com",
     license="Apache Software License",
-    url="https://github.com/disentcorp/dateroll",
+    url="https://github.com/disentcorp/ratecurve",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
@@ -27,12 +27,12 @@
         "Topic :: Utilities",
         "Operating System :: Unix",
     ],
     packages=[
         "ratecurve",
     ],
     include_package_data=True,
-    install_requires=["dateroll"],
+    install_requires=["numpy","pandas","scipy","dateroll"],
     license_files=("LICENSE",),
     python_requires=">=3.7",
     zip_safe=False,
 )
```

### Comparing `ratecurve-0.0.1/tests/test_curve.py` & `ratecurve-0.0.2/tests/test_curve.py`

 * *Files identical despite different names*

### Comparing `ratecurve-0.0.1/tests/test_equations.py` & `ratecurve-0.0.2/tests/test_equations.py`

 * *Files identical despite different names*

### Comparing `ratecurve-0.0.1/tests/test_suite.py` & `ratecurve-0.0.2/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `ratecurve-0.0.1/tests/test_utils.py` & `ratecurve-0.0.2/tests/test_utils.py`

 * *Files identical despite different names*

