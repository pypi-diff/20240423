# Comparing `tmp/pyneople-0.2.1.tar.gz` & `tmp/pyneople-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.2.1.tar", last modified: Sun Apr 21 12:23:16 2024, max compression
+gzip compressed data, was "pyneople-0.2.2.tar", last modified: Tue Apr 23 01:49:06 2024, max compression
```

## Comparing `pyneople-0.2.1.tar` & `pyneople-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:23:16.001203 pyneople-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-21 12:23:06.000000 pyneople-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-21 12:23:16.001203 pyneople-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-21 12:23:06.000000 pyneople-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-21 12:23:06.000000 pyneople-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 12:23:16.001203 pyneople-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-21 12:23:06.000000 pyneople-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:23:15.997203 pyneople-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:23:16.001203 pyneople-0.2.1/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/avatars.py
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/buff.py
--rw-r--r--   0 runner    (1001) docker     (127)    33657 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/character.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/character_fame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/character_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/character_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/equipments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/others.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-21 12:23:06.000000 pyneople-0.2.1/src/pyneople/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:23:16.001203 pyneople-0.2.1/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-21 12:23:15.000000 pyneople-0.2.1/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-21 12:23:15.000000 pyneople-0.2.1/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:23:15.000000 pyneople-0.2.1/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 12:23:15.000000 pyneople-0.2.1/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:49:06.834847 pyneople-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 01:48:55.000000 pyneople-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-23 01:49:06.834847 pyneople-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 01:48:55.000000 pyneople-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-23 01:48:55.000000 pyneople-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:49:06.834847 pyneople-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-23 01:48:55.000000 pyneople-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:49:06.830847 pyneople-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:49:06.834847 pyneople-0.2.2/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/avatars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/buff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33657 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/character_fame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/character_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/character_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/database_connecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7593 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/equipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/others.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-23 01:48:55.000000 pyneople-0.2.2/src/pyneople/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:49:06.834847 pyneople-0.2.2/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-23 01:49:06.000000 pyneople-0.2.2/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-23 01:49:06.000000 pyneople-0.2.2/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:49:06.000000 pyneople-0.2.2/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 01:49:06.000000 pyneople-0.2.2/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.2.1/LICENSE` & `pyneople-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/PKG-INFO` & `pyneople-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.1
+Version: 0.2.2
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.2.1/setup.py` & `pyneople-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.2.1",
+    version="0.2.2",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
```

### Comparing `pyneople-0.2.1/src/pyneople/METADATA.py` & `pyneople-0.2.2/src/pyneople/METADATA.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,16 @@
 
 # CharacterSearch 에서 선택 가능한 변수
 CHARACTER_SEARCH_NAME = {
     'server_id': 'serverId',
     'character_id': 'characterId',
     'character_name': 'characterName',
     'level': 'level',
+    'job_id' : 'jobId',
+    'job_grow_id' : 'jobGrowId',
     'job_name': 'jobName',
     'job_grow_name': 'jobGrowName',
     'fame': 'fame',
 }
 
 # CharacterInformation 에서 선택 가능한 변수
 CHARACTER_INFORMATION_NAME = {
```

### Comparing `pyneople-0.2.1/src/pyneople/avatars.py` & `pyneople-0.2.2/src/pyneople/avatars.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople/buff.py` & `pyneople-0.2.2/src/pyneople/buff.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople/character.py` & `pyneople-0.2.2/src/pyneople/character.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople/character_fame.py` & `pyneople-0.2.2/src/pyneople/character_fame.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople/character_information.py` & `pyneople-0.2.2/src/pyneople/character_information.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople/character_search.py` & `pyneople-0.2.2/src/pyneople/character_search.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople/equipments.py` & `pyneople-0.2.2/src/pyneople/equipments.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople/functions.py` & `pyneople-0.2.2/src/pyneople/functions.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople/others.py` & `pyneople-0.2.2/src/pyneople/others.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople/status.py` & `pyneople-0.2.2/src/pyneople/status.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople/timeline.py` & `pyneople-0.2.2/src/pyneople/timeline.py`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.1/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.2.2/src/pyneople.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.1
+Version: 0.2.2
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyneople-0.2.1/src/pyneople.egg-info/SOURCES.txt` & `pyneople-0.2.2/src/pyneople.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/pyneople/__init__.py
 src/pyneople/avatars.py
 src/pyneople/buff.py
 src/pyneople/character.py
 src/pyneople/character_fame.py
 src/pyneople/character_information.py
 src/pyneople/character_search.py
+src/pyneople/database_connecter.py
 src/pyneople/equipments.py
 src/pyneople/functions.py
 src/pyneople/others.py
 src/pyneople/status.py
 src/pyneople/timeline.py
 src/pyneople.egg-info/PKG-INFO
 src/pyneople.egg-info/SOURCES.txt
```

