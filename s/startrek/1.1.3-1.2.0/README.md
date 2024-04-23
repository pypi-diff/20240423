# Comparing `tmp/startrek-1.1.3.tar.gz` & `tmp/startrek-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/startrek-1.1.3.tar", last modified: Fri Apr 12 10:36:07 2024, max compression
+gzip compressed data, was "dist/startrek-1.2.0.tar", last modified: Tue Apr 23 09:02:34 2024, max compression
```

## Comparing `startrek-1.1.3.tar` & `startrek-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/
--rw-r--r--   0 moky       (501) staff       (20)      449 2024-04-12 10:36:07.000000 startrek-1.1.3/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       25 2021-05-06 07:15:56.000000 startrek-1.1.3/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-12 10:36:07.000000 startrek-1.1.3/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      826 2024-03-13 14:44:36.000000 startrek-1.1.3/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/
--rw-r--r--   0 moky       (501) staff       (20)     2520 2023-01-13 11:45:48.000000 startrek-1.1.3/startrek/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5463 2024-03-06 13:31:40.000000 startrek-1.1.3/startrek/arrival.py
--rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-06 13:32:13.000000 startrek-1.1.3/startrek/departure.py
--rw-r--r--   0 moky       (501) staff       (20)     4960 2024-03-06 13:33:03.000000 startrek-1.1.3/startrek/dock.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/fsm/
--rw-r--r--   0 moky       (501) staff       (20)     2056 2023-01-13 04:48:09.000000 startrek-1.1.3/startrek/fsm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2301 2024-02-26 16:17:15.000000 startrek-1.1.3/startrek/fsm/auto.py
--rw-r--r--   0 moky       (501) staff       (20)     8897 2024-03-06 13:23:59.000000 startrek-1.1.3/startrek/fsm/base.py
--rw-r--r--   0 moky       (501) staff       (20)     5808 2024-03-06 10:33:56.000000 startrek-1.1.3/startrek/fsm/machine.py
--rw-r--r--   0 moky       (501) staff       (20)     5449 2024-02-26 14:47:40.000000 startrek-1.1.3/startrek/fsm/runner.py
--rw-r--r--   0 moky       (501) staff       (20)     4506 2024-03-07 09:23:03.000000 startrek-1.1.3/startrek/fsm/ticker.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/net/
--rw-r--r--   0 moky       (501) staff       (20)     3283 2023-01-13 11:39:06.000000 startrek-1.1.3/startrek/net/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     8734 2024-03-13 09:27:10.000000 startrek-1.1.3/startrek/net/channel.py
--rw-r--r--   0 moky       (501) staff       (20)     3366 2024-03-13 09:14:10.000000 startrek-1.1.3/startrek/net/connection.py
--rw-r--r--   0 moky       (501) staff       (20)     3380 2024-03-06 08:44:28.000000 startrek-1.1.3/startrek/net/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     3867 2024-03-06 08:47:09.000000 startrek-1.1.3/startrek/net/hub.py
--rw-r--r--   0 moky       (501) staff       (20)    17022 2024-03-06 16:02:35.000000 startrek-1.1.3/startrek/net/state.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/port/
--rw-r--r--   0 moky       (501) staff       (20)     3722 2024-03-06 09:27:29.000000 startrek-1.1.3/startrek/port/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3100 2024-03-06 14:33:53.000000 startrek-1.1.3/startrek/port/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     4412 2024-03-13 09:17:53.000000 startrek-1.1.3/startrek/port/docker.py
--rw-r--r--   0 moky       (501) staff       (20)     2619 2024-01-26 17:39:19.000000 startrek-1.1.3/startrek/port/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     4127 2024-03-06 09:27:29.000000 startrek-1.1.3/startrek/port/ship.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/socket/
--rw-r--r--   0 moky       (501) staff       (20)     1899 2024-03-06 13:22:07.000000 startrek-1.1.3/startrek/socket/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4283 2024-03-14 10:29:49.000000 startrek-1.1.3/startrek/socket/active_conn.py
--rw-r--r--   0 moky       (501) staff       (20)    10666 2024-03-13 15:37:34.000000 startrek-1.1.3/startrek/socket/base_channel.py
--rw-r--r--   0 moky       (501) staff       (20)    10445 2024-03-13 14:50:15.000000 startrek-1.1.3/startrek/socket/base_conn.py
--rw-r--r--   0 moky       (501) staff       (20)     9744 2024-03-13 09:20:18.000000 startrek-1.1.3/startrek/socket/base_hub.py
--rw-r--r--   0 moky       (501) staff       (20)    10723 2024-03-13 14:50:40.000000 startrek-1.1.3/startrek/stardocker.py
--rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-13 09:51:25.000000 startrek-1.1.3/startrek/stargate.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek/types/
--rw-r--r--   0 moky       (501) staff       (20)     1678 2024-03-06 07:44:45.000000 startrek-1.1.3/startrek/types/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7196 2024-03-06 10:36:46.000000 startrek-1.1.3/startrek/types/mapping.py
--rw-r--r--   0 moky       (501) staff       (20)     3721 2024-03-08 06:09:38.000000 startrek-1.1.3/startrek/types/pair.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      449 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      894 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)        9 2024-04-12 10:36:07.000000 startrek-1.1.3/startrek.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/
+-rw-r--r--   0 moky       (501) staff       (20)      449 2024-04-23 09:02:34.000000 startrek-1.2.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       25 2021-05-06 07:15:56.000000 startrek-1.2.0/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-23 09:02:34.000000 startrek-1.2.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      826 2024-04-23 08:26:41.000000 startrek-1.2.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/
+-rw-r--r--   0 moky       (501) staff       (20)     2520 2023-01-13 11:45:48.000000 startrek-1.2.0/startrek/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5463 2024-03-06 13:31:40.000000 startrek-1.2.0/startrek/arrival.py
+-rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-06 13:32:13.000000 startrek-1.2.0/startrek/departure.py
+-rw-r--r--   0 moky       (501) staff       (20)     4960 2024-03-06 13:33:03.000000 startrek-1.2.0/startrek/dock.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/fsm/
+-rw-r--r--   0 moky       (501) staff       (20)     2056 2023-01-13 04:48:09.000000 startrek-1.2.0/startrek/fsm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2301 2024-02-26 16:17:15.000000 startrek-1.2.0/startrek/fsm/auto.py
+-rw-r--r--   0 moky       (501) staff       (20)     8897 2024-03-06 13:23:59.000000 startrek-1.2.0/startrek/fsm/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     5808 2024-03-06 10:33:56.000000 startrek-1.2.0/startrek/fsm/machine.py
+-rw-r--r--   0 moky       (501) staff       (20)     5794 2024-04-23 08:23:46.000000 startrek-1.2.0/startrek/fsm/runner.py
+-rw-r--r--   0 moky       (501) staff       (20)     4517 2024-04-23 08:26:09.000000 startrek-1.2.0/startrek/fsm/ticker.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/net/
+-rw-r--r--   0 moky       (501) staff       (20)     3283 2023-01-13 11:39:06.000000 startrek-1.2.0/startrek/net/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     8734 2024-03-13 09:27:10.000000 startrek-1.2.0/startrek/net/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)     3366 2024-03-13 09:14:10.000000 startrek-1.2.0/startrek/net/connection.py
+-rw-r--r--   0 moky       (501) staff       (20)     3380 2024-03-06 08:44:28.000000 startrek-1.2.0/startrek/net/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     3867 2024-03-06 08:47:09.000000 startrek-1.2.0/startrek/net/hub.py
+-rw-r--r--   0 moky       (501) staff       (20)    17022 2024-03-06 16:02:35.000000 startrek-1.2.0/startrek/net/state.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/port/
+-rw-r--r--   0 moky       (501) staff       (20)     3722 2024-03-06 09:27:29.000000 startrek-1.2.0/startrek/port/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3100 2024-03-06 14:33:53.000000 startrek-1.2.0/startrek/port/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4412 2024-03-13 09:17:53.000000 startrek-1.2.0/startrek/port/docker.py
+-rw-r--r--   0 moky       (501) staff       (20)     2619 2024-01-26 17:39:19.000000 startrek-1.2.0/startrek/port/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4127 2024-03-06 09:27:29.000000 startrek-1.2.0/startrek/port/ship.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/socket/
+-rw-r--r--   0 moky       (501) staff       (20)     1899 2024-03-06 13:22:07.000000 startrek-1.2.0/startrek/socket/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4358 2024-04-23 08:25:49.000000 startrek-1.2.0/startrek/socket/active_conn.py
+-rw-r--r--   0 moky       (501) staff       (20)    10666 2024-03-13 15:37:34.000000 startrek-1.2.0/startrek/socket/base_channel.py
+-rw-r--r--   0 moky       (501) staff       (20)    10445 2024-03-13 14:50:15.000000 startrek-1.2.0/startrek/socket/base_conn.py
+-rw-r--r--   0 moky       (501) staff       (20)     9754 2024-04-22 17:47:17.000000 startrek-1.2.0/startrek/socket/base_hub.py
+-rw-r--r--   0 moky       (501) staff       (20)    10723 2024-03-13 14:50:40.000000 startrek-1.2.0/startrek/stardocker.py
+-rw-r--r--   0 moky       (501) staff       (20)    11435 2024-04-22 17:47:32.000000 startrek-1.2.0/startrek/stargate.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek/types/
+-rw-r--r--   0 moky       (501) staff       (20)     1678 2024-03-06 07:44:45.000000 startrek-1.2.0/startrek/types/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7196 2024-03-06 10:36:46.000000 startrek-1.2.0/startrek/types/mapping.py
+-rw-r--r--   0 moky       (501) staff       (20)     3721 2024-03-08 06:09:38.000000 startrek-1.2.0/startrek/types/pair.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      449 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      894 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)        9 2024-04-23 09:02:34.000000 startrek-1.2.0/startrek.egg-info/top_level.txt
```

### Comparing `startrek-1.1.3/setup.py` & `startrek-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~~~~~~~
 
     Interstellar Transport
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '1.1.3'
+__version__ = '1.2.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
```

### Comparing `startrek-1.1.3/startrek/__init__.py` & `startrek-1.2.0/startrek/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/arrival.py` & `startrek-1.2.0/startrek/arrival.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/departure.py` & `startrek-1.2.0/startrek/departure.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/dock.py` & `startrek-1.2.0/startrek/dock.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/fsm/__init__.py` & `startrek-1.2.0/startrek/fsm/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/fsm/auto.py` & `startrek-1.2.0/startrek/fsm/auto.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/fsm/base.py` & `startrek-1.2.0/startrek/fsm/base.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/fsm/machine.py` & `startrek-1.2.0/startrek/fsm/machine.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/fsm/runner.py` & `startrek-1.2.0/startrek/fsm/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 import time
+import weakref
 from abc import ABC, abstractmethod
 from threading import Thread
 from typing import Optional
 
 
 class Processor(ABC):
 
