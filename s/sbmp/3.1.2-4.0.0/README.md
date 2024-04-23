# Comparing `tmp/sbmp-3.1.2.tar.gz` & `tmp/sbmp-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmp-3.1.2.tar", last modified: Mon Apr 22 17:02:16 2024, max compression
+gzip compressed data, was "sbmp-4.0.0.tar", last modified: Tue Apr 23 12:05:48 2024, max compression
```

## Comparing `sbmp-3.1.2.tar` & `sbmp-4.0.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-22 17:02:16.726237 sbmp-3.1.2/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)     1075 2024-01-08 11:37:56.000000 sbmp-3.1.2/LICENSE
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-22 17:02:16.725955 sbmp-3.1.2/PKG-INFO
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        6 2024-01-08 11:39:16.000000 sbmp-3.1.2/README.txt
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-22 17:02:16.724910 sbmp-3.1.2/sbmp/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)       18 2024-01-08 11:36:04.000000 sbmp-3.1.2/sbmp/__init__.py
--rw-------   0 jainambarbhaya   (501) staff       (20)    14742 2024-04-12 17:13:38.000000 sbmp-3.1.2/sbmp/iss.py
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-22 17:02:16.725702 sbmp-3.1.2/sbmp.egg-info/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-22 17:02:16.000000 sbmp-3.1.2/sbmp.egg-info/PKG-INFO
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      168 2024-04-22 17:02:16.000000 sbmp-3.1.2/sbmp.egg-info/SOURCES.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        1 2024-04-22 17:02:16.000000 sbmp-3.1.2/sbmp.egg-info/dependency_links.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        5 2024-04-22 17:02:16.000000 sbmp-3.1.2/sbmp.egg-info/top_level.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)       38 2024-04-22 17:02:16.726285 sbmp-3.1.2/setup.cfg
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      991 2024-04-22 17:02:13.000000 sbmp-3.1.2/setup.py
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 12:05:48.887874 sbmp-4.0.0/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)     1075 2024-01-08 11:37:56.000000 sbmp-4.0.0/LICENSE
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-23 12:05:48.887564 sbmp-4.0.0/PKG-INFO
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        6 2024-01-08 11:39:16.000000 sbmp-4.0.0/README.txt
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 12:05:48.886726 sbmp-4.0.0/sbmp/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)       37 2024-04-23 10:25:06.000000 sbmp-4.0.0/sbmp/__init__.py
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)    20983 2024-04-23 12:05:01.000000 sbmp-4.0.0/sbmp/awt.py
+-rw-------   0 jainambarbhaya   (501) staff       (20)    14742 2024-04-12 17:13:38.000000 sbmp-4.0.0/sbmp/iss.py
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 12:05:48.887364 sbmp-4.0.0/sbmp.egg-info/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-23 12:05:48.000000 sbmp-4.0.0/sbmp.egg-info/PKG-INFO
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      180 2024-04-23 12:05:48.000000 sbmp-4.0.0/sbmp.egg-info/SOURCES.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        1 2024-04-23 12:05:48.000000 sbmp-4.0.0/sbmp.egg-info/dependency_links.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        5 2024-04-23 12:05:48.000000 sbmp-4.0.0/sbmp.egg-info/top_level.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)       38 2024-04-23 12:05:48.887923 sbmp-4.0.0/setup.cfg
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      991 2024-04-23 12:05:39.000000 sbmp-4.0.0/setup.py
```

### Comparing `sbmp-3.1.2/LICENSE` & `sbmp-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmp-3.1.2/PKG-INFO` & `sbmp-4.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmp
-Version: 3.1.2
+Version: 4.0.0
 Summary: SBMP
 Home-page: 
 Author: Jainam Barbhaya
 Author-email: jainambarbhaya1509@gmail.com
 License: MIT
 Keywords: sbmp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sbmp-3.1.2/sbmp/iss.py` & `sbmp-4.0.0/sbmp/iss.py`

 * *Files identical despite different names*

### Comparing `sbmp-3.1.2/sbmp.egg-info/PKG-INFO` & `sbmp-4.0.0/sbmp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmp
-Version: 3.1.2
+Version: 4.0.0
 Summary: SBMP
 Home-page: 
 Author: Jainam Barbhaya
 Author-email: jainambarbhaya1509@gmail.com
 License: MIT
 Keywords: sbmp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sbmp-3.1.2/setup.py` & `sbmp-4.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     with open('CHANGELOG.txt', 'r') as changelog_file:
         changelog_content = changelog_file.read()
 except FileNotFoundError:
     changelog_content = 'No changelog available.'
 
 setup(
   name='sbmp',
-  version='3.1.2',
+  version='4.0.0',
   description='SBMP',
   long_description=readme_content + '\n\n' + changelog_content,
   url='',  
   author='Jainam Barbhaya',
   author_email='jainambarbhaya1509@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

