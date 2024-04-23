# Comparing `tmp/expyvalidations-0.0.2.tar.gz` & `tmp/expyvalidations-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expyvalidations-0.0.2.tar", last modified: Wed Apr 10 17:22:19 2024, max compression
+gzip compressed data, was "expyvalidations-0.0.4.tar", last modified: Tue Apr 23 00:08:06 2024, max compression
```

## Comparing `expyvalidations-0.0.2.tar` & `expyvalidations-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,34 @@
-drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     1071 2024-03-27 18:40:13.000000 expyvalidations-0.0.2/LICENSE
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      753 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/PKG-INFO
-drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/expyvalidations/
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       64 2024-04-10 17:22:11.000000 expyvalidations-0.0.2/expyvalidations/__init__.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      631 2024-04-09 22:31:52.000000 expyvalidations-0.0.2/expyvalidations/config.py
-drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/expyvalidations/excel/
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-03-27 18:27:29.000000 expyvalidations-0.0.2/expyvalidations/excel/__init__.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     5309 2024-04-09 23:17:48.000000 expyvalidations-0.0.2/expyvalidations/excel/checks.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)    11428 2024-04-09 23:16:18.000000 expyvalidations-0.0.2/expyvalidations/excel/excel.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      763 2024-04-09 23:16:52.000000 expyvalidations-0.0.2/expyvalidations/excel/model.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     3117 2024-04-10 17:20:28.000000 expyvalidations-0.0.2/expyvalidations/excel/servicos.py
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     9192 2024-04-09 21:58:11.000000 expyvalidations-0.0.2/expyvalidations/utils.py
-drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/expyvalidations.egg-info/
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      753 2024-04-10 17:22:19.000000 expyvalidations-0.0.2/expyvalidations.egg-info/PKG-INFO
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      499 2024-04-10 17:22:19.000000 expyvalidations-0.0.2/expyvalidations.egg-info/SOURCES.txt
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        1 2024-04-10 17:22:19.000000 expyvalidations-0.0.2/expyvalidations.egg-info/dependency_links.txt
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        1 2024-03-31 18:59:43.000000 expyvalidations-0.0.2/expyvalidations.egg-info/not-zip-safe
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       56 2024-04-10 17:22:19.000000 expyvalidations-0.0.2/expyvalidations.egg-info/requires.txt
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       16 2024-04-10 17:22:19.000000 expyvalidations-0.0.2/expyvalidations.egg-info/top_level.txt
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       38 2024-04-10 17:22:19.819889 expyvalidations-0.0.2/setup.cfg
--rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     1357 2024-03-31 19:06:08.000000 expyvalidations-0.0.2/setup.py
+drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-23 00:08:06.975979 expyvalidations-0.0.4/
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     1071 2024-03-27 18:40:13.000000 expyvalidations-0.0.4/LICENSE
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     3217 2024-04-23 00:08:06.975979 expyvalidations-0.0.4/PKG-INFO
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     2333 2024-04-17 22:47:28.000000 expyvalidations-0.0.4/README.md
+drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-23 00:08:06.975979 expyvalidations-0.0.4/expyvalidations/
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      106 2024-04-23 00:00:34.000000 expyvalidations-0.0.4/expyvalidations/__init__.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      365 2024-04-21 19:08:48.000000 expyvalidations-0.0.4/expyvalidations/config.py
+drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-23 00:08:06.975979 expyvalidations-0.0.4/expyvalidations/excel/
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-03-27 18:27:29.000000 expyvalidations-0.0.4/expyvalidations/excel/__init__.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)    15423 2024-04-22 23:51:02.000000 expyvalidations-0.0.4/expyvalidations/excel/excel.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      782 2024-04-21 19:24:27.000000 expyvalidations-0.0.4/expyvalidations/excel/models.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       93 2024-04-21 17:05:06.000000 expyvalidations-0.0.4/expyvalidations/exceptions.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      651 2024-04-21 19:12:07.000000 expyvalidations-0.0.4/expyvalidations/utils.py
+drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-23 00:08:06.975979 expyvalidations-0.0.4/expyvalidations/validations/
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-21 18:08:06.000000 expyvalidations-0.0.4/expyvalidations/validations/__init__.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      495 2024-04-21 18:43:40.000000 expyvalidations-0.0.4/expyvalidations/validations/bool.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      500 2024-04-17 23:23:41.000000 expyvalidations-0.0.4/expyvalidations/validations/cel.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      866 2024-04-21 18:16:55.000000 expyvalidations-0.0.4/expyvalidations/validations/cpf.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      726 2024-04-21 18:11:19.000000 expyvalidations-0.0.4/expyvalidations/validations/date.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     1288 2024-04-21 19:50:45.000000 expyvalidations-0.0.4/expyvalidations/validations/duplications.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      471 2024-04-21 16:15:43.000000 expyvalidations-0.0.4/expyvalidations/validations/email.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      658 2024-04-21 17:07:39.000000 expyvalidations-0.0.4/expyvalidations/validations/float.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      507 2024-04-21 17:33:37.000000 expyvalidations-0.0.4/expyvalidations/validations/int.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      282 2024-04-21 18:25:45.000000 expyvalidations-0.0.4/expyvalidations/validations/sex.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      145 2024-04-21 16:17:36.000000 expyvalidations-0.0.4/expyvalidations/validations/string.py
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      859 2024-04-21 18:28:01.000000 expyvalidations-0.0.4/expyvalidations/validations/time.py
+drwxrwxr-x   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        0 2024-04-23 00:08:06.975979 expyvalidations-0.0.4/expyvalidations.egg-info/
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     3217 2024-04-23 00:08:06.000000 expyvalidations-0.0.4/expyvalidations.egg-info/PKG-INFO
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)      880 2024-04-23 00:08:06.000000 expyvalidations-0.0.4/expyvalidations.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)        1 2024-04-23 00:08:06.000000 expyvalidations-0.0.4/expyvalidations.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       50 2024-04-23 00:08:06.000000 expyvalidations-0.0.4/expyvalidations.egg-info/requires.txt
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       16 2024-04-23 00:08:06.000000 expyvalidations-0.0.4/expyvalidations.egg-info/top_level.txt
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)       38 2024-04-23 00:08:06.975979 expyvalidations-0.0.4/setup.cfg
+-rw-rw-r--   0 ezequielmendonca  (1001) ezequielmendonca  (1001)     1517 2024-04-17 22:54:05.000000 expyvalidations-0.0.4/setup.py
```

### Comparing `expyvalidations-0.0.2/LICENSE` & `expyvalidations-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `expyvalidations-0.0.2/expyvalidations/excel/model.py` & `expyvalidations-0.0.4/expyvalidations/excel/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from enum import Enum
-from logging import WARNING
 from typing import Any, Callable
 from pydantic import BaseModel, Field
 
+
 class Types(Enum):
     STRING = "string"
     INTEGER = "int"
     FLOAT = "float"
     TIME = "time"
     BOOL = "bool"
     DATE = "date"
     EMAIL = "email"
     PHONE = "cel"
     CPF = "cpf"
     SEX = "sex"
 
+
 class TypeError(Enum):
     WARNING = "Warning"
     ERROR = "ERROR"
     DUPLICATED = "Duplication"
+    CRITICAL = "CRITICAL"
 
 
 class Error(BaseModel):
     row: int
     column: str | None
     type: TypeError = TypeError.ERROR
     message: str
 
 
 class ColumnDefinition(BaseModel):
     key: str
-    types: str
     default: Any = None
+    function_validation: Callable
     custom_function_before: Callable | None = Field(default=None)
     custom_function_after: Callable | None = Field(default=None)
```

### Comparing `expyvalidations-0.0.2/setup.py` & `expyvalidations-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,38 +11,42 @@
 
 if os.path.isdir(dist_dir):
     shutil.rmtree(dist_dir)
 
 if os.path.isdir(build_dir):
     shutil.rmtree(build_dir)
 
-# with open("README.md", "r", encoding="utf-8") as fh:
-#     long_description = fh.read()
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="expyvalidations",
     packages=setuptools.find_packages(),
     version=__version__,
     description="Sheets data validation",
-    # long_description=long_description,
+    long_description=long_description,
     long_description_content_type="text/markdown",
     author="exebixel",
     author_email="ezequielnat7@gmail.com",
     url="https://github.com/exebixel/expyvalidations",
+    license='MIT',
     install_requires=requirements,
     python_requires=">=3.7",
     classifiers=[
         "Operating System :: OS Independent",
         "Environment :: Console",
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
-    zip_safe=False,
+    project_urls={
+        "Documentation": "https://github.com/exebixel/expyvalidations/wiki",
+        "Source": "https://github.com/exebixel/expyvalidations",
+    }
 )
```

