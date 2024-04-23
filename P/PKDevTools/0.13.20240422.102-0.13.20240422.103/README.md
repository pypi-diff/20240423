# Comparing `tmp/PKDevTools-0.13.20240422.102.tar.gz` & `tmp/PKDevTools-0.13.20240422.103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240422.102.tar", last modified: Mon Apr 22 10:35:42 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240422.103.tar", last modified: Mon Apr 22 22:02:56 2024, max compression
```

## Comparing `PKDevTools-0.13.20240422.102.tar` & `PKDevTools-0.13.20240422.103.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 10:35:42.818467 PKDevTools-0.13.20240422.102/
--rw-rw-rw-   0        0        0     1086 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-22 10:35:42.802835 PKDevTools-0.13.20240422.102/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:35:42.818467 PKDevTools-0.13.20240422.102/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6380 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2534 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    13778 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5081 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0     9069 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-22 10:35:38.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:35:42.818467 PKDevTools-0.13.20240422.102/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-04-22 10:35:42.000000 PKDevTools-0.13.20240422.102/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2024-04-22 10:35:42.000000 PKDevTools-0.13.20240422.102/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 10:35:42.000000 PKDevTools-0.13.20240422.102/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-22 10:35:42.000000 PKDevTools-0.13.20240422.102/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 10:35:36.000000 PKDevTools-0.13.20240422.102/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-04-22 10:35:42.000000 PKDevTools-0.13.20240422.102/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-22 10:35:42.000000 PKDevTools-0.13.20240422.102/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-04-22 10:35:42.818467 PKDevTools-0.13.20240422.102/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/README.md
--rw-rw-rw-   0        0        0       86 2024-04-22 10:35:42.818467 PKDevTools-0.13.20240422.102/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-22 10:34:21.000000 PKDevTools-0.13.20240422.102/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 22:02:56.655359 PKDevTools-0.13.20240422.103/
+-rw-rw-rw-   0        0        0     1086 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-22 22:02:56.639738 PKDevTools-0.13.20240422.103/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 22:02:56.655359 PKDevTools-0.13.20240422.103/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6380 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2534 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    13778 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5081 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0     9417 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-22 22:02:51.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16118 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     5384 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-22 22:02:56.639738 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1122 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-22 22:02:49.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-04-22 22:02:56.655359 PKDevTools-0.13.20240422.103/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-22 22:02:56.655359 PKDevTools-0.13.20240422.103/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/setup.py
```

### Comparing `PKDevTools-0.13.20240422.102/LICENSE` & `PKDevTools-0.13.20240422.103/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/__init__.py` & `PKDevTools-0.13.20240422.103/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import pickle
 import warnings
 warnings.simplefilter("ignore", UserWarning)
 import logging
 import os
 import sys
 from queue import Empty
+from filelock import FileLock
 os.environ["PYTHONWARNINGS"]="ignore::UserWarning"
 import multiprocessing
 
 # usage: pkscreenercli.exe [-h] [-a ANSWERDEFAULT] [-c CRONINTERVAL] [-d] [-e] [-o OPTIONS] [-p] [-t] [-l] [-v]
 # pkscreenercli.exe: error: unrecognized arguments: --multiprocessing-fork parent_pid=4620 pipe_handle=708
 # https://github.com/pyinstaller/pyinstaller/wiki/Recipe-Multiprocessing
 # Module multiprocessing is organized differently in Python 3.4+
@@ -117,23 +118,27 @@
     def reloadDatabase(self):
         if self.refreshDatabase and isinstance(self.orig_objectDictionary,str):
             self.refreshDatabase = False
             # Looks like we got the filename instead of stock dictionary
             # Let's load the saved stocks' data
             cache_file = self.orig_objectDictionary
             try:
-                with open(os.path.join(Archiver.get_user_outputs_dir(), cache_file), "rb") as f:
-                    self.objectDictionary = pickle.load(f)
+                fileName = os.path.join(Archiver.get_user_outputs_dir(), f"{cache_file}")
+                with FileLock(f'{fileName}.lck'):
+                    with open(os.path.join(Archiver.get_user_outputs_dir(), cache_file), "rb") as f:
+                        self.objectDictionary = pickle.load(f)
             except:
                 self.objectDictionary = {}
                 pass
             try:
                 if "intraday" not in cache_file and self.configManager.calculatersiintraday:
-                    with open(os.path.join(Archiver.get_user_outputs_dir(), f"intraday_{cache_file}"), "rb") as f:
-                        self.secondaryObjectDictionary = pickle.load(f)
+                    fileName = os.path.join(Archiver.get_user_outputs_dir(), f"intraday_{cache_file}")
+                    with FileLock(f'{fileName}.lck'):
+                        with open(os.path.join(Archiver.get_user_outputs_dir(), f"intraday_{cache_file}"), "rb") as f:
+                            self.secondaryObjectDictionary = pickle.load(f)
                 else:
                     self.secondaryObjectDictionary = self.objectDictionary
             except:
                 self.secondaryObjectDictionary = {}
                 pass
 
     def run(self):
```

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240422.103/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240422.103/PKDevTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240422.102
+Version: 0.13.20240422.103
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240422.102.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240422.103.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240422.102/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240422.103/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/PKG-INFO` & `PKDevTools-0.13.20240422.103/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240422.102
+Version: 0.13.20240422.103
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240422.102.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240422.103.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240422.102/README.md` & `PKDevTools-0.13.20240422.103/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.102/setup.py` & `PKDevTools-0.13.20240422.103/setup.py`

 * *Files identical despite different names*

