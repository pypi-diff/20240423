# Comparing `tmp/crawlnet-0.0.5.tar.gz` & `tmp/crawlnet-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlnet-0.0.5.tar", last modified: Tue Apr 23 17:34:43 2024, max compression
+gzip compressed data, was "crawlnet-0.0.6.tar", last modified: Tue Apr 23 18:18:38 2024, max compression
```

## Comparing `crawlnet-0.0.5.tar` & `crawlnet-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:43.317258 crawlnet-0.0.5/
--rw-rw-rw-   0        0        0      794 2024-04-23 17:34:43.316258 crawlnet-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      151 2024-04-23 12:57:45.000000 crawlnet-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:43.295208 crawlnet-0.0.5/crawlnet/
--rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.5/crawlnet/__init__.py
--rw-rw-rw-   0        0        0    23821 2024-04-23 17:34:02.000000 crawlnet-0.0.5/crawlnet/cl3.py
--rw-rw-rw-   0        0        0    18103 2024-04-23 12:55:21.000000 crawlnet-0.0.5/crawlnet/cl4.py
-drwxrwxrwx   0        0        0        0 2024-04-23 17:34:43.315286 crawlnet-0.0.5/crawlnet.egg-info/
--rw-rw-rw-   0        0        0      794 2024-04-23 17:34:43.000000 crawlnet-0.0.5/crawlnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-04-23 17:34:43.000000 crawlnet-0.0.5/crawlnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 17:34:43.000000 crawlnet-0.0.5/crawlnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-04-23 17:34:43.000000 crawlnet-0.0.5/crawlnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-23 17:34:43.000000 crawlnet-0.0.5/crawlnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 17:34:43.317258 crawlnet-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      806 2024-04-23 17:34:39.000000 crawlnet-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:38.823805 crawlnet-0.0.6/
+-rw-rw-rw-   0        0        0      794 2024-04-23 18:18:38.823805 crawlnet-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2024-04-23 12:57:45.000000 crawlnet-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:38.782030 crawlnet-0.0.6/crawlnet/
+-rw-rw-rw-   0        0        0       56 2024-04-23 11:01:42.000000 crawlnet-0.0.6/crawlnet/__init__.py
+-rw-rw-rw-   0        0        0    24417 2024-04-23 18:18:01.000000 crawlnet-0.0.6/crawlnet/cl3.py
+-rw-rw-rw-   0        0        0    18103 2024-04-23 12:55:21.000000 crawlnet-0.0.6/crawlnet/cl4.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:18:38.811401 crawlnet-0.0.6/crawlnet.egg-info/
+-rw-rw-rw-   0        0        0      794 2024-04-23 18:18:38.000000 crawlnet-0.0.6/crawlnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2024-04-23 18:18:38.000000 crawlnet-0.0.6/crawlnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:18:38.000000 crawlnet-0.0.6/crawlnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-23 18:18:38.000000 crawlnet-0.0.6/crawlnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-23 18:18:38.000000 crawlnet-0.0.6/crawlnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:18:38.823805 crawlnet-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      806 2024-04-23 18:18:36.000000 crawlnet-0.0.6/setup.py
```

### Comparing `crawlnet-0.0.5/PKG-INFO` & `crawlnet-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlnet
-Version: 0.0.5
+Version: 0.0.6
 Summary: CrawlNet
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: `!pip install crawlnet`
```

### Comparing `crawlnet-0.0.5/crawlnet/cl3.py` & `crawlnet-0.0.6/crawlnet/cl3.py`

 * *Files 13% similar despite different names*

```diff
@@ -172,72 +172,66 @@
 
 ### To run
 python3 .\character_count.py x.txt
 python3 .\word_count.py x.txt
 """
 
 fuzzy_sets_u_n = """
-A = dict()
-B = dict()
-Y = dict()
-
-A = {"a": 0.2, "b": 0.3, "c": 0.6, "d": 0.6}
-B = {"a": 0.9, "b": 0.9, "c": 0.4, "d": 0.5}
-
-print('The First Fuzzy Set is :', A)
-print('The Second Fuzzy Set is :', B)
-
-
-for A_key, B_key in zip(A, B):
-	A_value = A[A_key]
-	B_value = B[B_key]
-
-	if A_value > B_value:
-		Y[A_key] = A_value
-	else:
-		Y[B_key] = B_value
-		
-print('Fuzzy Set Union is :', Y)
+import numpy as np
 
