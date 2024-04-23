# Comparing `tmp/tcp-1.1.2.tar.gz` & `tmp/tcp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tcp-1.1.2.tar", last modified: Wed Mar 13 11:09:19 2024, max compression
+gzip compressed data, was "dist/tcp-1.2.0.tar", last modified: Tue Apr 23 09:03:52 2024, max compression
```

## Comparing `tcp-1.1.2.tar` & `tcp-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:09:19.000000 tcp-1.1.2/
--rw-r--r--   0 moky       (501) staff       (20)      445 2024-03-13 11:09:19.000000 tcp-1.1.2/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 tcp-1.1.2/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-03-13 11:09:19.000000 tcp-1.1.2/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      849 2024-03-13 10:02:51.000000 tcp-1.1.2/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:09:19.000000 tcp-1.1.2/tcp/
--rw-r--r--   0 moky       (501) staff       (20)     2828 2023-01-13 12:35:58.000000 tcp-1.1.2/tcp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7571 2024-03-13 10:03:59.000000 tcp-1.1.2/tcp/channel.py
--rw-r--r--   0 moky       (501) staff       (20)    10080 2024-03-13 10:55:51.000000 tcp-1.1.2/tcp/hub.py
--rw-r--r--   0 moky       (501) staff       (20)     4471 2024-03-06 15:36:17.000000 tcp-1.1.2/tcp/startrek.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:09:19.000000 tcp-1.1.2/tcp.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      445 2024-03-13 11:09:19.000000 tcp-1.1.2/tcp.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      210 2024-03-13 11:09:19.000000 tcp-1.1.2/tcp.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-03-13 11:09:19.000000 tcp-1.1.2/tcp.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       16 2024-03-13 11:09:19.000000 tcp-1.1.2/tcp.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2024-03-13 11:09:19.000000 tcp-1.1.2/tcp.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:03:52.000000 tcp-1.2.0/
+-rw-r--r--   0 moky       (501) staff       (20)      445 2024-04-23 09:03:52.000000 tcp-1.2.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 tcp-1.2.0/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-23 09:03:52.000000 tcp-1.2.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      849 2024-04-23 08:31:29.000000 tcp-1.2.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp/
+-rw-r--r--   0 moky       (501) staff       (20)     2828 2023-01-13 12:35:58.000000 tcp-1.2.0/tcp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7571 2024-03-13 10:03:59.000000 tcp-1.2.0/tcp/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)    10086 2024-04-23 08:31:56.000000 tcp-1.2.0/tcp/hub.py
+-rw-r--r--   0 moky       (501) staff       (20)     4471 2024-03-06 15:36:17.000000 tcp-1.2.0/tcp/startrek.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      445 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      210 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       16 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2024-04-23 09:03:52.000000 tcp-1.2.0/tcp.egg-info/top_level.txt
```

### Comparing `tcp-1.1.2/setup.py` & `tcp-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~
 
     Transmission Control Protocol
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '1.1.2'
+__version__ = '1.2.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
@@ -30,10 +30,10 @@
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'startrek>=1.1.2'
+        'startrek>=1.2.0'
     ]
 )
```

### Comparing `tcp-1.1.2/tcp/__init__.py` & `tcp-1.2.0/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `tcp-1.1.2/tcp/channel.py` & `tcp-1.2.0/tcp/channel.py`

 * *Files identical despite different names*

### Comparing `tcp-1.1.2/tcp/hub.py` & `tcp-1.2.0/tcp/hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
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
     def remove(self, item: Optional[Channel],
                remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
         cached = super().remove(item=item, remote=remote, local=local)
         if cached is not None and cached is not item:
@@ -115,15 +115,15 @@
     """ Stream Server Hub """
 
     def __init__(self, delegate: ConnectionDelegate, daemonic: bool = True):
         super().__init__(delegate=delegate)
         self.__local = None   # SocketAddress
         self.__master = None  # socket.socket
         # running thread
-        self.__daemon = Daemon(target=self.run, daemonic=daemonic)
+        self.__daemon = Daemon(target=self, daemonic=daemonic)
         self.__running = False
 
     # Override
     def _create_connection(self, remote: SocketAddress, local: Optional[SocketAddress]) -> Optional[Connection]:
         conn = BaseConnection(remote=remote, local=local)
         conn.delegate = self.delegate  # gate
         return conn
```

### Comparing `tcp-1.1.2/tcp/startrek.py` & `tcp-1.2.0/tcp/startrek.py`

 * *Files identical despite different names*

