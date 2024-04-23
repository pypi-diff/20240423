# Comparing `tmp/flask_pikarmq-1.0.tar.gz` & `tmp/flask_pikarmq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_pikarmq-1.0.tar", last modified: Tue Apr 23 08:36:23 2024, max compression
+gzip compressed data, was "flask_pikarmq-1.0.1.tar", last modified: Tue Apr 23 08:46:48 2024, max compression
```

## Comparing `flask_pikarmq-1.0.tar` & `flask_pikarmq-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 08:36:23.379371 flask_pikarmq-1.0/
-drwxrwxrwx   0        0        0        0 2024-04-23 08:36:23.375222 flask_pikarmq-1.0/Flask_PikaRMQ.egg-info/
--rw-rw-rw-   0        0        0      727 2024-04-23 08:36:23.000000 flask_pikarmq-1.0/Flask_PikaRMQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-23 08:36:23.000000 flask_pikarmq-1.0/Flask_PikaRMQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:36:23.000000 flask_pikarmq-1.0/Flask_PikaRMQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-23 08:36:22.000000 flask_pikarmq-1.0/Flask_PikaRMQ.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-23 08:36:23.000000 flask_pikarmq-1.0/Flask_PikaRMQ.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-23 08:36:23.000000 flask_pikarmq-1.0/Flask_PikaRMQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2024-04-23 07:45:54.000000 flask_pikarmq-1.0/LICENSE
--rw-rw-rw-   0        0        0      727 2024-04-23 08:36:23.376357 flask_pikarmq-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-23 07:35:24.000000 flask_pikarmq-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 08:36:23.372226 flask_pikarmq-1.0/flask_pikarmq/
--rw-rw-rw-   0        0        0     2204 2024-04-23 08:35:53.000000 flask_pikarmq-1.0/flask_pikarmq/flask_pikarmq.py
--rw-rw-rw-   0        0        0       42 2024-04-23 08:36:23.379371 flask_pikarmq-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1020 2024-04-23 08:35:14.000000 flask_pikarmq-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:46:48.394613 flask_pikarmq-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-04-23 08:46:48.391613 flask_pikarmq-1.0.1/Flask_PikaRMQ.egg-info/
+-rw-rw-rw-   0        0        0      360 2024-04-23 08:46:48.000000 flask_pikarmq-1.0.1/Flask_PikaRMQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-23 08:46:48.000000 flask_pikarmq-1.0.1/Flask_PikaRMQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:46:48.000000 flask_pikarmq-1.0.1/Flask_PikaRMQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 08:36:22.000000 flask_pikarmq-1.0.1/Flask_PikaRMQ.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-23 08:46:48.000000 flask_pikarmq-1.0.1/Flask_PikaRMQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 08:46:48.000000 flask_pikarmq-1.0.1/Flask_PikaRMQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1073 2024-04-23 07:45:54.000000 flask_pikarmq-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      360 2024-04-23 08:46:48.393611 flask_pikarmq-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-23 07:35:24.000000 flask_pikarmq-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:46:48.395611 flask_pikarmq-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      648 2024-04-23 08:46:31.000000 flask_pikarmq-1.0.1/setup.py
```

### Comparing `flask_pikarmq-1.0/LICENSE` & `flask_pikarmq-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_pikarmq-1.0/setup.py` & `flask_pikarmq-1.0.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,32 +6,24 @@
 """
 
 from setuptools import setup
 
 
 setup(
     name="Flask-PikaRMQ",
-    version="1.0",
+    version="1.0.1",
     url="",
     license="BSD",
     author="Rasco Developers",
     author_email="rezahartono.rasco@gmail.com",
     description="This is Extension for RabbitMQ Microservice",
     long_description=__doc__,
-    py_modules=["flask_pikarmq/flask_pikarmq"],
+    py_modules=["flask_pikarmq"],
     # if you would be using a package instead use packages instead
     # of py_modules:
     # packages=['flask_sqlite3'],
     zip_safe=False,
     include_package_data=True,
     platforms="any",
     install_requires=["Flask", "pika"],
-    classifiers=[
-        "Environment :: Web Environment",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: BSD License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python",
-        "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
+    classifiers=[],
 )
```

