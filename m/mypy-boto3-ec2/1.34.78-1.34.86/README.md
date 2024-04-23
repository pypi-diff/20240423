# Comparing `tmp/mypy-boto3-ec2-1.34.78.tar.gz` & `tmp/mypy_boto3_ec2-1.34.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ec2-1.34.78.tar", last modified: Thu Apr  4 19:33:16 2024, max compression
+gzip compressed data, was "mypy_boto3_ec2-1.34.86.tar", last modified: Wed Apr 17 19:47:43 2024, max compression
```

## Comparing `mypy-boto3-ec2-1.34.78.tar` & `mypy_boto3_ec2-1.34.86.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:16.864019 mypy-boto3-ec2-1.34.78/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 19:32:30.000000 mypy-boto3-ec2-1.34.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-04 19:33:16.864019 mypy-boto3-ec2-1.34.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    48950 2024-04-04 19:32:30.000000 mypy-boto3-ec2-1.34.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:16.864019 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/
--rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-04-04 19:32:30.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-04-04 19:32:30.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 19:32:30.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   542226 2024-04-04 19:32:37.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   542223 2024-04-04 19:32:34.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    96819 2024-04-04 19:32:44.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    96819 2024-04-04 19:32:44.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   187422 2024-04-04 19:32:42.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)   187279 2024-04-04 19:32:41.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 19:32:30.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   271947 2024-04-04 19:32:40.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)   271869 2024-04-04 19:32:39.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   869264 2024-04-04 19:33:00.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   869264 2024-04-04 19:32:55.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 19:32:30.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-04-04 19:32:42.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    39737 2024-04-04 19:32:42.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 19:33:16.864019 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-04 19:33:16.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-04 19:33:16.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:16.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 19:33:16.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-04 19:33:16.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 19:33:16.000000 mypy-boto3-ec2-1.34.78/mypy_boto3_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 19:33:16.864019 mypy-boto3-ec2-1.34.78/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-04 19:32:30.000000 mypy-boto3-ec2-1.34.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:43.873910 mypy_boto3_ec2-1.34.86/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-17 19:47:43.873910 mypy_boto3_ec2-1.34.86/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    48950 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:43.869910 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47454 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   542214 2024-04-17 19:47:05.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   542211 2024-04-17 19:47:02.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    96841 2024-04-17 19:47:12.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96841 2024-04-17 19:47:12.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   187422 2024-04-17 19:47:10.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   187279 2024-04-17 19:47:10.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   271947 2024-04-17 19:47:08.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)   271869 2024-04-17 19:47:07.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   869264 2024-04-17 19:47:29.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   869264 2024-04-17 19:47:23.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39773 2024-04-17 19:47:11.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39737 2024-04-17 19:47:11.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:47:43.873910 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    50489 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 19:47:43.000000 mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:47:43.873910 mypy_boto3_ec2-1.34.86/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-17 19:46:59.000000 mypy_boto3_ec2-1.34.86/setup.py
```

### Comparing `mypy-boto3-ec2-1.34.78/LICENSE` & `mypy_boto3_ec2-1.34.86/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/PKG-INFO` & `mypy_boto3_ec2-1.34.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.34.78
-Summary: Type annotations for boto3.EC2 1.34.78 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.86
+Summary: Type annotations for boto3.EC2 1.34.86 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ec2-1.34.78/README.md` & `mypy_boto3_ec2-1.34.86/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/__init__.py` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/__init__.pyi` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/__main__.py` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EC2 1.34.78\n"
-        "Version:         1.34.78\n"
+        "Type annotations for boto3.EC2 1.34.86\n"
+        "Version:         1.34.86\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.78")
+    print("1.34.86")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/client.py` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4971,15 +4971,15 @@
         DryRun: bool = ...,
         LocationType: LocationTypeType = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
     ) -> DescribeInstanceTypeOfferingsResultTypeDef:
         """
-        Returns a list of all instance types offered.
+        Lists the instance types that are offered for the specified location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_instance_type_offerings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#describe_instance_type_offerings)
         """
 
     def describe_instance_types(
         self,
@@ -4987,15 +4987,15 @@
         DryRun: bool = ...,
         InstanceTypes: Sequence[InstanceTypeType] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
     ) -> DescribeInstanceTypesResultTypeDef:
         """
-        Describes the details of the instance types that are offered in a location.
+        Describes the specified instance types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_instance_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#describe_instance_types)
         """
 
     def describe_instances(
         self,
```

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/client.pyi` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4968,15 +4968,15 @@
         DryRun: bool = ...,
         LocationType: LocationTypeType = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
     ) -> DescribeInstanceTypeOfferingsResultTypeDef:
         """
-        Returns a list of all instance types offered.
+        Lists the instance types that are offered for the specified location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_instance_type_offerings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#describe_instance_type_offerings)
         """
 
     def describe_instance_types(
         self,
@@ -4984,15 +4984,15 @@
         DryRun: bool = ...,
         InstanceTypes: Sequence[InstanceTypeType] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
     ) -> DescribeInstanceTypesResultTypeDef:
         """
-        Describes the details of the instance types that are offered in a location.
+        Describes the specified instance types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.describe_instance_types)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/client/#describe_instance_types)
         """
 
     def describe_instances(
         self,
```

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/literals.py` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -2490,14 +2490,15 @@
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
```

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/literals.pyi` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2490,14 +2490,15 @@
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
```

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/paginator.py` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/paginator.pyi` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/service_resource.py` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/service_resource.pyi` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/type_defs.py` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/type_defs.pyi` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/waiter.py` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2/waiter.pyi` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2.egg-info/PKG-INFO` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.34.78
-Summary: Type annotations for boto3.EC2 1.34.78 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.86
+Summary: Type annotations for boto3.EC2 1.34.86 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ec2.svg?color=blue)](https://pypi.org/project/mypy-boto3-ec2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ec2)](https://pepy.tech/project/mypy-boto3-ec2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EC2 1.34.78](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
+[boto3.EC2 1.34.86](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-ec2-1.34.78/mypy_boto3_ec2.egg-info/SOURCES.txt` & `mypy_boto3_ec2-1.34.86/mypy_boto3_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.34.78/setup.py` & `mypy_boto3_ec2-1.34.86/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ec2",
-    version="1.34.78",
+    version="1.34.86",
     packages=["mypy_boto3_ec2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EC2 1.34.78 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.EC2 1.34.86 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

