# Comparing `tmp/py-readability-metrics-small-1.4.4.tar.gz` & `tmp/py_readability_metrics_small-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-readability-metrics-small-1.4.4.tar", last modified: Fri Apr 19 19:03:48 2024, max compression
+gzip compressed data, was "py_readability_metrics_small-1.5.tar", last modified: Tue Apr 23 00:44:38 2024, max compression
```

## Comparing `py-readability-metrics-small-1.4.4.tar` & `py_readability_metrics_small-1.5.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-19 19:03:48.047119 py-readability-metrics-small-1.4.4/
--rw-r--r--   0 bengray    (501) staff       (20)    11038 2024-04-19 19:03:48.046573 py-readability-metrics-small-1.4.4/PKG-INFO
--rw-r--r--   0 bengray    (501) staff       (20)     8215 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/README.md
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-19 19:03:48.035961 py-readability-metrics-small-1.4.4/py_readability_metrics_small.egg-info/
--rw-r--r--   0 bengray    (501) staff       (20)    11038 2024-04-19 19:03:47.000000 py-readability-metrics-small-1.4.4/py_readability_metrics_small.egg-info/PKG-INFO
--rw-r--r--   0 bengray    (501) staff       (20)      820 2024-04-19 19:03:47.000000 py-readability-metrics-small-1.4.4/py_readability_metrics_small.egg-info/SOURCES.txt
--rw-r--r--   0 bengray    (501) staff       (20)        1 2024-04-19 19:03:47.000000 py-readability-metrics-small-1.4.4/py_readability_metrics_small.egg-info/dependency_links.txt
--rw-r--r--   0 bengray    (501) staff       (20)        5 2024-04-19 19:03:47.000000 py-readability-metrics-small-1.4.4/py_readability_metrics_small.egg-info/requires.txt
--rw-r--r--   0 bengray    (501) staff       (20)       17 2024-04-19 19:03:47.000000 py-readability-metrics-small-1.4.4/py_readability_metrics_small.egg-info/top_level.txt
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-19 19:03:48.036800 py-readability-metrics-small-1.4.4/readability/
--rw-r--r--   0 bengray    (501) staff       (20)      381 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/__init__.py
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-19 19:03:48.037457 py-readability-metrics-small-1.4.4/readability/exceptions/
--rw-r--r--   0 bengray    (501) staff       (20)       48 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/exceptions/__init__.py
--rw-r--r--   0 bengray    (501) staff       (20)     2508 2024-04-19 14:45:52.000000 py-readability-metrics-small-1.4.4/readability/readability.py
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-19 19:03:48.042148 py-readability-metrics-small-1.4.4/readability/scorers/
--rw-r--r--   0 bengray    (501) staff       (20)      289 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/scorers/__init__.py
--rw-r--r--   0 bengray    (501) staff       (20)     2571 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/scorers/ari.py
--rw-r--r--   0 bengray    (501) staff       (20)     1043 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/scorers/coleman_liau.py
--rw-r--r--   0 bengray    (501) staff       (20)     1619 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/scorers/dale_chall.py
--rw-r--r--   0 bengray    (501) staff       (20)     2044 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/scorers/flesch.py
--rw-r--r--   0 bengray    (501) staff       (20)      912 2024-04-19 14:45:52.000000 py-readability-metrics-small-1.4.4/readability/scorers/flesch_kincaid.py
--rw-r--r--   0 bengray    (501) staff       (20)     1233 2024-04-19 14:45:52.000000 py-readability-metrics-small-1.4.4/readability/scorers/gunning_fog.py
--rw-r--r--   0 bengray    (501) staff       (20)     1091 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/scorers/linsear_write.py
--rw-r--r--   0 bengray    (501) staff       (20)     2431 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/scorers/smog.py
--rw-r--r--   0 bengray    (501) staff       (20)     1032 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/scorers/spache.py
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-19 19:03:48.044107 py-readability-metrics-small-1.4.4/readability/text/
--rw-r--r--   0 bengray    (501) staff       (20)       31 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/text/__init__.py
--rw-r--r--   0 bengray    (501) staff       (20)     4918 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/text/analyzer.py
--rw-r--r--   0 bengray    (501) staff       (20)      375 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/readability/text/syllables.py
--rw-r--r--   0 bengray    (501) staff       (20)       38 2024-04-19 19:03:48.047393 py-readability-metrics-small-1.4.4/setup.cfg
--rw-r--r--   0 bengray    (501) staff       (20)     1079 2024-04-19 19:03:25.000000 py-readability-metrics-small-1.4.4/setup.py
-drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-19 19:03:48.045220 py-readability-metrics-small-1.4.4/test/
--rw-r--r--   0 bengray    (501) staff       (20)        0 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/test/__init__.py
--rw-r--r--   0 bengray    (501) staff       (20)     4135 2024-04-19 14:44:44.000000 py-readability-metrics-small-1.4.4/test/test_readability.py
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.395785 py_readability_metrics_small-1.5/
+-rw-r--r--   0 bengray    (501) staff       (20)     1096 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/LICENSE
+-rw-r--r--   0 bengray    (501) staff       (20)     8855 2024-04-23 00:44:38.394865 py_readability_metrics_small-1.5/PKG-INFO
+-rw-r--r--   0 bengray    (501) staff       (20)     8215 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/README.md
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.394253 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/
+-rw-r--r--   0 bengray    (501) staff       (20)     8855 2024-04-23 00:44:37.000000 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/PKG-INFO
+-rw-r--r--   0 bengray    (501) staff       (20)      915 2024-04-23 00:44:38.000000 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/SOURCES.txt
+-rw-r--r--   0 bengray    (501) staff       (20)        1 2024-04-23 00:44:37.000000 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/dependency_links.txt
+-rw-r--r--   0 bengray    (501) staff       (20)        5 2024-04-23 00:44:37.000000 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/requires.txt
+-rw-r--r--   0 bengray    (501) staff       (20)       17 2024-04-23 00:44:37.000000 py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/top_level.txt
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.374995 py_readability_metrics_small-1.5/readability/
+-rw-r--r--   0 bengray    (501) staff       (20)      381 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/__init__.py
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.379411 py_readability_metrics_small-1.5/readability/data/
+-rw-r--r--   0 bengray    (501) staff       (20)    17705 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/data/dale_chall_porterstem.txt
+-rw-r--r--   0 bengray    (501) staff       (20)     5806 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/data/spache_easy_porterstem.txt
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.380553 py_readability_metrics_small-1.5/readability/exceptions/
+-rw-r--r--   0 bengray    (501) staff       (20)       48 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/exceptions/__init__.py
+-rw-r--r--   0 bengray    (501) staff       (20)     2506 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/readability.py
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.389138 py_readability_metrics_small-1.5/readability/scorers/
+-rw-r--r--   0 bengray    (501) staff       (20)      289 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/scorers/__init__.py
+-rw-r--r--   0 bengray    (501) staff       (20)     2569 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/ari.py
+-rw-r--r--   0 bengray    (501) staff       (20)     1041 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/coleman_liau.py
+-rw-r--r--   0 bengray    (501) staff       (20)     1617 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/dale_chall.py
+-rw-r--r--   0 bengray    (501) staff       (20)     2042 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/flesch.py
+-rw-r--r--   0 bengray    (501) staff       (20)      912 2024-04-19 14:45:52.000000 py_readability_metrics_small-1.5/readability/scorers/flesch_kincaid.py
+-rw-r--r--   0 bengray    (501) staff       (20)     1233 2024-04-19 14:45:52.000000 py_readability_metrics_small-1.5/readability/scorers/gunning_fog.py
+-rw-r--r--   0 bengray    (501) staff       (20)     1089 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/linsear_write.py
+-rw-r--r--   0 bengray    (501) staff       (20)     2431 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/scorers/smog.py
+-rw-r--r--   0 bengray    (501) staff       (20)     1030 2024-04-19 19:08:32.000000 py_readability_metrics_small-1.5/readability/scorers/spache.py
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.391963 py_readability_metrics_small-1.5/readability/text/
+-rw-r--r--   0 bengray    (501) staff       (20)       31 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/text/__init__.py
+-rw-r--r--   0 bengray    (501) staff       (20)     4918 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/text/analyzer.py
+-rw-r--r--   0 bengray    (501) staff       (20)      375 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/readability/text/syllables.py
+-rw-r--r--   0 bengray    (501) staff       (20)       38 2024-04-23 00:44:38.395996 py_readability_metrics_small-1.5/setup.cfg
+-rw-r--r--   0 bengray    (501) staff       (20)     1077 2024-04-23 00:44:27.000000 py_readability_metrics_small-1.5/setup.py
+drwxr-xr-x   0 bengray    (501) staff       (20)        0 2024-04-23 00:44:38.393091 py_readability_metrics_small-1.5/test/
+-rw-r--r--   0 bengray    (501) staff       (20)        0 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/test/__init__.py
+-rw-r--r--   0 bengray    (501) staff       (20)     4135 2024-04-19 14:44:44.000000 py_readability_metrics_small-1.5/test/test_readability.py
```

### Comparing `py-readability-metrics-small-1.4.4/README.md` & `py_readability_metrics_small-1.5/README.md`

 * *Files identical despite different names*

### Comparing `py-readability-metrics-small-1.4.4/py_readability_metrics_small.egg-info/SOURCES.txt` & `py_readability_metrics_small-1.5/py_readability_metrics_small.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+LICENSE
 README.md
 setup.py
 py_readability_metrics_small.egg-info/PKG-INFO
 py_readability_metrics_small.egg-info/SOURCES.txt
 py_readability_metrics_small.egg-info/dependency_links.txt
 py_readability_metrics_small.egg-info/requires.txt
 py_readability_metrics_small.egg-info/top_level.txt
 readability/__init__.py
 readability/readability.py