@@ -149,46 +150,58 @@
     """
         Daemon Thread
         ~~~~~~~~~~~~~
         The main thread won't wait the daemon threads exit
         when daemonic = True
     """
 
-    def __init__(self, target, daemonic: bool = True):
+    def __init__(self, target: Runnable, daemonic: bool = True):
         super().__init__()
-        self.__target = target  # Callable
+        self.__target = weakref.ref(target)  # Callable
         self.__daemon = daemonic
         self.__thread: Optional[Thread] = None
 
+    @property  # private
+    def target(self) -> Optional[Runnable]:
+        ref = self.__target
+        if ref is not None:
+            return ref()
+
     @property
     def alive(self) -> bool:
         thr = self.__thread
         if thr is not None:
             return thr.is_alive()
 
     def start(self):
         self.__force_stop()
-        thr = Thread(target=self.__target, daemon=self.__daemon)
-        thr.start()
-        self.__thread = thr
+        target = self.target
+        if target is not None:
+            thr = Thread(target=target.run, daemon=self.__daemon)
+            thr.start()
+            self.__thread = thr
 
     def stop(self):
         self.__force_stop()
 
+    def __del__(self):
+        self.__force_stop()
+
     def __force_stop(self):
         thr = self.__thread
         if thr is not None:
             self.__thread = None
             self._join(thr=thr)
 
     def _join(self, thr: Thread):
         # Waits at most seconds for this thread to die.
         # A timeout of 0 means to wait forever.
         self.join(thr=thr, timeout=1.0)
 
     @classmethod
     def join(cls, thr: Thread, timeout: float = None):
         try:
