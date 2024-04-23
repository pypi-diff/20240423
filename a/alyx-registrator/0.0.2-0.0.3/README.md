# Comparing `tmp/alyx_registrator-0.0.2.tar.gz` & `tmp/alyx_registrator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alyx_registrator-0.0.2.tar", last modified: Fri Apr  5 00:50:05 2024, max compression
+gzip compressed data, was "alyx_registrator-0.0.3.tar", last modified: Tue Apr 23 09:49:27 2024, max compression
```

## Comparing `alyx_registrator-0.0.2.tar` & `alyx_registrator-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6234 2024-04-05 00:49:56.033694 alyx_registrator-0.0.2/one_registrator/README.md
--rw-r--r--   0        0        0       51 2024-04-05 00:49:56.033694 alyx_registrator-0.0.2/one_registrator/__init__.py
--rw-r--r--   0        0        0    28212 2024-04-05 00:49:56.037694 alyx_registrator-0.0.2/one_registrator/registration.py
--rw-r--r--   0        0        0     9845 2024-04-05 00:49:56.037694 alyx_registrator-0.0.2/one_registrator/rules.json
--rw-r--r--   0        0        0     2904 2024-04-05 00:49:56.037694 alyx_registrator-0.0.2/one_registrator/utils.py
--rw-r--r--   0        0        0      660 2024-04-05 00:50:05.969614 alyx_registrator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 alyx_registrator-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6234 2024-04-23 09:49:18.258678 alyx_registrator-0.0.3/one_registrator/README.md
+-rw-r--r--   0        0        0       51 2024-04-23 09:49:18.258678 alyx_registrator-0.0.3/one_registrator/__init__.py
+-rw-r--r--   0        0        0    28212 2024-04-23 09:49:18.262678 alyx_registrator-0.0.3/one_registrator/registration.py
+-rw-r--r--   0        0        0    11125 2024-04-23 09:49:18.262678 alyx_registrator-0.0.3/one_registrator/rules.json
+-rw-r--r--   0        0        0     2904 2024-04-23 09:49:18.262678 alyx_registrator-0.0.3/one_registrator/utils.py
+-rw-r--r--   0        0        0      660 2024-04-23 09:49:27.506533 alyx_registrator-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      342 1970-01-01 00:00:00.000000 alyx_registrator-0.0.3/PKG-INFO
```

### Comparing `alyx_registrator-0.0.2/one_registrator/README.md` & `alyx_registrator-0.0.3/one_registrator/README.md`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.2/one_registrator/registration.py` & `alyx_registrator-0.0.3/one_registrator/registration.py`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.2/one_registrator/rules.json` & `alyx_registrator-0.0.3/one_registrator/rules.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9235714285714286%*

 * *Differences: {"'excluded_folders'": "{insert: [(4, 'screenshots'), (5, 'trash'), (6, 'draft'), (7, 'scratch'), "*

 * *                       "(8, 'Fiji_analysis'), (9, 'fiji_analysis'), (10, 'fijianalysis'), (11, "*

 * *                       "'Fiji_Analysis'), (12, 'FijiAnalysis'), (13, 'fijiAnalysis')]}",*

 * * "'re_patterns'": "{'FOV_NO': '^.*(?:FOV)|(?:fieldOfView)[-_ \\\\.]*?(\\\\d+).*$'}"}*

```diff
@@ -8,20 +8,30 @@
         "session_meta.json",
         "pipelines_arguments.json"
     ],
     "excluded_folders": [
         "figures",
         "preprocessing_saves",
         "screen_captures",
-        "suite2p"
+        "suite2p",
+        "screenshots",
+        "trash",
+        "draft",
+        "scratch",
+        "Fiji_analysis",
+        "fiji_analysis",
+        "fijianalysis",
+        "Fiji_Analysis",
+        "FijiAnalysis",
+        "fijiAnalysis"
     ],
     "re_patterns": {
         "ALYX_PATH_EID": "\\w+(?:\\|/)\\d{4}\\-\\d{2}\\-\\d{2}(?:\\|/)\\d{3}",
         "CONDENSED_DATE": ".*?(20\\d{4,6}).*?",
-        "FOV_NO": "^.*FOV.*?(\\d+).*$",
+        "FOV_NO": "^.*(?:FOV)|(?:fieldOfView)[-_ \\.]*?(\\d+).*$",
         "IOI_WHISKER": "^([a-zA-Z0-9]+)",
         "IOI_WITH_VERSIONS": ".*_[vV]\\d",
         "SESSION_NO": ".*?20\\d{4,6}_(\\d).*?",
         "TDMS_TRIALS_TABLE_TIME": "(\\d{4}_\\d{2}_\\d{2}_\\d{2}_\\d{2})\\.tdms$",
         "TDMS_VIDEO_TRIAL_NO": ".*?(\\d+)\\.tdms$",
         "TIFF_FRAME_NO": ".*(\\d{5})\\.tiff?$",
         "VGAT_MOUSE_NO": "Vgat.*?(\\d{1,3}).*jRGECO"
```

### Comparing `alyx_registrator-0.0.2/one_registrator/utils.py` & `alyx_registrator-0.0.3/one_registrator/utils.py`

 * *Files identical despite different names*

### Comparing `alyx_registrator-0.0.2/pyproject.toml` & `alyx_registrator-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 dependencies = [
     "numpy>=1.23",
     "alyx-connector>=1.16",
     "pandas>=1.4",
 ]
 requires-python = ">=3.11"
 dynamic = []
-version = "0.0.2"
+version = "0.0.3"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
```

