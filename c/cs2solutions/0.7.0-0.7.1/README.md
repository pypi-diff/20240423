# Comparing `tmp/cs2solutions-0.7.0.tar.gz` & `tmp/cs2solutions-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dejan/eth/CSII/cs2solutions/dist/.tmp-tjr5nexu/cs2solutions-0.7.0.tar", last modified: Mon Apr 22 07:53:50 2024, max compression
+gzip compressed data, was "/home/dejan/eth/CSII/cs2solutions/dist/.tmp-lxgfoiyd/cs2solutions-0.7.1.tar", last modified: Tue Apr 23 06:18:14 2024, max compression
```

## Comparing `cs2solutions-0.7.0.tar` & `cs2solutions-0.7.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-22 07:53:50.444540 cs2solutions-0.7.0/
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    35149 2024-02-20 16:57:23.000000 cs2solutions-0.7.0/LICENSE
--rw-r--r--   0 dejan     (1000) dejan     (1000)    42298 2024-04-22 07:53:50.444540 cs2solutions-0.7.0/PKG-INFO
--rw-rw-r--   0 dejan     (1000) dejan     (1000)      706 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/README.md
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     1279 2024-04-22 07:50:49.000000 cs2solutions-0.7.0/pyproject.toml
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       38 2024-04-22 07:53:50.444540 cs2solutions-0.7.0/setup.cfg
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-22 07:53:50.440540 cs2solutions-0.7.0/src/
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-22 07:53:50.444540 cs2solutions-0.7.0/src/cs2solutions/
--rw-rw-r--   0 dejan     (1000) dejan     (1000)      151 2024-04-22 07:50:49.000000 cs2solutions-0.7.0/src/cs2solutions/__init__.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     6885 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/aircraft.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)        0 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/cs.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     5975 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/cs2bot.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    10851 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/decomp.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    21154 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/discretization.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    10908 2024-04-16 07:25:19.000000 cs2solutions-0.7.0/src/cs2solutions/duckiebot.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     7763 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/intro.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    15366 2024-04-16 15:23:07.000000 cs2solutions-0.7.0/src/cs2solutions/intromimo.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    13252 2024-04-16 07:25:19.000000 cs2solutions-0.7.0/src/cs2solutions/lqg.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    10752 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/lqrfeedback.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    13341 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/morse.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    15555 2024-04-22 07:50:49.000000 cs2solutions-0.7.0/src/cs2solutions/norms.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       90 2024-02-20 16:57:23.000000 cs2solutions-0.7.0/src/cs2solutions/plot.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       68 2024-02-20 16:57:23.000000 cs2solutions-0.7.0/src/cs2solutions/test.py
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-22 07:53:50.444540 cs2solutions-0.7.0/src/cs2solutions.egg-info/
--rw-r--r--   0 dejan     (1000) dejan     (1000)    42298 2024-04-22 07:53:50.000000 cs2solutions-0.7.0/src/cs2solutions.egg-info/PKG-INFO
--rw-rw-r--   0 dejan     (1000) dejan     (1000)      645 2024-04-22 07:53:50.000000 cs2solutions-0.7.0/src/cs2solutions.egg-info/SOURCES.txt
--rw-rw-r--   0 dejan     (1000) dejan     (1000)        1 2024-04-22 07:53:50.000000 cs2solutions-0.7.0/src/cs2solutions.egg-info/dependency_links.txt
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       37 2024-04-22 07:53:50.000000 cs2solutions-0.7.0/src/cs2solutions.egg-info/requires.txt
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       13 2024-04-22 07:53:50.000000 cs2solutions-0.7.0/src/cs2solutions.egg-info/top_level.txt
+drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-23 06:18:14.254251 cs2solutions-0.7.1/
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    35149 2024-02-20 16:57:23.000000 cs2solutions-0.7.1/LICENSE
+-rw-r--r--   0 dejan     (1000) dejan     (1000)    42364 2024-04-23 06:18:14.254251 cs2solutions-0.7.1/PKG-INFO
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)      706 2024-03-25 18:09:11.000000 cs2solutions-0.7.1/README.md
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)     1324 2024-04-23 06:07:16.000000 cs2solutions-0.7.1/pyproject.toml
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)       38 2024-04-23 06:18:14.254251 cs2solutions-0.7.1/setup.cfg
+drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-23 06:18:14.250251 cs2solutions-0.7.1/src/
+drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-23 06:18:14.254251 cs2solutions-0.7.1/src/cs2solutions/
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)      151 2024-04-22 07:50:49.000000 cs2solutions-0.7.1/src/cs2solutions/__init__.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)     6885 2024-03-25 18:09:11.000000 cs2solutions-0.7.1/src/cs2solutions/aircraft.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)        0 2024-03-25 18:09:11.000000 cs2solutions-0.7.1/src/cs2solutions/cs.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)     5975 2024-03-25 18:09:11.000000 cs2solutions-0.7.1/src/cs2solutions/cs2bot.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    10851 2024-03-25 18:09:11.000000 cs2solutions-0.7.1/src/cs2solutions/decomp.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    21154 2024-03-25 18:09:11.000000 cs2solutions-0.7.1/src/cs2solutions/discretization.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    10908 2024-04-16 07:25:19.000000 cs2solutions-0.7.1/src/cs2solutions/duckiebot.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)     7763 2024-03-25 18:09:11.000000 cs2solutions-0.7.1/src/cs2solutions/intro.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    15366 2024-04-16 15:23:07.000000 cs2solutions-0.7.1/src/cs2solutions/intromimo.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    13252 2024-04-16 07:25:19.000000 cs2solutions-0.7.1/src/cs2solutions/lqg.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    10752 2024-03-25 18:09:11.000000 cs2solutions-0.7.1/src/cs2solutions/lqrfeedback.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    13341 2024-03-25 18:09:11.000000 cs2solutions-0.7.1/src/cs2solutions/morse.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    15555 2024-04-22 07:50:49.000000 cs2solutions-0.7.1/src/cs2solutions/norms.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)       90 2024-02-20 16:57:23.000000 cs2solutions-0.7.1/src/cs2solutions/plot.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)       68 2024-02-20 16:57:23.000000 cs2solutions-0.7.1/src/cs2solutions/test.py
+drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-23 06:18:14.254251 cs2solutions-0.7.1/src/cs2solutions.egg-info/
+-rw-r--r--   0 dejan     (1000) dejan     (1000)    42364 2024-04-23 06:18:14.000000 cs2solutions-0.7.1/src/cs2solutions.egg-info/PKG-INFO
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)      645 2024-04-23 06:18:14.000000 cs2solutions-0.7.1/src/cs2solutions.egg-info/SOURCES.txt
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)        1 2024-04-23 06:18:14.000000 cs2solutions-0.7.1/src/cs2solutions.egg-info/dependency_links.txt
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)       58 2024-04-23 06:18:14.000000 cs2solutions-0.7.1/src/cs2solutions.egg-info/requires.txt
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)       13 2024-04-23 06:18:14.000000 cs2solutions-0.7.1/src/cs2solutions.egg-info/top_level.txt
```

### Comparing `cs2solutions-0.7.0/LICENSE` & `cs2solutions-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/PKG-INFO` & `cs2solutions-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2solutions
-Version: 0.7.0
+Version: 0.7.1
 Summary: A package containing solutions for the CS2 lecture at ETH Zürich
 Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -691,14 +691,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: control
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: sympy
+Requires-Dist: widget
+Requires-Dist: ipympl
+Requires-Dist: pandas
 
 # [cs2solutions]
 
 Python solution and helper package for the Control Systems II Jupyter Notebooks at ETHz. 
 Exercise Notebooks can be found on: https://github.com/idsc-frazzoli/CS2-2024-notebooks
 
 ## pip Installation
