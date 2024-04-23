# Comparing `tmp/fourcats-flask-0.1.2.tar.gz` & `tmp/fourcats_flask-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fourcats-flask-0.1.2.tar", last modified: Wed Jan 11 08:23:58 2023, max compression
+gzip compressed data, was "fourcats_flask-0.1.3.tar", last modified: Tue Apr 23 06:58:47 2024, max compression
```

## Comparing `fourcats-flask-0.1.2.tar` & `fourcats_flask-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 08:23:58.188099 fourcats-flask-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-11 08:23:58.188099 fourcats-flask-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 08:23:58.184099 fourcats-flask-0.1.2/fourcats_flask/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 08:23:58.184099 fourcats-flask-0.1.2/fourcats_flask/pluins/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/pluins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/pluins/excepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/pluins/global_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/pluins/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 08:23:58.188099 fourcats-flask-0.1.2/fourcats_flask/refactor/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/refactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/refactor/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/refactor/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/refactor/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/refactor/http_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/refactor/request_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/refactor/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/refactor/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/fourcats_flask/refactor/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 08:23:58.184099 fourcats-flask-0.1.2/fourcats_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-11 08:23:58.000000 fourcats-flask-0.1.2/fourcats_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-01-11 08:23:58.000000 fourcats-flask-0.1.2/fourcats_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 08:23:58.000000 fourcats-flask-0.1.2/fourcats_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-11 08:23:58.000000 fourcats-flask-0.1.2/fourcats_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-11 08:23:58.000000 fourcats-flask-0.1.2/fourcats_flask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 08:23:58.188099 fourcats-flask-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-01-11 08:23:50.000000 fourcats-flask-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:58:47.425884 fourcats_flask-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-23 06:58:47.425884 fourcats_flask-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:58:47.421884 fourcats_flask-0.1.3/fourcats_flask/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-23 06:58:40.000000 fourcats_flask-0.1.3/fourcats_flask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:58:47.421884 fourcats_flask-0.1.3/fourcats_flask/pluins/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/pluins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/pluins/excepts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/pluins/global_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/pluins/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:58:47.421884 fourcats_flask-0.1.3/fourcats_flask/refactor/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/refactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/refactor/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/refactor/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/refactor/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/refactor/http_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/refactor/request_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/refactor/requester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/refactor/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/fourcats_flask/refactor/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 06:58:47.421884 fourcats_flask-0.1.3/fourcats_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-23 06:58:47.000000 fourcats_flask-0.1.3/fourcats_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-23 06:58:47.000000 fourcats_flask-0.1.3/fourcats_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 06:58:47.000000 fourcats_flask-0.1.3/fourcats_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-23 06:58:47.000000 fourcats_flask-0.1.3/fourcats_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 06:58:47.000000 fourcats_flask-0.1.3/fourcats_flask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 06:58:47.425884 fourcats_flask-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-23 06:58:39.000000 fourcats_flask-0.1.3/setup.py
```

### Comparing `fourcats-flask-0.1.2/LICENSE` & `fourcats_flask-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/PKG-INFO` & `fourcats_flask-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: fourcats-flask
-Version: 0.1.2
-Summary: A flask encapsulated based on personal habits for fast use.
-Home-page: https://github.com/FourCats-Py/FourCats-Flask
-Download-URL: https://github.com/FourCats-Py/FourCats-Flask/archive/0.1.2.tar.gz
-Author: ShiWeiDong
-Author-email: shiweidong1993@gmail.com
-Keywords: fourcats,flask
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # `FourCats-Flask`
 
 ### Statement
 
  - `FourCats-Flask` is a module with personal habits based on `Flask` and `Flask-RESTX` encapsulation. The main purpose of encapsulation is to provide a more convenient initialization method for partners.
 
 ### Simple Example
```

### Comparing `fourcats-flask-0.1.2/fourcats_flask/__init__.py` & `fourcats_flask-0.1.3/fourcats_flask/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     NotFoundException,
     ParameterException,
     ForbiddenException,
     BadRequestException,
     AuthFailedException,
 )
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

