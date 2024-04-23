# Comparing `tmp/radixtarget-1.0.0.8.tar.gz` & `tmp/radixtarget-1.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radixtarget-1.0.0.8.tar", max compression
+gzip compressed data, was "radixtarget-1.0.0.9.tar", max compression
```

## Comparing `radixtarget-1.0.0.8.tar` & `radixtarget-1.0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1104 2024-04-22 18:35:24.051533 radixtarget-1.0.0.8/README.md
--rw-r--r--   0        0        0      818 2024-04-22 18:35:40.499762 radixtarget-1.0.0.8/pyproject.toml
--rw-r--r--   0        0        0       37 2024-04-22 18:35:24.051533 radixtarget-1.0.0.8/radixtarget/__init__.py
--rw-r--r--   0        0        0      882 2024-04-22 18:35:24.051533 radixtarget-1.0.0.8/radixtarget/radixtarget.py
--rw-r--r--   0        0        0        0 2024-04-22 18:35:24.051533 radixtarget-1.0.0.8/radixtarget/test/__init__.py
--rw-r--r--   0        0        0   454463 2024-04-22 18:35:24.051533 radixtarget-1.0.0.8/radixtarget/test/cidrs.txt
--rw-r--r--   0        0        0     3091 2024-04-22 18:35:24.051533 radixtarget-1.0.0.8/radixtarget/test/test_pyradix.py
--rw-r--r--   0        0        0      205 2024-04-22 18:35:24.051533 radixtarget-1.0.0.8/radixtarget/tree/base.py
--rw-r--r--   0        0        0      974 2024-04-22 18:35:24.051533 radixtarget-1.0.0.8/radixtarget/tree/dns.py
--rw-r--r--   0        0        0     1398 2024-04-22 18:35:24.051533 radixtarget-1.0.0.8/radixtarget/tree/ip.py
--rw-r--r--   0        0        0     1862 1970-01-01 00:00:00.000000 radixtarget-1.0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1152 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/README.md
+-rw-r--r--   0        0        0      818 2024-04-22 18:39:53.703949 radixtarget-1.0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/__init__.py
+-rw-r--r--   0        0        0      882 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/radixtarget.py
+-rw-r--r--   0        0        0        0 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/test/__init__.py
+-rw-r--r--   0        0        0   454463 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/test/cidrs.txt
+-rw-r--r--   0        0        0     3091 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/test/test_pyradix.py
+-rw-r--r--   0        0        0      205 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/tree/base.py
+-rw-r--r--   0        0        0      974 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/tree/dns.py
+-rw-r--r--   0        0        0     1398 2024-04-22 18:39:38.323991 radixtarget-1.0.0.9/radixtarget/tree/ip.py
+-rw-r--r--   0        0        0     1910 1970-01-01 00:00:00.000000 radixtarget-1.0.0.9/PKG-INFO
```

### Comparing `radixtarget-1.0.0.8/README.md` & `radixtarget-1.0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,34 @@
+Metadata-Version: 2.1
+Name: radixtarget
+Version: 1.0.0.9
+Summary: Check whether an IP address belongs to a cloud provider
+Home-page: https://github.com/blacklanternsecurity/radixtarget
+License: GPL-3.0
+Author: TheTechromancer
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: PyPi, https://pypi.org/project/radixtarget/
+Project-URL: Repository, https://github.com/blacklanternsecurity/radixtarget
+Description-Content-Type: text/markdown
+
 # RadixTarget
 
 RadixTarget is a performant radix implementation designed for quick lookups of IP addresses/networks and DNS hostnames. Written in pure python and capable of roughly 100,000 lookups per second regardless of the size of the database.
 
 Used by:
 - [BBOT (Bighuge BLS OSINT Tool)](https://github.com/blacklanternsecurity/bbot)
 - [cloudcheck](https://github.com/blacklanternsecurity/cloudcheck)
 
-### Installation
+### Installation ([PyPi](https://pypi.org/project/radixtarget/))
 
 ```bash
 pip install radixtarget
 ```
 
 ### Example Usage
 
@@ -35,8 +53,8 @@
 rt.insert("test.www.example.com")
 
 rt.search("net") # "net"
 rt.search("evilcorp.net") # "net"
 rt.search("www.example.com") # "www.example.com"
 rt.search("asdf.test.www.example.com") # "test.www.example.com"
 rt.search("example.com") # None
-```
+```
```

### Comparing `radixtarget-1.0.0.8/pyproject.toml` & `radixtarget-1.0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radixtarget"
-version = "v1.0.0.8"
+version = "v1.0.0.9"
 description = "Check whether an IP address belongs to a cloud provider"
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/radixtarget"
 homepage = "https://github.com/blacklanternsecurity/radixtarget"
```

### Comparing `radixtarget-1.0.0.8/radixtarget/radixtarget.py` & `radixtarget-1.0.0.9/radixtarget/radixtarget.py`

 * *Files identical despite different names*

### Comparing `radixtarget-1.0.0.8/radixtarget/test/cidrs.txt` & `radixtarget-1.0.0.9/radixtarget/test/cidrs.txt`

 * *Files identical despite different names*

### Comparing `radixtarget-1.0.0.8/radixtarget/test/test_pyradix.py` & `radixtarget-1.0.0.9/radixtarget/test/test_pyradix.py`

 * *Files identical despite different names*

### Comparing `radixtarget-1.0.0.8/radixtarget/tree/dns.py` & `radixtarget-1.0.0.9/radixtarget/tree/dns.py`

 * *Files identical despite different names*

### Comparing `radixtarget-1.0.0.8/radixtarget/tree/ip.py` & `radixtarget-1.0.0.9/radixtarget/tree/ip.py`

 * *Files identical despite different names*

### Comparing `radixtarget-1.0.0.8/PKG-INFO` & `radixtarget-1.0.0.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,16 @@
-Metadata-Version: 2.1
-Name: radixtarget
-Version: 1.0.0.8
-Summary: Check whether an IP address belongs to a cloud provider
-Home-page: https://github.com/blacklanternsecurity/radixtarget
-License: GPL-3.0
-Author: TheTechromancer
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Project-URL: PyPi, https://pypi.org/project/radixtarget/
-Project-URL: Repository, https://github.com/blacklanternsecurity/radixtarget
-Description-Content-Type: text/markdown
-
 # RadixTarget
 
 RadixTarget is a performant radix implementation designed for quick lookups of IP addresses/networks and DNS hostnames. Written in pure python and capable of roughly 100,000 lookups per second regardless of the size of the database.
 
 Used by:
 - [BBOT (Bighuge BLS OSINT Tool)](https://github.com/blacklanternsecurity/bbot)
 - [cloudcheck](https://github.com/blacklanternsecurity/cloudcheck)
 
-### Installation
+### Installation ([PyPi](https://pypi.org/project/radixtarget/))
 
 ```bash
 pip install radixtarget
 ```
 
 ### Example Usage
 
@@ -53,8 +35,8 @@
 rt.insert("test.www.example.com")
 
 rt.search("net") # "net"
 rt.search("evilcorp.net") # "net"
 rt.search("www.example.com") # "www.example.com"
 rt.search("asdf.test.www.example.com") # "test.www.example.com"
 rt.search("example.com") # None
-```
+```
```

