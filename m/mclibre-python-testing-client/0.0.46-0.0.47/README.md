# Comparing `tmp/mclibre_python_testing_client-0.0.46.tar.gz` & `tmp/mclibre_python_testing_client-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mclibre_python_testing_client-0.0.46.tar", last modified: Tue Apr 23 16:40:05 2024, max compression
+gzip compressed data, was "mclibre_python_testing_client-0.0.47.tar", last modified: Tue Apr 23 19:46:16 2024, max compression
```

## Comparing `mclibre_python_testing_client-0.0.46.tar` & `mclibre_python_testing_client-0.0.47.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 16:40:05.351105 mclibre_python_testing_client-0.0.46/
--rw-rw-rw-   0        0        0    35184 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.46/LICENSE
--rw-rw-rw-   0        0        0      847 2024-04-23 16:40:05.350105 mclibre_python_testing_client-0.0.46/PKG-INFO
--rw-rw-rw-   0        0        0      187 2020-02-17 09:13:41.000000 mclibre_python_testing_client-0.0.46/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 16:40:05.321099 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client/
--rw-rw-rw-   0        0        0        0 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client/__init__.py
--rw-rw-rw-   0        0        0      135 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client/__main__.py
--rw-rw-rw-   0        0        0    18397 2024-04-23 16:26:37.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client/mptc.py
-drwxrwxrwx   0        0        0        0 2024-04-23 16:40:05.349104 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/
--rw-rw-rw-   0        0        0      847 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2024-04-23 16:40:05.000000 mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 16:40:05.351105 mclibre_python_testing_client-0.0.46/setup.cfg
--rw-rw-rw-   0        0        0     1074 2024-04-23 09:29:27.000000 mclibre_python_testing_client-0.0.46/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:46:16.058113 mclibre_python_testing_client-0.0.47/
+-rw-rw-rw-   0        0        0    35184 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.47/LICENSE
+-rw-rw-rw-   0        0        0      847 2024-04-23 19:46:16.057112 mclibre_python_testing_client-0.0.47/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2020-02-17 09:13:41.000000 mclibre_python_testing_client-0.0.47/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 19:46:15.991097 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client/
+-rw-rw-rw-   0        0        0        0 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client/__init__.py
+-rw-rw-rw-   0        0        0      135 2019-01-05 07:43:04.000000 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client/__main__.py
+-rw-rw-rw-   0        0        0    18640 2024-04-23 19:44:30.000000 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client/mptc.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:46:16.055112 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client.egg-info/
+-rw-rw-rw-   0        0        0      847 2024-04-23 19:46:15.000000 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-23 19:46:15.000000 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 19:46:15.000000 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-23 19:46:15.000000 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-23 19:46:15.000000 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2024-04-23 19:46:15.000000 mclibre_python_testing_client-0.0.47/mclibre_python_testing_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 19:46:16.058113 mclibre_python_testing_client-0.0.47/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2024-04-23 19:44:57.000000 mclibre_python_testing_client-0.0.47/setup.py
```

### Comparing `mclibre_python_testing_client-0.0.46/LICENSE` & `mclibre_python_testing_client-0.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `mclibre_python_testing_client-0.0.46/PKG-INFO` & `mclibre_python_testing_client-0.0.47/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mclibre_python_testing_client
-Version: 0.0.46
+Version: 0.0.47
 Summary: Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/
 Home-page: https://github.com/BartolomeSintes/mclibre-python-testing/
 Author: Bartolome Sintes
 Author-email: bartolome.sintes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mclibre_python_testing_client-0.0.46/mclibre_python_testing_client/mptc.py` & `mclibre_python_testing_client-0.0.47/mclibre_python_testing_client/mptc.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,24 @@
 
         try:
             program.randrange = lambda *args : random_values.pop(0)
         except:
             pass
 
         try:
+            program.random.randint = lambda *args : random_values.pop(0)
+        except:
+            pass
+
+        try:
+            program.randint = lambda *args : random_values.pop(0)
+        except:
+            pass
+
+        try:
             program.random.choice = lambda *args : choice_values.pop(0)
         except:
             pass
 
         try:
             program.choice = lambda *args : choice_values.pop(0)
         except:
```

### Comparing `mclibre_python_testing_client-0.0.46/mclibre_python_testing_client.egg-info/PKG-INFO` & `mclibre_python_testing_client-0.0.47/mclibre_python_testing_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mclibre_python_testing_client
-Version: 0.0.46
+Version: 0.0.47
 Summary: Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/
 Home-page: https://github.com/BartolomeSintes/mclibre-python-testing/
 Author: Bartolome Sintes
 Author-email: bartolome.sintes@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mclibre_python_testing_client-0.0.46/setup.py` & `mclibre_python_testing_client-0.0.47/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mclibre_python_testing_client",
-    version="0.0.46",
+    version="0.0.47",
     author="Bartolome Sintes",
     author_email="bartolome.sintes@gmail.com",
     description="Testing tool for some of the exercises in mclibre.org's Python course available at https://www.mclibre.org/consultar/python/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BartolomeSintes/mclibre-python-testing/",
     # packages=setuptools.find_packages(),
     packages=["mclibre_python_testing_client"],
     # scripts=["mclibre-python-testing-client/mptc.py"],
-    entry_points={"console_scripts": ["mptc = mclibre_python_testing_client.mptc:main"]},
+    entry_points={
+        "console_scripts": ["mptc = mclibre_python_testing_client.mptc:main"]
+    },
     install_requires=["requests", "pytest"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Operating System :: OS Independent",
     ],
 )
```

