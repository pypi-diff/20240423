# Comparing `tmp/sigmoid_check-0.0.1.tar.gz` & `tmp/sigmoid_check-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmoid_check-0.0.1.tar", last modified: Tue Apr 23 18:47:53 2024, max compression
+gzip compressed data, was "sigmoid_check-0.0.2.tar", last modified: Tue Apr 23 20:15:44 2024, max compression
```

## Comparing `sigmoid_check-0.0.1.tar` & `sigmoid_check-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 18:47:53.933935 sigmoid_check-0.0.1/
--rw-rw-rw-   0        0        0    11538 2024-04-23 18:15:46.000000 sigmoid_check-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2756 2024-04-23 18:47:53.934941 sigmoid_check-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1881 2024-04-23 18:29:06.000000 sigmoid_check-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2024-04-23 18:47:53.936946 sigmoid_check-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1165 2024-04-23 18:42:53.000000 sigmoid_check-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:47:53.912934 sigmoid_check-0.0.1/sigmoid_check/
-drwxrwxrwx   0        0        0        0 2024-04-23 18:47:53.922945 sigmoid_check-0.0.1/sigmoid_check/python_odyssey/
--rw-rw-rw-   0        0        0        0 2024-04-23 18:24:15.000000 sigmoid_check-0.0.1/sigmoid_check/python_odyssey/__init__.py
--rw-rw-rw-   0        0        0     6550 2024-04-23 18:28:36.000000 sigmoid_check-0.0.1/sigmoid_check/python_odyssey/lesson_10.py
-drwxrwxrwx   0        0        0        0 2024-04-23 18:47:53.931937 sigmoid_check-0.0.1/sigmoid_check/sigmoid_check.egg-info/
--rw-rw-rw-   0        0        0     2756 2024-04-23 18:47:53.000000 sigmoid_check-0.0.1/sigmoid_check/sigmoid_check.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-04-23 18:47:53.000000 sigmoid_check-0.0.1/sigmoid_check/sigmoid_check.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 18:47:53.000000 sigmoid_check-0.0.1/sigmoid_check/sigmoid_check.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-23 18:47:53.000000 sigmoid_check-0.0.1/sigmoid_check/sigmoid_check.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 20:15:43.995977 sigmoid_check-0.0.2/
+-rw-rw-rw-   0        0        0    11538 2024-04-23 18:15:46.000000 sigmoid_check-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2756 2024-04-23 20:15:43.995977 sigmoid_check-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1881 2024-04-23 18:29:06.000000 sigmoid_check-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-23 20:15:44.001985 sigmoid_check-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2024-04-23 20:13:46.000000 sigmoid_check-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:15:43.977657 sigmoid_check-0.0.2/sigmoid_check/
+-rw-rw-rw-   0        0        0        0 2024-04-23 19:00:37.000000 sigmoid_check-0.0.2/sigmoid_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:15:43.991981 sigmoid_check-0.0.2/sigmoid_check/python_odyssey/
+-rw-rw-rw-   0        0        0       31 2024-04-23 19:00:20.000000 sigmoid_check-0.0.2/sigmoid_check/python_odyssey/__init__.py
+-rw-rw-rw-   0        0        0     6550 2024-04-23 18:28:36.000000 sigmoid_check-0.0.2/sigmoid_check/python_odyssey/lesson_10.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:15:43.992979 sigmoid_check-0.0.2/sigmoid_check.egg-info/
+-rw-rw-rw-   0        0        0     2756 2024-04-23 20:15:43.000000 sigmoid_check-0.0.2/sigmoid_check.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-23 20:15:43.000000 sigmoid_check-0.0.2/sigmoid_check.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 20:15:43.000000 sigmoid_check-0.0.2/sigmoid_check.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 20:15:43.000000 sigmoid_check-0.0.2/sigmoid_check.egg-info/top_level.txt
```

### Comparing `sigmoid_check-0.0.1/LICENSE` & `sigmoid_check-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.1/PKG-INFO` & `sigmoid_check-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmoid_check
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for checking the implementation of tasks in Sigmoid Courses
 Author: SigmoidAI - Balamatiuc Eduard
 Author-email: balamatiuc2@gmail.com
 License: Apache License 2.0
 Keywords: tasks,check,sigmoid,sigmoidai,sigmoid_check
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sigmoid_check-0.0.1/README.md` & `sigmoid_check-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.1/setup.py` & `sigmoid_check-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="sigmoid_check",
-    version="0.0.1",
+    version="0.0.2",
+    packages=find_packages(),
     description="A package for checking the implementation of tasks in Sigmoid Courses",
-    package_dir={"": "sigmoid_check"},
-    packages=find_packages(where="sigmoid_check"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="SigmoidAI - Balamatiuc Eduard",
     author_email="balamatiuc2@gmail.com",
     keywords=["tasks", "check", "sigmoid", "sigmoidai", "sigmoid_check"],
     license="Apache License 2.0",
     classifiers=[
```

### Comparing `sigmoid_check-0.0.1/sigmoid_check/python_odyssey/lesson_10.py` & `sigmoid_check-0.0.2/sigmoid_check/python_odyssey/lesson_10.py`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.1/sigmoid_check/sigmoid_check.egg-info/PKG-INFO` & `sigmoid_check-0.0.2/sigmoid_check.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: sigmoid-check
-Version: 0.0.1
+Name: sigmoid_check
+Version: 0.0.2
 Summary: A package for checking the implementation of tasks in Sigmoid Courses
 Author: SigmoidAI - Balamatiuc Eduard
 Author-email: balamatiuc2@gmail.com
 License: Apache License 2.0
 Keywords: tasks,check,sigmoid,sigmoidai,sigmoid_check
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

