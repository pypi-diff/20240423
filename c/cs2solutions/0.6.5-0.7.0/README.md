# Comparing `tmp/cs2solutions-0.6.5.tar.gz` & `tmp/cs2solutions-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/dejan/eth/CSII/cs2solutions/dist/.tmp-b6fphnh9/cs2solutions-0.6.5.tar", last modified: Tue Apr 16 15:25:22 2024, max compression
+gzip compressed data, was "/home/dejan/eth/CSII/cs2solutions/dist/.tmp-tjr5nexu/cs2solutions-0.7.0.tar", last modified: Mon Apr 22 07:53:50 2024, max compression
```

## Comparing `cs2solutions-0.6.5.tar` & `cs2solutions-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-16 15:25:22.020220 cs2solutions-0.6.5/
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    35149 2024-02-20 16:57:23.000000 cs2solutions-0.6.5/LICENSE
--rw-r--r--   0 dejan     (1000) dejan     (1000)    42298 2024-04-16 15:25:22.020220 cs2solutions-0.6.5/PKG-INFO
--rw-rw-r--   0 dejan     (1000) dejan     (1000)      706 2024-03-25 18:09:11.000000 cs2solutions-0.6.5/README.md
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     1279 2024-04-16 15:24:25.000000 cs2solutions-0.6.5/pyproject.toml
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       38 2024-04-16 15:25:22.020220 cs2solutions-0.6.5/setup.cfg
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-16 15:25:22.016220 cs2solutions-0.6.5/src/
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-16 15:25:22.016220 cs2solutions-0.6.5/src/cs2solutions/
--rw-rw-r--   0 dejan     (1000) dejan     (1000)      142 2024-04-16 13:43:18.000000 cs2solutions-0.6.5/src/cs2solutions/__init__.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     6885 2024-03-25 18:09:11.000000 cs2solutions-0.6.5/src/cs2solutions/aircraft.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)        0 2024-03-25 18:09:11.000000 cs2solutions-0.6.5/src/cs2solutions/cs.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     5975 2024-03-25 18:09:11.000000 cs2solutions-0.6.5/src/cs2solutions/cs2bot.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    10851 2024-03-25 18:09:11.000000 cs2solutions-0.6.5/src/cs2solutions/decomp.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    21154 2024-03-25 18:09:11.000000 cs2solutions-0.6.5/src/cs2solutions/discretization.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    10908 2024-04-16 07:25:19.000000 cs2solutions-0.6.5/src/cs2solutions/duckiebot.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)     7763 2024-03-25 18:09:11.000000 cs2solutions-0.6.5/src/cs2solutions/intro.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    15366 2024-04-16 15:23:07.000000 cs2solutions-0.6.5/src/cs2solutions/intromimo.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    13252 2024-04-16 07:25:19.000000 cs2solutions-0.6.5/src/cs2solutions/lqg.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    10752 2024-03-25 18:09:11.000000 cs2solutions-0.6.5/src/cs2solutions/lqrfeedback.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)    13341 2024-03-25 18:09:11.000000 cs2solutions-0.6.5/src/cs2solutions/morse.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       90 2024-02-20 16:57:23.000000 cs2solutions-0.6.5/src/cs2solutions/plot.py
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       68 2024-02-20 16:57:23.000000 cs2solutions-0.6.5/src/cs2solutions/test.py
-drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-16 15:25:22.020220 cs2solutions-0.6.5/src/cs2solutions.egg-info/
--rw-r--r--   0 dejan     (1000) dejan     (1000)    42298 2024-04-16 15:25:22.000000 cs2solutions-0.6.5/src/cs2solutions.egg-info/PKG-INFO
--rw-rw-r--   0 dejan     (1000) dejan     (1000)      619 2024-04-16 15:25:22.000000 cs2solutions-0.6.5/src/cs2solutions.egg-info/SOURCES.txt
--rw-rw-r--   0 dejan     (1000) dejan     (1000)        1 2024-04-16 15:25:22.000000 cs2solutions-0.6.5/src/cs2solutions.egg-info/dependency_links.txt
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       37 2024-04-16 15:25:22.000000 cs2solutions-0.6.5/src/cs2solutions.egg-info/requires.txt
--rw-rw-r--   0 dejan     (1000) dejan     (1000)       13 2024-04-16 15:25:22.000000 cs2solutions-0.6.5/src/cs2solutions.egg-info/top_level.txt
+drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-22 07:53:50.444540 cs2solutions-0.7.0/
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    35149 2024-02-20 16:57:23.000000 cs2solutions-0.7.0/LICENSE
+-rw-r--r--   0 dejan     (1000) dejan     (1000)    42298 2024-04-22 07:53:50.444540 cs2solutions-0.7.0/PKG-INFO
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)      706 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/README.md
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)     1279 2024-04-22 07:50:49.000000 cs2solutions-0.7.0/pyproject.toml
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)       38 2024-04-22 07:53:50.444540 cs2solutions-0.7.0/setup.cfg
+drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-22 07:53:50.440540 cs2solutions-0.7.0/src/
+drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-22 07:53:50.444540 cs2solutions-0.7.0/src/cs2solutions/
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)      151 2024-04-22 07:50:49.000000 cs2solutions-0.7.0/src/cs2solutions/__init__.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)     6885 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/aircraft.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)        0 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/cs.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)     5975 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/cs2bot.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    10851 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/decomp.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    21154 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/discretization.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    10908 2024-04-16 07:25:19.000000 cs2solutions-0.7.0/src/cs2solutions/duckiebot.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)     7763 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/intro.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    15366 2024-04-16 15:23:07.000000 cs2solutions-0.7.0/src/cs2solutions/intromimo.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    13252 2024-04-16 07:25:19.000000 cs2solutions-0.7.0/src/cs2solutions/lqg.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    10752 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/lqrfeedback.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    13341 2024-03-25 18:09:11.000000 cs2solutions-0.7.0/src/cs2solutions/morse.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)    15555 2024-04-22 07:50:49.000000 cs2solutions-0.7.0/src/cs2solutions/norms.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)       90 2024-02-20 16:57:23.000000 cs2solutions-0.7.0/src/cs2solutions/plot.py
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)       68 2024-02-20 16:57:23.000000 cs2solutions-0.7.0/src/cs2solutions/test.py
+drwxrwxr-x   0 dejan     (1000) dejan     (1000)        0 2024-04-22 07:53:50.444540 cs2solutions-0.7.0/src/cs2solutions.egg-info/
+-rw-r--r--   0 dejan     (1000) dejan     (1000)    42298 2024-04-22 07:53:50.000000 cs2solutions-0.7.0/src/cs2solutions.egg-info/PKG-INFO
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)      645 2024-04-22 07:53:50.000000 cs2solutions-0.7.0/src/cs2solutions.egg-info/SOURCES.txt
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)        1 2024-04-22 07:53:50.000000 cs2solutions-0.7.0/src/cs2solutions.egg-info/dependency_links.txt
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)       37 2024-04-22 07:53:50.000000 cs2solutions-0.7.0/src/cs2solutions.egg-info/requires.txt
+-rw-rw-r--   0 dejan     (1000) dejan     (1000)       13 2024-04-22 07:53:50.000000 cs2solutions-0.7.0/src/cs2solutions.egg-info/top_level.txt
```

### Comparing `cs2solutions-0.6.5/LICENSE` & `cs2solutions-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/PKG-INFO` & `cs2solutions-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2solutions
-Version: 0.6.5
+Version: 0.7.0
 Summary: A package containing solutions for the CS2 lecture at ETH Zürich
 Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `cs2solutions-0.6.5/README.md` & `cs2solutions-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/pyproject.toml` & `cs2solutions-0.7.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/solutions"]
 
 [project]
 name = "cs2solutions"
-version = "0.6.5"
+version = "0.7.0"
 dependencies =[
     "control",
     "matplotlib",
     "numpy",
     "scipy",
     "sympy"
 ]
```

