# Comparing `tmp/crawlnet-0.0.2.tar.gz` & `tmp/crawlnet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlnet-0.0.2.tar", last modified: Tue Apr 23 12:58:54 2024, max compression
+gzip compressed data, was "crawlnet-0.0.3.tar", last modified: Tue Apr 23 13:17:00 2024, max compression
```

## Comparing `crawlnet-0.0.2.tar` & `crawlnet-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 12:58:54.991434 crawlnet-0.0.2/
--rw-rw-rw-   0        0        0      794 2024-04-23 12:58:54.990189 crawlnet-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      151 2024-04-23 12:57:45.000000 crawlnet-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 12:58:54.964859 crawlnet-0.0.2/crawlnet/
--rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.2/crawlnet/__init__.py
--rw-rw-rw-   0        0        0    21578 2024-04-23 10:43:27.000000 crawlnet-0.0.2/crawlnet/cl3.py
--rw-rw-rw-   0        0        0    18103 2024-04-23 12:55:21.000000 crawlnet-0.0.2/crawlnet/cl4.py
-drwxrwxrwx   0        0        0        0 2024-04-23 12:58:54.989179 crawlnet-0.0.2/crawlnet.egg-info/
--rw-rw-rw-   0        0        0      794 2024-04-23 12:58:54.000000 crawlnet-0.0.2/crawlnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-23 12:58:54.000000 crawlnet-0.0.2/crawlnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 12:58:54.000000 crawlnet-0.0.2/crawlnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-23 12:58:54.000000 crawlnet-0.0.2/crawlnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-23 12:58:54.000000 crawlnet-0.0.2/crawlnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 12:58:54.991434 crawlnet-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-04-23 12:56:04.000000 crawlnet-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:17:00.321701 crawlnet-0.0.3/
+-rw-rw-rw-   0        0        0      794 2024-04-23 13:17:00.321701 crawlnet-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2024-04-23 12:57:45.000000 crawlnet-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 13:17:00.259197 crawlnet-0.0.3/crawlnet/
+-rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.3/crawlnet/__init__.py
+-rw-rw-rw-   0        0        0    21573 2024-04-23 13:16:42.000000 crawlnet-0.0.3/crawlnet/cl3.py
+-rw-rw-rw-   0        0        0    18103 2024-04-23 12:55:21.000000 crawlnet-0.0.3/crawlnet/cl4.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:17:00.321701 crawlnet-0.0.3/crawlnet.egg-info/
+-rw-rw-rw-   0        0        0      794 2024-04-23 13:17:00.000000 crawlnet-0.0.3/crawlnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-23 13:17:00.000000 crawlnet-0.0.3/crawlnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 13:17:00.000000 crawlnet-0.0.3/crawlnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-23 13:17:00.000000 crawlnet-0.0.3/crawlnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-23 13:17:00.000000 crawlnet-0.0.3/crawlnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 13:17:00.321701 crawlnet-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-04-23 13:16:22.000000 crawlnet-0.0.3/setup.py
```

### Comparing `crawlnet-0.0.2/PKG-INFO` & `crawlnet-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlnet
-Version: 0.0.2
+Version: 0.0.3
 Summary: CrawlNet
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: `!pip install crawlnet`
```

### Comparing `crawlnet-0.0.2/crawlnet/cl3.py` & `crawlnet-0.0.3/crawlnet/cl3.py`

 * *Files 2% similar despite different names*

```diff
@@ -679,15 +679,15 @@
     "mapreduce_character_count": mapreduce_character_count,
     "fuzzy_sets_u_n": fuzzy_sets_u_n,
     "optimize_gen_algo_spray_dry": optimize_gen_algo_spray_dry,
     "clonal_select_algo": clonal_select_algo,
     "Deap": Deap,
     "ant_colony": ant_colony,
     "arti_immune_pr_damage_class": arti_immune_pr_damage_class,
-    "arti_immune_pr_damage_class": arti_immune_pr_damage_class,
+    "art_neural_style_transfer": art_neural_style_transfer
 }
 
 
 class Writer:
     def __init__(self, filename):
         self.filename = os.path.join(os.getcwd(), filename)
         self.masterDict = masterDict
```

### Comparing `crawlnet-0.0.2/crawlnet/cl4.py` & `crawlnet-0.0.3/crawlnet/cl4.py`

 * *Files identical despite different names*

### Comparing `crawlnet-0.0.2/crawlnet.egg-info/PKG-INFO` & `crawlnet-0.0.3/crawlnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlnet
-Version: 0.0.2
+Version: 0.0.3
 Summary: CrawlNet
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: `!pip install crawlnet`
```

### Comparing `crawlnet-0.0.2/setup.py` & `crawlnet-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 DESCRIPTION = "CrawlNet"
 
 # Setting up
 setup(
     name="crawlnet",
     version=VERSION,
     author="Hrushikesh Kachgunde",
```

