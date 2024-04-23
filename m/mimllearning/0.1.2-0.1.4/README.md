# Comparing `tmp/mimllearning-0.1.2.tar.gz` & `tmp/mimllearning-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimllearning-0.1.2.tar", last modified: Tue Apr 23 17:17:24 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mimllearning-0.1.2.tar` & `mimllearning-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:17:24.105838 mimllearning-0.1.2/
--rw-rw-rw-   0        0        0      334 2024-04-23 17:17:24.102376 mimllearning-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 17:17:24.101359 mimllearning-0.1.2/mimllearning.egg-info/
--rw-rw-rw-   0        0        0      334 2024-04-23 17:17:23.000000 mimllearning-0.1.2/mimllearning.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      974 2024-04-23 17:17:23.000000 mimllearning-0.1.2/mimllearning.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:17:23.000000 mimllearning-0.1.2/mimllearning.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2024-04-23 17:17:23.000000 mimllearning-0.1.2/mimllearning.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 17:17:24.105838 mimllearning-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      522 2024-04-23 17:16:38.000000 mimllearning-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:17:23.953974 mimllearning-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 17:17:24.070147 mimllearning-0.1.2/src/miml/
--rw-rw-rw-   0        0        0        0 2024-04-23 17:12:03.000000 mimllearning-0.1.2/src/miml/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:17:24.074204 mimllearning-0.1.2/src/miml/classifier/
--rw-rw-rw-   0        0        0      101 2024-04-22 22:05:52.000000 mimllearning-0.1.2/src/miml/classifier/__init__.py
--rw-rw-rw-   0        0        0     1783 2024-04-22 22:08:10.000000 mimllearning-0.1.2/src/miml/classifier/miml_classifier.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:17:24.080772 mimllearning-0.1.2/src/miml/data/
--rw-rw-rw-   0        0        0       93 2024-04-22 22:05:52.000000 mimllearning-0.1.2/src/miml/data/__init__.py
--rw-rw-rw-   0        0        0     9087 2024-04-22 21:54:22.000000 mimllearning-0.1.2/src/miml/data/bag.py
--rw-rw-rw-   0        0        0     6846 2024-04-21 21:48:44.000000 mimllearning-0.1.2/src/miml/data/instance.py
--rw-rw-rw-   0        0        0    15284 2024-04-21 22:25:46.000000 mimllearning-0.1.2/src/miml/data/miml_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:17:24.090157 mimllearning-0.1.2/src/miml/datasets/
--rw-rw-rw-   0        0        0       57 2024-04-22 22:06:42.000000 mimllearning-0.1.2/src/miml/datasets/__init__.py
--rw-rw-rw-   0        0        0     2482 2024-04-21 22:14:03.000000 mimllearning-0.1.2/src/miml/datasets/arff_to_csv.py
--rw-rw-rw-   0        0        0     4744 2024-04-21 22:14:03.000000 mimllearning-0.1.2/src/miml/datasets/load_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:17:24.091669 mimllearning-0.1.2/src/miml/test/
--rw-rw-rw-   0        0        0     2119 2024-04-22 21:54:22.000000 mimllearning-0.1.2/src/miml/test/data_test.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:17:24.095107 mimllearning-0.1.2/src/miml/transformation/
--rw-rw-rw-   0        0        0       52 2024-04-22 22:05:52.000000 mimllearning-0.1.2/src/miml/transformation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:17:24.095107 mimllearning-0.1.2/src/miml/tutorial/
--rw-rw-rw-   0        0        0      726 2024-04-22 21:54:22.000000 mimllearning-0.1.2/src/miml/tutorial/demo.py
--rw-rw-rw-   0        0        0      526 2024-04-23 17:04:33.000000 mimllearning-0.1.2/src/miml/tutorial/demopypi.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 mimllearning-0.1.4/.gitattributes
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.4/readme.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 mimllearning-0.1.4/todo.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.1.4/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0    83682 2020-02-02 00:00:00.000000 mimllearning-0.1.4/documentation/Formato datos tfg.png
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/mi/iterated_discrim_apr_classifier.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/data/__init__.py
+-rw-r--r--   0        0        0     9087 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/data/instance.py
+-rw-r--r--   0        0        0    15284 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/datasets/arff_to_csv.py
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/datasets/load_dataset.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/datasets/toy.csv
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/tutorial/demo.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 mimllearning-0.1.4/src/miml/tutorial/demopypi.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 mimllearning-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 mimllearning-0.1.4/README.md
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 mimllearning-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mimllearning-0.1.4/PKG-INFO
```

### Comparing `mimllearning-0.1.2/src/miml/classifier/miml_classifier.py` & `mimllearning-0.1.4/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.2/src/miml/data/bag.py` & `mimllearning-0.1.4/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.2/src/miml/data/instance.py` & `mimllearning-0.1.4/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.2/src/miml/data/miml_dataset.py` & `mimllearning-0.1.4/src/miml/data/miml_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.2/src/miml/datasets/arff_to_csv.py` & `mimllearning-0.1.4/src/miml/datasets/arff_to_csv.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.2/src/miml/datasets/load_dataset.py` & `mimllearning-0.1.4/src/miml/datasets/load_dataset.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.2/src/miml/test/data_test.py` & `mimllearning-0.1.4/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.2/src/miml/tutorial/demo.py` & `mimllearning-0.1.4/src/miml/tutorial/demo.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.1.2/src/miml/tutorial/demopypi.py` & `mimllearning-0.1.4/src/miml/tutorial/demopypi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import 
+import mimllearning as miml
 
 dataset_train = load_dataset("../datasets/miml_birds_random_80train.arff", delimiter="'")
 dataset_test = load_dataset("../datasets/miml_birds_random_20test.arff", delimiter="'")
 
 #classifier = MIMLtoMLClassifier(KNeighborsClassifier(), ArithmeticTransformation())
 classifier = MIMLtoMIBRClassifier(AllPositiveAPRClassifier())
```