### Comparing `cs2solutions-0.6.5/src/cs2solutions/aircraft.py` & `cs2solutions-0.7.0/src/cs2solutions/aircraft.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/src/cs2solutions/cs2bot.py` & `cs2solutions-0.7.0/src/cs2solutions/cs2bot.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/src/cs2solutions/decomp.py` & `cs2solutions-0.7.0/src/cs2solutions/decomp.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/src/cs2solutions/discretization.py` & `cs2solutions-0.7.0/src/cs2solutions/discretization.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/src/cs2solutions/duckiebot.py` & `cs2solutions-0.7.0/src/cs2solutions/duckiebot.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/src/cs2solutions/intro.py` & `cs2solutions-0.7.0/src/cs2solutions/intro.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/src/cs2solutions/intromimo.py` & `cs2solutions-0.7.0/src/cs2solutions/intromimo.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/src/cs2solutions/lqg.py` & `cs2solutions-0.7.0/src/cs2solutions/lqg.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/src/cs2solutions/lqrfeedback.py` & `cs2solutions-0.7.0/src/cs2solutions/lqrfeedback.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/src/cs2solutions/morse.py` & `cs2solutions-0.7.0/src/cs2solutions/morse.py`

 * *Files identical despite different names*

### Comparing `cs2solutions-0.6.5/src/cs2solutions.egg-info/PKG-INFO` & `cs2solutions-0.7.0/src/cs2solutions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs2solutions
-Version: 0.6.5
+Version: 0.7.0
 Summary: A package containing solutions for the CS2 lecture at ETH Zürich
 Author-email: Kalle Laitinen <klaitinen@ethz.ch>, Dejan Milojevic <dejanmi@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 Maintainer-email: Kalle Laitinen <klaitinen@ethz.ch>, Niclas Scheuer <nscheuer@ethz.ch>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `cs2solutions-0.6.5/src/cs2solutions.egg-info/SOURCES.txt` & `cs2solutions-0.7.0/src/cs2solutions.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/cs2solutions/discretization.py
 src/cs2solutions/duckiebot.py
 src/cs2solutions/intro.py
 src/cs2solutions/intromimo.py
 src/cs2solutions/lqg.py
 src/cs2solutions/lqrfeedback.py
 src/cs2solutions/morse.py
+src/cs2solutions/norms.py
 src/cs2solutions/plot.py
 src/cs2solutions/test.py
 src/cs2solutions.egg-info/PKG-INFO
 src/cs2solutions.egg-info/SOURCES.txt
 src/cs2solutions.egg-info/dependency_links.txt
 src/cs2solutions.egg-info/requires.txt
 src/cs2solutions.egg-info/top_level.txt
```