### Comparing `fourcats-flask-0.1.2/fourcats_flask/pluins/excepts.py` & `fourcats_flask-0.1.3/fourcats_flask/pluins/excepts.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask/pluins/global_logger.py` & `fourcats_flask-0.1.3/fourcats_flask/pluins/global_logger.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask/pluins/token.py` & `fourcats_flask-0.1.3/fourcats_flask/pluins/token.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask/refactor/api.py` & `fourcats_flask-0.1.3/fourcats_flask/refactor/api.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask/refactor/app.py` & `fourcats_flask-0.1.3/fourcats_flask/refactor/app.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask/refactor/argument.py` & `fourcats_flask-0.1.3/fourcats_flask/refactor/argument.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask/refactor/http_code.py` & `fourcats_flask-0.1.3/fourcats_flask/refactor/http_code.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask/refactor/request_parser.py` & `fourcats_flask-0.1.3/fourcats_flask/refactor/request_parser.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask/refactor/requester.py` & `fourcats_flask-0.1.3/fourcats_flask/refactor/requester.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask/refactor/response.py` & `fourcats_flask-0.1.3/fourcats_flask/refactor/response.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask/refactor/sqlalchemy.py` & `fourcats_flask-0.1.3/fourcats_flask/refactor/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/fourcats_flask.egg-info/PKG-INFO` & `fourcats_flask-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 Metadata-Version: 2.1
 Name: fourcats-flask
-Version: 0.1.2
+Version: 0.1.3
 Summary: A flask encapsulated based on personal habits for fast use.
 Home-page: https://github.com/FourCats-Py/FourCats-Flask
-Download-URL: https://github.com/FourCats-Py/FourCats-Flask/archive/0.1.2.tar.gz
+Download-URL: https://github.com/FourCats-Py/FourCats-Flask/archive/0.1.3.tar.gz
 Author: ShiWeiDong
 Author-email: shiweidong1993@gmail.com
 Keywords: fourcats,flask
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: flask-restx<1.2.0,>=0.5.0
+Requires-Dist: Flask<2.3.0
+Requires-Dist: loguru>=0.6.0
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: Flask-HTTPAuth>=4.7.0
+Requires-Dist: mergedict>=1.0.0
+Requires-Dist: urllib3>=1.26.10
+Requires-Dist: SQLAlchemy<2.0.0
+Requires-Dist: Flask-SQLAlchemy<=2.5.1
+Requires-Dist: Flask-Cors>=3.0.10
+Requires-Dist: PyJWT>=2.4.0
+Requires-Dist: fourcats-utils>=0.0.4
 
 # `FourCats-Flask`
 
 ### Statement
 
  - `FourCats-Flask` is a module with personal habits based on `Flask` and `Flask-RESTX` encapsulation. The main purpose of encapsulation is to provide a more convenient initialization method for partners.
```

### Comparing `fourcats-flask-0.1.2/fourcats_flask.egg-info/SOURCES.txt` & `fourcats_flask-0.1.3/fourcats_flask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fourcats-flask-0.1.2/setup.py` & `fourcats_flask-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,12 +22,13 @@
     long_description_content_type="text/markdown",
     author="ShiWeiDong",
     author_email="shiweidong1993@gmail.com",
     url="https://github.com/FourCats-Py/FourCats-Flask",
     download_url="https://github.com/FourCats-Py/FourCats-Flask/archive/{}.tar.gz".format(version),
     keywords=["fourcats", "flask"],
     install_requires=[
-        "flask-restx>=0.5.1", "loguru>=0.6.0", "PyYAML>=6.0", "Flask-HTTPAuth>=4.7.0", "mergedict>=1.0.0",
-        "urllib3>=1.26.10",  "Flask-SQLAlchemy>=2.5.1", "Flask-Cors>=3.0.10", "PyJWT>=2.4.0", "fourcats-utils>=0.0.4"
+        "flask-restx>=0.5.0, <1.2.0", "Flask<2.3.0", "loguru>=0.6.0", "PyYAML>=6.0", "Flask-HTTPAuth>=4.7.0",
+        "mergedict>=1.0.0", "urllib3>=1.26.10", "SQLAlchemy<2.0.0",  "Flask-SQLAlchemy<=2.5.1", "Flask-Cors>=3.0.10",
+        "PyJWT>=2.4.0", "fourcats-utils>=0.0.4"
     ],
     python_requires=">=3.8"
 )
```

