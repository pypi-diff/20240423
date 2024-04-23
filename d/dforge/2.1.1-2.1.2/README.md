# Comparing `tmp/dforge-2.1.1.tar.gz` & `tmp/dforge-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dforge-2.1.1.tar", last modified: Mon Apr 22 08:59:25 2024, max compression
+gzip compressed data, was "dforge-2.1.2.tar", last modified: Tue Apr 23 08:03:05 2024, max compression
```

## Comparing `dforge-2.1.1.tar` & `dforge-2.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 08:59:25.331423 dforge-2.1.1/
--rw-rw-rw-   0        0        0    35823 2024-04-02 14:56:57.000000 dforge-2.1.1/LICENSE
--rw-rw-rw-   0        0        0     3286 2024-04-22 08:59:25.331423 dforge-2.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 08:59:25.292762 dforge-2.1.1/dforge/
--rw-rw-rw-   0        0        0       57 2024-04-13 09:40:54.000000 dforge-2.1.1/dforge/__init__.py
--rw-rw-rw-   0        0        0    26688 2024-04-22 08:20:09.000000 dforge-2.1.1/dforge/core.py
--rw-rw-rw-   0        0        0     2373 2024-04-10 09:39:04.000000 dforge-2.1.1/dforge/plotData.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:59:25.331423 dforge-2.1.1/dforge.egg-info/
--rw-rw-rw-   0        0        0     3286 2024-04-22 08:59:25.000000 dforge-2.1.1/dforge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-22 08:59:25.000000 dforge-2.1.1/dforge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 08:59:25.000000 dforge-2.1.1/dforge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-22 08:59:25.000000 dforge-2.1.1/dforge.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 08:59:25.000000 dforge-2.1.1/dforge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 08:59:25.335428 dforge-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      779 2024-04-22 08:56:26.000000 dforge-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:03:05.040460 dforge-2.1.2/
+-rw-rw-rw-   0        0        0    35823 2024-04-02 14:56:57.000000 dforge-2.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3286 2024-04-23 08:03:05.040460 dforge-2.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 08:03:05.014443 dforge-2.1.2/dforge/
+-rw-rw-rw-   0        0        0       57 2024-04-13 09:40:54.000000 dforge-2.1.2/dforge/__init__.py
+-rw-rw-rw-   0        0        0    27667 2024-04-23 08:01:44.000000 dforge-2.1.2/dforge/core.py
+-rw-rw-rw-   0        0        0     2373 2024-04-10 09:39:04.000000 dforge-2.1.2/dforge/plotData.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:03:05.039479 dforge-2.1.2/dforge.egg-info/
+-rw-rw-rw-   0        0        0     3286 2024-04-23 08:03:04.000000 dforge-2.1.2/dforge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-23 08:03:04.000000 dforge-2.1.2/dforge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:03:04.000000 dforge-2.1.2/dforge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-23 08:03:04.000000 dforge-2.1.2/dforge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 08:03:04.000000 dforge-2.1.2/dforge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:03:05.041461 dforge-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      779 2024-04-23 08:02:58.000000 dforge-2.1.2/setup.py
```

### Comparing `dforge-2.1.1/LICENSE` & `dforge-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dforge-2.1.1/PKG-INFO` & `dforge-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dforge
-Version: 2.1.1
+Version: 2.1.2
 Summary: A package for efortless data manager.
 Home-page: https://github.com/LuizaRusnac/dforge.git
 Author: Luiza Rusnac
 Author-email: luiza.rusnac93@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dforge-2.1.1/dforge/core.py` & `dforge-2.1.2/dforge/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -176,14 +176,32 @@
     def show_columns(self, columns_name):
         """ Method for printing the specified columns
 
         Args: 
             columns_name (str or list of str): Column names to be showing
         """
         print(self.dataframe[columns_name])
+    
+    def save_data(self, filename, file_extension='csv', **kwargs):
+        """ Method for saving dataframe on supported formats.
+
+        Args:
+            filename (str): The filename for the saved dataframe.
+            file_extention (str): The desired file extension. Supported files: ['csv', 'xlsx', 'xls', 'json', 'parquet', 'feather', 'pickle'].
+                Optional. Default = 'csv'
+        """
+        supported_extensions = ['csv', 'xlsx', 'xls', 'json', 'parquet', 'feather', 'pickle']
+        
+        if file_extension in supported_extensions:
+            file_extension = 'excel' if file_extension == 'xlsx' or file_extension == 'xls' else file_extension
+            read_function = getattr(pd, f"to_{file_extension}")
+            self.dataframe = read_function(filename, **kwargs)
+        else:
+            raise ValueError("Unsupported file extension. Supported extensions are: {}".format(', '.join(supported_extensions)))
+
 
 class PDNumPro(PDBuilder):
     """
     A class for performing numeric analysis on Pandas DataFrames.
 
     This class extends the functionality of CreateDataPD class and provides additional methods 
     for numeric analysis, data transformation, and visualization.
@@ -523,8 +541,10 @@
         Args:
             nr_folds (int): Number of folds.
             label_column (str): The name of label columns for creating the folds.
         """
         skf = StratifiedKFold(n_splits=nr_folds, shuffle=True, random_state=42) 
         self.dataframe["fold"] = -1  
         for fold, (train_idx, val_idx) in enumerate(skf.split(self.dataframe, self.dataframe[label_column])):
-            self.dataframe.loc[val_idx, 'fold'] = fold
+            self.dataframe.loc[val_idx, 'fold'] = fold
+
+
```

### Comparing `dforge-2.1.1/dforge/plotData.py` & `dforge-2.1.2/dforge/plotData.py`

 * *Files identical despite different names*

### Comparing `dforge-2.1.1/dforge.egg-info/PKG-INFO` & `dforge-2.1.2/dforge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dforge
-Version: 2.1.1
+Version: 2.1.2
 Summary: A package for efortless data manager.
 Home-page: https://github.com/LuizaRusnac/dforge.git
 Author: Luiza Rusnac
 Author-email: luiza.rusnac93@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dforge-2.1.1/setup.py` & `dforge-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dforge',
-    version='2.1.1',
+    version='2.1.2',
     packages=find_packages(),
     author='Luiza Rusnac',
     author_email='luiza.rusnac93@gmail.com',
     description='A package for efortless data manager.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/LuizaRusnac/dforge.git',
```

