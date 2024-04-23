# Comparing `tmp/convert-us-to-uk-0.1.3.tar.gz` & `tmp/convert-us-to-uk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert-us-to-uk-0.1.3.tar", last modified: Thu Apr 18 11:35:35 2024, max compression
+gzip compressed data, was "convert-us-to-uk-0.1.4.tar", last modified: Tue Apr 23 13:00:05 2024, max compression
```

## Comparing `convert-us-to-uk-0.1.3.tar` & `convert-us-to-uk-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:35:35.819270 convert-us-to-uk-0.1.3/
--rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1936 2024-04-18 11:35:35.805665 convert-us-to-uk-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1606 2024-04-17 15:44:02.000000 convert-us-to-uk-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 11:35:35.772834 convert-us-to-uk-0.1.3/convert_us_to_uk/
--rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.3/convert_us_to_uk/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-04-18 11:33:40.000000 convert-us-to-uk-0.1.3/convert_us_to_uk/converter.py
--rw-rw-rw-   0        0        0    40123 2024-04-17 12:49:20.000000 convert-us-to-uk-0.1.3/convert_us_to_uk/us_to_uk_trans.csv
-drwxrwxrwx   0        0        0        0 2024-04-18 11:35:35.805665 convert-us-to-uk-0.1.3/convert_us_to_uk.egg-info/
--rw-rw-rw-   0        0        0     1936 2024-04-18 11:35:35.000000 convert-us-to-uk-0.1.3/convert_us_to_uk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2024-04-18 11:35:35.000000 convert-us-to-uk-0.1.3/convert_us_to_uk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:35:35.000000 convert-us-to-uk-0.1.3/convert_us_to_uk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-18 11:35:35.000000 convert-us-to-uk-0.1.3/convert_us_to_uk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-18 11:35:35.000000 convert-us-to-uk-0.1.3/convert_us_to_uk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 11:35:35.819270 convert-us-to-uk-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      696 2024-04-18 11:35:28.000000 convert-us-to-uk-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:00:05.530028 convert-us-to-uk-0.1.4/
+-rw-rw-rw-   0        0        0       43 2024-04-17 15:15:06.000000 convert-us-to-uk-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1990 2024-04-23 13:00:05.525588 convert-us-to-uk-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1660 2024-04-18 11:43:12.000000 convert-us-to-uk-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 13:00:05.500211 convert-us-to-uk-0.1.4/convert_us_to_uk/
+-rw-rw-rw-   0        0        0        0 2024-04-17 12:42:42.000000 convert-us-to-uk-0.1.4/convert_us_to_uk/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-04-18 11:33:40.000000 convert-us-to-uk-0.1.4/convert_us_to_uk/converter.py
+-rw-rw-rw-   0        0        0    40125 2024-04-23 12:59:33.000000 convert-us-to-uk-0.1.4/convert_us_to_uk/us_to_uk_trans.csv
+drwxrwxrwx   0        0        0        0 2024-04-23 13:00:05.520366 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-04-23 13:00:05.000000 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-04-23 13:00:05.000000 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 13:00:05.000000 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-23 13:00:05.000000 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-23 13:00:05.000000 convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 13:00:05.530028 convert-us-to-uk-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      696 2024-04-23 12:59:48.000000 convert-us-to-uk-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:00:05.524923 convert-us-to-uk-0.1.4/tests/
+-rw-rw-rw-   0        0        0      296 2024-04-17 14:23:12.000000 convert-us-to-uk-0.1.4/tests/test_converter.py
```

### Comparing `convert-us-to-uk-0.1.3/PKG-INFO` & `convert-us-to-uk-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
@@ -17,14 +17,15 @@
 ```
 pip install convert-us-to-uk
 ```
 
 ## Usage
 
 ```python
+from convert_us_to_uk.converter import convert_to_uk
 text = "Colors are my favorite things."
 uk_text = convert_to_uk(text)
 print(uk_text)
 # OUTPUT: "Colours are my favourite things."
 ```
 
 ## Motivation
```

### Comparing `convert-us-to-uk-0.1.3/README.md` & `convert-us-to-uk-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ```
 pip install convert-us-to-uk
 ```
 
 ## Usage
 
 ```python
+from convert_us_to_uk.converter import convert_to_uk
 text = "Colors are my favorite things."
 uk_text = convert_to_uk(text)
 print(uk_text)
 # OUTPUT: "Colours are my favourite things."
 ```
 
 ## Motivation
```

### Comparing `convert-us-to-uk-0.1.3/convert_us_to_uk/converter.py` & `convert-us-to-uk-0.1.4/convert_us_to_uk/converter.py`

 * *Files identical despite different names*

### Comparing `convert-us-to-uk-0.1.3/convert_us_to_uk/us_to_uk_trans.csv` & `convert-us-to-uk-0.1.4/convert_us_to_uk/us_to_uk_trans.csv`

 * *Files 0% similar despite different names*

```diff
@@ -292,16 +292,16 @@
 computerized,computerised
 computerizes,computerises
 computerizing,computerising
 conceptualize,conceptualise
 conceptualized,conceptualised
 conceptualizes,conceptualises
 conceptualizing,conceptualising
-connection,connexion
-connections,connexions
+connection,connection
+connections,connections
 contextualize,contextualise
 contextualized,contextualised
 contextualizes,contextualises
 contextualizing,contextualising
 cozier,cosier
 cozies,cosies
 coziest,cosiest
```

### Comparing `convert-us-to-uk-0.1.3/convert_us_to_uk.egg-info/PKG-INFO` & `convert-us-to-uk-0.1.4/convert_us_to_uk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-us-to-uk
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple utility to convert US spelling to UK spelling.
 Home-page: https://github.com/oliverblane/convert-us-to-uk/tree/main
 Author: Oliver Blane
 Author-email: oliverblane72@gmail.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
@@ -17,14 +17,15 @@
 ```
 pip install convert-us-to-uk
 ```
 
 ## Usage
 
 ```python
+from convert_us_to_uk.converter import convert_to_uk
 text = "Colors are my favorite things."
 uk_text = convert_to_uk(text)
 print(uk_text)
 # OUTPUT: "Colours are my favourite things."
 ```
 
 ## Motivation
```

### Comparing `convert-us-to-uk-0.1.3/setup.py` & `convert-us-to-uk-0.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='convert-us-to-uk',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     include_package_data=True,
     description='A simple utility to convert US spelling to UK spelling.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Oliver Blane',
     author_email='oliverblane72@gmail.com',
```

