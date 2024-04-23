# Comparing `tmp/mypy-boto3-ce-1.34.71.tar.gz` & `tmp/mypy_boto3_ce-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ce-1.34.71.tar", last modified: Tue Mar 26 19:32:58 2024, max compression
+gzip compressed data, was "mypy_boto3_ce-1.34.90.tar", last modified: Tue Apr 23 19:34:20 2024, max compression
```

## Comparing `mypy-boto3-ce-1.34.71.tar` & `mypy_boto3_ce-1.34.90.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:57.996915 mypy-boto3-ce-1.34.71/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-26 19:31:58.000000 mypy-boto3-ce-1.34.71/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-03-26 19:32:57.996915 mypy-boto3-ce-1.34.71/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-03-26 19:31:58.000000 mypy-boto3-ce-1.34.71/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:57.992915 mypy-boto3-ce-1.34.71/mypy_boto3_ce/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 19:31:58.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-26 19:31:58.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-26 19:31:58.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34811 2024-03-26 19:31:59.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34808 2024-03-26 19:31:58.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13502 2024-03-26 19:31:59.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13502 2024-03-26 19:31:59.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 19:31:58.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    62442 2024-03-26 19:32:00.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    62442 2024-03-26 19:32:00.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-26 19:31:58.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 19:32:57.996915 mypy-boto3-ce-1.34.71/mypy_boto3_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-03-26 19:32:57.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-26 19:32:57.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:32:57.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 19:32:57.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 19:32:57.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 19:32:57.000000 mypy-boto3-ce-1.34.71/mypy_boto3_ce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 19:32:57.996915 mypy-boto3-ce-1.34.71/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-03-26 19:31:58.000000 mypy-boto3-ce-1.34.71/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.640570 mypy_boto3_ce-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-23 19:34:20.640570 mypy_boto3_ce-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.636570 mypy_boto3_ce-1.34.90/mypy_boto3_ce/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34811 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34808 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13586 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13586 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    62490 2024-04-23 19:33:14.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62490 2024-04-23 19:33:14.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:20.640570 mypy_boto3_ce-1.34.90/mypy_boto3_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-23 19:34:20.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 19:34:20.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:20.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:20.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:20.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 19:34:20.000000 mypy_boto3_ce-1.34.90/mypy_boto3_ce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:20.640570 mypy_boto3_ce-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-23 19:33:13.000000 mypy_boto3_ce-1.34.90/setup.py
```

### Comparing `mypy-boto3-ce-1.34.71/LICENSE` & `mypy_boto3_ce-1.34.90/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.34.71/PKG-INFO` & `mypy_boto3_ce-1.34.90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.34.71
-Summary: Type annotations for boto3.CostExplorer 1.34.71 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.90
+Summary: Type annotations for boto3.CostExplorer 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.34.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ce-1.34.71/README.md` & `mypy_boto3_ce-1.34.90/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.34.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ce-1.34.71/mypy_boto3_ce/__main__.py` & `mypy_boto3_ce-1.34.90/mypy_boto3_ce/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostExplorer 1.34.71\n"
-        "Version:         1.34.71\n"
+        "Type annotations for boto3.CostExplorer 1.34.90\n"
+        "Version:         1.34.90\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.71")
+    print("1.34.90")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ce-1.34.71/mypy_boto3_ce/client.py` & `mypy_boto3_ce-1.34.90/mypy_boto3_ce/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.34.71/mypy_boto3_ce/client.pyi` & `mypy_boto3_ce-1.34.90/mypy_boto3_ce/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.34.71/mypy_boto3_ce/literals.py` & `mypy_boto3_ce-1.34.90/mypy_boto3_ce/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -271,24 +272,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -485,14 +488,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-ce-1.34.71/mypy_boto3_ce/literals.pyi` & `mypy_boto3_ce-1.34.90/mypy_boto3_ce/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -251,14 +251,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -271,24 +272,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -485,14 +488,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy-boto3-ce-1.34.71/mypy_boto3_ce/type_defs.py` & `mypy_boto3_ce-1.34.90/mypy_boto3_ce/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -585,14 +585,15 @@
     },
 )
 ReservationPurchaseRecommendationMetadataTypeDef = TypedDict(
     "ReservationPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": NotRequired[str],
         "GenerationTimestamp": NotRequired[str],
+        "AdditionalMetadata": NotRequired[str],
     },
 )
 ReservationAggregatesTypeDef = TypedDict(
     "ReservationAggregatesTypeDef",
     {
         "UtilizationPercentage": NotRequired[str],
         "UtilizationPercentageInUnits": NotRequired[str],
```

### Comparing `mypy-boto3-ce-1.34.71/mypy_boto3_ce/type_defs.pyi` & `mypy_boto3_ce-1.34.90/mypy_boto3_ce/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -585,14 +585,15 @@
     },
 )
 ReservationPurchaseRecommendationMetadataTypeDef = TypedDict(
     "ReservationPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": NotRequired[str],
         "GenerationTimestamp": NotRequired[str],
+        "AdditionalMetadata": NotRequired[str],
     },
 )
 ReservationAggregatesTypeDef = TypedDict(
     "ReservationAggregatesTypeDef",
     {
         "UtilizationPercentage": NotRequired[str],
         "UtilizationPercentageInUnits": NotRequired[str],
```

### Comparing `mypy-boto3-ce-1.34.71/mypy_boto3_ce.egg-info/PKG-INFO` & `mypy_boto3_ce-1.34.90/mypy_boto3_ce.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ce
-Version: 1.34.71
-Summary: Type annotations for boto3.CostExplorer 1.34.71 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.90
+Summary: Type annotations for boto3.CostExplorer 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ce.svg?color=blue)](https://pypi.org/project/mypy-boto3-ce)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ce/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ce)](https://pepy.tech/project/mypy-boto3-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostExplorer 1.34.71](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
+[boto3.CostExplorer 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ce-1.34.71/mypy_boto3_ce.egg-info/SOURCES.txt` & `mypy_boto3_ce-1.34.90/mypy_boto3_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ce-1.34.71/setup.py` & `mypy_boto3_ce-1.34.90/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ce",
-    version="1.34.71",
+    version="1.34.90",
     packages=["mypy_boto3_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CostExplorer 1.34.71 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.CostExplorer 1.34.90 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

