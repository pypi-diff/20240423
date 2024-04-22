# Comparing `tmp/sqlUts-1.0.1.tar.gz` & `tmp/sqlUts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlUts-1.0.1.tar", last modified: Mon Apr 22 21:49:47 2024, max compression
+gzip compressed data, was "sqlUts-1.0.2.tar", last modified: Mon Apr 22 21:51:17 2024, max compression
```

## Comparing `sqlUts-1.0.1.tar` & `sqlUts-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 21:49:47.497484 sqlUts-1.0.1/
--rw-rw-rw-   0        0        0      387 2023-05-02 14:14:50.000000 sqlUts-1.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-05-02 14:14:50.000000 sqlUts-1.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-05-02 14:14:50.000000 sqlUts-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3658 2024-04-22 21:49:47.494484 sqlUts-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2679 2023-05-02 14:14:50.000000 sqlUts-1.0.1/README.md
--rw-rw-rw-   0        0        0      214 2024-04-22 21:38:54.000000 sqlUts-1.0.1/commands.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 21:49:47.497484 sqlUts-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      881 2024-04-22 21:49:32.000000 sqlUts-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 21:49:47.386518 sqlUts-1.0.1/sqlUts/
--rw-rw-rw-   0        0        0     1658 2024-04-22 21:49:39.000000 sqlUts-1.0.1/sqlUts/__init__.py
--rw-rw-rw-   0        0        0       17 2024-04-22 21:49:19.000000 sqlUts-1.0.1/sqlUts/version.py
-drwxrwxrwx   0        0        0        0 2024-04-22 21:49:47.491481 sqlUts-1.0.1/sqlUts.egg-info/
--rw-rw-rw-   0        0        0     3658 2024-04-22 21:49:46.000000 sqlUts-1.0.1/sqlUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-22 21:49:47.000000 sqlUts-1.0.1/sqlUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 21:49:46.000000 sqlUts-1.0.1/sqlUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-22 21:49:46.000000 sqlUts-1.0.1/sqlUts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 21:49:46.000000 sqlUts-1.0.1/sqlUts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 21:51:17.650652 sqlUts-1.0.2/
+-rw-rw-rw-   0        0        0      387 2023-05-02 14:14:50.000000 sqlUts-1.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-05-02 14:14:50.000000 sqlUts-1.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-02 14:14:50.000000 sqlUts-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3658 2024-04-22 21:51:17.648649 sqlUts-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2679 2023-05-02 14:14:50.000000 sqlUts-1.0.2/README.md
+-rw-rw-rw-   0        0        0      214 2024-04-22 21:38:54.000000 sqlUts-1.0.2/commands.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 21:51:17.650652 sqlUts-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      845 2024-04-22 21:51:09.000000 sqlUts-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:51:17.584651 sqlUts-1.0.2/sqlUts/
+-rw-rw-rw-   0        0        0     1658 2024-04-22 21:49:39.000000 sqlUts-1.0.2/sqlUts/__init__.py
+-rw-rw-rw-   0        0        0       17 2024-04-22 21:49:19.000000 sqlUts-1.0.2/sqlUts/version.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:51:17.642651 sqlUts-1.0.2/sqlUts.egg-info/
+-rw-rw-rw-   0        0        0     3658 2024-04-22 21:51:16.000000 sqlUts-1.0.2/sqlUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-22 21:51:17.000000 sqlUts-1.0.2/sqlUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 21:51:16.000000 sqlUts-1.0.2/sqlUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-22 21:51:16.000000 sqlUts-1.0.2/sqlUts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 21:51:16.000000 sqlUts-1.0.2/sqlUts.egg-info/top_level.txt
```

### Comparing `sqlUts-1.0.1/LICENCE.txt` & `sqlUts-1.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `sqlUts-1.0.1/PKG-INFO` & `sqlUts-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlUts
-Version: 1.0.1
+Version: 1.0.2
 Summary: An orm package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: sqlUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sqlUts-1.0.1/README.md` & `sqlUts-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlUts-1.0.1/setup.py` & `sqlUts-1.0.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup, find_packages, Extension
-from sqlUts.version import version
 
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Education',
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='sqlUts',
-  version=version,
+  version='1.0.2',
   description='An orm package',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='',  
   author='Melque Lima',
   author_email='melque_ex@yahoo.com.br',
   license='MIT',
```

### Comparing `sqlUts-1.0.1/sqlUts/__init__.py` & `sqlUts-1.0.2/sqlUts/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlUts-1.0.1/sqlUts.egg-info/PKG-INFO` & `sqlUts-1.0.2/sqlUts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlUts
-Version: 1.0.1
+Version: 1.0.2
 Summary: An orm package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: sqlUts
 Classifier: Development Status :: 5 - Production/Stable
```

