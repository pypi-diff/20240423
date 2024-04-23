# Comparing `tmp/pulumi_ns1-3.3.0a1713561640.tar.gz` & `tmp/pulumi_ns1-3.3.0a1713900531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_ns1-3.3.0a1713561640.tar", last modified: Fri Apr 19 21:27:13 2024, max compression
+gzip compressed data, was "pulumi_ns1-3.3.0a1713900531.tar", last modified: Tue Apr 23 19:58:39 2024, max compression
```

## Comparing `pulumi_ns1-3.3.0a1713561640.tar` & `pulumi_ns1-3.3.0a1713900531.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38901 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/account_whitelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    87418 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    12838 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/data_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)    11258 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/dnsview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_dns_sec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_monitoring_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9023 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    45912 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/monitoring_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/notify_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    46058 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17050 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/pulsar_job.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    44687 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    19239 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    81870 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/tsigkey.py
--rw-r--r--   0 runner    (1001) docker     (127)    89390 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    42852 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-19 21:27:13.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-19 21:27:13.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:27:13.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:27:13.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 21:27:13.000000 pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 21:27:07.000000 pulumi_ns1-3.3.0a1713561640/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:27:13.666736 pulumi_ns1-3.3.0a1713561640/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:58:39.771608 pulumi_ns1-3.3.0a1713900531/
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-23 19:58:39.771608 pulumi_ns1-3.3.0a1713900531/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:58:39.767608 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38901 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/account_whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87262 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16619 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:58:39.771608 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12682 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11102 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13624 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/dnsview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/get_dns_sec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/get_monitoring_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/get_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8883 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/get_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45756 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/monitoring_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11069 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/notify_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46058 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17050 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/pulsar_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    44531 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19239 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81714 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/tsigkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89234 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42852 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:58:39.771608 pulumi_ns1-3.3.0a1713900531/pulumi_ns1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-23 19:58:39.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-23 19:58:39.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:58:39.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 19:58:39.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 19:58:39.000000 pulumi_ns1-3.3.0a1713900531/pulumi_ns1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-23 19:58:33.000000 pulumi_ns1-3.3.0a1713900531/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:58:39.771608 pulumi_ns1-3.3.0a1713900531/setup.cfg
```

### Comparing `pulumi_ns1-3.3.0a1713561640/PKG-INFO` & `pulumi_ns1-3.3.0a1713900531/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ns1
-Version: 3.3.0a1713561640
+Version: 3.3.0a1713900531
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi,ns1
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ns1-3.3.0a1713561640/README.md` & `pulumi_ns1-3.3.0a1713900531/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/__init__.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/_inputs.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/_utilities.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/account_whitelist.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/account_whitelist.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,27 +101,25 @@
         """
         Provides a NS1 Global IP Whitelist resource.
 
         This can be used to create, modify, and delete Global IP Whitelists.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.AccountWhitelist("example",
             name="Example Whitelist",
             values=[
                 "1.1.1.1",
                 "2.2.2.2",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         > You current source IP must be present in one of the whitelists to prevent locking yourself out.
 
         ## NS1 Documentation
 
         [Global IP Whitelist Doc](https://ns1.com/api?docId=2282)
 
@@ -145,27 +143,25 @@
         """
         Provides a NS1 Global IP Whitelist resource.
 
         This can be used to create, modify, and delete Global IP Whitelists.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.AccountWhitelist("example",
             name="Example Whitelist",
             values=[
                 "1.1.1.1",
                 "2.2.2.2",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         > You current source IP must be present in one of the whitelists to prevent locking yourself out.
 
         ## NS1 Documentation
 
         [Global IP Whitelist Doc](https://ns1.com/api?docId=2282)
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/api_key.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1140,15 +1140,14 @@
                  teams: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Provides a NS1 Api Key resource. This can be used to create, modify, and delete api keys.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.Team("example", name="Example team")
         example_api_key = ns1.APIKey("example",
             name="Example key",
@@ -1156,15 +1155,14 @@
             ip_whitelists=[
                 "1.1.1.1",
                 "2.2.2.2",
             ],
             dns_view_zones=False,
             account_manage_users=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Permissions
 
         An API key will inherit permissions from the teams it is assigned to.
         If a key is assigned to a team and also has individual permissions set on the key, the individual permissions
         will be overridden by the inherited team permissions.
         In a future release, setting permissions on a key that is part of a team will be explicitly disabled.
@@ -1238,15 +1236,14 @@
                  args: Optional[APIKeyArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a NS1 Api Key resource. This can be used to create, modify, and delete api keys.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.Team("example", name="Example team")
         example_api_key = ns1.APIKey("example",
             name="Example key",
@@ -1254,15 +1251,14 @@
             ip_whitelists=[
                 "1.1.1.1",
                 "2.2.2.2",
             ],
             dns_view_zones=False,
             account_manage_users=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Permissions
 
         An API key will inherit permissions from the teams it is assigned to.
         If a key is assigned to a team and also has individual permissions set on the key, the individual permissions
         will be overridden by the inherited team permissions.
         In a future release, setting permissions on a key that is part of a team will be explicitly disabled.
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/application.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/__init__.pyi` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/config/vars.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/data_feed.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/data_feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,14 @@
                  source_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a NS1 Data Feed resource. This can be used to create, modify, and delete data feeds.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.DataSource("example",
             name="example",
             sourcetype="nsone_v1")
@@ -166,15 +165,14 @@
         useast_monitor_feed = ns1.DataFeed("useast_monitor_feed",
             name="useast_monitor_feed",
             source_id=example_monitoring.id,
             config={
                 "jobid": example_job["id"],
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Datafeed Api Doc](https://ns1.com/api#data-feeds)
 
         ## Import
 
@@ -196,15 +194,14 @@
                  args: DataFeedArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a NS1 Data Feed resource. This can be used to create, modify, and delete data feeds.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.DataSource("example",
             name="example",
             sourcetype="nsone_v1")
@@ -226,15 +223,14 @@
         useast_monitor_feed = ns1.DataFeed("useast_monitor_feed",
             name="useast_monitor_feed",
             source_id=example_monitoring.id,
             config={
                 "jobid": example_job["id"],
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Datafeed Api Doc](https://ns1.com/api#data-feeds)
 
         ## Import
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/data_source.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,24 +136,22 @@
                  sourcetype: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a NS1 Data Source resource. This can be used to create, modify, and delete data sources.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.DataSource("example",
             name="example",
             sourcetype="nsone_v1")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Datasource Api Doc](https://ns1.com/api#data-sources)
 
         ## Import
 
@@ -175,24 +173,22 @@
                  args: DataSourceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a NS1 Data Source resource. This can be used to create, modify, and delete data sources.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.DataSource("example",
             name="example",
             sourcetype="nsone_v1")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Datasource Api Doc](https://ns1.com/api#data-sources)
 
         ## Import
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/dataset.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/dataset.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/dnsview.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/dnsview.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_dns_sec.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/get_dns_sec.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,26 +82,24 @@
 def get_dns_sec(zone: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDNSSecResult:
     """
     Provides DNSSEC details about a NS1 Zone.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get DNSSEC details about a NS1 Zone.
     example_zone = ns1.Zone("example",
         zone="terraform.example.io",
         dnssec=True)
     example = ns1.get_dns_sec_output(zone=example_zone.zone)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str zone: The name of the zone to get DNSSEC details for.
     """
     __args__ = dict()
     __args__['zone'] = zone
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
@@ -118,24 +116,22 @@
 def get_dns_sec_output(zone: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDNSSecResult]:
     """
     Provides DNSSEC details about a NS1 Zone.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get DNSSEC details about a NS1 Zone.
     example_zone = ns1.Zone("example",
         zone="terraform.example.io",
         dnssec=True)
     example = ns1.get_dns_sec_output(zone=example_zone.zone)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str zone: The name of the zone to get DNSSEC details for.
     """
     ...
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_monitoring_regions.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/get_monitoring_regions.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,23 +62,21 @@
 def get_monitoring_regions(regions: Optional[Sequence[pulumi.InputType['GetMonitoringRegionsRegionArgs']]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetMonitoringRegionsResult:
     """
     Provides details of all available monitoring regions.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get details of all available monitoring regions.
     example = ns1.get_monitoring_regions()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetMonitoringRegionsRegionArgs']] regions: A set of the available monitoring regions. Regions is
            documented below.
     """
     __args__ = dict()
     __args__['regions'] = regions
@@ -94,22 +92,20 @@
 def get_monitoring_regions_output(regions: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetMonitoringRegionsRegionArgs']]]]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMonitoringRegionsResult]:
     """
     Provides details of all available monitoring regions.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get details of all available monitoring regions.
     example = ns1.get_monitoring_regions()
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[pulumi.InputType['GetMonitoringRegionsRegionArgs']] regions: A set of the available monitoring regions. Regions is
            documented below.
     """
     ...
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_networks.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/get_networks.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,23 +62,21 @@
     """
     Provides details about NS1 Networks. Use this if you would simply like to read
     information from NS1 into your configurations. For read/write operations, you
     should use a resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get details about NS1 Networks.
     example = ns1.get_networks()
     ```
-    <!--End PulumiCodeChooser -->
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('ns1:index/getNetworks:getNetworks', __args__, opts=opts, typ=GetNetworksResult).value
 
     return AwaitableGetNetworksResult(
         id=pulumi.get(__ret__, 'id'),
@@ -90,18 +88,16 @@
     """
     Provides details about NS1 Networks. Use this if you would simply like to read
     information from NS1 into your configurations. For read/write operations, you
     should use a resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get details about NS1 Networks.
     example = ns1.get_networks()
     ```
-    <!--End PulumiCodeChooser -->
     """
     ...
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_record.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/get_record.py`

 * *Files 6% similar despite different names*

```diff
@@ -190,25 +190,23 @@
     """
     Provides details about a NS1 Record. Use this if you would simply like to read
     information from NS1 into your configurations. For read/write operations, you
     should use a resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get details about a NS1 Record.
     example = ns1.get_record(zone="example.io",
         domain="terraform.example.io",
         type="A")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str domain: The records' domain.
     :param str type: The records' RR type.
     :param str zone: The zone the record belongs to.
     """
     __args__ = dict()
@@ -243,25 +241,23 @@
     """
     Provides details about a NS1 Record. Use this if you would simply like to read
     information from NS1 into your configurations. For read/write operations, you
     should use a resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get details about a NS1 Record.
     example = ns1.get_record(zone="example.io",
         domain="terraform.example.io",
         type="A")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str domain: The records' domain.
     :param str type: The records' RR type.
     :param str zone: The zone the record belongs to.
     """
     ...
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/get_zone.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/get_zone.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,23 +248,21 @@
     """
     Provides details about a NS1 Zone. Use this if you would simply like to read
     information from NS1 into your configurations. For read/write operations, you
     should use a resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get details about a NS1 Zone.
     example = ns1.get_zone(zone="terraform.example.io")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] additional_primaries: List of additional IPv4 addresses for the primary
            zone.
     :param str zone: The domain name of the zone.
     """
     __args__ = dict()
@@ -305,23 +303,21 @@
     """
     Provides details about a NS1 Zone. Use this if you would simply like to read
     information from NS1 into your configurations. For read/write operations, you
     should use a resource.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_ns1 as ns1
 
     # Get details about a NS1 Zone.
     example = ns1.get_zone(zone="terraform.example.io")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param Sequence[str] additional_primaries: List of additional IPv4 addresses for the primary
            zone.
     :param str zone: The domain name of the zone.
     """
     ...
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/monitoring_job.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/monitoring_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,15 +560,14 @@
                  rules: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['MonitoringJobRuleArgs']]]]] = None,
                  __props__=None):
         """
         Provides a NS1 Monitoring Job resource. This can be used to create, modify, and delete monitoring jobs.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         uswest_monitor = ns1.MonitoringJob("uswest_monitor",
             name="uswest",
             active=True,
@@ -590,15 +589,14 @@
             },
             rules=[ns1.MonitoringJobRuleArgs(
                 value="200 OK",
                 comparison="contains",
                 key="output",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [MonitoringJob Api Doc](https://ns1.com/api#monitoring-jobs)
 
         ## Import
 
@@ -633,15 +631,14 @@
                  args: MonitoringJobArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a NS1 Monitoring Job resource. This can be used to create, modify, and delete monitoring jobs.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         uswest_monitor = ns1.MonitoringJob("uswest_monitor",
             name="uswest",
             active=True,
@@ -663,15 +660,14 @@
             },
             rules=[ns1.MonitoringJobRuleArgs(
                 value="200 OK",
                 comparison="contains",
                 key="output",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [MonitoringJob Api Doc](https://ns1.com/api#monitoring-jobs)
 
         ## Import
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/notify_list.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/notify_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,15 +102,14 @@
                  notifications: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotifyListNotificationArgs']]]]] = None,
                  __props__=None):
         """
         Provides a NS1 Notify List resource. This can be used to create, modify, and delete notify lists.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         nl = ns1.NotifyList("nl",
             name="my notify list",
             notifications=[
@@ -124,15 +123,14 @@
                     type="email",
                     config={
                         "email": "test@test.com",
                     },
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [NotifyList Api Doc](https://ns1.com/api#notification-lists)
 
         ## Import
 
@@ -152,15 +150,14 @@
                  args: Optional[NotifyListArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a NS1 Notify List resource. This can be used to create, modify, and delete notify lists.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         nl = ns1.NotifyList("nl",
             name="my notify list",
             notifications=[
@@ -174,15 +171,14 @@
                     type="email",
                     config={
                         "email": "test@test.com",
                     },
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [NotifyList Api Doc](https://ns1.com/api#notification-lists)
 
         ## Import
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/outputs.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/provider.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/pulsar_job.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/pulsar_job.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/record.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/record.py`

 * *Files 1% similar despite different names*

```diff
@@ -511,15 +511,14 @@
                  zone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a NS1 Record resource. This can be used to create, modify, and delete records.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_external as external
         import pulumi_ns1 as ns1
         import pulumi_std as std
 
@@ -619,15 +618,14 @@
                 search="/(^\\\\.)|(\\\\.$)/",
                 replace="").result,
             domain=std.replace(text=domain,
                 search="/(^\\\\.)|(\\\\.$)/",
                 replace="").result,
             type="CNAME")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Record Api Doc](https://ns1.com/api#records)
 
         ## Import
 
@@ -671,15 +669,14 @@
                  args: RecordArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a NS1 Record resource. This can be used to create, modify, and delete records.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import json
         import pulumi_external as external
         import pulumi_ns1 as ns1
         import pulumi_std as std
 
@@ -779,15 +776,14 @@
                 search="/(^\\\\.)|(\\\\.$)/",
                 replace="").result,
             domain=std.replace(text=domain,
                 search="/(^\\\\.)|(\\\\.$)/",
                 replace="").result,
             type="CNAME")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Record Api Doc](https://ns1.com/api#records)
 
         ## Import
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/subnet.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/team.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/team.py`

 * *Files 1% similar despite different names*

```diff
@@ -1059,15 +1059,14 @@
                  __props__=None):
         """
         Provides a NS1 Team resource. This can be used to create, modify, and delete
         teams. The credentials used must have the `manage_teams` permission set.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         # Create a new NS1 Team
         example = ns1.Team("example",
             name="Example team",
@@ -1100,15 +1099,14 @@
                 domain="terraform.example.io",
                 include_subdomains=False,
                 zone="example.io",
                 type="A",
             )],
             data_manage_datasources=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Team Api Docs](https://ns1.com/api#team)
 
         ## Import
 
@@ -1162,15 +1160,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a NS1 Team resource. This can be used to create, modify, and delete
         teams. The credentials used must have the `manage_teams` permission set.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         # Create a new NS1 Team
         example = ns1.Team("example",
             name="Example team",
@@ -1203,15 +1200,14 @@
                 domain="terraform.example.io",
                 include_subdomains=False,
                 zone="example.io",
                 type="A",
             )],
             data_manage_datasources=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## NS1 Documentation
 
         [Team Api Docs](https://ns1.com/api#team)
 
         ## Import
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/tsigkey.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/tsigkey.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,25 +131,23 @@
                  secret: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a NS1 TSIG Key resource. This can be used to create, modify, and delete TSIG keys.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.Tsigkey("example",
             name="ExampleTsigKey",
             algorithm="hmac-sha256",
             secret="Ok1qR5IW1ajVka5cHPEJQIXfLyx5V3PSkFBROAzOn21JumDq6nIpoj6H8rfj5Uo+Ok55ZWQ0Wgrf302fDscHLA==")
         ```
-        <!--End PulumiCodeChooser -->
         ## NS1 Documentation
 
         [TSIG Keys Api Doc](https://ns1.com/api/#tsig)
 
         ## Import
 
         ```sh
@@ -169,25 +167,23 @@
                  args: TsigkeyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a NS1 TSIG Key resource. This can be used to create, modify, and delete TSIG keys.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.Tsigkey("example",
             name="ExampleTsigKey",
             algorithm="hmac-sha256",
             secret="Ok1qR5IW1ajVka5cHPEJQIXfLyx5V3PSkFBROAzOn21JumDq6nIpoj6H8rfj5Uo+Ok55ZWQ0Wgrf302fDscHLA==")
         ```
-        <!--End PulumiCodeChooser -->
         ## NS1 Documentation
 
         [TSIG Keys Api Doc](https://ns1.com/api/#tsig)
 
         ## Import
 
         ```sh
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/user.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1195,15 +1195,14 @@
         """
         Provides a NS1 User resource. Creating a user sends an invitation email to the
         user's email address. This can be used to create, modify, and delete users.
         The credentials used must have the `manage_users` permission set.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.Team("example",
             name="Example team",
             ip_whitelists=[
@@ -1217,15 +1216,14 @@
             username="example_user",
             email="user@example.com",
             teams=[example.id],
             notify={
                 "billing": False,
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Permissions
 
         A user will inherit permissions from the teams they are assigned to.
         If a user is assigned to a team and also has individual permissions set on the user, the individual permissions
         will be overridden by the inherited team permissions.
         In a future release, setting permissions on a user that is part of a team will be explicitly disabled.
@@ -1296,15 +1294,14 @@
         """
         Provides a NS1 User resource. Creating a user sends an invitation email to the
         user's email address. This can be used to create, modify, and delete users.
         The credentials used must have the `manage_users` permission set.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_ns1 as ns1
 
         example = ns1.Team("example",
             name="Example team",
             ip_whitelists=[
@@ -1318,15 +1315,14 @@
             username="example_user",
             email="user@example.com",
             teams=[example.id],
             notify={
                 "billing": False,
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Permissions
 
         A user will inherit permissions from the teams they are assigned to.
         If a user is assigned to a team and also has individual permissions set on the user, the individual permissions
         will be overridden by the inherited team permissions.
         In a future release, setting permissions on a user that is part of a team will be explicitly disabled.
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1/zone.py` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/PKG-INFO` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_ns1
-Version: 3.3.0a1713561640
+Version: 3.3.0a1713900531
 Summary: A Pulumi package for creating and managing ns1 cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-ns1
 Keywords: pulumi,ns1
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_ns1-3.3.0a1713561640/pulumi_ns1.egg-info/SOURCES.txt` & `pulumi_ns1-3.3.0a1713900531/pulumi_ns1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_ns1-3.3.0a1713561640/pyproject.toml` & `pulumi_ns1-3.3.0a1713900531/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_ns1"
   description = "A Pulumi package for creating and managing ns1 cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "ns1"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.3.0a1713561640"
+  version = "3.3.0a1713900531"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-ns1"
 
 [build-system]
```

