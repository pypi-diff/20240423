# Comparing `tmp/PKDevTools-0.13.20240422.103.tar.gz` & `tmp/PKDevTools-0.13.20240423.104.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240422.103.tar", last modified: Mon Apr 22 22:02:56 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240423.104.tar", last modified: Tue Apr 23 08:00:40 2024, max compression
```

## Comparing `PKDevTools-0.13.20240422.103.tar` & `PKDevTools-0.13.20240423.104.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 22:02:56.655359 PKDevTools-0.13.20240422.103/
--rw-rw-rw-   0        0        0     1086 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-22 22:02:56.639738 PKDevTools-0.13.20240422.103/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 22:02:56.655359 PKDevTools-0.13.20240422.103/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6380 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2534 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    13778 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5081 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0     9417 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-22 22:02:51.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-22 22:02:56.639738 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-22 22:02:49.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-22 22:02:56.000000 PKDevTools-0.13.20240422.103/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-04-22 22:02:56.655359 PKDevTools-0.13.20240422.103/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/README.md
--rw-rw-rw-   0        0        0       86 2024-04-22 22:02:56.655359 PKDevTools-0.13.20240422.103/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-22 22:01:31.000000 PKDevTools-0.13.20240422.103/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:00:40.697316 PKDevTools-0.13.20240423.104/
+-rw-rw-rw-   0        0        0     1086 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-23 08:00:40.681700 PKDevTools-0.13.20240423.104/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:00:40.697316 PKDevTools-0.13.20240423.104/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6380 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2534 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    13778 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5081 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0     9625 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-23 08:00:36.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16118 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     5384 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:00:40.697316 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1122 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 08:00:34.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-04-23 08:00:40.697316 PKDevTools-0.13.20240423.104/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-23 08:00:40.697316 PKDevTools-0.13.20240423.104/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/setup.py
```

### Comparing `PKDevTools-0.13.20240422.103/LICENSE` & `PKDevTools-0.13.20240423.104/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/__init__.py` & `PKDevTools-0.13.20240423.104/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,22 +53,25 @@
     def __init__(
         self,
         processorMethod,
         task_queue,
         result_queue,
         processingCounter,
         processingResultsCounter,
-        objectDictionary,
+        objectDictionaryPrimary,
+        objectDictionarySecondary,
         proxyServer,
         keyboardInterruptEvent,
         defaultLogger,
         fetcher=None,
         configManager=None,
         candlePatterns=None,
         screener=None,
+        dbFileNamePrimary=None,
+        dbFileNameSecondary=None,
         stockList=None,
         dataCallbackHandler=None,
         progressCallbackHandler=None,
     ):
         multiprocessing.Process.__init__(self)
         self.multiprocessingForWindows()
         assert (
@@ -81,20 +84,21 @@
         self.result_queue = result_queue
         # processingCounter and processingResultsCounter
         # are sunchronized counters that can be used within
         # processorMethod via hostRef.processingCounter
         # or hostRef.processingResultsCounter
         self.processingCounter = processingCounter
         self.processingResultsCounter = processingResultsCounter
+        self.dbFileNamePrimary = dbFileNamePrimary
+        self.dbFileNameSecondary = dbFileNameSecondary
         # A helper object dictionary that can contain anything
         # and can be accessed using hostRef.objectDictionary
         # within processorMethod
-        self.objectDictionary = objectDictionary
-        self.orig_objectDictionary = objectDictionary
-        self.secondaryObjectDictionary = objectDictionary
+        self.objectDictionaryPrimary = objectDictionaryPrimary
+        self.objectDictionarySecondary = objectDictionarySecondary
         # A proxyServer that can contain proxyServer info
         # and can be accessed using hostRef.proxyServer
         # within processorMethod
         self.proxyServer = proxyServer
         # A logger that can contain logger reference
         # and can be accessed using hostRef.default_logger
         # within processorMethod
@@ -112,37 +116,37 @@
         self.fetcher = fetcher
         self.configManager = configManager
         self.candlePatterns = candlePatterns
         self.screener = screener
         self.refreshDatabase = True
 
     def reloadDatabase(self):
-        if self.refreshDatabase and isinstance(self.orig_objectDictionary,str):
+        if self.refreshDatabase and self.dbFileNamePrimary is not None:
             self.refreshDatabase = False
             # Looks like we got the filename instead of stock dictionary
             # Let's load the saved stocks' data
-            cache_file = self.orig_objectDictionary
+            cache_file_primary = self.dbFileNamePrimary
             try:
-                fileName = os.path.join(Archiver.get_user_outputs_dir(), f"{cache_file}")
+                fileName = os.path.join(Archiver.get_user_outputs_dir(), f"{cache_file_primary}")
                 with FileLock(f'{fileName}.lck'):
-                    with open(os.path.join(Archiver.get_user_outputs_dir(), cache_file), "rb") as f:
-                        self.objectDictionary = pickle.load(f)
+                    with open(os.path.join(Archiver.get_user_outputs_dir(), cache_file_primary), "rb") as f:
+                        self.objectDictionaryPrimary = pickle.load(f)
             except:
-                self.objectDictionary = {}
+                self.objectDictionaryPrimary = multiprocessing.Manager().dict()
                 pass
+        if self.refreshDatabase and self.dbFileNameSecondary is not None:
             try:
-                if "intraday" not in cache_file and self.configManager.calculatersiintraday:
-                    fileName = os.path.join(Archiver.get_user_outputs_dir(), f"intraday_{cache_file}")
-                    with FileLock(f'{fileName}.lck'):
-                        with open(os.path.join(Archiver.get_user_outputs_dir(), f"intraday_{cache_file}"), "rb") as f:
-                            self.secondaryObjectDictionary = pickle.load(f)
-                else:
-                    self.secondaryObjectDictionary = self.objectDictionary
+                cache_file_secondary = self.dbFileNameSecondary
+                fileName = os.path.join(Archiver.get_user_outputs_dir(), f"{cache_file_secondary}")
+                with FileLock(f'{fileName}.lck'):
+                    with open(os.path.join(Archiver.get_user_outputs_dir(), f"{cache_file_secondary}"), "rb") as f:
+                        self.objectDictionarySecondary = pickle.load(f)
+
             except:
-                self.secondaryObjectDictionary = {}
+                self.objectDictionarySecondary = multiprocessing.Manager().dict()
                 pass
 
     def run(self):
         try:
             while not self.keyboardInterruptEvent.is_set():
                 try:
                     if self.refreshDatabase:
```

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240423.104/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240423.104/PKDevTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240422.103
+Version: 0.13.20240423.104
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240422.103.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240423.104.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240422.103/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240423.104/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/PKG-INFO` & `PKDevTools-0.13.20240423.104/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240422.103
+Version: 0.13.20240423.104
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240422.103.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240423.104.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240422.103/README.md` & `PKDevTools-0.13.20240423.104/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240422.103/setup.py` & `PKDevTools-0.13.20240423.104/setup.py`

 * *Files identical despite different names*