```

### Comparing `cs2solutions-0.7.0/README.md` & `cs2solutions-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/pyproject.toml` & `cs2solutions-0.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 build-backend = "setuptools.build_meta"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/solutions"]
 
 [project]
 name = "cs2solutions"
-version = "0.7.0"
+version = "0.7.1"
 dependencies =[
     "control",
     "matplotlib",
     "numpy",
     "scipy",
-    "sympy"
+    "sympy",
+    "widget",
+    "ipympl",
+    "pandas"
 ]
 requires-python = ">=3.9"
 authors = [
   { name="Kalle Laitinen", email="klaitinen@ethz.ch" },
   { name="Dejan Milojevic", email="dejanmi@ethz.ch" },
   { name="Niclas Scheuer", email="nscheuer@ethz.ch" }
 ]
```

### Comparing `cs2solutions-0.7.0/src/cs2solutions/aircraft.py` & `cs2solutions-0.7.1/src/cs2solutions/aircraft.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions/cs2bot.py` & `cs2solutions-0.7.1/src/cs2solutions/cs2bot.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions/decomp.py` & `cs2solutions-0.7.1/src/cs2solutions/decomp.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions/discretization.py` & `cs2solutions-0.7.1/src/cs2solutions/discretization.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions/duckiebot.py` & `cs2solutions-0.7.1/src/cs2solutions/duckiebot.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions/intro.py` & `cs2solutions-0.7.1/src/cs2solutions/intro.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions/intromimo.py` & `cs2solutions-0.7.1/src/cs2solutions/intromimo.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions/lqg.py` & `cs2solutions-0.7.1/src/cs2solutions/lqg.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions/lqrfeedback.py` & `cs2solutions-0.7.1/src/cs2solutions/lqrfeedback.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions/morse.py` & `cs2solutions-0.7.1/src/cs2solutions/morse.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions/norms.py` & `cs2solutions-0.7.1/src/cs2solutions/norms.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.7.0/src/cs2solutions.egg-info/PKG-INFO` & `cs2solutions-0.7.1/src/cs2solutions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2solutions
-Version: 0.7.0
+Version: 0.7.1
 Summary: A package containing solutions for the CS2 lecture at ETH Zürich
 Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -691,14 +691,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: control
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: sympy
+Requires-Dist: widget
+Requires-Dist: ipympl
+Requires-Dist: pandas
 
 # [cs2solutions]
 
 Python solution and helper package for the Control Systems II Jupyter Notebooks at ETHz. 
 Exercise Notebooks can be found on: https://github.com/idsc-frazzoli/CS2-2024-notebooks
 
 ## pip Installation
```

### Comparing `cs2solutions-0.7.0/src/cs2solutions.egg-info/SOURCES.txt` & `cs2solutions-0.7.1/src/cs2solutions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