+readability/data/dale_chall_porterstem.txt
+readability/data/spache_easy_porterstem.txt
 readability/exceptions/__init__.py
 readability/scorers/__init__.py
 readability/scorers/ari.py
 readability/scorers/coleman_liau.py
 readability/scorers/dale_chall.py
 readability/scorers/flesch.py
 readability/scorers/flesch_kincaid.py
```

### Comparing `py-readability-metrics-small-1.4.4/readability/readability.py` & `py_readability_metrics_small-1.5/readability/readability.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .text import Analyzer
 from .scorers import ARI, ColemanLiau, DaleChall, Flesch, \
     FleschKincaid, GunningFog, LinsearWrite, Smog, Spache
 import warnings
 
 class Readability:
-    def __init__(self, text, min_words=100):
+    def __init__(self, text, min_words=0):
         self._analyzer = Analyzer()
         self._statistics = self._analyzer.analyze(text)
         self._min_words = min_words
         # if self._min_words < 100:
         #     warnings.warn(
         #         "Documents with fewer than 100 words may affect the accuracy of readability tests"
         #     )
```

### Comparing `py-readability-metrics-small-1.4.4/readability/scorers/ari.py` & `py_readability_metrics_small-1.5/readability/scorers/ari.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def __str__(self):
         return "score: {}, grade_levels: {}, ages: {}". \
             format(self.score, self.grade_levels, self.ages)
 
 
 class ARI:
