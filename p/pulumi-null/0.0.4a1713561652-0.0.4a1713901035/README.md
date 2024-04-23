# Comparing `tmp/pulumi_null-0.0.4a1713561652.tar.gz` & `tmp/pulumi_null-0.0.4a1713901035.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_null-0.0.4a1713561652.tar", last modified: Fri Apr 19 21:30:12 2024, max compression
+gzip compressed data, was "pulumi_null-0.0.4a1713901035.tar", last modified: Tue Apr 23 20:00:50 2024, max compression
```

## Comparing `pulumi_null-0.0.4a1713561652.tar` & `pulumi_null-0.0.4a1713901035.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:12.467425 pulumi_null-0.0.4a1713561652/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-19 21:30:12.467425 pulumi_null-0.0.4a1713561652/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-19 21:30:05.000000 pulumi_null-0.0.4a1713561652/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:12.467425 pulumi_null-0.0.4a1713561652/pulumi_null/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-19 21:30:05.000000 pulumi_null-0.0.4a1713561652/pulumi_null/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:30:05.000000 pulumi_null-0.0.4a1713561652/pulumi_null/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-04-19 21:30:05.000000 pulumi_null-0.0.4a1713561652/pulumi_null/get_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-19 21:30:05.000000 pulumi_null-0.0.4a1713561652/pulumi_null/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 21:30:05.000000 pulumi_null-0.0.4a1713561652/pulumi_null/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:05.000000 pulumi_null-0.0.4a1713561652/pulumi_null/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2024-04-19 21:30:05.000000 pulumi_null-0.0.4a1713561652/pulumi_null/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:30:12.467425 pulumi_null-0.0.4a1713561652/pulumi_null.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-19 21:30:12.000000 pulumi_null-0.0.4a1713561652/pulumi_null.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 21:30:12.000000 pulumi_null-0.0.4a1713561652/pulumi_null.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:30:12.000000 pulumi_null-0.0.4a1713561652/pulumi_null.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:30:12.000000 pulumi_null-0.0.4a1713561652/pulumi_null.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 21:30:12.000000 pulumi_null-0.0.4a1713561652/pulumi_null.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-19 21:30:05.000000 pulumi_null-0.0.4a1713561652/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:30:12.467425 pulumi_null-0.0.4a1713561652/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:50.915794 pulumi_null-0.0.4a1713901035/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-23 20:00:50.915794 pulumi_null-0.0.4a1713901035/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-23 20:00:44.000000 pulumi_null-0.0.4a1713901035/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:50.911794 pulumi_null-0.0.4a1713901035/pulumi_null/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-23 20:00:44.000000 pulumi_null-0.0.4a1713901035/pulumi_null/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 20:00:44.000000 pulumi_null-0.0.4a1713901035/pulumi_null/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-04-23 20:00:44.000000 pulumi_null-0.0.4a1713901035/pulumi_null/get_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-23 20:00:44.000000 pulumi_null-0.0.4a1713901035/pulumi_null/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 20:00:44.000000 pulumi_null-0.0.4a1713901035/pulumi_null/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:44.000000 pulumi_null-0.0.4a1713901035/pulumi_null/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-23 20:00:44.000000 pulumi_null-0.0.4a1713901035/pulumi_null/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:00:50.915794 pulumi_null-0.0.4a1713901035/pulumi_null.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-04-23 20:00:50.000000 pulumi_null-0.0.4a1713901035/pulumi_null.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-23 20:00:50.000000 pulumi_null-0.0.4a1713901035/pulumi_null.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:00:50.000000 pulumi_null-0.0.4a1713901035/pulumi_null.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 20:00:50.000000 pulumi_null-0.0.4a1713901035/pulumi_null.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 20:00:50.000000 pulumi_null-0.0.4a1713901035/pulumi_null.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-23 20:00:44.000000 pulumi_null-0.0.4a1713901035/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:00:50.915794 pulumi_null-0.0.4a1713901035/setup.cfg
```

### Comparing `pulumi_null-0.0.4a1713561652/PKG-INFO` & `pulumi_null-0.0.4a1713901035/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_null
-Version: 0.0.4a1713561652
+Version: 0.0.4a1713901035
 Summary: A Pulumi package for creating and managing Null cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-null
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_null-0.0.4a1713561652/README.md` & `pulumi_null-0.0.4a1713901035/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1713561652/pulumi_null/__init__.py` & `pulumi_null-0.0.4a1713901035/pulumi_null/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1713561652/pulumi_null/_utilities.py` & `pulumi_null-0.0.4a1713901035/pulumi_null/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1713561652/pulumi_null/get_data_source.py` & `pulumi_null-0.0.4a1713901035/pulumi_null/get_data_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1713561652/pulumi_null/provider.py` & `pulumi_null-0.0.4a1713901035/pulumi_null/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_null-0.0.4a1713561652/pulumi_null/resource.py` & `pulumi_null-0.0.4a1713901035/pulumi_null/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,14 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  triggers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_aws as aws
         import pulumi_null as null
         import pulumi_std as std
 
         cluster = []
@@ -90,30 +89,28 @@
         # map, the null_resource will be replaced each time the instance ids
         # change, and thus the remote-exec provisioner will be re-run.
         cluster_resource = null.Resource("cluster", triggers={
             "cluster_instance_ids": std.join(separator=",",
                 input=[__item["id"] for __item in cluster]).result,
         })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: A map of arbitrary strings that, when changed, will force the null resource to be replaced, re-running any associated provisioners.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ResourceArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_aws as aws
         import pulumi_null as null
         import pulumi_std as std
 
         cluster = []
@@ -130,15 +127,14 @@
         # map, the null_resource will be replaced each time the instance ids
         # change, and thus the remote-exec provisioner will be re-run.
         cluster_resource = null.Resource("cluster", triggers={
             "cluster_instance_ids": std.join(separator=",",
                 input=[__item["id"] for __item in cluster]).result,
         })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ResourceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_null-0.0.4a1713561652/pulumi_null.egg-info/PKG-INFO` & `pulumi_null-0.0.4a1713901035/pulumi_null.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_null
-Version: 0.0.4a1713561652
+Version: 0.0.4a1713901035
 Summary: A Pulumi package for creating and managing Null cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com/
 Project-URL: Repository, https://github.com/pulumi/pulumi-null
 Keywords: pulumi,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_null-0.0.4a1713561652/pyproject.toml` & `pulumi_null-0.0.4a1713901035/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_null"
   description = "A Pulumi package for creating and managing Null cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.4a1713561652"
+  version = "0.0.4a1713901035"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com/"
     Repository = "https://github.com/pulumi/pulumi-null"
 
 [build-system]
```

