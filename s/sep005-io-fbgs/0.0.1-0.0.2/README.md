# Comparing `tmp/sep005_io_fbgs-0.0.1.tar.gz` & `tmp/sep005_io_fbgs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sep005_io_fbgs-0.0.1.tar", last modified: Wed Oct  4 10:12:45 2023, max compression
+gzip compressed data, was "sep005_io_fbgs-0.0.2.tar", last modified: Tue Apr 23 11:47:46 2024, max compression
```

## Comparing `sep005_io_fbgs-0.0.1.tar` & `sep005_io_fbgs-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 10:12:45.517040 sep005_io_fbgs-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-04 10:12:45.517040 sep005_io_fbgs-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-10-04 10:12:34.000000 sep005_io_fbgs-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 10:12:45.517040 sep005_io_fbgs-0.0.1/sep005_io_fbgs/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-04 10:12:34.000000 sep005_io_fbgs-0.0.1/sep005_io_fbgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2023-10-04 10:12:34.000000 sep005_io_fbgs-0.0.1/sep005_io_fbgs/fbgs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 10:12:45.517040 sep005_io_fbgs-0.0.1/sep005_io_fbgs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-04 10:12:45.000000 sep005_io_fbgs-0.0.1/sep005_io_fbgs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-04 10:12:45.000000 sep005_io_fbgs-0.0.1/sep005_io_fbgs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-04 10:12:45.000000 sep005_io_fbgs-0.0.1/sep005_io_fbgs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-04 10:12:45.000000 sep005_io_fbgs-0.0.1/sep005_io_fbgs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-04 10:12:45.517040 sep005_io_fbgs-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2023-10-04 10:12:34.000000 sep005_io_fbgs-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-04 10:12:45.517040 sep005_io_fbgs-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-10-04 10:12:34.000000 sep005_io_fbgs-0.0.1/tests/test_fbgs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:47:46.308539 sep005_io_fbgs-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-23 11:47:46.308539 sep005_io_fbgs-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-23 11:47:42.000000 sep005_io_fbgs-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:47:46.308539 sep005_io_fbgs-0.0.2/sep005_io_fbgs/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 11:47:42.000000 sep005_io_fbgs-0.0.2/sep005_io_fbgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-23 11:47:42.000000 sep005_io_fbgs-0.0.2/sep005_io_fbgs/fbgs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:47:46.308539 sep005_io_fbgs-0.0.2/sep005_io_fbgs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-23 11:47:46.000000 sep005_io_fbgs-0.0.2/sep005_io_fbgs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 11:47:46.000000 sep005_io_fbgs-0.0.2/sep005_io_fbgs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 11:47:46.000000 sep005_io_fbgs-0.0.2/sep005_io_fbgs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 11:47:46.000000 sep005_io_fbgs-0.0.2/sep005_io_fbgs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 11:47:46.308539 sep005_io_fbgs-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-23 11:47:42.000000 sep005_io_fbgs-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 11:47:46.308539 sep005_io_fbgs-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-23 11:47:42.000000 sep005_io_fbgs-0.0.2/tests/test_fbgs.py
```

### Comparing `sep005_io_fbgs-0.0.1/PKG-INFO` & `sep005_io_fbgs-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sep005_io_fbgs
-Version: 0.0.1
+Version: 0.0.2
 Summary: FBGS file read functions compliant with SDyPy SEP005
 Home-page: https://github.com/OWI-Lab
 Author: Wout Weijtjens
 Author-email: wout.weijtjens@vub.be
 Maintainer: Wout Weijtjens
 Maintainer-email: wout.weijtjens@vub.be
 License: MIT license
```

### Comparing `sep005_io_fbgs-0.0.1/README.rst` & `sep005_io_fbgs-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sep005_io_fbgs-0.0.1/sep005_io_fbgs/fbgs.py` & `sep005_io_fbgs-0.0.2/sep005_io_fbgs/fbgs.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,17 +17,18 @@
         """
         self.channels = channels # SEP005 compliant channel objects
         self.error_status = None
 
 
 
     @classmethod
-    def from_df(cls, df:pd.DataFrame, mode='engineering_units', dt_format='%Y-%m-%dT%H:%M:%S%z'):
+    def from_df(cls, df:pd.DataFrame, mode='engineering_units', dt_format='%Y-%m-%dT%H:%M:%S%z', qa:bool=True):
         """
         Import FBGS data from a dataframe
