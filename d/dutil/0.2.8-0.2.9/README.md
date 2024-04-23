# Comparing `tmp/dutil-0.2.8.tar.gz` & `tmp/dutil-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dutil-0.2.8.tar", last modified: Fri Oct 30 10:11:33 2020, max compression
+gzip compressed data, was "dist/dutil-0.2.9.tar", last modified: Mon Nov 16 11:54:46 2020, max compression
```

## Comparing `dutil-0.2.8.tar` & `dutil-0.2.9.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:33.524856 dutil-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1104 2020-10-30 10:11:33.524856 dutil-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      286 2020-10-30 10:11:22.000000 dutil-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:33.520856 dutil-0.2.8/dutil/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:22.000000 dutil-0.2.8/dutil/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:33.520856 dutil-0.2.8/dutil/jupyter/
--rw-r--r--   0 runner    (1001) docker     (116)       85 2020-10-30 10:11:22.000000 dutil-0.2.8/dutil/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      187 2020-10-30 10:11:22.000000 dutil-0.2.8/dutil/jupyter/_jupyter.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:33.520856 dutil-0.2.8/dutil/pipeline/
--rw-r--r--   0 runner    (1001) docker     (116)      210 2020-10-30 10:11:22.000000 dutil-0.2.8/dutil/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9131 2020-10-30 10:11:22.000000 dutil-0.2.8/dutil/pipeline/_cached.py
--rw-r--r--   0 runner    (1001) docker     (116)     1677 2020-10-30 10:11:22.000000 dutil-0.2.8/dutil/pipeline/_dask.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:33.520856 dutil-0.2.8/dutil/stats/
--rw-r--r--   0 runner    (1001) docker     (116)      140 2020-10-30 10:11:22.000000 dutil-0.2.8/dutil/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1141 2020-10-30 10:11:22.000000 dutil-0.2.8/dutil/stats/_quantiles.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:33.520856 dutil-0.2.8/dutil/transform/
--rw-r--r--   0 runner    (1001) docker     (116)       90 2020-10-30 10:11:22.000000 dutil-0.2.8/dutil/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      697 2020-10-30 10:11:22.000000 dutil-0.2.8/dutil/transform/_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:33.520856 dutil-0.2.8/dutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1104 2020-10-30 10:11:33.000000 dutil-0.2.8/dutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      562 2020-10-30 10:11:33.000000 dutil-0.2.8/dutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-30 10:11:33.000000 dutil-0.2.8/dutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2020-10-30 10:11:33.000000 dutil-0.2.8/dutil.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       62 2020-10-30 10:11:33.000000 dutil-0.2.8/dutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2020-10-30 10:11:33.000000 dutil-0.2.8/dutil.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (116)      173 2020-10-30 10:11:33.524856 dutil-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1462 2020-10-30 10:11:22.000000 dutil-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:33.524856 dutil-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:22.000000 dutil-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-30 10:11:22.000000 dutil-0.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (116)    11375 2020-10-30 10:11:22.000000 dutil-0.2.8/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (116)      609 2020-10-30 10:11:22.000000 dutil-0.2.8/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (116)     2405 2020-10-30 10:11:22.000000 dutil-0.2.8/tests/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:46.812146 dutil-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     1146 2020-11-16 11:54:46.812146 dutil-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      320 2020-11-16 11:54:39.000000 dutil-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:46.812146 dutil-0.2.9/dutil/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:46.812146 dutil-0.2.9/dutil/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      187 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/jupyter/_jupyter.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:46.812146 dutil-0.2.9/dutil/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (116)      210 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9131 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/pipeline/_cached.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1677 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/pipeline/_dask.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:46.812146 dutil-0.2.9/dutil/stats/
+-rw-r--r--   0 runner    (1001) docker     (116)      140 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1141 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/stats/_quantiles.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:46.812146 dutil-0.2.9/dutil/string/
+-rw-r--r--   0 runner    (1001) docker     (116)      104 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      982 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/string/_string.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:46.812146 dutil-0.2.9/dutil/transform/
+-rw-r--r--   0 runner    (1001) docker     (116)       90 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      697 2020-11-16 11:54:39.000000 dutil-0.2.9/dutil/transform/_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:46.812146 dutil-0.2.9/dutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1146 2020-11-16 11:54:46.000000 dutil-0.2.9/dutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      632 2020-11-16 11:54:46.000000 dutil-0.2.9/dutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-16 11:54:46.000000 dutil-0.2.9/dutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       20 2020-11-16 11:54:46.000000 dutil-0.2.9/dutil.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       92 2020-11-16 11:54:46.000000 dutil-0.2.9/dutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       12 2020-11-16 11:54:46.000000 dutil-0.2.9/dutil.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (116)      173 2020-11-16 11:54:46.812146 dutil-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1531 2020-11-16 11:54:39.000000 dutil-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:46.812146 dutil-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:39.000000 dutil-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-16 11:54:39.000000 dutil-0.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11375 2020-11-16 11:54:39.000000 dutil-0.2.9/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (116)      609 2020-11-16 11:54:39.000000 dutil-0.2.9/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (116)      645 2020-11-16 11:54:39.000000 dutil-0.2.9/tests/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2405 2020-11-16 11:54:39.000000 dutil-0.2.9/tests/test_transform.py
```

### Comparing `dutil-0.2.8/PKG-INFO` & `dutil-0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dutil
-Version: 0.2.8
+Version: 0.2.9
 Summary: A few useful tools for data wrangling
 Home-page: https://github.com/mysterious-ben/dutil
 Author: Yaroslav Kopotilov
 Author-email: UNKNOWN
 License: Apache License, Version 2.0
 Description: # dutil
         