-            thr.join(timeout=timeout)
+            if thr.is_alive():
+                thr.join(timeout=timeout)
         except RuntimeError as error:
             print('[ERROR] failed to join thread: %s, timeout: %d' % (error, timeout))
             # traceback.print_exc()
```

### Comparing `startrek-1.1.3/startrek/fsm/ticker.py` & `startrek-1.2.0/startrek/fsm/ticker.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     # at least wait 1/60 of a second
     MIN_INTERVAL = 1.0/60
 
     def __init__(self, interval: float):
         super().__init__(interval=interval)
         self.__last_time = 0
-        self.__daemon = Daemon(target=self.run)
+        self.__daemon = Daemon(target=self)
         self.__lock = threading.Lock()
         self.__tickers = WeakSet()
 
     # Override
     def setup(self):
         super().setup()
         self.__last_time = time.time()
@@ -107,14 +107,15 @@
     def remove_ticker(self, ticker: Ticker):
         with self.__lock:
             self.__tickers.discard(ticker)
 
     def start(self):
         self.__daemon.start()
 
+    # Override
     def stop(self):
         super().stop()
         self.__daemon.stop()
 
 
 #
 #   Singleton for Prime Metronome
```

### Comparing `startrek-1.1.3/startrek/net/__init__.py` & `startrek-1.2.0/startrek/net/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/net/channel.py` & `startrek-1.2.0/startrek/net/channel.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/net/connection.py` & `startrek-1.2.0/startrek/net/connection.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/net/delegate.py` & `startrek-1.2.0/startrek/net/delegate.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/net/hub.py` & `startrek-1.2.0/startrek/net/hub.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/net/state.py` & `startrek-1.2.0/startrek/net/state.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/port/__init__.py` & `startrek-1.2.0/startrek/port/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/port/delegate.py` & `startrek-1.2.0/startrek/port/delegate.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/port/docker.py` & `startrek-1.2.0/startrek/port/docker.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/port/gate.py` & `startrek-1.2.0/startrek/port/gate.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/port/ship.py` & `startrek-1.2.0/startrek/port/ship.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/socket/__init__.py` & `startrek-1.2.0/startrek/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/socket/active_conn.py` & `startrek-1.2.0/startrek/socket/active_conn.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,45 +29,47 @@
 # ==============================================================================
 
 import time
 import weakref
 from typing import Optional
 
 from ..types import SocketAddress
