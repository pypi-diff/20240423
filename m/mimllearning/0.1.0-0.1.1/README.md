# Comparing `tmp/mimllearning-0.1.0.tar.gz` & `tmp/mimllearning-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimllearning-0.1.0.tar", last modified: Mon Apr 22 23:54:44 2024, max compression
+gzip compressed data, was "mimllearning-0.1.1.tar", last modified: Tue Apr 23 16:54:36 2024, max compression
```

## Comparing `mimllearning-0.1.0.tar` & `mimllearning-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 23:54:44.289358 mimllearning-0.1.0/
--rw-rw-rw-   0        0        0      334 2024-04-22 23:54:44.285817 mimllearning-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 23:54:44.285817 mimllearning-0.1.0/mimllearning.egg-info/
--rw-rw-rw-   0        0        0      334 2024-04-22 23:54:44.000000 mimllearning-0.1.0/mimllearning.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2024-04-22 23:54:44.000000 mimllearning-0.1.0/mimllearning.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 23:54:44.000000 mimllearning-0.1.0/mimllearning.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 23:54:44.000000 mimllearning-0.1.0/mimllearning.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 23:54:44.289358 mimllearning-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      400 2024-04-22 23:53:38.000000 mimllearning-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.897359 mimllearning-0.1.1/
+-rw-rw-rw-   0        0        0      334 2024-04-23 16:54:36.897359 mimllearning-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.833186 mimllearning-0.1.1/classifier/
+-rw-rw-rw-   0        0        0      101 2024-04-22 22:05:52.000000 mimllearning-0.1.1/classifier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.842733 mimllearning-0.1.1/classifier/mi/
+-rw-rw-rw-   0        0        0      234 2024-04-22 22:05:52.000000 mimllearning-0.1.1/classifier/mi/__init__.py
+-rw-rw-rw-   0        0        0     1290 2024-04-21 22:25:46.000000 mimllearning-0.1.1/classifier/mi/all_positive_apr_classifier.py
+-rw-rw-rw-   0        0        0      480 2024-04-22 21:54:22.000000 mimllearning-0.1.1/classifier/mi/apr_classifier.py
+-rw-rw-rw-   0        0        0     2695 2024-04-21 22:25:46.000000 mimllearning-0.1.1/classifier/mi/iterated_discrim_apr_classifier.py
+-rw-rw-rw-   0        0        0     1246 2024-04-22 21:54:22.000000 mimllearning-0.1.1/classifier/mi/miles_classifier.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.848919 mimllearning-0.1.1/classifier/mimlTOmi/
+-rw-rw-rw-   0        0        0      115 2024-04-22 22:06:16.000000 mimllearning-0.1.1/classifier/mimlTOmi/__init__.py
+-rw-rw-rw-   0        0        0     3496 2024-04-21 21:48:44.000000 mimllearning-0.1.1/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-rw-rw-   0        0        0     1062 2024-04-18 20:06:41.000000 mimllearning-0.1.1/classifier/mimlTOmi/miml_to_mi_classifier.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.848919 mimllearning-0.1.1/classifier/mimlTOml/
+-rw-rw-rw-   0        0        0       55 2024-04-22 22:05:52.000000 mimllearning-0.1.1/classifier/mimlTOml/__init__.py
+-rw-rw-rw-   0        0        0     2704 2024-04-18 19:37:28.000000 mimllearning-0.1.1/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-rw-rw-   0        0        0     1783 2024-04-22 22:08:10.000000 mimllearning-0.1.1/classifier/miml_classifier.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.859882 mimllearning-0.1.1/data/
+-rw-rw-rw-   0        0        0       93 2024-04-22 22:05:52.000000 mimllearning-0.1.1/data/__init__.py
+-rw-rw-rw-   0        0        0     9087 2024-04-22 21:54:22.000000 mimllearning-0.1.1/data/bag.py
+-rw-rw-rw-   0        0        0     6846 2024-04-21 21:48:44.000000 mimllearning-0.1.1/data/instance.py
+-rw-rw-rw-   0        0        0    15284 2024-04-21 22:25:46.000000 mimllearning-0.1.1/data/miml_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.864923 mimllearning-0.1.1/datasets/
+-rw-rw-rw-   0        0        0       57 2024-04-22 22:06:42.000000 mimllearning-0.1.1/datasets/__init__.py
+-rw-rw-rw-   0        0        0     2482 2024-04-21 22:14:03.000000 mimllearning-0.1.1/datasets/arff_to_csv.py
+-rw-rw-rw-   0        0        0     4744 2024-04-21 22:14:03.000000 mimllearning-0.1.1/datasets/load_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.897359 mimllearning-0.1.1/mimllearning.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-04-23 16:54:36.000000 mimllearning-0.1.1/mimllearning.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1050 2024-04-23 16:54:36.000000 mimllearning-0.1.1/mimllearning.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 16:54:36.000000 mimllearning-0.1.1/mimllearning.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-23 16:54:36.000000 mimllearning-0.1.1/mimllearning.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 16:54:36.897359 mimllearning-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      400 2024-04-23 16:54:07.000000 mimllearning-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.880803 mimllearning-0.1.1/transformation/
+-rw-rw-rw-   0        0        0       52 2024-04-22 22:05:52.000000 mimllearning-0.1.1/transformation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.880803 mimllearning-0.1.1/transformation/mimlTOmi/
+-rw-rw-rw-   0        0        0       78 2024-04-22 22:05:52.000000 mimllearning-0.1.1/transformation/mimlTOmi/__init__.py
+-rw-rw-rw-   0        0        0     1423 2024-04-22 21:54:22.000000 mimllearning-0.1.1/transformation/mimlTOmi/binary_relevance_transformation.py
+drwxrwxrwx   0        0        0        0 2024-04-23 16:54:36.893318 mimllearning-0.1.1/transformation/mimlTOml/
+-rw-rw-rw-   0        0        0      205 2024-04-22 22:05:52.000000 mimllearning-0.1.1/transformation/mimlTOml/__init__.py
+-rw-rw-rw-   0        0        0     1974 2024-04-21 21:48:44.000000 mimllearning-0.1.1/transformation/mimlTOml/arithmetic.py
+-rw-rw-rw-   0        0        0     2089 2024-04-22 21:55:22.000000 mimllearning-0.1.1/transformation/mimlTOml/geometric.py
+-rw-rw-rw-   0        0        0      382 2024-04-21 19:59:53.000000 mimllearning-0.1.1/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-rw-rw-   0        0        0     2085 2024-04-21 19:59:53.000000 mimllearning-0.1.1/transformation/mimlTOml/minmax.py
```

