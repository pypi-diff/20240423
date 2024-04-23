# Comparing `tmp/udp-1.1.2.tar.gz` & `tmp/udp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/udp-1.1.2.tar", last modified: Wed Mar 13 11:08:46 2024, max compression
+gzip compressed data, was "dist/udp-1.2.0.tar", last modified: Tue Apr 23 09:04:45 2024, max compression
```

## Comparing `udp-1.1.2.tar` & `udp-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:08:46.000000 udp-1.1.2/
--rw-r--r--   0 moky       (501) staff       (20)      438 2024-03-13 11:08:46.000000 udp-1.1.2/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 udp-1.1.2/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-03-13 11:08:46.000000 udp-1.1.2/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      835 2024-03-13 10:18:16.000000 udp-1.1.2/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:08:46.000000 udp-1.1.2/udp/
--rw-r--r--   0 moky       (501) staff       (20)     2832 2023-01-13 16:49:26.000000 udp-1.1.2/udp/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:08:46.000000 udp-1.1.2/udp/ba/
--rw-r--r--   0 moky       (501) staff       (20)     1944 2021-09-16 08:10:15.000000 udp-1.1.2/udp/ba/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9574 2024-02-26 16:22:28.000000 udp-1.1.2/udp/ba/array.py
--rw-r--r--   0 moky       (501) staff       (20)     3345 2021-09-16 08:10:15.000000 udp-1.1.2/udp/ba/convert.py
--rw-r--r--   0 moky       (501) staff       (20)     7763 2023-01-13 16:00:06.000000 udp-1.1.2/udp/ba/data.py
--rw-r--r--   0 moky       (501) staff       (20)     7219 2023-01-13 15:58:57.000000 udp-1.1.2/udp/ba/helper.py
--rw-r--r--   0 moky       (501) staff       (20)     8436 2021-09-16 08:10:15.000000 udp-1.1.2/udp/ba/integer.py
--rw-r--r--   0 moky       (501) staff       (20)     4852 2021-09-16 08:10:15.000000 udp-1.1.2/udp/ba/mutable.py
--rw-r--r--   0 moky       (501) staff       (20)    15161 2023-01-13 16:00:39.000000 udp-1.1.2/udp/ba/utils.py
--rw-r--r--   0 moky       (501) staff       (20)     9393 2024-03-06 16:08:05.000000 udp-1.1.2/udp/channel.py
--rw-r--r--   0 moky       (501) staff       (20)     8157 2024-03-13 10:56:10.000000 udp-1.1.2/udp/hub.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:08:46.000000 udp-1.1.2/udp/mtp/
--rw-r--r--   0 moky       (501) staff       (20)     1678 2021-09-16 08:10:15.000000 udp-1.1.2/udp/mtp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    15551 2023-01-02 14:11:01.000000 udp-1.1.2/udp/mtp/header.py
--rw-r--r--   0 moky       (501) staff       (20)     4505 2023-01-02 14:11:01.000000 udp-1.1.2/udp/mtp/package.py
--rw-r--r--   0 moky       (501) staff       (20)     8003 2023-01-02 14:11:01.000000 udp-1.1.2/udp/mtp/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6708 2021-09-16 08:10:15.000000 udp-1.1.2/udp/mtp/protocol.py
--rw-r--r--   0 moky       (501) staff       (20)    11523 2024-03-06 16:13:05.000000 udp-1.1.2/udp/startrek.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-03-13 11:08:46.000000 udp-1.1.2/udp.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      438 2024-03-13 11:08:46.000000 udp-1.1.2/udp.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      442 2024-03-13 11:08:46.000000 udp-1.1.2/udp.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-03-13 11:08:46.000000 udp-1.1.2/udp.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       16 2024-03-13 11:08:46.000000 udp-1.1.2/udp.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2024-03-13 11:08:46.000000 udp-1.1.2/udp.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:04:45.000000 udp-1.2.0/
+-rw-r--r--   0 moky       (501) staff       (20)      438 2024-04-23 09:04:45.000000 udp-1.2.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 udp-1.2.0/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-04-23 09:04:45.000000 udp-1.2.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      835 2024-04-23 08:32:23.000000 udp-1.2.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:04:45.000000 udp-1.2.0/udp/
+-rw-r--r--   0 moky       (501) staff       (20)     2832 2023-01-13 16:49:26.000000 udp-1.2.0/udp/__init__.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:04:45.000000 udp-1.2.0/udp/ba/
+-rw-r--r--   0 moky       (501) staff       (20)     1944 2021-09-16 08:10:15.000000 udp-1.2.0/udp/ba/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9574 2024-02-26 16:22:28.000000 udp-1.2.0/udp/ba/array.py
+-rw-r--r--   0 moky       (501) staff       (20)     3345 2021-09-16 08:10:15.000000 udp-1.2.0/udp/ba/convert.py
+-rw-r--r--   0 moky       (501) staff       (20)     7763 2023-01-13 16:00:06.000000 udp-1.2.0/udp/ba/data.py
+-rw-r--r--   0 moky       (501) staff       (20)     7219 2023-01-13 15:58:57.000000 udp-1.2.0/udp/ba/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)     8436 2021-09-16 08:10:15.000000 udp-1.2.0/udp/ba/integer.py
+-rw-r--r--   0 moky       (501) staff       (20)     4852 2021-09-16 08:10:15.000000 udp-1.2.0/udp/ba/mutable.py
+-rw-r--r--   0 moky       (501) staff       (20)    15161 2023-01-13 16:00:39.000000 udp-1.2.0/udp/ba/utils.py
+-rw-r--r--   0 moky       (501) staff       (20)     9393 2024-03-06 16:08:05.000000 udp-1.2.0/udp/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)     8167 2024-04-22 17:50:56.000000 udp-1.2.0/udp/hub.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:04:45.000000 udp-1.2.0/udp/mtp/
+-rw-r--r--   0 moky       (501) staff       (20)     1678 2021-09-16 08:10:15.000000 udp-1.2.0/udp/mtp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    15551 2023-01-02 14:11:01.000000 udp-1.2.0/udp/mtp/header.py
+-rw-r--r--   0 moky       (501) staff       (20)     4505 2023-01-02 14:11:01.000000 udp-1.2.0/udp/mtp/package.py
+-rw-r--r--   0 moky       (501) staff       (20)     8003 2023-01-02 14:11:01.000000 udp-1.2.0/udp/mtp/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6708 2021-09-16 08:10:15.000000 udp-1.2.0/udp/mtp/protocol.py
+-rw-r--r--   0 moky       (501) staff       (20)    11523 2024-03-06 16:13:05.000000 udp-1.2.0/udp/startrek.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      438 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      442 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       16 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2024-04-23 09:04:45.000000 udp-1.2.0/udp.egg-info/top_level.txt
```

### Comparing `udp-1.1.2/setup.py` & `udp-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~
 
     User Datagram Protocol
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