+
         """
         if mode == 'engineering_units' or mode == 'eu':
             pass # do Nothing
         elif mode == 'wavelength' or mode == 'wl':
             raise NotImplementedError(f'Data model (wavelength/wl) is not implemented')
         else:
             raise NotImplementedError(f'Data mode {mode} is not a valid option')
@@ -36,19 +37,32 @@
             error_status = df['Error status']
         else:
             error_status = None
 
         timestamp = datetime.datetime.strptime(df['Date'][0], dt_format)
 
         # FBGS data sometimes has a bad timestamping, e.g. only to second precision.
-        for idx, row in df.iterrows():
-            timestamp_i = datetime.datetime.strptime(row['Date'], dt_format)
-            if timestamp_i > timestamp:
-                fs = idx/(timestamp_i-timestamp).total_seconds()
-                break
+        dt_e = datetime.datetime.strptime(df['Date'].iloc[-1], dt_format).replace(microsecond=0) \
+                + datetime.timedelta(seconds=1) # Floor to the second then add 1
+        duration = (dt_e-timestamp).total_seconds()  # Due to the rounding to second precision this
+        fs = round(len(df)/duration, 2) # Assumption: Sampling frequency is defined up to 2 decimal points
+
+
+
+        if duration*fs != len(df):
+            warnings.warn(
+                f'QA: Inconsistent number of samples found ({len(df)}) for estimated sampling frequency of {fs},'
+                f' set qa to False if you want to still consider this file.',
+                UserWarning
+            )
+            if qa:
+                # Failed QA: Returning empty
+                return cls(channels=[], error_status=error_status)
+
+
 
         # Convert timestamp to UTC
         timestamp = timestamp.astimezone(utc)
 
         channels = []
         for c in df.columns:
             if c not in ['Date','Time', 'Linenumber', 'Error status']:
@@ -61,26 +75,27 @@
                     'unit_str':''
                 }
                 channels.append(channel)
 
         return cls(channels=channels, error_status=error_status)
 
 
-def read_fbgs(path: Union[str, Path]) -> list:
+def read_fbgs(path: Union[str, Path], qa:bool = True) -> list:
     """
     Primary function to read fbgs files based on path
 
+    qa : Quality assurance applied, rejecting files with a bad length. When set to False this check is skipped
 
     """
     if not os.path.isfile(path):
         warnings.warn('FAILED IMPORT: No FBGS file at: ' + path, UserWarning)
         signals = []
         return signals
 
     df = _open_fbgs_file(path, sep='\t')
-    fbg = FBG.from_df(df)
+    fbg = FBG.from_df(df, qa=qa)
 
     return fbg.channels
 
 def _open_fbgs_file(path: Union[str, Path], **kwargs) -> pd.DataFrame:
     df = pd.read_csv(path, **kwargs)
     return df
```

### Comparing `sep005_io_fbgs-0.0.1/sep005_io_fbgs.egg-info/PKG-INFO` & `sep005_io_fbgs-0.0.2/sep005_io_fbgs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sep005-io-fbgs
-Version: 0.0.1
+Name: sep005_io_fbgs
+Version: 0.0.2
 Summary: FBGS file read functions compliant with SDyPy SEP005
 Home-page: https://github.com/OWI-Lab
 Author: Wout Weijtjens
 Author-email: wout.weijtjens@vub.be
 Maintainer: Wout Weijtjens
 Maintainer-email: wout.weijtjens@vub.be
 License: MIT license
```

### Comparing `sep005_io_fbgs-0.0.1/setup.py` & `sep005_io_fbgs-0.0.2/setup.py`

 * *Files identical despite different names*