-from ..fsm import Daemon
+from ..fsm import Daemon, Runnable
 from ..net import Hub
 
 from .base_conn import BaseConnection
 
 
-class ActiveConnection(BaseConnection):
+class ActiveConnection(BaseConnection, Runnable):
     """ Active connection for client """
 
     def __init__(self, remote: SocketAddress, local: Optional[SocketAddress]):
         super().__init__(remote=remote, local=local)
         self.__hub_ref = None
-        self.__daemon = Daemon(target=self.run)
+        self.__daemon = Daemon(target=self)
 
     @property
-    def hub(self) -> Hub:
-        return self.__hub_ref()
+    def hub(self) -> Optional[Hub]:
+        ref = self.__hub_ref
+        if ref is not None:
+            return ref()
 
     @property  # Override
     def closed(self) -> bool:
         return self.fsm is None
 
     # Override
     def start(self, hub: Hub):
         self.__hub_ref = weakref.ref(hub)
         # 1. start state machine
         self._start_machine()
         # 2. start a background thread to check channel
         self.__daemon.start()
 
-    # protected
+    # Override
     def run(self):
         expired = 0
         last_time = 0
         interval = 8
         while not self.closed:
             time.sleep(1.0)
             now = time.time()
```

### Comparing `startrek-1.1.3/startrek/socket/base_channel.py` & `startrek-1.2.0/startrek/socket/base_channel.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/socket/base_conn.py` & `startrek-1.2.0/startrek/socket/base_conn.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/socket/base_hub.py` & `startrek-1.2.0/startrek/socket/base_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Connection]:
         # 1. remove cached item
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
             cached.close()
         # 2. set new item
         old = super().set(item=item, remote=remote, local=local)
-        assert old is None, 'should not happen'
+        assert old is None, 'should not happen: %s' % old
         return cached
 
     # Override
     def remove(self, item: Optional[Connection],
                remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Connection]:
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
```

### Comparing `startrek-1.1.3/startrek/stardocker.py` & `startrek-1.2.0/startrek/stardocker.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/stargate.py` & `startrek-1.2.0/startrek/stargate.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Docker]:
         # 1. remove cached item
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
             cached.close()
         # 2. set new item
         old = super().set(item=item, remote=remote, local=local)
-        assert old is None, 'should not happen'
+        assert old is None, 'should not happen: %s' % old
         return cached
 
     # Override
     def remove(self, item: Optional[Docker],
                remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Docker]:
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
```

### Comparing `startrek-1.1.3/startrek/types/__init__.py` & `startrek-1.2.0/startrek/types/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/types/mapping.py` & `startrek-1.2.0/startrek/types/mapping.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek/types/pair.py` & `startrek-1.2.0/startrek/types/pair.py`

 * *Files identical despite different names*

### Comparing `startrek-1.1.3/startrek.egg-info/SOURCES.txt` & `startrek-1.2.0/startrek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