@@ -18,14 +18,15 @@
         
         ## Modules
         
         - `jupyter` (tools for jupyter notebooks)
         - `pipeline` (data caching and pipelines)
         - `stats` (statistical functions)
         - `transform` (data transformations)
+        - `string` (string manipulations)
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dutil-0.2.8/dutil/pipeline/_cached.py` & `dutil-0.2.9/dutil/pipeline/_cached.py`

 * *Files identical despite different names*

### Comparing `dutil-0.2.8/dutil/pipeline/_dask.py` & `dutil-0.2.9/dutil/pipeline/_dask.py`

 * *Files identical despite different names*

### Comparing `dutil-0.2.8/dutil/stats/_quantiles.py` & `dutil-0.2.9/dutil/stats/_quantiles.py`

 * *Files identical despite different names*

### Comparing `dutil-0.2.8/dutil/transform/_transform.py` & `dutil-0.2.9/dutil/transform/_transform.py`

 * *Files identical despite different names*

### Comparing `dutil-0.2.8/dutil.egg-info/PKG-INFO` & `dutil-0.2.9/dutil.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dutil
-Version: 0.2.8
+Version: 0.2.9
 Summary: A few useful tools for data wrangling
 Home-page: https://github.com/mysterious-ben/dutil
 Author: Yaroslav Kopotilov
 Author-email: UNKNOWN
 License: Apache License, Version 2.0
 Description: # dutil
         
@@ -18,14 +18,15 @@
         
         ## Modules
         
         - `jupyter` (tools for jupyter notebooks)
         - `pipeline` (data caching and pipelines)
         - `stats` (statistical functions)
         - `transform` (data transformations)
+        - `string` (string manipulations)
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dutil-0.2.8/dutil.egg-info/SOURCES.txt` & `dutil-0.2.9/dutil.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 dutil/jupyter/__init__.py
 dutil/jupyter/_jupyter.py
 dutil/pipeline/__init__.py
 dutil/pipeline/_cached.py
 dutil/pipeline/_dask.py
 dutil/stats/__init__.py
 dutil/stats/_quantiles.py
+dutil/string/__init__.py
+dutil/string/_string.py
 dutil/transform/__init__.py
 dutil/transform/_transform.py
 tests/__init__.py
 tests/conftest.py
 tests/test_pipeline.py
 tests/test_stats.py
+tests/test_string.py
 tests/test_transform.py
```

### Comparing `dutil-0.2.8/setup.py` & `dutil-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         'pandas',
         'pyarrow',
         'dill',
         'loguru',
         'xxhash',
         'dask[delayed]',
         'ipython',
+        'fuzzywuzzy',
+        'python_Levenshtein',
     ],
     entry_points={'console_scripts': []},
     packages=find_packages(),
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
@@ -38,14 +40,15 @@
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     python_requires='>=3.7',
     test_suite='tests',
     setup_requires=[
         'pytest-runner',
         'setuptools',
+        'wheel',
     ],
     tests_require=[
         'pytest',
     ]
 )
```

### Comparing `dutil-0.2.8/tests/test_pipeline.py` & `dutil-0.2.9/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `dutil-0.2.8/tests/test_stats.py` & `dutil-0.2.9/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dutil-0.2.8/tests/test_transform.py` & `dutil-0.2.9/tests/test_transform.py`

 * *Files identical despite different names*

