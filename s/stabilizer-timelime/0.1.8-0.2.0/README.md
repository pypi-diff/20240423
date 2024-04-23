# Comparing `tmp/stabilizer_timelime-0.1.8.tar.gz` & `tmp/stabilizer_timelime-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stabilizer_timelime-0.1.8.tar", max compression
+gzip compressed data, was "stabilizer_timelime-0.2.0.tar", max compression
```

## Comparing `stabilizer_timelime-0.1.8.tar` & `stabilizer_timelime-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,37 @@
--rw-r--r--   0        0        0     1492 2024-04-16 18:48:45.808071 stabilizer_timelime-0.1.8/LICENSE
--rw-r--r--   0        0        0      776 2024-04-16 20:19:56.407964 stabilizer_timelime-0.1.8/README.md
--rw-r--r--   0        0        0      774 2024-04-21 16:22:30.299292 stabilizer_timelime-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.1.8/stabilizer_timelime/src/__init__.py
--rw-r--r--   0        0        0       24 2024-04-15 19:42:45.228609 stabilizer_timelime-0.1.8/stabilizer_timelime/src/dataslurper/__init__.py
--rw-r--r--   0        0        0     4801 2024-04-19 18:20:35.183976 stabilizer_timelime-0.1.8/stabilizer_timelime/src/dataslurper/prudenceChecker.py
--rw-r--r--   0        0        0     8171 2024-04-19 18:20:58.398569 stabilizer_timelime-0.1.8/stabilizer_timelime/src/dataslurper/slurpdata.py
--rw-r--r--   0        0        0      517 2024-04-21 16:22:21.965311 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-15 19:46:28.151618 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/config.py
--rw-r--r--   0        0        0     6148 2024-04-21 14:52:45.759246 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/.DS_Store
--rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/CFS.py
--rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
--rw-r--r--   0        0        0     7270 2024-04-15 19:28:57.554189 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/DE.py
--rw-r--r--   0        0        0     9862 2024-04-15 19:29:45.282751 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
--rw-r--r--   0        0        0    10716 2024-04-15 23:28:50.247476 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
--rw-r--r--   0        0        0     2531 2024-04-15 19:35:14.983457 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/Stats_files.py
--rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/__init__.py
--rw-r--r--   0        0        0     3128 2024-04-15 20:03:02.460402 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
--rwxr-xr-x   0        0        0     8784 2024-04-15 22:32:53.920281 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/birch.py
--rw-r--r--   0        0        0    11445 2024-04-15 22:40:20.361407 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
--rw-r--r--   0        0        0     4221 2024-04-15 19:28:50.926587 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
--rw-r--r--   0        0        0     9306 2024-04-15 23:03:18.017939 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
--rw-r--r--   0        0        0     2361 2024-04-21 16:20:19.485703 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/generate_results.py
--rw-r--r--   0        0        0     4149 2024-04-19 19:52:55.063561 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
--rw-r--r--   0        0        0     8124 2024-04-15 19:30:24.992210 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/learners.py
--rw-r--r--   0        0        0     5317 2024-04-15 19:34:25.519136 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/optimizer.py
--rw-r--r--   0        0        0    13670 2024-04-15 19:39:18.188946 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
--rw-r--r--   0        0        0     5568 2024-04-15 19:32:22.898327 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py
--rw-r--r--   0        0        0    36371 2024-04-21 15:55:43.694010 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/scott_knott.py
--rw-r--r--   0        0        0     7377 2024-04-15 21:47:14.987970 stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/utils.py
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 stabilizer_timelime-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1492 2024-04-16 18:48:45.808071 stabilizer_timelime-0.2.0/LICENSE
+-rw-r--r--   0        0        0      776 2024-04-16 20:19:56.407964 stabilizer_timelime-0.2.0/README.md
+-rw-r--r--   0        0        0      774 2024-04-23 16:23:01.427188 stabilizer_timelime-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 00:03:23.296661 stabilizer_timelime-0.2.0/stabilizer_timelime/src/__init__.py
+-rw-r--r--   0        0        0       24 2024-04-15 19:42:45.228609 stabilizer_timelime-0.2.0/stabilizer_timelime/src/dataslurper/__init__.py
+-rw-r--r--   0        0        0     4801 2024-04-19 18:20:35.183976 stabilizer_timelime-0.2.0/stabilizer_timelime/src/dataslurper/prudenceChecker.py
+-rw-r--r--   0        0        0     8171 2024-04-19 18:20:58.398569 stabilizer_timelime-0.2.0/stabilizer_timelime/src/dataslurper/slurpdata.py
+-rw-r--r--   0        0        0      517 2024-04-21 16:22:21.965311 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-15 19:46:28.151618 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/config.py
+-rw-r--r--   0        0        0     6148 2024-04-21 14:52:45.759246 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/.DS_Store
+-rwxr-xr-x   0        0        0    10689 2024-04-14 16:32:20.312051 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/CFS.py
+-rwxr-xr-x   0        0        0    11922 2024-04-14 16:32:21.643298 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/CFS_regression.py
+-rw-r--r--   0        0        0     7270 2024-04-15 19:28:57.554189 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/DE.py
+-rw-r--r--   0        0        0     9862 2024-04-15 19:29:45.282751 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py
+-rw-r--r--   0        0        0    10716 2024-04-15 23:28:50.247476 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py
+-rw-r--r--   0        0        0     2531 2024-04-15 19:35:14.983457 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Stats_files.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:32:19.433820 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/__init__.py
+-rw-r--r--   0        0        0     3128 2024-04-15 20:03:02.460402 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/attribute_selector.py
+-rwxr-xr-x   0        0        0     8784 2024-04-15 22:32:53.920281 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/birch.py
+-rw-r--r--   0        0        0    11445 2024-04-15 22:40:20.361407 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py
+-rw-r--r--   0        0        0     4221 2024-04-15 19:28:50.926587 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py
+-rw-r--r--   0        0        0     9306 2024-04-15 23:03:18.017939 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/default_bellwether.py
+-rw-r--r--   0        0        0     2408 2024-04-23 16:19:09.557286 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/generate_results.py
+-rw-r--r--   0        0        0     4149 2024-04-19 19:52:55.063561 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/init_datafiles.py
+-rw-r--r--   0        0        0     8124 2024-04-15 19:30:24.992210 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/learners.py
+-rw-r--r--   0        0        0     5317 2024-04-15 19:34:25.519136 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/optimizer.py
+-rw-r--r--   0        0        0    13670 2024-04-15 19:39:18.188946 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py
+-rw-r--r--   0        0        0     5568 2024-04-15 19:32:22.898327 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py
+-rw-r--r--   0        0        0     9951 2024-04-23 16:20:41.196495 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/scott_knott.py
+-rw-r--r--   0        0        0     7377 2024-04-15 21:47:14.987970 stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/utils.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:22:21.372525 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 16:22:21.372785 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/__init__.py
+-rw-r--r--   0        0        0    11030 2024-04-23 16:22:21.373200 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/othertools.py
+-rw-r--r--   0        0        0    10035 2024-04-23 16:22:21.373488 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/planner.py
+-rw-r--r--   0        0        0     2012 2024-04-23 16:22:21.373671 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/runexp.py
+-rw-r--r--   0        0        0     1891 2024-04-23 16:22:21.373856 stabilizer_timelime-0.2.0/stabilizer_timelime/src/timeLIME/src/split_dataset.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 stabilizer_timelime-0.2.0/PKG-INFO
```

### Comparing `stabilizer_timelime-0.1.8/LICENSE` & `stabilizer_timelime-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/README.md` & `stabilizer_timelime-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/pyproject.toml` & `stabilizer_timelime-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "stabilizer_timelime"
-version = "0.1.8"
+version = "0.2.0"
 authors = ["Sukhad Joshi <sjoshi32@ncsu.edu>"]
 description = "Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/dataslurper/prudenceChecker.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/dataslurper/prudenceChecker.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/dataslurper/slurpdata.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/dataslurper/slurpdata.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/__init__.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/__init__.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/config.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/config.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/.DS_Store` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/CFS.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/CFS.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/CFS_regression.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/CFS_regression.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/DE.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/DE.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Find_bellwethers.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Performance_Calculator.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/Stats_files.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/Stats_files.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/attribute_selector.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/attribute_selector.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/birch.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/birch.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/birch_bellwether_p_CFS.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/collect_bellwethers.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/default_bellwether.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/default_bellwether.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/generate_results.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/generate_results.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
