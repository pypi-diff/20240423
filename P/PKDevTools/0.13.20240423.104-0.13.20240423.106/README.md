# Comparing `tmp/PKDevTools-0.13.20240423.104.tar.gz` & `tmp/PKDevTools-0.13.20240423.106.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240423.104.tar", last modified: Tue Apr 23 08:00:40 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240423.106.tar", last modified: Tue Apr 23 17:46:42 2024, max compression
```

## Comparing `PKDevTools-0.13.20240423.104.tar` & `PKDevTools-0.13.20240423.106.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 08:00:40.697316 PKDevTools-0.13.20240423.104/
--rw-rw-rw-   0        0        0     1086 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-23 08:00:40.681700 PKDevTools-0.13.20240423.104/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:00:40.697316 PKDevTools-0.13.20240423.104/PKDevTools/classes/
--rw-rw-rw-   0        0        0     3402 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6380 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11963 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     2534 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    13778 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5081 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0     9625 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     1916 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-23 08:00:36.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16118 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     5384 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:00:40.697316 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 08:00:34.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      176 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-23 08:00:40.000000 PKDevTools-0.13.20240423.104/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-04-23 08:00:40.697316 PKDevTools-0.13.20240423.104/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/README.md
--rw-rw-rw-   0        0        0       86 2024-04-23 08:00:40.697316 PKDevTools-0.13.20240423.104/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-04-23 07:58:50.000000 PKDevTools-0.13.20240423.104/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:46:42.033310 PKDevTools-0.13.20240423.106/
+-rw-rw-rw-   0        0        0     1086 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-23 17:46:42.017094 PKDevTools-0.13.20240423.106/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:46:42.033310 PKDevTools-0.13.20240423.106/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     3402 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6380 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11963 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     2534 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    13778 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5081 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    10832 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     1916 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-23 17:46:37.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:46:42.017094 PKDevTools-0.13.20240423.106/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-04-23 17:46:41.000000 PKDevTools-0.13.20240423.106/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1122 2024-04-23 17:46:41.000000 PKDevTools-0.13.20240423.106/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 17:46:41.000000 PKDevTools-0.13.20240423.106/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-04-23 17:46:41.000000 PKDevTools-0.13.20240423.106/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 17:46:35.000000 PKDevTools-0.13.20240423.106/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      176 2024-04-23 17:46:41.000000 PKDevTools-0.13.20240423.106/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-23 17:46:41.000000 PKDevTools-0.13.20240423.106/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-04-23 17:46:42.033310 PKDevTools-0.13.20240423.106/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-23 17:46:42.033310 PKDevTools-0.13.20240423.106/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-04-23 17:45:36.000000 PKDevTools-0.13.20240423.106/setup.py
```

### Comparing `PKDevTools-0.13.20240423.104/LICENSE` & `PKDevTools-0.13.20240423.106/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/__init__.py` & `PKDevTools-0.13.20240423.106/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,23 +42,24 @@
     if sys.platform.startswith("win"):
         import multiprocessing.popen_spawn_win32 as forking
     else:
         import multiprocessing.popen_fork as forking
 except ImportError:
     print("Contact developer! Your platform does not support multiprocessing!")
 
-from PKDevTools.classes.log import default_logger
+from PKDevTools.classes.multiprocessing_logging import SubProcessLogHandler
 from PKDevTools.classes import Archiver
 
 class PKMultiProcessorClient(multiprocessing.Process):
     def __init__(
         self,
         processorMethod,
         task_queue,
         result_queue,
+        logging_queue,
         processingCounter,
         processingResultsCounter,
         objectDictionaryPrimary,
         objectDictionarySecondary,
         proxyServer,
         keyboardInterruptEvent,
         defaultLogger,
@@ -78,14 +79,15 @@
             processorMethod is not None
         ), "processorMethod argument must not be None. This is the meyhod that will do the processing."
         assert task_queue is not None, "task_queue argument must not be None."
         assert (result_queue is not None or dataCallbackHandler is not None), "result_queue or dataCallbackHandler argument must not be None."
         self.processorMethod = processorMethod
         self.task_queue = task_queue
         self.result_queue = result_queue
+        self.logging_queue = logging_queue
         # processingCounter and processingResultsCounter
         # are sunchronized counters that can be used within
         # processorMethod via hostRef.processingCounter
         # or hostRef.processingResultsCounter
         self.processingCounter = processingCounter
         self.processingResultsCounter = processingResultsCounter
         self.dbFileNamePrimary = dbFileNamePrimary
@@ -98,32 +100,55 @@
         # A proxyServer that can contain proxyServer info
         # and can be accessed using hostRef.proxyServer
         # within processorMethod
         self.proxyServer = proxyServer
         # A logger that can contain logger reference
         # and can be accessed using hostRef.default_logger
         # within processorMethod
-        self.default_logger = defaultLogger
+        self.default_logger = None
+        self.logLevel = defaultLogger.level
 
         self.keyboardInterruptEvent = keyboardInterruptEvent
-        if defaultLogger is not None:
-            self.default_logger.info("PKMultiProcessorClient initialized.")
-        else:
-            # Let's get the root logger by default
-            self.default_logger = logging.getLogger(name=None)
         self.stockList = stockList
         self.dataCallbackHandler = dataCallbackHandler
         self.progressCallbackHandler = progressCallbackHandler
         self.fetcher = fetcher
         self.configManager = configManager
         self.candlePatterns = candlePatterns
         self.screener = screener
         self.refreshDatabase = True
 