### Comparing `udp-1.1.2/udp/__init__.py` & `udp-1.2.0/udp/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/ba/__init__.py` & `udp-1.2.0/udp/ba/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/ba/array.py` & `udp-1.2.0/udp/ba/array.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/ba/convert.py` & `udp-1.2.0/udp/ba/convert.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/ba/data.py` & `udp-1.2.0/udp/ba/data.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/ba/helper.py` & `udp-1.2.0/udp/ba/helper.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/ba/integer.py` & `udp-1.2.0/udp/ba/integer.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/ba/mutable.py` & `udp-1.2.0/udp/ba/mutable.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/ba/utils.py` & `udp-1.2.0/udp/ba/utils.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/channel.py` & `udp-1.2.0/udp/channel.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/hub.py` & `udp-1.2.0/udp/hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
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
```

### Comparing `udp-1.1.2/udp/mtp/__init__.py` & `udp-1.2.0/udp/mtp/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/mtp/header.py` & `udp-1.2.0/udp/mtp/header.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/mtp/package.py` & `udp-1.2.0/udp/mtp/package.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/mtp/packer.py` & `udp-1.2.0/udp/mtp/packer.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/mtp/protocol.py` & `udp-1.2.0/udp/mtp/protocol.py`

 * *Files identical despite different names*

### Comparing `udp-1.1.2/udp/startrek.py` & `udp-1.2.0/udp/startrek.py`

 * *Files identical despite different names*

