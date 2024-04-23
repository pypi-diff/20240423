# Comparing `tmp/dataminer-0.1.4.tar.gz` & `tmp/dataminer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataminer-0.1.4.tar", last modified: Mon Apr 15 09:34:58 2024, max compression
+gzip compressed data, was "dataminer-0.1.5.tar", last modified: Tue Apr 23 07:19:11 2024, max compression
```

## Comparing `dataminer-0.1.4.tar` & `dataminer-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:58.124333 dataminer-0.1.4/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)    11357 2024-04-15 09:34:42.000000 dataminer-0.1.4/LICENSE
--rw-r--r--   0 javaite   (1000) javaite   (1000)      544 2024-04-15 09:34:58.124333 dataminer-0.1.4/PKG-INFO
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:42.000000 dataminer-0.1.4/README.md
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:58.120333 dataminer-0.1.4/dataminer/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/__init__.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:58.124333 dataminer-0.1.4/dataminer/datax/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/datax/__init__.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     4302 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/datax/job_helpers.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     3558 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/datax/runner.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:58.124333 dataminer-0.1.4/dataminer/sqla/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/sqla/__init__.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     1618 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/sqla/engine_helpers.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     1627 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/sqla/inspect_helpers.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      332 2024-04-15 09:34:42.000000 dataminer-0.1.4/dataminer/sqla/query_helpers.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-15 09:34:58.120333 dataminer-0.1.4/dataminer.egg-info/
--rw-r--r--   0 javaite   (1000) javaite   (1000)      544 2024-04-15 09:34:58.000000 dataminer-0.1.4/dataminer.egg-info/PKG-INFO
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      423 2024-04-15 09:34:58.000000 dataminer-0.1.4/dataminer.egg-info/SOURCES.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        1 2024-04-15 09:34:58.000000 dataminer-0.1.4/dataminer.egg-info/dependency_links.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       20 2024-04-15 09:34:58.000000 dataminer-0.1.4/dataminer.egg-info/requires.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       10 2024-04-15 09:34:58.000000 dataminer-0.1.4/dataminer.egg-info/top_level.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       38 2024-04-15 09:34:58.124333 dataminer-0.1.4/setup.cfg
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      725 2024-04-15 09:34:42.000000 dataminer-0.1.4/setup.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-23 07:19:11.555513 dataminer-0.1.5/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)    11357 2024-04-23 07:18:48.000000 dataminer-0.1.5/LICENSE
+-rw-r--r--   0 javaite   (1000) javaite   (1000)      544 2024-04-23 07:19:11.555513 dataminer-0.1.5/PKG-INFO
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-23 07:18:48.000000 dataminer-0.1.5/README.md
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-23 07:19:11.551514 dataminer-0.1.5/dataminer/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-23 07:18:48.000000 dataminer-0.1.5/dataminer/__init__.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-23 07:19:11.551514 dataminer-0.1.5/dataminer/datax/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-23 07:18:48.000000 dataminer-0.1.5/dataminer/datax/__init__.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     4302 2024-04-23 07:18:48.000000 dataminer-0.1.5/dataminer/datax/job_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     3913 2024-04-23 07:18:48.000000 dataminer-0.1.5/dataminer/datax/runner.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-23 07:19:11.555513 dataminer-0.1.5/dataminer/sqla/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-23 07:18:48.000000 dataminer-0.1.5/dataminer/sqla/__init__.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     1618 2024-04-23 07:18:48.000000 dataminer-0.1.5/dataminer/sqla/engine_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     1627 2024-04-23 07:18:48.000000 dataminer-0.1.5/dataminer/sqla/inspect_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      332 2024-04-23 07:18:48.000000 dataminer-0.1.5/dataminer/sqla/query_helpers.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-23 07:19:11.551514 dataminer-0.1.5/dataminer.egg-info/
+-rw-r--r--   0 javaite   (1000) javaite   (1000)      544 2024-04-23 07:19:11.000000 dataminer-0.1.5/dataminer.egg-info/PKG-INFO
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      423 2024-04-23 07:19:11.000000 dataminer-0.1.5/dataminer.egg-info/SOURCES.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        1 2024-04-23 07:19:11.000000 dataminer-0.1.5/dataminer.egg-info/dependency_links.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       20 2024-04-23 07:19:11.000000 dataminer-0.1.5/dataminer.egg-info/requires.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       10 2024-04-23 07:19:11.000000 dataminer-0.1.5/dataminer.egg-info/top_level.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       38 2024-04-23 07:19:11.555513 dataminer-0.1.5/setup.cfg
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      725 2024-04-23 07:18:48.000000 dataminer-0.1.5/setup.py
```

### Comparing `dataminer-0.1.4/LICENSE` & `dataminer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.4/PKG-INFO` & `dataminer-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataminer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of data processing tools.
 Home-page: https://gitee.com/javaite_code/dataminer.git
 Author: javaite
 Author-email: javaite@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `dataminer-0.1.4/dataminer/datax/job_helpers.py` & `dataminer-0.1.5/dataminer/datax/job_helpers.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.4/dataminer/datax/runner.py` & `dataminer-0.1.5/dataminer/datax/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,31 +67,41 @@
 
         try:
             Path(self.datax_path)
         except Exception as e:
             raise ValueError(f"Invalid path: {self.datax_path}") from e
 
         with tempfile.NamedTemporaryFile(
-                mode="w", encoding="utf-8", suffix=".json"
+            mode="w", encoding="utf-8", suffix=".json"
         ) as tf:
             job_file = Path(tf.name).resolve()
             tf.seek(0)
             json.dump(job, tf, indent=4, ensure_ascii=False)
             tf.flush()
             tf.seek(0)
 
             cmd = f"{sys.executable} {self.datax_path} {job_file}"
-            result = subprocess.run(
-                cmd,
-                shell=True,
-                check=True,
-                stdout=subprocess.PIPE,
-                stderr=subprocess.PIPE,
-                encoding="utf-8",
-            )
+
+            try:
+                result = subprocess.run(
+                    cmd,
+                    shell=True,
+                    check=True,
+                    stdout=subprocess.PIPE,
+                    stderr=subprocess.PIPE,
+                    encoding="utf-8",
+                )
+            except subprocess.CalledProcessError as e:
+                datax_result = {
+                    "args": e.args[1],
+                    "returncode": e.returncode,
+                    "stdout": e.stdout,
+                    "stderr": e.stderr,
+                }
+                return datax_result
 
             datax_result = {
                 "args": result.args,
                 "returncode": result.returncode,
                 "stdout": result.stdout,
                 "stderr": result.stderr,
             }
```

### Comparing `dataminer-0.1.4/dataminer/sqla/engine_helpers.py` & `dataminer-0.1.5/dataminer/sqla/engine_helpers.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.4/dataminer/sqla/inspect_helpers.py` & `dataminer-0.1.5/dataminer/sqla/inspect_helpers.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.4/dataminer.egg-info/PKG-INFO` & `dataminer-0.1.5/dataminer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataminer
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of data processing tools.
 Home-page: https://gitee.com/javaite_code/dataminer.git
 Author: javaite
 Author-email: javaite@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `dataminer-0.1.4/setup.py` & `dataminer-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dataminer',
-    version='0.1.4',
+    version='0.1.5',
     packages=find_packages(),
     install_requires=[
         'sqlalchemy',
         'oracledb',
     ],
     author='javaite',
     author_email='javaite@126.com',
```