-    def reloadDatabase(self):
+    def _setupLogger(self):
+        # create the logger to use.
+        logger = logging.getLogger('PKDevTools.subprocess')
+        # The only handler desired is the SubProcessLogHandler.  If any others
+        # exist, remove them. In this case, on Unix and Linux the StreamHandler
+        # will be inherited.
+
+        for handler in logger.handlers:
+            # just a check for my sanity
+            assert not isinstance(handler, SubProcessLogHandler)
+            logger.removeHandler(handler)
+        # add the handler
+        handler = SubProcessLogHandler(self.logging_queue)
+        formatter = logging.Formatter(
+            fmt="\n%(asctime)s - %(name)s - %(levelname)s - %(filename)s - %(module)s - %(funcName)s - %(lineno)d\n%(message)s\n"
+        )
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
+
+        # On Windows, the level will not be inherited.  Also, we could just
+        # set the level to log everything here and filter it in the main
+        # process handlers.  For now, just set it from the global default.
+        logger.setLevel(self.logLevel)
+        self.default_logger = logger
+        if self.default_logger is not None:
+            self.default_logger.info("PKMultiProcessorClient initialized.")
+
+    def _reloadDatabase(self):
         if self.refreshDatabase and self.dbFileNamePrimary is not None:
             self.refreshDatabase = False
             # Looks like we got the filename instead of stock dictionary
             # Let's load the saved stocks' data
             cache_file_primary = self.dbFileNamePrimary
             try:
                 fileName = os.path.join(Archiver.get_user_outputs_dir(), f"{cache_file_primary}")
@@ -143,20 +168,21 @@
 
             except:
                 self.objectDictionarySecondary = multiprocessing.Manager().dict()
                 pass
 
     def run(self):
         try:
+            self._setupLogger()
             while not self.keyboardInterruptEvent.is_set():
                 try:
                     if self.refreshDatabase:
                         # Maybe the database pickle file changed/re-saved.
                         # We'd need to reload again
-                        self.reloadDatabase()
+                        self._reloadDatabase()
 
                     next_task = None
                     answer = None
                     if self.task_queue is not None:
                         next_task = self.task_queue.get()
                         if next_task is not None:
                             # Inject a reference to this instance of the client
```

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import time
 import warnings
 # from inspect import getcallargs, getfullargspec
 from collections import OrderedDict
 from functools import wraps
 from PKDevTools.classes.Singleton import SingletonType
 from threading import get_ident
+import threading
 
 try:
     from collections.abc import Iterable
 except ImportError:
     from collections import Iterable
 
 from itertools import *
```

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/multiprocessing_logging.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,14 +35,78 @@
 
 try:
     from queue import Empty
 except ImportError:  # Python 2.
     from Queue import Empty  # type: ignore[no-redef]
 __version__ = "0.3.4"
 
+class SubProcessLogHandler(logging.Handler):
+    """handler used by subprocesses
+
+    It simply puts items on a Queue for the main process to log.
+
+    """
+
+    def __init__(self, queue):
+        logging.Handler.__init__(self)
+        self.queue = queue
+
+    def emit(self, record):
+        self.queue.put_nowait(self._format_record(record))
+
+    def _format_record(self, record):
+        # ensure that exc_info and args
+        # have been stringified. Removes any chance of
+        # unpickleable things inside and possibly reduces
+        # message size sent over the pipe.
+        if record.args:
+            record.msg = record.msg % record.args
+            record.args = None
+        if record.exc_info:
+            self.format(record)
+            record.exc_info = None
+
+        return record
+    
+class LogQueueReader(threading.Thread):
+    """thread to write subprocesses log records to main process log
+
+    This thread reads the records written by subprocesses and writes them to
+    the handlers defined in the main process's handlers.
+
+    """
+
+    def __init__(self, queue):
+        threading.Thread.__init__(self)
+        self.queue = queue
+        self.daemon = True
+
+    def run(self):
+        """read from the queue and write to the log handlers
+
+        The logging documentation says logging is thread safe, so there
+        shouldn't be contention between normal logging (from the main
+        process) and this thread.
+
+        Note that we're using the name of the original logger.
+
+        """
+        while True:
+            try:
+                record = self.queue.get()
+                # get the logger for this record
+                logger = logging.getLogger(record.name)
+                logger.callHandlers(record)
+            except (KeyboardInterrupt, SystemExit):
+                raise
+            except EOFError:
+                break
+            except:
+                import traceback, sys
+                traceback.print_exc(file=sys.stderr)
 
 def install_mp_handler(logger=None):
     """Wraps the handlers in the given Logger with an MultiProcessingHandler.
 
     :param logger: whose handlers to wrap. By default, the root logger.
     """
     if logger is None:
```

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240423.106/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240423.106/PKDevTools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240423.104
+Version: 0.13.20240423.106
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240423.104.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240423.106.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240423.104/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240423.106/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/PKG-INFO` & `PKDevTools-0.13.20240423.106/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240423.104
+Version: 0.13.20240423.106
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240423.104.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240423.106.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240423.104/README.md` & `PKDevTools-0.13.20240423.106/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240423.104/setup.py` & `PKDevTools-0.13.20240423.106/setup.py`

 * *Files identical despite different names*

