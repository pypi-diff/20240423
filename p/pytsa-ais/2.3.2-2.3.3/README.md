# Comparing `tmp/pytsa_ais-2.3.2.tar.gz` & `tmp/pytsa_ais-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytsa_ais-2.3.2.tar", max compression
+gzip compressed data, was "pytsa_ais-2.3.3.tar", max compression
```

## Comparing `pytsa_ais-2.3.2.tar` & `pytsa_ais-2.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35130 2024-02-02 12:50:18.000000 pytsa_ais-2.3.2/LICENSE
--rw-r--r--   0        0        0    15713 2024-04-12 09:18:41.000000 pytsa_ais-2.3.2/README.md
--rw-r--r--   0        0        0      952 2024-04-23 07:40:02.244003 pytsa_ais-2.3.2/pyproject.toml
--rw-r--r--   0        0        0      415 2024-04-23 07:40:07.960003 pytsa_ais-2.3.2/pytsa/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:27:45.000000 pytsa_ais-2.3.2/pytsa/data/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 15:27:34.000000 pytsa_ais-2.3.2/pytsa/data/geometry/__init__.py
--rw-r--r--   0        0        0   188008 2024-02-02 15:12:30.000000 pytsa_ais-2.3.2/pytsa/data/geometry/denmark.json
--rw-r--r--   0        0        0   177598 2024-02-02 15:12:30.000000 pytsa_ais-2.3.2/pytsa/data/geometry/germany.json
--rw-r--r--   0        0        0   431855 2024-02-02 15:12:30.000000 pytsa_ais-2.3.2/pytsa/data/geometry/netherlands_detailed.json
--rw-r--r--   0        0        0  1727337 2024-02-02 15:12:30.000000 pytsa_ais-2.3.2/pytsa/data/geometry/norway.json
--rw-r--r--   0        0        0  1026703 2024-02-02 15:12:30.000000 pytsa_ais-2.3.2/pytsa/data/geometry/sweden.json
--rw-r--r--   0        0        0        0 2023-12-06 13:21:15.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/__init__.py
--rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/diffquants.pkl
--rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/dquants.pkl
--rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/squants.pkl
--rw-r--r--   0        0        0    80168 2024-04-22 06:01:35.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/tquants.pkl
--rw-r--r--   0        0        0    80168 2024-04-22 06:01:35.000000 pytsa_ais-2.3.2/pytsa/data/quantiles/trquants.pkl
--rw-r--r--   0        0        0      119 2024-03-11 08:08:58.000000 pytsa_ais-2.3.2/pytsa/decoder/__init__.py
--rw-r--r--   0        0        0     7229 2024-03-11 08:05:09.000000 pytsa_ais-2.3.2/pytsa/decoder/ais_decoder.py
--rw-r--r--   0        0        0     1548 2024-04-19 11:16:21.000000 pytsa_ais-2.3.2/pytsa/decoder/filedescriptor.py
--rw-r--r--   0        0        0     2170 2024-02-05 10:42:29.000000 pytsa_ais-2.3.2/pytsa/logger.py
--rw-r--r--   0        0        0     6472 2024-04-19 11:52:30.000000 pytsa_ais-2.3.2/pytsa/structs.py
--rw-r--r--   0        0        0       71 2024-02-06 07:57:43.000000 pytsa_ais-2.3.2/pytsa/trajectories/__init__.py
--rw-r--r--   0        0        0     9694 2024-04-19 08:41:02.000000 pytsa_ais-2.3.2/pytsa/trajectories/inspect.py
--rw-r--r--   0        0        0     5813 2024-04-15 11:06:38.000000 pytsa_ais-2.3.2/pytsa/trajectories/rules.py
--rw-r--r--   0        0        0      673 2023-11-16 08:49:43.000000 pytsa_ais-2.3.2/pytsa/tsea/__init__.py
--rw-r--r--   0        0        0    29053 2024-04-23 07:39:41.352004 pytsa_ais-2.3.2/pytsa/tsea/search_agent.py
--rw-r--r--   0        0        0     8204 2024-04-23 07:05:46.236046 pytsa_ais-2.3.2/pytsa/tsea/split.py
--rw-r--r--   0        0        0    15089 2024-03-27 13:02:29.244484 pytsa_ais-2.3.2/pytsa/tsea/targetship.py
--rw-r--r--   0        0        0    14189 2024-04-19 11:22:56.000000 pytsa_ais-2.3.2/pytsa/utils.py
--rw-r--r--   0        0        0     2162 2024-02-05 11:00:57.000000 pytsa_ais-2.3.2/pytsa/visualization/__init__.py
--rw-r--r--   0        0        0     7950 2024-02-06 07:04:35.000000 pytsa_ais-2.3.2/pytsa/visualization/ecdf.py
--rw-r--r--   0        0        0    15336 2024-04-15 13:35:43.000000 pytsa_ais-2.3.2/pytsa/visualization/misc.py
--rw-r--r--   0        0        0    16726 1970-01-01 00:00:00.000000 pytsa_ais-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0    35130 2024-02-02 12:50:18.000000 pytsa_ais-2.3.3/LICENSE
+-rw-r--r--   0        0        0    15713 2024-04-12 09:18:41.000000 pytsa_ais-2.3.3/README.md
+-rw-r--r--   0        0        0      952 2024-04-23 08:26:33.511946 pytsa_ais-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0      415 2024-04-23 08:26:38.695946 pytsa_ais-2.3.3/pytsa/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:27:45.000000 pytsa_ais-2.3.3/pytsa/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 15:27:34.000000 pytsa_ais-2.3.3/pytsa/data/geometry/__init__.py
+-rw-r--r--   0        0        0   188008 2024-02-02 15:12:30.000000 pytsa_ais-2.3.3/pytsa/data/geometry/denmark.json
+-rw-r--r--   0        0        0   177598 2024-02-02 15:12:30.000000 pytsa_ais-2.3.3/pytsa/data/geometry/germany.json
+-rw-r--r--   0        0        0   431855 2024-02-02 15:12:30.000000 pytsa_ais-2.3.3/pytsa/data/geometry/netherlands_detailed.json
+-rw-r--r--   0        0        0  1727337 2024-02-02 15:12:30.000000 pytsa_ais-2.3.3/pytsa/data/geometry/norway.json
+-rw-r--r--   0        0        0  1026703 2024-02-02 15:12:30.000000 pytsa_ais-2.3.3/pytsa/data/geometry/sweden.json
+-rw-r--r--   0        0        0        0 2023-12-06 13:21:15.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/__init__.py
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/diffquants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/dquants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:34.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/squants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:35.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/tquants.pkl
+-rw-r--r--   0        0        0    80168 2024-04-22 06:01:35.000000 pytsa_ais-2.3.3/pytsa/data/quantiles/trquants.pkl
+-rw-r--r--   0        0        0      119 2024-03-11 08:08:58.000000 pytsa_ais-2.3.3/pytsa/decoder/__init__.py
+-rw-r--r--   0        0        0     7229 2024-03-11 08:05:09.000000 pytsa_ais-2.3.3/pytsa/decoder/ais_decoder.py
+-rw-r--r--   0        0        0     1548 2024-04-19 11:16:21.000000 pytsa_ais-2.3.3/pytsa/decoder/filedescriptor.py
+-rw-r--r--   0        0        0     2170 2024-02-05 10:42:29.000000 pytsa_ais-2.3.3/pytsa/logger.py
+-rw-r--r--   0        0        0     6472 2024-04-19 11:52:30.000000 pytsa_ais-2.3.3/pytsa/structs.py
+-rw-r--r--   0        0        0       71 2024-02-06 07:57:43.000000 pytsa_ais-2.3.3/pytsa/trajectories/__init__.py
+-rw-r--r--   0        0        0     9694 2024-04-19 08:41:02.000000 pytsa_ais-2.3.3/pytsa/trajectories/inspect.py
+-rw-r--r--   0        0        0     5813 2024-04-15 11:06:38.000000 pytsa_ais-2.3.3/pytsa/trajectories/rules.py
+-rw-r--r--   0        0        0      673 2023-11-16 08:49:43.000000 pytsa_ais-2.3.3/pytsa/tsea/__init__.py
+-rw-r--r--   0        0        0    29053 2024-04-23 07:39:41.352004 pytsa_ais-2.3.3/pytsa/tsea/search_agent.py
+-rw-r--r--   0        0        0     8323 2024-04-23 08:23:14.755950 pytsa_ais-2.3.3/pytsa/tsea/split.py
+-rw-r--r--   0        0        0    15089 2024-03-27 13:02:29.244484 pytsa_ais-2.3.3/pytsa/tsea/targetship.py
+-rw-r--r--   0        0        0    14189 2024-04-19 11:22:56.000000 pytsa_ais-2.3.3/pytsa/utils.py
+-rw-r--r--   0        0        0     2162 2024-02-05 11:00:57.000000 pytsa_ais-2.3.3/pytsa/visualization/__init__.py
+-rw-r--r--   0        0        0     7950 2024-02-06 07:04:35.000000 pytsa_ais-2.3.3/pytsa/visualization/ecdf.py
+-rw-r--r--   0        0        0    15336 2024-04-15 13:35:43.000000 pytsa_ais-2.3.3/pytsa/visualization/misc.py
+-rw-r--r--   0        0        0    16726 1970-01-01 00:00:00.000000 pytsa_ais-2.3.3/PKG-INFO
```

### Comparing `pytsa_ais-2.3.2/LICENSE` & `pytsa_ais-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/README.md` & `pytsa_ais-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pyproject.toml` & `pytsa_ais-2.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytsa-ais"
-version = "2.3.2"
+version = "2.3.3"
 description = "Toolbox for extracting trajectories and monitoring vessels from raw AIS records."
 authors = ["Niklas Paulig <niklas.paulig@tu-dresden.de>"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pytsa_ais-2.3.2/pytsa/data/geometry/denmark.json` & `pytsa_ais-2.3.3/pytsa/data/geometry/denmark.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/data/geometry/germany.json` & `pytsa_ais-2.3.3/pytsa/data/geometry/germany.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/data/geometry/netherlands_detailed.json` & `pytsa_ais-2.3.3/pytsa/data/geometry/netherlands_detailed.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/data/geometry/norway.json` & `pytsa_ais-2.3.3/pytsa/data/geometry/norway.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/data/geometry/sweden.json` & `pytsa_ais-2.3.3/pytsa/data/geometry/sweden.json`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/data/quantiles/diffquants.pkl` & `pytsa_ais-2.3.3/pytsa/data/quantiles/diffquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/data/quantiles/dquants.pkl` & `pytsa_ais-2.3.3/pytsa/data/quantiles/dquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/data/quantiles/squants.pkl` & `pytsa_ais-2.3.3/pytsa/data/quantiles/squants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/data/quantiles/tquants.pkl` & `pytsa_ais-2.3.3/pytsa/data/quantiles/tquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/data/quantiles/trquants.pkl` & `pytsa_ais-2.3.3/pytsa/data/quantiles/trquants.pkl`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/decoder/ais_decoder.py` & `pytsa_ais-2.3.3/pytsa/decoder/ais_decoder.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/decoder/filedescriptor.py` & `pytsa_ais-2.3.3/pytsa/decoder/filedescriptor.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/logger.py` & `pytsa_ais-2.3.3/pytsa/logger.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/structs.py` & `pytsa_ais-2.3.3/pytsa/structs.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/trajectories/inspect.py` & `pytsa_ais-2.3.3/pytsa/trajectories/inspect.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/trajectories/rules.py` & `pytsa_ais-2.3.3/pytsa/trajectories/rules.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/tsea/__init__.py` & `pytsa_ais-2.3.3/pytsa/tsea/__init__.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/tsea/search_agent.py` & `pytsa_ais-2.3.3/pytsa/tsea/search_agent.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/tsea/split.py` & `pytsa_ais-2.3.3/pytsa/tsea/split.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,18 @@
     _TQUANTILES = pickle.load(f)
     
 # Convert quantiles to dictionaries
 # with the quantile as key and the
 # quantile value as value. 
 # ==================================
 _NQ = 10001 # Number of quantiles
-_QVALUES = np.linspace(0,100,_NQ) # Quantile values
+# We have to round the quantiles to
+# avoid floating point errors when using
+# them as keys in dictionaries.
+_QVALUES = np.round(np.linspace(0,1,_NQ),4) # Quantile values
 # Empirical quantiles for the
 # turning rate [°/s] between two 
 # consecutive messages.
 TRQUANTILES = {_QVALUES[k]: _TRQUANTILES[k] for k in range(_NQ)}
 
 # Empirical quantiles for the
 # change in speed [kn] between two
```

### Comparing `pytsa_ais-2.3.2/pytsa/tsea/targetship.py` & `pytsa_ais-2.3.3/pytsa/tsea/targetship.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/utils.py` & `pytsa_ais-2.3.3/pytsa/utils.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/visualization/__init__.py` & `pytsa_ais-2.3.3/pytsa/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/visualization/ecdf.py` & `pytsa_ais-2.3.3/pytsa/visualization/ecdf.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/pytsa/visualization/misc.py` & `pytsa_ais-2.3.3/pytsa/visualization/misc.py`

 * *Files identical despite different names*

### Comparing `pytsa_ais-2.3.2/PKG-INFO` & `pytsa_ais-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytsa-ais
-Version: 2.3.2
+Version: 2.3.3
 Summary: Toolbox for extracting trajectories and monitoring vessels from raw AIS records.
 Author: Niklas Paulig
 Author-email: niklas.paulig@tu-dresden.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

