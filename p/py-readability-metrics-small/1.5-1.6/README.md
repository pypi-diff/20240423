# Comparing `tmp/py_readability_metrics_small-1.5.tar.gz` & `tmp/py_readability_metrics_small-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_readability_metrics_small-1.5.tar", last modified: Tue Apr 23 00:44:38 2024, max compression
+gzip compressed data, was "py_readability_metrics_small-1.6.tar", last modified: Tue Apr 23 00:48:14 2024, max compression
```

## Comparing `py_readability_metrics_small-1.5.tar` & `py_readability_metrics_small-1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.395785 py_readability_metrics_small-1.5/
--rw-r--r--   0 bengray    (501) staff       (20)     1096 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/LICENSE
--rw-r--r--   0 bengray    (501) staff       (20)     8855 2024-04-23 00:44:38.394865 py_readability_metrics_small-1.5/PKG-INFO
--rw-r--r--   0 bengray    (501) staff       (20)     8215 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/README.md
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.394253 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/
--rw-r--r--   0 bengray    (501) staff       (20)     8855 2024-04-23 00:44:37.000000 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/PKG-INFO
--rw-r--r--   0 bengray    (501) staff       (20)      915 2024-04-23 00:44:38.000000 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/SOURCES.txt
--rw-r--r--   0 bengray    (501) staff       (20)        1 2024-04-23 00:44:37.000000 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/dependency_links.txt
--rw-r--r--   0 bengray    (501) staff       (20)        5 2024-04-23 00:44:37.000000 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/requires.txt
--rw-r--r--   0 bengray    (501) staff       (20)       17 2024-04-23 00:44:37.000000 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/top_level.txt
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.374995 py_readability_metrics_small-1.5/readability/
--rw-r--r--   0 bengray    (501) staff       (20)      381 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/__init__.py
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.379411 py_readability_metrics_small-1.5/readability/data/
--rw-r--r--   0 bengray    (501) staff       (20)    17705 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/data/dale_chall_porterstem.txt
--rw-r--r--   0 bengray    (501) staff       (20)     5806 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/data/spache_easy_porterstem.txt
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.380553 py_readability_metrics_small-1.5/readability/exceptions/
--rw-r--r--   0 bengray    (501) staff       (20)       48 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/exceptions/__init__.py
--rw-r--r--   0 bengray    (501) staff       (20)     2506 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/readability.py
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.389138 py_readability_metrics_small-1.5/readability/scorers/
--rw-r--r--   0 bengray    (501) staff       (20)      289 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/scorers/__init__.py
--rw-r--r--   0 bengray    (501) staff       (20)     2569 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/ari.py
--rw-r--r--   0 bengray    (501) staff       (20)     1041 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/coleman_liau.py
--rw-r--r--   0 bengray    (501) staff       (20)     1617 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/dale_chall.py
--rw-r--r--   0 bengray    (501) staff       (20)     2042 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/flesch.py
--rw-r--r--   0 bengray    (501) staff       (20)      912 2024-04-19 14:45:52.000000 py_readability_metrics_small-1.5/readability/scorers/flesch_kincaid.py
--rw-r--r--   0 bengray    (501) staff       (20)     1233 2024-04-19 14:45:52.000000 py_readability_metrics_small-1.5/readability/scorers/gunning_fog.py
--rw-r--r--   0 bengray    (501) staff       (20)     1089 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/linsear_write.py
--rw-r--r--   0 bengray    (501) staff       (20)     2431 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/scorers/smog.py
--rw-r--r--   0 bengray    (501) staff       (20)     1030 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/spache.py
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.391963 py_readability_metrics_small-1.5/readability/text/
--rw-r--r--   0 bengray    (501) staff       (20)       31 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/text/__init__.py
--rw-r--r--   0 bengray    (501) staff       (20)     4918 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/text/analyzer.py
--rw-r--r--   0 bengray    (501) staff       (20)      375 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/text/syllables.py
--rw-r--r--   0 bengray    (501) staff       (20)       38 2024-04-23 00:44:38.395996 py_readability_metrics_small-1.5/setup.cfg
--rw-r--r--   0 bengray    (501) staff       (20)     1077 2024-04-23 00:44:27.000000 py_readability_metrics_small-1.5/setup.py
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.393091 py_readability_metrics_small-1.5/test/
--rw-r--r--   0 bengray    (501) staff       (20)        0 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/test/__init__.py
--rw-r--r--   0 bengray    (501) staff       (20)     4135 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/test/test_readability.py
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:48:14.876668 py_readability_metrics_small-1.6/
+-rw-r--r--   0 bengray    (501) staff       (20)     1096 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/LICENSE
+-rw-r--r--   0 bengray    (501) staff       (20)     8855 2024-04-23 00:48:14.875918 py_readability_metrics_small-1.6/PKG-INFO
+-rw-r--r--   0 bengray    (501) staff       (20)     8215 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/README.md
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:48:14.874999 py_readability_metrics_small-1.6/py_readability_metrics_small.egg-info/
+-rw-r--r--   0 bengray    (501) staff       (20)     8855 2024-04-23 00:48:14.000000 py_readability_metrics_small-1.6/py_readability_metrics_small.egg-info/PKG-INFO
+-rw-r--r--   0 bengray    (501) staff       (20)      915 2024-04-23 00:48:14.000000 py_readability_metrics_small-1.6/py_readability_metrics_small.egg-info/SOURCES.txt
+-rw-r--r--   0 bengray    (501) staff       (20)        1 2024-04-23 00:48:14.000000 py_readability_metrics_small-1.6/py_readability_metrics_small.egg-info/dependency_links.txt
+-rw-r--r--   0 bengray    (501) staff       (20)        5 2024-04-23 00:48:14.000000 py_readability_metrics_small-1.6/py_readability_metrics_small.egg-info/requires.txt
+-rw-r--r--   0 bengray    (501) staff       (20)       17 2024-04-23 00:48:14.000000 py_readability_metrics_small-1.6/py_readability_metrics_small.egg-info/top_level.txt
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:48:14.857665 py_readability_metrics_small-1.6/readability/
+-rw-r--r--   0 bengray    (501) staff       (20)      381 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/readability/__init__.py
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:48:14.860942 py_readability_metrics_small-1.6/readability/data/
+-rw-r--r--   0 bengray    (501) staff       (20)    17705 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/readability/data/dale_chall_porterstem.txt
+-rw-r--r--   0 bengray    (501) staff       (20)     5806 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/readability/data/spache_easy_porterstem.txt
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:48:14.861717 py_readability_metrics_small-1.6/readability/exceptions/
+-rw-r--r--   0 bengray    (501) staff       (20)       48 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/readability/exceptions/__init__.py
+-rw-r--r--   0 bengray    (501) staff       (20)     2506 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.6/readability/readability.py
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:48:14.869453 py_readability_metrics_small-1.6/readability/scorers/
+-rw-r--r--   0 bengray    (501) staff       (20)      289 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/readability/scorers/__init__.py
+-rw-r--r--   0 bengray    (501) staff       (20)     2569 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.6/readability/scorers/ari.py
+-rw-r--r--   0 bengray    (501) staff       (20)     1041 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.6/readability/scorers/coleman_liau.py
+-rw-r--r--   0 bengray    (501) staff       (20)     1617 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.6/readability/scorers/dale_chall.py
+-rw-r--r--   0 bengray    (501) staff       (20)     2042 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.6/readability/scorers/flesch.py
+-rw-r--r--   0 bengray    (501) staff       (20)      916 2024-04-23 00:47:38.000000 py_readability_metrics_small-1.6/readability/scorers/flesch_kincaid.py
+-rw-r--r--   0 bengray    (501) staff       (20)     1233 2024-04-19 14:45:52.000000 py_readability_metrics_small-1.6/readability/scorers/gunning_fog.py
+-rw-r--r--   0 bengray    (501) staff       (20)     1089 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.6/readability/scorers/linsear_write.py
+-rw-r--r--   0 bengray    (501) staff       (20)     2431 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/readability/scorers/smog.py
+-rw-r--r--   0 bengray    (501) staff       (20)     1030 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.6/readability/scorers/spache.py
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:48:14.872033 py_readability_metrics_small-1.6/readability/text/
+-rw-r--r--   0 bengray    (501) staff       (20)       31 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/readability/text/__init__.py
+-rw-r--r--   0 bengray    (501) staff       (20)     4918 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/readability/text/analyzer.py
+-rw-r--r--   0 bengray    (501) staff       (20)      375 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/readability/text/syllables.py
+-rw-r--r--   0 bengray    (501) staff       (20)       38 2024-04-23 00:48:14.876793 py_readability_metrics_small-1.6/setup.cfg
+-rw-r--r--   0 bengray    (501) staff       (20)     1077 2024-04-23 00:47:58.000000 py_readability_metrics_small-1.6/setup.py
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:48:14.873596 py_readability_metrics_small-1.6/test/
+-rw-r--r--   0 bengray    (501) staff       (20)        0 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/test/__init__.py
+-rw-r--r--   0 bengray    (501) staff       (20)     4135 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.6/test/test_readability.py
```

### Comparing `py_readability_metrics_small-1.5/LICENSE` & `py_readability_metrics_small-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/PKG-INFO` & `py_readability_metrics_small-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-readability-metrics-small
-Version: 1.5
+Version: 1.6
 Summary: Score text "Readability" with popular formulas and metrics including Flesch-Kincaid, Gunning Fog, ARI, Dale Chall, SMOG, Spache and more
 Home-page: https://github.com/ben-gray-dev/py-readability-metrics-small
 Author: Ben Gray
 Author-email: bgray27613@gmail.com
 License: MIT
 Keywords: readability metrics text difficulty grade level
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py_readability_metrics_small-1.5/README.md` & `py_readability_metrics_small-1.6/README.md`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/PKG-INFO` & `py_readability_metrics_small-1.6/py_readability_metrics_small.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-readability-metrics-small
-Version: 1.5
+Version: 1.6
 Summary: Score text "Readability" with popular formulas and metrics including Flesch-Kincaid, Gunning Fog, ARI, Dale Chall, SMOG, Spache and more
 Home-page: https://github.com/ben-gray-dev/py-readability-metrics-small
 Author: Ben Gray
 Author-email: bgray27613@gmail.com
 License: MIT
 Keywords: readability metrics text difficulty grade level
 Classifier: Programming Language :: Python :: 3
```

