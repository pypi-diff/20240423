# Comparing `tmp/miml_package-0.0.9.tar.gz` & `tmp/miml_package-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "miml_package-0.3.0.tar", last modified: Mon Apr 22 23:47:16 2024, max compression
```

## Comparing `miml_package-0.0.9.tar` & `miml_package-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,9 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 miml_package-0.0.9/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miml_package-0.0.9/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 miml_package-0.0.9/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0    83682 2020-02-02 00:00:00.000000 miml_package-0.0.9/documentation/Formato datos tfg.png
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/classifier/abstract_classifier.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/classifier/knn_classifier.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/data/__init__.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/data/bag.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/data/instance.py
--rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/datasets/arff_to_csv.py
--rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/datasets/load_dataset.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/datasets/toy.csv
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/transformation/mimlTOmi/binary_relevance.py
--rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/tutorial/binary_relevance.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/tutorial/binary_relevance_transformation.py
--rw-r--r--   0        0        0    12257 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/tutorial/demo_MIML.ipynb
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/tutorial/instance_test.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/tutorial/main.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/tutorial/show_data.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 miml_package-0.0.9/src/miml/tutorial/update_data.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 miml_package-0.0.9/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 miml_package-0.0.9/README.md
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 miml_package-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 miml_package-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 23:47:16.452965 miml_package-0.3.0/
+-rw-rw-rw-   0        0        0      334 2024-04-22 23:47:16.452965 miml_package-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 23:47:16.452965 miml_package-0.3.0/miml_package.egg-info/
+-rw-rw-rw-   0        0        0      334 2024-04-22 23:47:16.000000 miml_package-0.3.0/miml_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2024-04-22 23:47:16.000000 miml_package-0.3.0/miml_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 23:47:16.000000 miml_package-0.3.0/miml_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 23:47:16.000000 miml_package-0.3.0/miml_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 23:47:16.452965 miml_package-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      400 2024-04-22 23:44:51.000000 miml_package-0.3.0/setup.py
```

