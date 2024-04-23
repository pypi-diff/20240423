# Comparing `tmp/meantools-1.1.1.tar.gz` & `tmp/meantools-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meantools-1.1.1.tar", last modified: Tue Apr 23 11:38:13 2024, max compression
+gzip compressed data, was "meantools-1.1.2.tar", last modified: Tue Apr 23 11:43:05 2024, max compression
```

## Comparing `meantools-1.1.1.tar` & `meantools-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 singh018   (501) staff       (20)        0 2024-04-23 11:38:13.511704 meantools-1.1.1/
--rw-r--r--   0 singh018   (501) staff       (20)     1095 2024-04-22 10:08:19.000000 meantools-1.1.1/LICENSE.md
--rw-r--r--   0 singh018   (501) staff       (20)     1055 2024-04-23 11:38:13.511406 meantools-1.1.1/PKG-INFO
--rw-r--r--   0 singh018   (501) staff       (20)      303 2022-08-26 12:41:43.000000 meantools-1.1.1/README.rst
--rw-r--r--   0 singh018   (501) staff       (20)    20923 2024-03-18 13:52:25.000000 meantools-1.1.1/clusters.py
--rwxr-xr-x   0 singh018   (501) staff       (20)    13394 2024-03-20 14:55:54.000000 meantools-1.1.1/corrMultiomics_mod.py
--rw-r--r--   0 singh018   (501) staff       (20)    26386 2024-03-21 15:50:55.000000 meantools-1.1.1/format_databases.py
--rwxr-xr-x   0 singh018   (501) staff       (20)    36507 2024-03-20 14:05:01.000000 meantools-1.1.1/gizmos.py
--rw-r--r--   0 singh018   (501) staff       (20)     2713 2023-01-18 07:39:12.000000 meantools-1.1.1/graphics.py
--rw-r--r--   0 singh018   (501) staff       (20)    43865 2024-03-26 13:56:41.000000 meantools-1.1.1/heraldPathways_mod.py
-drwxr-xr-x   0 singh018   (501) staff       (20)        0 2024-04-23 11:38:13.511083 meantools-1.1.1/meantools.egg-info/
--rw-r--r--   0 singh018   (501) staff       (20)     1055 2024-04-23 11:38:13.000000 meantools-1.1.1/meantools.egg-info/PKG-INFO
--rw-r--r--   0 singh018   (501) staff       (20)      368 2024-04-23 11:38:13.000000 meantools-1.1.1/meantools.egg-info/SOURCES.txt
--rw-r--r--   0 singh018   (501) staff       (20)        1 2024-04-23 11:38:13.000000 meantools-1.1.1/meantools.egg-info/dependency_links.txt
--rw-r--r--   0 singh018   (501) staff       (20)      132 2024-04-23 11:38:13.000000 meantools-1.1.1/meantools.egg-info/requires.txt
--rw-r--r--   0 singh018   (501) staff       (20)        1 2024-04-23 11:38:13.000000 meantools-1.1.1/meantools.egg-info/top_level.txt
--rw-r--r--   0 singh018   (501) staff       (20)     2615 2023-10-17 08:52:57.000000 meantools-1.1.1/mutual_ranks.py
--rwxr-xr-x   0 singh018   (501) staff       (20)    19836 2024-01-18 12:21:15.000000 meantools-1.1.1/pathMassTransitions_mod.py
--rwxr-xr-x   0 singh018   (501) staff       (20)    29925 2024-02-19 22:25:39.000000 meantools-1.1.1/paveWays.py
--rw-r--r--   0 singh018   (501) staff       (20)    15534 2024-02-09 11:11:38.000000 meantools-1.1.1/queryMassNPDB_mod.py
--rw-r--r--   0 singh018   (501) staff       (20)       38 2024-04-23 11:38:13.511765 meantools-1.1.1/setup.cfg
--rw-r--r--   0 singh018   (501) staff       (20)     1140 2024-04-23 11:38:03.000000 meantools-1.1.1/setup.py
+drwxr-xr-x   0 singh018   (501) staff       (20)        0 2024-04-23 11:43:05.891821 meantools-1.1.2/
+-rw-r--r--   0 singh018   (501) staff       (20)     1095 2024-04-22 10:08:19.000000 meantools-1.1.2/LICENSE.md
+-rw-r--r--   0 singh018   (501) staff       (20)      698 2024-04-23 11:43:05.891670 meantools-1.1.2/PKG-INFO
+-rw-r--r--   0 singh018   (501) staff       (20)      303 2022-08-26 12:41:43.000000 meantools-1.1.2/README.rst
+-rw-r--r--   0 singh018   (501) staff       (20)    20923 2024-03-18 13:52:25.000000 meantools-1.1.2/clusters.py
+-rwxr-xr-x   0 singh018   (501) staff       (20)    13394 2024-03-20 14:55:54.000000 meantools-1.1.2/corrMultiomics_mod.py
+-rw-r--r--   0 singh018   (501) staff       (20)    26386 2024-03-21 15:50:55.000000 meantools-1.1.2/format_databases.py
+-rwxr-xr-x   0 singh018   (501) staff       (20)    36507 2024-03-20 14:05:01.000000 meantools-1.1.2/gizmos.py
+-rw-r--r--   0 singh018   (501) staff       (20)     2713 2023-01-18 07:39:12.000000 meantools-1.1.2/graphics.py
+-rw-r--r--   0 singh018   (501) staff       (20)    43865 2024-03-26 13:56:41.000000 meantools-1.1.2/heraldPathways_mod.py
+drwxr-xr-x   0 singh018   (501) staff       (20)        0 2024-04-23 11:43:05.891467 meantools-1.1.2/meantools.egg-info/
+-rw-r--r--   0 singh018   (501) staff       (20)      698 2024-04-23 11:43:05.000000 meantools-1.1.2/meantools.egg-info/PKG-INFO
+-rw-r--r--   0 singh018   (501) staff       (20)      368 2024-04-23 11:43:05.000000 meantools-1.1.2/meantools.egg-info/SOURCES.txt
+-rw-r--r--   0 singh018   (501) staff       (20)        1 2024-04-23 11:43:05.000000 meantools-1.1.2/meantools.egg-info/dependency_links.txt
+-rw-r--r--   0 singh018   (501) staff       (20)      122 2024-04-23 11:43:05.000000 meantools-1.1.2/meantools.egg-info/requires.txt
+-rw-r--r--   0 singh018   (501) staff       (20)        1 2024-04-23 11:43:05.000000 meantools-1.1.2/meantools.egg-info/top_level.txt
+-rw-r--r--   0 singh018   (501) staff       (20)     2615 2023-10-17 08:52:57.000000 meantools-1.1.2/mutual_ranks.py
+-rwxr-xr-x   0 singh018   (501) staff       (20)    19836 2024-01-18 12:21:15.000000 meantools-1.1.2/pathMassTransitions_mod.py
+-rwxr-xr-x   0 singh018   (501) staff       (20)    29925 2024-02-19 22:25:39.000000 meantools-1.1.2/paveWays.py
+-rw-r--r--   0 singh018   (501) staff       (20)    15534 2024-02-09 11:11:38.000000 meantools-1.1.2/queryMassNPDB_mod.py
+-rw-r--r--   0 singh018   (501) staff       (20)       38 2024-04-23 11:43:05.891867 meantools-1.1.2/setup.cfg
+-rw-r--r--   0 singh018   (501) staff       (20)     1127 2024-04-23 11:42:49.000000 meantools-1.1.2/setup.py
```

### Comparing `meantools-1.1.1/LICENSE.md` & `meantools-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/clusters.py` & `meantools-1.1.2/clusters.py`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/corrMultiomics_mod.py` & `meantools-1.1.2/corrMultiomics_mod.py`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/format_databases.py` & `meantools-1.1.2/format_databases.py`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/gizmos.py` & `meantools-1.1.2/gizmos.py`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/graphics.py` & `meantools-1.1.2/graphics.py`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/heraldPathways_mod.py` & `meantools-1.1.2/heraldPathways_mod.py`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/mutual_ranks.py` & `meantools-1.1.2/mutual_ranks.py`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/pathMassTransitions_mod.py` & `meantools-1.1.2/pathMassTransitions_mod.py`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/paveWays.py` & `meantools-1.1.2/paveWays.py`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/queryMassNPDB_mod.py` & `meantools-1.1.2/queryMassNPDB_mod.py`

 * *Files identical despite different names*