+# from .scott_knott import run
 from .scott_knott import run
-
 import csv
 
 
 def generate_combined_files(seeds: list):
     source_folder = "results/with_CFS_DE/{}/Stats_new/"
     destination_folder = "results/with_CFS_DE/Stats_new/"
 
@@ -40,35 +40,28 @@
 
         with open(os.path.join(folder_path, "combined_" + filename), 'w') as f:
             for item, values in merged_items.items():
                 f.write(item + "\n")
                 f.write(" ".join(values) + "\n\n")
 
 
-def run_scott_knot(goals: list):
-    latex = False
-
-
 def generate_results(seeds: list, goals: list):
     # Merge files together
     generate_combined_files(seeds)
 
     metrics = ["sa", "mre"]
 
     for goal in goals:
         for metric in metrics:
-            filepath = "results/with_CFS_DE/Stats_new/combined_monthly_{0}_{1}.txt".format(goal, metric)
+            filepath = "results/with_CFS_DE/Stats_new/combined_{0}_{1}.txt".format(goal, metric)
 
             if not os.path.isfile(filepath):
                 print(filepath, " is not a valid path/ does not exist")
                 continue
             
+            run(filename=filepath)
             res = run(filename=filepath)
 
-            with open("{0}_{1}.csv".format(goal, metric), "r") as f:
+            with open("{0}_{1}.csv".format(goal, metric), "w") as f:
                 writer = csv.writer(f)
-                writer.writerow(["rank", "treatment", "Median", "IQR"])
-                writer.writerows(res)
-
-
-    
-    
+                writer.writerow(["rank", "treatment", "Median", "IQR", "10th Perc.", "25th Perc.", "75th Perc.", "90th Perc."])
+                writer.writerows(res)
```

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/init_datafiles.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/init_datafiles.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/learners.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/learners.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/optimizer.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/optimizer.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/predictor_advance_v1.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/predictor_baseline.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/stabilizer_timelime/src/stabilizer/src/utils.py` & `stabilizer_timelime-0.2.0/stabilizer_timelime/src/stabilizer/src/utils.py`

 * *Files identical despite different names*

### Comparing `stabilizer_timelime-0.1.8/PKG-INFO` & `stabilizer_timelime-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stabilizer_timelime
-Version: 0.1.8
+Version: 0.2.0
 Summary: Packaged project that contains code to scrape GitHub data, build and run stabilizer and timeline
 Author: Sukhad Joshi
 Author-email: sjoshi32@ncsu.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