-    def __init__(self, stats, min_words=100):
+    def __init__(self, stats, min_words=0):
         self._stats = stats
         if stats.num_words < min_words:
             raise ReadabilityException('{} words required.'.format(min_words))
 
     def score(self):
         score = self._score()
         return Result(
```

### Comparing `py-readability-metrics-small-1.4.4/readability/scorers/coleman_liau.py` & `py_readability_metrics_small-1.5/readability/scorers/coleman_liau.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     def __str__(self):
         return "score: {}, grade_level: '{}'". \
             format(self.score, self.grade_level)
 
 
 class ColemanLiau:
-    def __init__(self, stats, min_words=100):
+    def __init__(self, stats, min_words=0):
         self._stats = stats
         if stats.num_words < min_words:
             raise ReadabilityException('{} words required.'.format(min_words))
 
     def score(self):
         score = self._score()
         return Result(
```

### Comparing `py-readability-metrics-small-1.4.4/readability/scorers/dale_chall.py` & `py_readability_metrics_small-1.5/readability/scorers/dale_chall.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     def __str__(self):
         return "score: {}, grade_levels: {}". \
             format(self.score, self.grade_levels)
 
 
 class DaleChall:
-    def __init__(self, stats, min_words=100):
+    def __init__(self, stats, min_words=0):
         self._stats = stats
         if stats.num_words < min_words:
             raise ReadabilityException('{} words required.'.format(min_words))
 
     def score(self):
         score = self._score()
         return Result(
```

### Comparing `py-readability-metrics-small-1.4.4/readability/scorers/flesch.py` & `py_readability_metrics_small-1.5/readability/scorers/flesch.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     def __str__(self):
         return "score: {}, ease: '{}', grade_levels: {}". \
             format(self.score, self.ease, self.grade_levels)
 
 
 class Flesch:
-    def __init__(self, stats, min_words=100):
+    def __init__(self, stats, min_words=0):
         self._stats = stats
         if stats.num_words < min_words:
             raise ReadabilityException('{} words required.'.format(min_words))
 
     def score(self):
         score = self._score()
         return Result(
```

### Comparing `py-readability-metrics-small-1.4.4/readability/scorers/flesch_kincaid.py` & `py_readability_metrics_small-1.5/readability/scorers/flesch_kincaid.py`

 * *Files identical despite different names*

### Comparing `py-readability-metrics-small-1.4.4/readability/scorers/gunning_fog.py` & `py_readability_metrics_small-1.5/readability/scorers/gunning_fog.py`

 * *Files identical despite different names*

### Comparing `py-readability-metrics-small-1.4.4/readability/scorers/linsear_write.py` & `py_readability_metrics_small-1.5/readability/scorers/linsear_write.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     def __str__(self):
         return "score: {}, grade_level: '{}'". \
             format(self.score, self.grade_level)
 
 
 class LinsearWrite:
-    def __init__(self, stats, min_words=100):
+    def __init__(self, stats, min_words=0):
         self._stats = stats
         if stats.num_words < min_words:
             raise ReadabilityException('{} words required.'.format(min_words))
 
     def score(self):
         score = self._score()
         return Result(
```

### Comparing `py-readability-metrics-small-1.4.4/readability/scorers/smog.py` & `py_readability_metrics_small-1.5/readability/scorers/smog.py`

 * *Files identical despite different names*

### Comparing `py-readability-metrics-small-1.4.4/readability/scorers/spache.py` & `py_readability_metrics_small-1.5/readability/scorers/spache.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
     def __str__(self):
         return "score: {}, grade_level: '{}'". \
             format(self.score, self.grade_level)
 
 
 class Spache:
-    def __init__(self, stats, min_words=100):
+    def __init__(self, stats, min_words=0):
         self._stats = stats
         if stats.num_words < min_words:
             raise ReadabilityException('{} words required.'.format(min_words))
 
     def score(self):
         score = self._score()
         return Result(
```

### Comparing `py-readability-metrics-small-1.4.4/readability/text/analyzer.py` & `py_readability_metrics_small-1.5/readability/text/analyzer.py`

 * *Files identical despite different names*

### Comparing `py-readability-metrics-small-1.4.4/setup.py` & `py_readability_metrics_small-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='py-readability-metrics-small',
-    version='1.4.4',
+    version='1.5',
     author='Ben Gray',
     author_email='bgray27613@gmail.com',
     description='Score text "Readability" with popular formulas and metrics including Flesch-Kincaid, Gunning Fog, ARI, Dale Chall, SMOG, Spache and more',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ben-gray-dev/py-readability-metrics-small',
     keywords="readability metrics text difficulty grade level",
```

### Comparing `py-readability-metrics-small-1.4.4/test/test_readability.py` & `py_readability_metrics_small-1.5/test/test_readability.py`

 * *Files identical despite different names*