-
-
-for A_key, B_key in zip(A, B):
-	A_value = A[A_key]
-	B_value = B[B_key]
-
-	if A_value < B_value:
-		Y[A_key] = A_value
-	else:
-		Y[B_key] = B_value
-print('Fuzzy Set Intersection is :', Y)
-
-A = dict()
-Y = dict()
- 
-A = {"a": 0.2, "b": 0.3, "c": 0.6, "d": 0.6}
- 
-print('The Fuzzy Set is :', A)
- 
- 
-for A_key in A:
-   Y[A_key]= 1-A[A_key]
-         
-print('Fuzzy Set Complement is :', Y)
-
-for A_key, B_key in zip(A, B):
-    A_value = A[A_key]
-    B_value = B[B_key]
-    B_value = 1 - B_value
- 
-    if A_value < B_value:
-        Y[A_key] = A_value
-    else:
-        Y[B_key] = B_value
-         
-print('Fuzzy Set Difference is :', Y)
+# Function to perform Union operation on fuzzy sets
+def fuzzy_union(A, B):
+    return np.maximum(A, B)
+
+# Function to perform Intersection operation on fuzzy sets
+def fuzzy_intersection(A, B):
+    return np.minimum(A, B)
+
+#Function to perform Complement operation on a fuzzy set
+def fuzzy_complement(A):
+    return 1 - A
+
+# Function to perform Difference operation on fuzzy sets
+def fuzzy_difference(A, B):
+    return np.maximum(A, 1 - B)
+
+# Function to create fuzzy relation by Cartesian product of two fuzzy sets
+def cartesian_product(A, B):
+    return np.outer(A, B)
+
+# Function to perform Max-Min composition on two fuzzy relations
+def max_min_composition(R, S):
+    return np.max(np.minimum.outer(R, S), axis=1)
+
+# Example usage
+A = np.array([0.2, 0.4, 0.6, 0.8]) # Fuzzy set A
+B = np.array([0.3, 0.5, 0.7, 0.9]) # Fuzzy set B
+# Operations on fuzzy sets
+union_result = fuzzy_union(A, B)
+intersection_result = fuzzy_intersection(A, B)
+complement_A = fuzzy_complement(A)
+difference_result = fuzzy_difference(A, B)
+print("Union:", union_result)
+print("Intersection:", intersection_result)
+print("Complement of A:", complement_A)
+print("Difference:", difference_result)
+# Fuzzy relations
+R = np.array([0.2, 0.5, 0.4]) # Fuzzy relation R
+S = np.array([0.6, 0.3, 0.7]) # Fuzzy relation S
+
+# Cartesian product of fuzzy relations
+cartesian_result = cartesian_product(R, S)
+
+# Max-Min composition of fuzzy relations
+composition_result = max_min_composition(R, S)
+
+print("Cartesian product of R and S:")
+print(cartesian_result)
+print("Max-Min composition of R and S:")
+print(composition_result)
 """
 
 optimize_gen_algo_spray_dry = """
 import random
 
 from deap import base, creator, tools, algorithms
```

### Comparing `crawlnet-0.0.5/crawlnet/cl4.py` & `crawlnet-0.0.6/crawlnet/cl4.py`

 * *Files identical despite different names*

### Comparing `crawlnet-0.0.5/crawlnet.egg-info/PKG-INFO` & `crawlnet-0.0.6/crawlnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlnet
-Version: 0.0.5
+Version: 0.0.6
 Summary: CrawlNet
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: `!pip install crawlnet`
```

### Comparing `crawlnet-0.0.5/setup.py` & `crawlnet-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 DESCRIPTION = "CrawlNet"
 
 # Setting up
 setup(
     name="crawlnet",
     version=VERSION,
     author="Hrushikesh Kachgunde",
```

