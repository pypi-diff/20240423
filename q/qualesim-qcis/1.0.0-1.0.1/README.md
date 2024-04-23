# Comparing `tmp/qualesim-qcis-1.0.0.tar.gz` & `tmp/qualesim-qcis-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-qcis-1.0.0.tar", last modified: Fri Mar 29 08:18:07 2024, max compression
+gzip compressed data, was "qualesim-qcis-1.0.1.tar", last modified: Tue Apr 23 03:08:52 2024, max compression
```

## Comparing `qualesim-qcis-1.0.0.tar` & `qualesim-qcis-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:18:07.508378 qualesim-qcis-1.0.0/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      546 2024-03-29 08:18:07.508378 qualesim-qcis-1.0.0/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-08 01:22:27.000000 qualesim-qcis-1.0.0/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:18:07.508378 qualesim-qcis-1.0.0/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:18:07.508378 qualesim-qcis-1.0.0/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      186 2024-03-29 08:08:44.000000 qualesim-qcis-1.0.0/data/bin/dqcsfeqcis
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:18:07.508378 qualesim-qcis-1.0.0/qualesim_qcis/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     5082 2024-03-29 08:08:44.000000 qualesim-qcis-1.0.0/qualesim_qcis/QCIS_inst.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     3636 2024-03-29 08:08:44.000000 qualesim-qcis-1.0.0/qualesim_qcis/QCIS_lexer.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6293 2024-03-29 08:08:44.000000 qualesim-qcis-1.0.0/qualesim_qcis/QCIS_parser.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    20161 2024-03-29 08:11:16.000000 qualesim-qcis-1.0.0/qualesim_qcis/frontend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      249 2024-03-29 08:08:44.000000 qualesim-qcis-1.0.0/qualesim_qcis/utils.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-03-29 08:18:07.508378 qualesim-qcis-1.0.0/qualesim_qcis.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      546 2024-03-29 08:18:07.000000 qualesim-qcis-1.0.0/qualesim_qcis.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      355 2024-03-29 08:18:07.000000 qualesim-qcis-1.0.0/qualesim_qcis.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-03-29 08:18:07.000000 qualesim-qcis-1.0.0/qualesim_qcis.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       10 2024-03-29 08:18:07.000000 qualesim-qcis-1.0.0/qualesim_qcis.egg-info/requires.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       14 2024-03-29 08:18:07.000000 qualesim-qcis-1.0.0/qualesim_qcis.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-03-29 08:18:07.508378 qualesim-qcis-1.0.0/setup.cfg
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1066 2024-03-29 08:08:44.000000 qualesim-qcis-1.0.0/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:08:52.200313 qualesim-qcis-1.0.1/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      546 2024-04-23 03:08:52.200313 qualesim-qcis-1.0.1/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-08 01:22:27.000000 qualesim-qcis-1.0.1/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:08:52.196313 qualesim-qcis-1.0.1/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:08:52.196313 qualesim-qcis-1.0.1/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      186 2024-03-29 08:08:44.000000 qualesim-qcis-1.0.1/data/bin/dqcsfeqcis
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:08:52.196313 qualesim-qcis-1.0.1/qualesim_qcis/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     5082 2024-03-29 08:08:44.000000 qualesim-qcis-1.0.1/qualesim_qcis/QCIS_inst.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     3636 2024-03-29 08:08:44.000000 qualesim-qcis-1.0.1/qualesim_qcis/QCIS_lexer.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6293 2024-03-29 08:08:44.000000 qualesim-qcis-1.0.1/qualesim_qcis/QCIS_parser.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    20161 2024-04-23 03:07:56.000000 qualesim-qcis-1.0.1/qualesim_qcis/frontend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      251 2024-04-23 03:08:06.000000 qualesim-qcis-1.0.1/qualesim_qcis/utils.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:08:52.200313 qualesim-qcis-1.0.1/qualesim_qcis.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      546 2024-04-23 03:08:52.000000 qualesim-qcis-1.0.1/qualesim_qcis.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      355 2024-04-23 03:08:52.000000 qualesim-qcis-1.0.1/qualesim_qcis.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-23 03:08:52.000000 qualesim-qcis-1.0.1/qualesim_qcis.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       10 2024-04-23 03:08:52.000000 qualesim-qcis-1.0.1/qualesim_qcis.egg-info/requires.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       14 2024-04-23 03:08:52.000000 qualesim-qcis-1.0.1/qualesim_qcis.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-23 03:08:52.200313 qualesim-qcis-1.0.1/setup.cfg
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1066 2024-04-23 03:08:15.000000 qualesim-qcis-1.0.1/setup.py
```

### Comparing `qualesim-qcis-1.0.0/PKG-INFO` & `qualesim-qcis-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-qcis
-Version: 1.0.0
+Version: 1.0.1
 Summary: QuaLeSim frontend for QCIS.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-qcis.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim qcis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-qcis-1.0.0/qualesim_qcis/QCIS_inst.py` & `qualesim-qcis-1.0.1/qualesim_qcis/QCIS_inst.py`

 * *Files identical despite different names*

### Comparing `qualesim-qcis-1.0.0/qualesim_qcis/QCIS_lexer.py` & `qualesim-qcis-1.0.1/qualesim_qcis/QCIS_lexer.py`

 * *Files identical despite different names*

### Comparing `qualesim-qcis-1.0.0/qualesim_qcis/QCIS_parser.py` & `qualesim-qcis-1.0.1/qualesim_qcis/QCIS_parser.py`

 * *Files identical despite different names*

### Comparing `qualesim-qcis-1.0.0/qualesim_qcis/frontend.py` & `qualesim-qcis-1.0.1/qualesim_qcis/frontend.py`

 * *Files identical despite different names*

### Comparing `qualesim-qcis-1.0.0/qualesim_qcis.egg-info/PKG-INFO` & `qualesim-qcis-1.0.1/qualesim_qcis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-qcis
-Version: 1.0.0
+Version: 1.0.1
 Summary: QuaLeSim frontend for QCIS.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-qcis.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim qcis
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-qcis-1.0.0/setup.py` & `qualesim-qcis-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-qcis",
-    version="1.0.0",
+    version="1.0.1",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="QuaLeSim frontend for QCIS.",
     license="GPLv3",
     keywords="qualesim qcis",
     url="https://gitee.com/hpcl_quanta/dqcsim-qcis.git",
     long_description=read("README.md"),
```

