# Comparing `tmp/EasyDataPy-1.3.tar.gz` & `tmp/easydatapy-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyDataPy-1.3.tar", last modified: Thu Feb 29 17:59:28 2024, max compression
+gzip compressed data, was "easydatapy-1.4.tar", last modified: Tue Apr 23 15:13:58 2024, max compression
```

## Comparing `EasyDataPy-1.3.tar` & `easydatapy-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 salehahmad  (1000) salehahmad  (1000)        0 2024-02-29 17:59:28.682008 EasyDataPy-1.3/
-drwxrwxr-x   0 salehahmad  (1000) salehahmad  (1000)        0 2024-02-29 17:59:28.682008 EasyDataPy-1.3/EasyDataPy/
--rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)     9551 2024-02-29 17:56:09.000000 EasyDataPy-1.3/EasyDataPy/EasyDataPy.py
--rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)       25 2024-01-03 17:19:24.000000 EasyDataPy-1.3/EasyDataPy/__init__.py
-drwxrwxr-x   0 salehahmad  (1000) salehahmad  (1000)        0 2024-02-29 17:59:28.682008 EasyDataPy-1.3/EasyDataPy.egg-info/
--rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)     3204 2024-02-29 17:59:28.000000 EasyDataPy-1.3/EasyDataPy.egg-info/PKG-INFO
--rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)      225 2024-02-29 17:59:28.000000 EasyDataPy-1.3/EasyDataPy.egg-info/SOURCES.txt
--rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)        1 2024-02-29 17:59:28.000000 EasyDataPy-1.3/EasyDataPy.egg-info/dependency_links.txt
--rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)       33 2024-02-29 17:59:28.000000 EasyDataPy-1.3/EasyDataPy.egg-info/requires.txt
--rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)       11 2024-02-29 17:59:28.000000 EasyDataPy-1.3/EasyDataPy.egg-info/top_level.txt
--rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)     3204 2024-02-29 17:59:28.682008 EasyDataPy-1.3/PKG-INFO
--rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)       38 2024-02-29 17:59:28.682008 EasyDataPy-1.3/setup.cfg
--rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)      941 2024-02-29 17:55:57.000000 EasyDataPy-1.3/setup.py
+drwxrwxr-x   0 salehahmad  (1000) salehahmad  (1000)        0 2024-04-23 15:13:58.443642 easydatapy-1.4/
+drwxrwxr-x   0 salehahmad  (1000) salehahmad  (1000)        0 2024-04-23 15:13:58.443642 easydatapy-1.4/EasyDataPy/
+-rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)     9554 2024-04-23 15:12:02.000000 easydatapy-1.4/EasyDataPy/EasyDataPy.py
+-rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)       25 2024-01-03 17:19:24.000000 easydatapy-1.4/EasyDataPy/__init__.py
+drwxrwxr-x   0 salehahmad  (1000) salehahmad  (1000)        0 2024-04-23 15:13:58.443642 easydatapy-1.4/EasyDataPy.egg-info/
+-rw-r--r--   0 salehahmad  (1000) salehahmad  (1000)     3297 2024-04-23 15:13:58.000000 easydatapy-1.4/EasyDataPy.egg-info/PKG-INFO
+-rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)      225 2024-04-23 15:13:58.000000 easydatapy-1.4/EasyDataPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)        1 2024-04-23 15:13:58.000000 easydatapy-1.4/EasyDataPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)       33 2024-04-23 15:13:58.000000 easydatapy-1.4/EasyDataPy.egg-info/requires.txt
+-rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)       11 2024-04-23 15:13:58.000000 easydatapy-1.4/EasyDataPy.egg-info/top_level.txt
+-rw-r--r--   0 salehahmad  (1000) salehahmad  (1000)     3297 2024-04-23 15:13:58.443642 easydatapy-1.4/PKG-INFO
+-rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)       38 2024-04-23 15:13:58.443642 easydatapy-1.4/setup.cfg
+-rw-rw-r--   0 salehahmad  (1000) salehahmad  (1000)      941 2024-04-23 15:13:42.000000 easydatapy-1.4/setup.py
```

### Comparing `EasyDataPy-1.3/EasyDataPy/EasyDataPy.py` & `easydatapy-1.4/EasyDataPy/EasyDataPy.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 # Example Usage
 
     # Pass the dataFrame downloaded through build_time_series function into this function:
 #plot_time_series(data_frame)
 
 
 # In[ ]:
-def download_dataset(series_ids, Easydata_key, start_date, end_date, file_type="csv"):
+def download_dataset(series_ids, start_date, end_date, file_type="csv"):
     """
     Download and combine multiple series into a DataFrame.
 
     Parameters
     ----------
     series_ids : list
         List of series IDs to download.
@@ -286,15 +286,15 @@
 
     for series_id in series_ids:
         try:
             # Construct the URL for the HTTP GET request
             url = f"https://easydata.sbp.org.pk/api/v1/series/{series_id}/data?api_key={Easydata_key}&start_date={start_date}&end_date={end_date}&format={file_type}"
 
             # Make the HTTP GET request and read data into DataFrame
-            df = pd.read_csv(url)
+            df = pd.read_csv(url,usecols=range(8))
             df["Series_ID"] = df.iloc[1][2]  # Add series ID as a column
             series_data.append(df)
 
             print(f"Downloaded data for Series ID: {series_id}")
 
         except Exception as e:
             print(f"Error downloading data for Series ID: {series_id}\n{e}")
```

### Comparing `EasyDataPy-1.3/EasyDataPy.egg-info/PKG-INFO` & `easydatapy-1.4/EasyDataPy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: EasyDataPy
-Version: 1.3
+Version: 1.4
 Summary: EasyDataPy through EasyData API key of State Bank of Pakistan helps to obtain information on and download a series of interest in Python for further analysis
 Author: Dr. Syed Ateeb Akhter Shah
 Author-email: syed.ateeb@wmich.edu
 Keywords: EasyData,EasyDataPy
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
+Requires-Dist: plotly
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: readme_md
 
 # EasyDataPy
 
 EasyDataPy aKa EDpy for short, is a unofficial Python library/package to read in data from EasyData platform of the State Bank of Pakistan
 
 # Details about EasyData Database of the State Bank of Pakistan
```

### Comparing `EasyDataPy-1.3/PKG-INFO` & `easydatapy-1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: EasyDataPy
-Version: 1.3
+Version: 1.4
 Summary: EasyDataPy through EasyData API key of State Bank of Pakistan helps to obtain information on and download a series of interest in Python for further analysis
 Author: Dr. Syed Ateeb Akhter Shah
 Author-email: syed.ateeb@wmich.edu
 Keywords: EasyData,EasyDataPy
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
+Requires-Dist: plotly
+Requires-Dist: pandas
+Requires-Dist: requests
+Requires-Dist: readme_md
 
 # EasyDataPy
 
 EasyDataPy aKa EDpy for short, is a unofficial Python library/package to read in data from EasyData platform of the State Bank of Pakistan
 
 # Details about EasyData Database of the State Bank of Pakistan
```

### Comparing `EasyDataPy-1.3/setup.py` & `easydatapy-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 long_description = Path('readme.md').read_text()
 print(long_description)
 
 setup(
     name='EasyDataPy',
-    version='1.3',
+    version='1.4',
     description='EasyDataPy through EasyData API key of State Bank of Pakistan helps to obtain information on and download a series of interest in Python for further analysis',
     long_description=long_description,
     author='Dr. Syed Ateeb Akhter Shah',
     author_email='syed.ateeb@wmich.edu',
     packages=['EasyDataPy'],
     install_requires=[
         'plotly',
```