### Comparing `py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/SOURCES.txt` & `py_readability_metrics_small-1.6/py_readability_metrics_small.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/data/dale_chall_porterstem.txt` & `py_readability_metrics_small-1.6/readability/data/dale_chall_porterstem.txt`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/data/spache_easy_porterstem.txt` & `py_readability_metrics_small-1.6/readability/data/spache_easy_porterstem.txt`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/readability.py` & `py_readability_metrics_small-1.6/readability/readability.py`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/scorers/ari.py` & `py_readability_metrics_small-1.6/readability/scorers/ari.py`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/scorers/coleman_liau.py` & `py_readability_metrics_small-1.6/readability/scorers/coleman_liau.py`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/scorers/dale_chall.py` & `py_readability_metrics_small-1.6/readability/scorers/dale_chall.py`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/scorers/flesch.py` & `py_readability_metrics_small-1.6/readability/scorers/flesch.py`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/scorers/flesch_kincaid.py` & `py_readability_metrics_small-1.6/readability/scorers/flesch_kincaid.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         return "score: {}, grade_level: '{}'". \
             format(self.score, self.grade_level)
 
 
 class FleschKincaid:
     def __init__(self, stats, min_words=0):
         self._stats = stats
-        if stats.num_words < min_words:
-            raise ReadabilityException('{} words required.'.format(min_words))
+        # if stats.num_words < min_words:
+        #     raise ReadabilityException('{} words required.'.format(min_words))
 
     def score(self):
         score = self._score()
         return Result(
             score=score,
             grade_level=self._grade_level(score)
         )
