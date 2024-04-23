# Comparing `tmp/nest-sw-0.1.2.tar.gz` & `tmp/nest-sw-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nest-sw-0.1.2.tar", last modified: Tue Mar  5 14:59:04 2024, max compression
+gzip compressed data, was "nest-sw-0.1.3.tar", last modified: Tue Apr 23 20:18:13 2024, max compression
```

## Comparing `nest-sw-0.1.2.tar` & `nest-sw-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 binli      (501) staff       (20)        0 2024-03-05 14:59:04.599981 nest-sw-0.1.2/
-drwxr-xr-x   0 binli      (501) staff       (20)        0 2024-03-05 14:59:04.598587 nest-sw-0.1.2/NEST/
--rw-r--r--   0 binli      (501) staff       (20)       42 2024-03-05 04:13:57.000000 nest-sw-0.1.2/NEST/__init__.py
--rw-rw-r--   0 binli      (501) staff       (20)     1969 2024-02-27 15:00:24.000000 nest-sw-0.1.2/NEST/checkArgs.py
--rw-rw-r--   0 binli      (501) staff       (20)     1883 2024-02-27 15:00:24.000000 nest-sw-0.1.2/NEST/enrichScore.py
--rw-rw-r--   0 binli      (501) staff       (20)     2380 2024-03-05 04:32:37.000000 nest-sw-0.1.2/NEST/nest.py
--rw-rw-r--   0 binli      (501) staff       (20)      139 2024-02-27 15:00:24.000000 nest-sw-0.1.2/NEST/pvalFun.py
--rw-rw-r--   0 binli      (501) staff       (20)     2396 2024-02-27 15:00:24.000000 nest-sw-0.1.2/NEST/statFun_lm.py
--rw-r--r--   0 binli      (501) staff       (20)      272 2024-03-05 14:59:04.599766 nest-sw-0.1.2/PKG-INFO
--rw-r--r--   0 binli      (501) staff       (20)        0 2024-03-05 04:01:01.000000 nest-sw-0.1.2/README.md
-drwxr-xr-x   0 binli      (501) staff       (20)        0 2024-03-05 14:59:04.599495 nest-sw-0.1.2/nest_sw.egg-info/
--rw-r--r--   0 binli      (501) staff       (20)      272 2024-03-05 14:59:04.000000 nest-sw-0.1.2/nest_sw.egg-info/PKG-INFO
--rw-r--r--   0 binli      (501) staff       (20)      275 2024-03-05 14:59:04.000000 nest-sw-0.1.2/nest_sw.egg-info/SOURCES.txt
--rw-r--r--   0 binli      (501) staff       (20)        1 2024-03-05 14:59:04.000000 nest-sw-0.1.2/nest_sw.egg-info/dependency_links.txt
--rw-r--r--   0 binli      (501) staff       (20)      114 2024-03-05 14:59:04.000000 nest-sw-0.1.2/nest_sw.egg-info/requires.txt
--rw-r--r--   0 binli      (501) staff       (20)        5 2024-03-05 14:59:04.000000 nest-sw-0.1.2/nest_sw.egg-info/top_level.txt
--rw-r--r--   0 binli      (501) staff       (20)       38 2024-03-05 14:59:04.600052 nest-sw-0.1.2/setup.cfg
--rw-r--r--   0 binli      (501) staff       (20)      663 2024-03-05 14:58:58.000000 nest-sw-0.1.2/setup.py
+drwxr-xr-x   0 binli      (501) staff       (20)        0 2024-04-23 20:18:13.105211 nest-sw-0.1.3/
+drwxr-xr-x   0 binli      (501) staff       (20)        0 2024-04-23 20:18:13.103048 nest-sw-0.1.3/NEST/
+-rw-r--r--   0 binli      (501) staff       (20)       42 2024-04-23 20:17:21.000000 nest-sw-0.1.3/NEST/__init__.py
+-rw-rw-r--   0 binli      (501) staff       (20)     1969 2024-02-27 15:00:24.000000 nest-sw-0.1.3/NEST/checkArgs.py
+-rw-rw-r--   0 binli      (501) staff       (20)     1883 2024-02-27 15:00:24.000000 nest-sw-0.1.3/NEST/enrichScore.py
+-rw-rw-r--   0 binli      (501) staff       (20)     2384 2024-04-23 20:17:18.000000 nest-sw-0.1.3/NEST/nest.py
+-rw-rw-r--   0 binli      (501) staff       (20)      139 2024-02-27 15:00:24.000000 nest-sw-0.1.3/NEST/pvalFun.py
+-rw-rw-r--   0 binli      (501) staff       (20)     2396 2024-02-27 15:00:24.000000 nest-sw-0.1.3/NEST/statFun_lm.py
+-rw-r--r--   0 binli      (501) staff       (20)      272 2024-04-23 20:18:13.104933 nest-sw-0.1.3/PKG-INFO
+-rw-r--r--   0 binli      (501) staff       (20)        0 2024-03-05 04:01:01.000000 nest-sw-0.1.3/README.md
+drwxr-xr-x   0 binli      (501) staff       (20)        0 2024-04-23 20:18:13.104587 nest-sw-0.1.3/nest_sw.egg-info/
+-rw-r--r--   0 binli      (501) staff       (20)      272 2024-04-23 20:18:13.000000 nest-sw-0.1.3/nest_sw.egg-info/PKG-INFO
+-rw-r--r--   0 binli      (501) staff       (20)      275 2024-04-23 20:18:13.000000 nest-sw-0.1.3/nest_sw.egg-info/SOURCES.txt
+-rw-r--r--   0 binli      (501) staff       (20)        1 2024-04-23 20:18:13.000000 nest-sw-0.1.3/nest_sw.egg-info/dependency_links.txt
+-rw-r--r--   0 binli      (501) staff       (20)      114 2024-04-23 20:18:13.000000 nest-sw-0.1.3/nest_sw.egg-info/requires.txt
+-rw-r--r--   0 binli      (501) staff       (20)        5 2024-04-23 20:18:13.000000 nest-sw-0.1.3/nest_sw.egg-info/top_level.txt
+-rw-r--r--   0 binli      (501) staff       (20)       38 2024-04-23 20:18:13.105305 nest-sw-0.1.3/setup.cfg
+-rw-r--r--   0 binli      (501) staff       (20)      663 2024-04-23 20:17:48.000000 nest-sw-0.1.3/setup.py
```

### Comparing `nest-sw-0.1.2/NEST/checkArgs.py` & `nest-sw-0.1.3/NEST/checkArgs.py`

 * *Files identical despite different names*

### Comparing `nest-sw-0.1.2/NEST/enrichScore.py` & `nest-sw-0.1.3/NEST/enrichScore.py`

 * *Files identical despite different names*

### Comparing `nest-sw-0.1.2/NEST/nest.py` & `nest-sw-0.1.3/NEST/nest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
-from checkArgs import check_args
-from pvalFun import pval_fun
-from enrichScore import enrichScore
-from statFun_lm import stat_fun_lm
+from .checkArgs import check_args
+from .pvalFun import pval_fun
+from .enrichScore import enrichScore
+from .statFun_lm import stat_fun_lm
 
 
 def nest(statFun,args, net_maps, n_cores=1, seed=None):
     '''
     Input:
         statFun:
         args:
```

### Comparing `nest-sw-0.1.2/NEST/statFun_lm.py` & `nest-sw-0.1.3/NEST/statFun_lm.py`

 * *Files identical despite different names*

### Comparing `nest-sw-0.1.2/setup.py` & `nest-sw-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="nest-sw",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         'numpy>=1.24.1',
         'pandas>=1.5.3',
         'nibabel>=5.0.0',
         'nilearn>=0.10.3',
         'matplotlib>=3.6.3',
```