### Comparing `meantools-1.1.1/setup.py` & `meantools-1.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='meantools',
-    version='1.1.1',
+    version='1.1.2',
     description='Integration of multi-omics data for biosynthetic pathway discovery',
     long_description=open('README.rst').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/kumarsaurabh20/meantools',
     author='Kumar Saurabh Singh',
     author_email='kumar.singh@wur.nl',
     license='MIT',
     packages=find_packages(),
-    install_requires=['numpy', 'scipy', 'matplotlib', 'rdkit', 'itertools', 'networkx', 'pandas', 'sqlite3', 'tqdm', 'svgutils', 'svgelements', 'scipy', 'markov_clustering', 'seaborn', 'subprocess'],
+    install_requires=['numpy', 'scipy', 'matplotlib', 'rdkit', 'networkx', 'pandas', 'sqlite3', 'tqdm', 'svgutils', 'svgelements', 'scipy', 'markov_clustering', 'seaborn', 'subprocess'],
     classifiers=[
         'Programming Language :: Python :: 3'
     ],
     include_package_data=True,
     package_data={'data': ['data/*.csv', 'data/chem_prop.tsv', 'data/lotus_v101023.sqlite', 'data/mvc.db', 'cluster_one-1.0.jar']},
     python_requires='>=3.8',
     scripts=['corrMultiomics_mod.py', 'format_databases.py', 'gizmos.py', 'heraldPathways_mod.py', 'mutual_ranks.py', 'pathMassTransitions_mod.py', 'paveWays.py', 'queryMassNPDB_mod.py', 'clusters.py', 'graphics.py']
```