```

### Comparing `py_readability_metrics_small-1.5/readability/scorers/gunning_fog.py` & `py_readability_metrics_small-1.6/readability/scorers/gunning_fog.py`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/scorers/linsear_write.py` & `py_readability_metrics_small-1.6/readability/scorers/linsear_write.py`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/scorers/smog.py` & `py_readability_metrics_small-1.6/readability/scorers/smog.py`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/scorers/spache.py` & `py_readability_metrics_small-1.6/readability/scorers/spache.py`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/readability/text/analyzer.py` & `py_readability_metrics_small-1.6/readability/text/analyzer.py`

 * *Files identical despite different names*

### Comparing `py_readability_metrics_small-1.5/setup.py` & `py_readability_metrics_small-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='py-readability-metrics-small',
-    version='1.5',
+    version='1.6',
     author='Ben Gray',
     author_email='bgray27613@gmail.com',
     description='Score text "Readability" with popular formulas and metrics including Flesch-Kincaid, Gunning Fog, ARI, Dale Chall, SMOG, Spache and more',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ben-gray-dev/py-readability-metrics-small',
     keywords="readability metrics text difficulty grade level",
```

### Comparing `py_readability_metrics_small-1.5/test/test_readability.py` & `py_readability_metrics_small-1.6/test/test_readability.py`

 * *Files identical despite different names*

