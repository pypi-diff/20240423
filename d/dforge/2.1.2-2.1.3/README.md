# Comparing `tmp/dforge-2.1.2.tar.gz` & `tmp/dforge-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dforge-2.1.2.tar", last modified: Tue Apr 23 08:03:05 2024, max compression
+gzip compressed data, was "dforge-2.1.3.tar", last modified: Tue Apr 23 08:19:09 2024, max compression
```

## Comparing `dforge-2.1.2.tar` & `dforge-2.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 08:03:05.040460 dforge-2.1.2/
--rw-rw-rw-   0        0        0    35823 2024-04-02 14:56:57.000000 dforge-2.1.2/LICENSE
--rw-rw-rw-   0        0        0     3286 2024-04-23 08:03:05.040460 dforge-2.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-23 08:03:05.014443 dforge-2.1.2/dforge/
--rw-rw-rw-   0        0        0       57 2024-04-13 09:40:54.000000 dforge-2.1.2/dforge/__init__.py
--rw-rw-rw-   0        0        0    27667 2024-04-23 08:01:44.000000 dforge-2.1.2/dforge/core.py
--rw-rw-rw-   0        0        0     2373 2024-04-10 09:39:04.000000 dforge-2.1.2/dforge/plotData.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:03:05.039479 dforge-2.1.2/dforge.egg-info/
--rw-rw-rw-   0        0        0     3286 2024-04-23 08:03:04.000000 dforge-2.1.2/dforge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-23 08:03:04.000000 dforge-2.1.2/dforge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:03:04.000000 dforge-2.1.2/dforge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-23 08:03:04.000000 dforge-2.1.2/dforge.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-23 08:03:04.000000 dforge-2.1.2/dforge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 08:03:05.041461 dforge-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      779 2024-04-23 08:02:58.000000 dforge-2.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:19:09.129608 dforge-2.1.3/
+-rw-rw-rw-   0        0        0    35823 2024-04-02 14:56:57.000000 dforge-2.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3286 2024-04-23 08:19:09.128617 dforge-2.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 08:19:09.095595 dforge-2.1.3/dforge/
+-rw-rw-rw-   0        0        0       57 2024-04-13 09:40:54.000000 dforge-2.1.3/dforge/__init__.py
+-rw-rw-rw-   0        0        0    27662 2024-04-23 08:18:31.000000 dforge-2.1.3/dforge/core.py
+-rw-rw-rw-   0        0        0     2373 2024-04-10 09:39:04.000000 dforge-2.1.3/dforge/plotData.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:19:09.126603 dforge-2.1.3/dforge.egg-info/
+-rw-rw-rw-   0        0        0     3286 2024-04-23 08:19:09.000000 dforge-2.1.3/dforge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-23 08:19:09.000000 dforge-2.1.3/dforge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:19:09.000000 dforge-2.1.3/dforge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-23 08:19:09.000000 dforge-2.1.3/dforge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 08:19:09.000000 dforge-2.1.3/dforge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:19:09.129608 dforge-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-04-23 08:19:04.000000 dforge-2.1.3/setup.py
```

### Comparing `dforge-2.1.2/LICENSE` & `dforge-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dforge-2.1.2/PKG-INFO` & `dforge-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dforge
-Version: 2.1.2
+Version: 2.1.3
 Summary: A package for efortless data manager.
 Home-page: https://github.com/LuizaRusnac/dforge.git
 Author: Luiza Rusnac
 Author-email: luiza.rusnac93@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dforge-2.1.2/dforge/core.py` & `dforge-2.1.3/dforge/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,16 +189,16 @@
             file_extention (str): The desired file extension. Supported files: ['csv', 'xlsx', 'xls', 'json', 'parquet', 'feather', 'pickle'].
                 Optional. Default = 'csv'
         """
         supported_extensions = ['csv', 'xlsx', 'xls', 'json', 'parquet', 'feather', 'pickle']
         
         if file_extension in supported_extensions:
             file_extension = 'excel' if file_extension == 'xlsx' or file_extension == 'xls' else file_extension
-            read_function = getattr(pd, f"to_{file_extension}")
-            self.dataframe = read_function(filename, **kwargs)
+            save_function = getattr(self.dataframe, f"to_{file_extension}")
+            save_function(filename, **kwargs)
         else:
             raise ValueError("Unsupported file extension. Supported extensions are: {}".format(', '.join(supported_extensions)))
 
 
 class PDNumPro(PDBuilder):
     """
     A class for performing numeric analysis on Pandas DataFrames.
```

### Comparing `dforge-2.1.2/dforge/plotData.py` & `dforge-2.1.3/dforge/plotData.py`

 * *Files identical despite different names*

### Comparing `dforge-2.1.2/dforge.egg-info/PKG-INFO` & `dforge-2.1.3/dforge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dforge
-Version: 2.1.2
+Version: 2.1.3
 Summary: A package for efortless data manager.
 Home-page: https://github.com/LuizaRusnac/dforge.git
 Author: Luiza Rusnac
 Author-email: luiza.rusnac93@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dforge-2.1.2/setup.py` & `dforge-2.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dforge',
-    version='2.1.2',
+    version='2.1.3',
     packages=find_packages(),
     author='Luiza Rusnac',
     author_email='luiza.rusnac93@gmail.com',
     description='A package for efortless data manager.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/LuizaRusnac/dforge.git',
@@ -18,9 +18,10 @@
     ],
     python_requires='>=3.6',
     install_requires=[
         'matplotlib',
         'numpy',
         'pandas',
         'scikit-learn',
+        'tabulate',
     ],
 )
```

