# Comparing `tmp/dforge-1.0.0.tar.gz` & `tmp/dforge-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dforge-1.0.0.tar", last modified: Sat Apr 13 10:02:04 2024, max compression
+gzip compressed data, was "dforge-2.1.1.tar", last modified: Mon Apr 22 08:59:25 2024, max compression
```

## Comparing `dforge-1.0.0.tar` & `dforge-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 10:02:04.132129 dforge-1.0.0/
--rw-rw-rw-   0        0        0    35823 2024-04-02 14:56:57.000000 dforge-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3286 2024-04-13 10:02:04.132129 dforge-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 10:02:04.084126 dforge-1.0.0/dforge/
--rw-rw-rw-   0        0        0       57 2024-04-13 09:40:54.000000 dforge-1.0.0/dforge/__init__.py
--rw-rw-rw-   0        0        0    24945 2024-04-13 09:39:35.000000 dforge-1.0.0/dforge/core.py
--rw-rw-rw-   0        0        0     2373 2024-04-10 09:39:04.000000 dforge-1.0.0/dforge/plotData.py
-drwxrwxrwx   0        0        0        0 2024-04-13 10:02:04.128125 dforge-1.0.0/dforge.egg-info/
--rw-rw-rw-   0        0        0     3286 2024-04-13 10:02:03.000000 dforge-1.0.0/dforge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-13 10:02:03.000000 dforge-1.0.0/dforge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 10:02:03.000000 dforge-1.0.0/dforge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-13 10:02:03.000000 dforge-1.0.0/dforge.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-13 10:02:03.000000 dforge-1.0.0/dforge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 10:02:04.132129 dforge-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      779 2024-04-13 09:50:55.000000 dforge-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:59:25.331423 dforge-2.1.1/
+-rw-rw-rw-   0        0        0    35823 2024-04-02 14:56:57.000000 dforge-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3286 2024-04-22 08:59:25.331423 dforge-2.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 08:59:25.292762 dforge-2.1.1/dforge/
+-rw-rw-rw-   0        0        0       57 2024-04-13 09:40:54.000000 dforge-2.1.1/dforge/__init__.py
+-rw-rw-rw-   0        0        0    26688 2024-04-22 08:20:09.000000 dforge-2.1.1/dforge/core.py
+-rw-rw-rw-   0        0        0     2373 2024-04-10 09:39:04.000000 dforge-2.1.1/dforge/plotData.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:59:25.331423 dforge-2.1.1/dforge.egg-info/
+-rw-rw-rw-   0        0        0     3286 2024-04-22 08:59:25.000000 dforge-2.1.1/dforge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-22 08:59:25.000000 dforge-2.1.1/dforge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 08:59:25.000000 dforge-2.1.1/dforge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-22 08:59:25.000000 dforge-2.1.1/dforge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 08:59:25.000000 dforge-2.1.1/dforge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 08:59:25.335428 dforge-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      779 2024-04-22 08:56:26.000000 dforge-2.1.1/setup.py
```

### Comparing `dforge-1.0.0/LICENSE` & `dforge-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dforge-1.0.0/PKG-INFO` & `dforge-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dforge
-Version: 1.0.0
+Version: 2.1.1
 Summary: A package for efortless data manager.
 Home-page: https://github.com/LuizaRusnac/dforge.git
 Author: Luiza Rusnac
 Author-email: luiza.rusnac93@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dforge-1.0.0/dforge/core.py` & `dforge-2.1.1/dforge/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 import numpy as np
 import random
 import math
+from tabulate import tabulate
 from dforge.plotData import CustomPlot
 from sklearn.model_selection import StratifiedKFold
 
 class PDBuilder:
     """  A class used to create a Pandas DataFrame with the possibility of reading from a file.
     
     This class provides a convenient way to create Pandas DataFrames by specifying columns and values,
@@ -303,14 +304,46 @@
                 'maxim': self.dataframe[column_name].max(),
                 'unique_values': self.dataframe[column_name].unique(),
                 'histogram': {'hist': hist, 'bins': bins},
                 'None_values': {'nr_values': self.dataframe[column_name].isna().sum(),
                                 'idxs': pd.Index(self.dataframe[column_name]).get_indexer_for(self.dataframe[column_name][self.dataframe[column_name].isna()])}
             }
         return stats_dict
+    
+    def show_numeric_columns_statistics(self, column_names='Numeric'):
+        """ Method computing columns statistics and show it in table.
+
+        Args:
+            column_names (str or list of str): Default is 'Numeric' and is computing the
+                statistics for all numeric columns and show in a table. Can be computed for
+                a column as string or for multiple columns as list of strings. If the column
+                given is not a numeric one, a warrning will be shown.
+        """
+        if column_names == 'Numeric':
+            column_names = self.find_numeric_columns()  
+
+        statistics = []
+        if isinstance(column_names, str):
+            column_names = [column_names] 
+
+        if isinstance(column_names, list):
+            for column in column_names:
+                if pd.api.types.is_numeric_dtype(self.dataframe[column]):
+                    columns_statistics = self.column_statistics(column)
+                    statistics.append([column, round(columns_statistics['mean'], 2),
+                                    round(columns_statistics['std'], 2), 
+                                    round(columns_statistics['minim'], 2),
+                                    round(columns_statistics['maxim'], 2)])
+                else:
+                    print(f"\033[93mWarrning: The column '{column}' contains non-numeric data and statistics cannot be computed.\033[0m")
+        else:
+            raise TypeError("column_names must be either string or list")
+
+        table_header = ['MEAN', 'STD', 'MIN', 'MAX']
+        print(tabulate(statistics, headers=table_header, tablefmt='fancy_grid', numalign='right'))
 
     def plot_histogram(self, column_name, **kwargs):
         """ Method for plotting the histogram of a column
 
         Args:
             column_name (str): The name of the column to plot hystogram
         """
@@ -435,15 +468,15 @@
         If this method is called, the dictionary will be populated with changes that were made for the column.
 
         Args:
             column_name (str): The name of the column to be changed to numeric
             overwrite (bool): If True, the column will be overwrite, otherwise, a new column will be creaded with {column_name}_numeric. (Optional)
         """
         unique_values = self.dataframe[column_name].unique()
-        self.dictionary[column_name] = {"values": unique_values, "number_values": list(range(len(unique_values)))}
+        self.dictionary_discretized_data[column_name] = {"values": unique_values, "number_values": list(range(len(unique_values)))}
         mapping = {value: index for index, value in enumerate(unique_values)}
         self.dataframe[column_name] = self.dataframe[column_name].map(mapping) if overwrite else self.dataframe[f"{column_name}_numeric"]
 
     def non_numeric_columns_to_numeric(self, overwrite=True):
         """ Method for changing all the non-numeric columns to numeric ones.
 
         Args:
```

### Comparing `dforge-1.0.0/dforge/plotData.py` & `dforge-2.1.1/dforge/plotData.py`

 * *Files identical despite different names*

### Comparing `dforge-1.0.0/dforge.egg-info/PKG-INFO` & `dforge-2.1.1/dforge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dforge
-Version: 1.0.0
+Version: 2.1.1
 Summary: A package for efortless data manager.
 Home-page: https://github.com/LuizaRusnac/dforge.git
 Author: Luiza Rusnac
 Author-email: luiza.rusnac93@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dforge-1.0.0/setup.py` & `dforge-2.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dforge',
-    version='1.0.0',
+    version='2.1.1',
     packages=find_packages(),
     author='Luiza Rusnac',
     author_email='luiza.rusnac93@gmail.com',
     description='A package for efortless data manager.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/LuizaRusnac/dforge.git',
```

