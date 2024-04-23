# Comparing `tmp/pulumi_splunk-1.3.0a1713561402.tar.gz` & `tmp/pulumi_splunk-1.3.0a1713904842.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_splunk-1.3.0a1713561402.tar", last modified: Fri Apr 19 21:22:16 2024, max compression
+gzip compressed data, was "pulumi_splunk-1.3.0a1713904842.tar", last modified: Tue Apr 23 20:46:38 2024, max compression
```

## Comparing `pulumi_splunk-1.3.0a1713561402.tar` & `pulumi_splunk-1.3.0a1713904842.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:16.216618 pulumi_splunk-1.3.0a1713561402/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-19 21:22:16.216618 pulumi_splunk-1.3.0a1713561402/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:16.212618 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   148655 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/admin_saml_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    38906 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/apps_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    22055 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/authentication_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    45992 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/authorization_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:16.216618 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    10194 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/configs_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/data_ui_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/generic_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/global_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)   155006 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23938 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    42272 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30131 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    19073 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_cooked.py
--rw-r--r--   0 runner    (1001) docker     (127)    36774 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    34401 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_udp.py
--rw-r--r--   0 runner    (1001) docker     (127)   127784 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44187 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    43639 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    32121 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    28027 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   514639 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/saved_searches.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk/sh_indexes_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:16.216618 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-19 21:22:16.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-19 21:22:16.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:22:16.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 21:22:16.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-19 21:22:16.000000 pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-19 21:22:09.000000 pulumi_splunk-1.3.0a1713561402/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:22:16.216618 pulumi_splunk-1.3.0a1713561402/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148655 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/admin_saml_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38750 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/apps_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21899 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/authentication_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45836 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/authorization_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/configs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/data_ui_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/generic_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24990 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/global_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154850 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23782 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42116 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29975 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_cooked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36618 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13939 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34245 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127784 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44031 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43483 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31965 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27871 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   514483 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/saved_searches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk/sh_indexes_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-23 20:46:38.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-23 20:46:38.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:46:38.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 20:46:38.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 20:46:38.000000 pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 20:46:31.000000 pulumi_splunk-1.3.0a1713904842/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:46:38.097815 pulumi_splunk-1.3.0a1713904842/setup.cfg
```

### Comparing `pulumi_splunk-1.3.0a1713561402/PKG-INFO` & `pulumi_splunk-1.3.0a1713904842/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1713561402
+Version: 1.3.0a1713904842
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi,splunk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_splunk-1.3.0a1713561402/README.md` & `pulumi_splunk-1.3.0a1713904842/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/__init__.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/_inputs.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/_utilities.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/admin_saml_groups.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/admin_saml_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,27 +102,25 @@
         """
         ## # Resource: AdminSamlGroups
 
         Manage external groups in an IdP response to internal Splunk roles.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         saml_group = splunk.AdminSamlGroups("saml-group",
             name="mygroup",
             roles=[
                 "admin",
                 "power",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         SAML groups can be imported using the id, e.g.
 
         ```sh
         $ pulumi import splunk:index/adminSamlGroups:AdminSamlGroups saml-group mygroup
@@ -142,27 +140,25 @@
         """
         ## # Resource: AdminSamlGroups
 
         Manage external groups in an IdP response to internal Splunk roles.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         saml_group = splunk.AdminSamlGroups("saml-group",
             name="mygroup",
             roles=[
                 "admin",
                 "power",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         SAML groups can be imported using the id, e.g.
 
         ```sh
         $ pulumi import splunk:index/adminSamlGroups:AdminSamlGroups saml-group mygroup
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/apps_local.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/apps_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -511,25 +511,23 @@
         """
         ## # Resource: AppsLocal
 
         Create, install and manage apps on your Splunk instance
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         amazon_connect_app = splunk.AppsLocal("amazon_connect_app",
             filename=True,
             name="/usr/home/amazon_connect_app_for_splunk-0.0.1.tar.gz",
             explicit_appname="amazon_connect_app_for_splunk")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['AppsLocalAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] auth: Splunkbase session token for operations like install and update that require login. Use auth or session when installing or updating an app through Splunkbase.
         :param pulumi.Input[str] author: For apps posted to Splunkbase, use your Splunk account username. For internal apps, include your name and contact information.
         :param pulumi.Input[bool] configured: Custom setup complete indication:
@@ -563,25 +561,23 @@
         """
         ## # Resource: AppsLocal
 
         Create, install and manage apps on your Splunk instance
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         amazon_connect_app = splunk.AppsLocal("amazon_connect_app",
             filename=True,
             name="/usr/home/amazon_connect_app_for_splunk-0.0.1.tar.gz",
             explicit_appname="amazon_connect_app_for_splunk")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AppsLocalArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/authentication_users.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/authentication_users.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,27 +333,25 @@
         """
         ## # Resource: AuthenticationUsers
 
         Create and update user information or delete the user.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         user01 = splunk.AuthenticationUsers("user01",
             name="user01",
             email="user01@example.com",
             password="password01",
             force_change_pass=False,
             roles=["terraform-user01-role"])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_app: User default app. Overrides the default app inherited from the user roles.
         :param pulumi.Input[str] email: User email address.
         :param pulumi.Input[bool] force_change_pass: Force user to change password indication
         :param pulumi.Input[str] name: Unique user login name.
@@ -372,27 +370,25 @@
         """
         ## # Resource: AuthenticationUsers
 
         Create and update user information or delete the user.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         user01 = splunk.AuthenticationUsers("user01",
             name="user01",
             email="user01@example.com",
             password="password01",
             force_change_pass=False,
             roles=["terraform-user01-role"])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AuthenticationUsersArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/authorization_roles.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/authorization_roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -465,15 +465,14 @@
         """
         ## # Resource: AuthorizationRoles
 
         Create and update role information.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         role01 = splunk.AuthorizationRoles("role01",
             name="terraform-user01-role",
             default_app="search",
@@ -493,15 +492,14 @@
             ],
             search_indexes_defaults=[
                 "_audit",
                 "_internal",
                 "main",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] capabilities: List of capabilities assigned to role.
         :param pulumi.Input[int] cumulative_realtime_search_jobs_quota: Maximum number of concurrently running real-time searches that all members of this role can have.
         :param pulumi.Input[int] cumulative_search_jobs_quota: Maximum number of concurrently running searches for all role members. Warning message logged when limit is reached.
         :param pulumi.Input[str] default_app: Specify the folder name of the default app to use for this role. A user-specific default app overrides this.
@@ -524,15 +522,14 @@
         """
         ## # Resource: AuthorizationRoles
 
         Create and update role information.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         role01 = splunk.AuthorizationRoles("role01",
             name="terraform-user01-role",
             default_app="search",
@@ -552,15 +549,14 @@
             ],
             search_indexes_defaults=[
                 "_audit",
                 "_internal",
                 "main",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param AuthorizationRolesArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/__init__.pyi` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/config/vars.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/configs_conf.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/configs_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,27 +129,25 @@
         """
         ## # Resource: ConfigsConf
 
         Create and manage configuration file stanzas.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         new_conf_stanza = splunk.ConfigsConf("new-conf-stanza",
             name="custom-conf/custom",
             variables={
                 "disabled": "false",
                 "custom_key": "value",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: A '/' separated string consisting of {conf_file_name}/{stanza_name} ex. props/custom_stanza
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] variables: A map of key value pairs for a stanza.
         """
         ...
@@ -161,27 +159,25 @@
         """
         ## # Resource: ConfigsConf
 
         Create and manage configuration file stanzas.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         new_conf_stanza = splunk.ConfigsConf("new-conf-stanza",
             name="custom-conf/custom",
             variables={
                 "disabled": "false",
                 "custom_key": "value",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ConfigsConfArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/data_ui_views.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/data_ui_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,28 +131,26 @@
                  __props__=None):
         """
         ## # Resource: DataUiViews
 
         Create and manage splunk dashboards/views.
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         dashboard = splunk.DataUiViews("dashboard",
             name="Terraform_Sample_Dashboard",
             eai_data="<dashboard version=\\"1.1\\"><label>Terraform</label><description>Terraform operations</description><row><panel><chart><search><query>index=_internal sourcetype=splunkd_access useragent=\\"splunk-simple-go-client\\" | timechart fixedrange=f values(status) by uri_path</query><earliest>-24h@h</earliest><latest>now</latest><sampleRatio>1</sampleRatio></search><option name=\\"charting.axisLabelsX.majorLabelStyle.overflowMode\\">ellipsisNone</option><option name=\\"charting.axisLabelsX.majorLabelStyle.rotation\\">0</option><option name=\\"charting.axisTitleX.visibility\\">collapsed</option><option name=\\"charting.axisTitleY.text\\">HTTP status codes</option><option name=\\"charting.axisTitleY.visibility\\">visible</option><option name=\\"charting.axisTitleY2.visibility\\">visible</option><option name=\\"charting.axisX.abbreviation\\">none</option><option name=\\"charting.axisX.scale\\">linear</option><option name=\\"charting.axisY.abbreviation\\">none</option><option name=\\"charting.axisY.scale\\">linear</option><option name=\\"charting.axisY2.abbreviation\\">none</option><option name=\\"charting.axisY2.enabled\\">0</option><option name=\\"charting.axisY2.scale\\">inherit</option><option name=\\"charting.chart\\">column</option><option name=\\"charting.chart.bubbleMaximumSize\\">50</option><option name=\\"charting.chart.bubbleMinimumSize\\">10</option><option name=\\"charting.chart.bubbleSizeBy\\">area</option><option name=\\"charting.chart.nullValueMode\\">connect</option><option name=\\"charting.chart.showDataLabels\\">none</option><option name=\\"charting.chart.sliceCollapsingThreshold\\">0.01</option><option name=\\"charting.chart.stackMode\\">default</option><option name=\\"charting.chart.style\\">shiny</option><option name=\\"charting.drilldown\\">none</option><option name=\\"charting.layout.splitSeries\\">0</option><option name=\\"charting.layout.splitSeries.allowIndependentYRanges\\">0</option><option name=\\"charting.legend.labelStyle.overflowMode\\">ellipsisMiddle</option><option name=\\"charting.legend.mode\\">standard</option><option name=\\"charting.legend.placement\\">right</option><option name=\\"charting.lineWidth\\">2</option><option name=\\"trellis.enabled\\">0</option><option name=\\"trellis.scales.shared\\">1</option><option name=\\"trellis.size\\">small</option><option name=\\"trellis.splitBy\\">_aggregation</option></chart></panel></row></dashboard>",
             acl=splunk.DataUiViewsAclArgs(
                 owner="admin",
                 app="search",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] eai_data: Dashboard XML definition.
         :param pulumi.Input[str] name: Dashboard name.
                * `eai:data` - (Required) Dashboard XML definition.
         """
@@ -164,28 +162,26 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## # Resource: DataUiViews
 
         Create and manage splunk dashboards/views.
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         dashboard = splunk.DataUiViews("dashboard",
             name="Terraform_Sample_Dashboard",
             eai_data="<dashboard version=\\"1.1\\"><label>Terraform</label><description>Terraform operations</description><row><panel><chart><search><query>index=_internal sourcetype=splunkd_access useragent=\\"splunk-simple-go-client\\" | timechart fixedrange=f values(status) by uri_path</query><earliest>-24h@h</earliest><latest>now</latest><sampleRatio>1</sampleRatio></search><option name=\\"charting.axisLabelsX.majorLabelStyle.overflowMode\\">ellipsisNone</option><option name=\\"charting.axisLabelsX.majorLabelStyle.rotation\\">0</option><option name=\\"charting.axisTitleX.visibility\\">collapsed</option><option name=\\"charting.axisTitleY.text\\">HTTP status codes</option><option name=\\"charting.axisTitleY.visibility\\">visible</option><option name=\\"charting.axisTitleY2.visibility\\">visible</option><option name=\\"charting.axisX.abbreviation\\">none</option><option name=\\"charting.axisX.scale\\">linear</option><option name=\\"charting.axisY.abbreviation\\">none</option><option name=\\"charting.axisY.scale\\">linear</option><option name=\\"charting.axisY2.abbreviation\\">none</option><option name=\\"charting.axisY2.enabled\\">0</option><option name=\\"charting.axisY2.scale\\">inherit</option><option name=\\"charting.chart\\">column</option><option name=\\"charting.chart.bubbleMaximumSize\\">50</option><option name=\\"charting.chart.bubbleMinimumSize\\">10</option><option name=\\"charting.chart.bubbleSizeBy\\">area</option><option name=\\"charting.chart.nullValueMode\\">connect</option><option name=\\"charting.chart.showDataLabels\\">none</option><option name=\\"charting.chart.sliceCollapsingThreshold\\">0.01</option><option name=\\"charting.chart.stackMode\\">default</option><option name=\\"charting.chart.style\\">shiny</option><option name=\\"charting.drilldown\\">none</option><option name=\\"charting.layout.splitSeries\\">0</option><option name=\\"charting.layout.splitSeries.allowIndependentYRanges\\">0</option><option name=\\"charting.legend.labelStyle.overflowMode\\">ellipsisMiddle</option><option name=\\"charting.legend.mode\\">standard</option><option name=\\"charting.legend.placement\\">right</option><option name=\\"charting.lineWidth\\">2</option><option name=\\"trellis.enabled\\">0</option><option name=\\"trellis.scales.shared\\">1</option><option name=\\"trellis.size\\">small</option><option name=\\"trellis.splitBy\\">_aggregation</option></chart></panel></row></dashboard>",
             acl=splunk.DataUiViewsAclArgs(
                 owner="admin",
                 app="search",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param DataUiViewsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/generic_acl.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/generic_acl.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  acl: Optional[pulumi.Input[pulumi.InputType['GenericAclAclArgs']]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         my_app = splunk.GenericAcl("my_app",
             path="apps/local/my_app",
             acl=splunk.GenericAclAclArgs(
@@ -136,15 +135,14 @@
             acl=splunk.GenericAclAclArgs(
                 app="my_app",
                 owner="joe_user",
                 reads=["team_joe"],
                 writes=["team_joe"],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Generic ACL resources can be imported by specifying their owner, app, and path with a colon-delimited string as the ID:
 
         ```sh
         $ pulumi import splunk:index/genericAcl:GenericAcl splunk_generic_acl <owner>:<app>:<path>
@@ -163,15 +161,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: GenericAclArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         my_app = splunk.GenericAcl("my_app",
             path="apps/local/my_app",
             acl=splunk.GenericAclAclArgs(
@@ -188,15 +185,14 @@
             acl=splunk.GenericAclAclArgs(
                 app="my_app",
                 owner="joe_user",
                 reads=["team_joe"],
                 writes=["team_joe"],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Generic ACL resources can be imported by specifying their owner, app, and path with a colon-delimited string as the ID:
 
         ```sh
         $ pulumi import splunk:index/genericAcl:GenericAcl splunk_generic_acl <owner>:<app>:<path>
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/global_http_event_collector.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/global_http_event_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,25 +271,23 @@
         """
         ## # Resource: GlobalHttpEventCollector
 
         Update Global HTTP Event Collector input configuration.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         http = splunk.GlobalHttpEventCollector("http",
             disabled=False,
             enable_ssl=True,
             port=8088)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] dedicated_io_threads: Number of threads used by HTTP Input server.
         :param pulumi.Input[bool] disabled: Input disabled indicator.
         :param pulumi.Input[bool] enable_ssl: Enable SSL protocol for HTTP data input. `true` = SSL enabled, `false` = SSL disabled.
         :param pulumi.Input[int] max_sockets: Maximum number of simultaneous HTTP connections accepted. Adjusting this value may cause server performance issues and is not generally recommended. Possible values for this setting vary by OS.
@@ -307,25 +305,23 @@
         """
         ## # Resource: GlobalHttpEventCollector
 
         Update Global HTTP Event Collector input configuration.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         http = splunk.GlobalHttpEventCollector("http",
             disabled=False,
             enable_ssl=True,
             port=8088)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param GlobalHttpEventCollectorArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/indexes.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/indexes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1506,25 +1506,23 @@
         ## Authorization and authentication
 
         By default, all users can list all indexes. However, if the indexes_list_all capability is enabled in authorize.conf, access to all indexes is limited to only those roles with this capability.
         To enable indexes_list_all capability restrictions on the data/indexes endpoint, create a [capability::indexes_list_all] stanza in authorize.conf. Specify indexes_list_all=enabled for any role permitted to list all indexes from this endpoint.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         user01_index = splunk.Indexes("user01-index",
             name="user01-index",
             max_hot_buckets=6,
             max_total_data_size_mb=1000000)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['IndexesAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[int] block_sign_size: Controls how many events make up a block for block signatures. If this is set to 0, block signing is disabled for this index. <br>A recommended value is 100.
         :param pulumi.Input[str] bucket_rebuild_memory_hint: Suggestion for the bucket rebuild process for the size of the time-series (tsidx) file to make.
                <be>Caution: This is an advanced parameter. Inappropriate use of this parameter causes splunkd to not start if rebuild is required. Do not set this parameter unless instructed by Splunk Support.
@@ -1622,25 +1620,23 @@
         ## Authorization and authentication
 
         By default, all users can list all indexes. However, if the indexes_list_all capability is enabled in authorize.conf, access to all indexes is limited to only those roles with this capability.
         To enable indexes_list_all capability restrictions on the data/indexes endpoint, create a [capability::indexes_list_all] stanza in authorize.conf. Specify indexes_list_all=enabled for any role permitted to list all indexes from this endpoint.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         user01_index = splunk.Indexes("user01-index",
             name="user01-index",
             max_hot_buckets=6,
             max_total_data_size_mb=1000000)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param IndexesArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_http_event_collector.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_http_event_collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,14 @@
         """
         ## # Resource: InputsHttpEventCollector
 
         Create or update HTTP Event Collector input configuration tokens.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         hec_token_01 = splunk.InputsHttpEventCollector("hec-token-01",
             name="hec-token-01",
             index="main",
@@ -392,15 +391,14 @@
             acl=splunk.InputsHttpEventCollectorAclArgs(
                 owner="user01",
                 sharing="global",
                 reads=["admin"],
                 writes=["admin"],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsHttpEventCollectorAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[bool] disabled: Input disabled indicator
         :param pulumi.Input[str] host: Default host value for events with this token
         :param pulumi.Input[str] index: Index to store generated events
@@ -420,15 +418,14 @@
         """
         ## # Resource: InputsHttpEventCollector
 
         Create or update HTTP Event Collector input configuration tokens.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         hec_token_01 = splunk.InputsHttpEventCollector("hec-token-01",
             name="hec-token-01",
             index="main",
@@ -444,15 +441,14 @@
             acl=splunk.InputsHttpEventCollectorAclArgs(
                 owner="user01",
                 sharing="global",
                 reads=["admin"],
                 writes=["admin"],
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsHttpEventCollectorArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_monitor.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,25 +566,23 @@
         """
         ## # Resource: InputsMonitor
 
         Create or update a new file or directory monitor input.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         monitor = splunk.InputsMonitor("monitor",
             name="opt/splunk/var/log/splunk/health.log",
             recursive=True,
             sourcetype="text")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsMonitorAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] blacklist: Specify a regular expression for a file path. The file path that matches this regular expression is not indexed.
         :param pulumi.Input[str] crc_salt: A string that modifies the file tracking identity for files in this input. The magic value <SOURCE> invokes special behavior.
         :param pulumi.Input[bool] disabled: Indicates if input monitoring is disabled.
@@ -610,25 +608,23 @@
         """
         ## # Resource: InputsMonitor
 
         Create or update a new file or directory monitor input.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         monitor = splunk.InputsMonitor("monitor",
             name="opt/splunk/var/log/splunk/health.log",
             recursive=True,
             sourcetype="text")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsMonitorArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_script.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,24 +375,22 @@
         """
         ## # Resource: InputsScript
 
         Create or update scripted inputs.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         script = splunk.InputsScript("script",
             name="opt/splunk/bin/scripts/readme.txt",
             interval=360)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsScriptAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[bool] disabled: Specifies whether the input script is disabled.
         :param pulumi.Input[str] host: Sets the host for events from this input. Defaults to whatever host sent the event.
         :param pulumi.Input[str] index: Sets the index for events from this input. Defaults to the main index.
@@ -414,24 +412,22 @@
         """
         ## # Resource: InputsScript
 
         Create or update scripted inputs.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         script = splunk.InputsScript("script",
             name="opt/splunk/bin/scripts/readme.txt",
             interval=360)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsScriptArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_cooked.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_cooked.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,26 +256,24 @@
         """
         ## # Resource: InputsTcpCooked
 
         Create or update cooked TCP input information and create new containers for managing cooked data.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_cooked = splunk.InputsTcpCooked("tcp_cooked",
             name="50000",
             disabled=False,
             connection_host="dns",
             restrict_to_host="splunk")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsTcpCookedAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] connection_host: Valid values: (ip | dns | none)
                Set the host for the remote server that is sending data.
                ip sets the host to the IP address of the remote server sending data.
@@ -296,26 +294,24 @@
         """
         ## # Resource: InputsTcpCooked
 
         Create or update cooked TCP input information and create new containers for managing cooked data.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_cooked = splunk.InputsTcpCooked("tcp_cooked",
             name="50000",
             disabled=False,
             connection_host="dns",
             restrict_to_host="splunk")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsTcpCookedArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_raw.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,28 +449,26 @@
         """
         ## # Resource: InputsTcpRaw
 
         Create or update raw TCP input information for managing raw tcp inputs from forwarders.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_raw = splunk.InputsTcpRaw("tcp_raw",
             name="41000",
             index="main",
             queue="indexQueue",
             source="new",
             sourcetype="new",
             disabled=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsTcpRawAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] connection_host: Valid values: (ip | dns | none)
                Set the host for the remote server that is sending data.
                ip sets the host to the IP address of the remote server sending data.
@@ -503,28 +501,26 @@
         """
         ## # Resource: InputsTcpRaw
 
         Create or update raw TCP input information for managing raw tcp inputs from forwarders.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_raw = splunk.InputsTcpRaw("tcp_raw",
             name="41000",
             index="main",
             queue="indexQueue",
             source="new",
             sourcetype="new",
             disabled=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsTcpRawArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_splunk_tcp_token.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_splunk_tcp_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,24 +137,22 @@
         """
         ## # Resource: InputsTcpSplunkTcpToken
 
         Manage receiver access using tokens.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_splunk_tcp_token = splunk.InputsTcpSplunkTcpToken("tcp_splunk_tcp_token",
             name="new-splunk-tcp-token",
             token="D66C45B3-7C28-48A1-A13A-027914146501")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsTcpSplunkTcpTokenAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] name: Required. Name for the token to create.
         :param pulumi.Input[str] token: Optional. Token value to use. If unspecified, a token is generated automatically.
         """
@@ -167,24 +165,22 @@
         """
         ## # Resource: InputsTcpSplunkTcpToken
 
         Manage receiver access using tokens.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_splunk_tcp_token = splunk.InputsTcpSplunkTcpToken("tcp_splunk_tcp_token",
             name="new-splunk-tcp-token",
             token="D66C45B3-7C28-48A1-A13A-027914146501")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsTcpSplunkTcpTokenArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_tcp_ssl.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_tcp_ssl.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,24 +201,22 @@
         """
         ## # Resource: InputsTcpSsl
 
         Access or update the SSL configuration for the host.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         test = splunk.InputsTcpSsl("test",
             disabled=False,
             require_client_cert=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] disabled: Indicates if input is disabled.
         :param pulumi.Input[str] password: Server certificate password, if any.
         :param pulumi.Input[bool] require_client_cert: Determines whether a client must authenticate.
         :param pulumi.Input[str] root_ca: Certificate authority list (root file)
@@ -233,24 +231,22 @@
         """
         ## # Resource: InputsTcpSsl
 
         Access or update the SSL configuration for the host.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         test = splunk.InputsTcpSsl("test",
             disabled=False,
             require_client_cert=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsTcpSslArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/inputs_udp.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/inputs_udp.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,27 +458,25 @@
         """
         ## # Resource: InputsTcpRaw
 
         Create and manage UDP data inputs.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         udp = splunk.InputsUdp("udp",
             name="41000",
             index="main",
             source="new",
             sourcetype="new",
             disabled=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['InputsUdpAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] connection_host: Valid values: (ip | dns | none)
                Set the host for the remote server that is sending data.
                ip sets the host to the IP address of the remote server sending data.
@@ -506,27 +504,25 @@
         """
         ## # Resource: InputsTcpRaw
 
         Create and manage UDP data inputs.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         udp = splunk.InputsUdp("udp",
             name="41000",
             index="main",
             source="new",
             sourcetype="new",
             disabled=False)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param InputsUdpArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_default.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_default.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,29 +383,27 @@
         """
         ## # Resource: OutputsTcpDefault
 
         Manage to global tcpout properties.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_default = splunk.OutputsTcpDefault("tcp_default",
             name="tcpout",
             disabled=False,
             default_group="test-indexers",
             drop_events_on_queue_full=60,
             index_and_forward=True,
             send_cooked_data=True,
             max_queue_size="100KB")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['OutputsTcpDefaultAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] default_group: Comma-separated list of one or more target group names, specified later in [tcpout:<target_group>] stanzas of outputs.conf.spec file.
                The forwarder sends all data to the specified groups. If you do not want to forward data automatically, do not set this attribute. Can be overridden by an inputs.conf _TCP_ROUTING setting, which in turn can be overridden by a props.conf/transforms.conf modifier.
         :param pulumi.Input[bool] disabled: Disables default tcpout settings
@@ -436,29 +434,27 @@
         """
         ## # Resource: OutputsTcpDefault
 
         Manage to global tcpout properties.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_default = splunk.OutputsTcpDefault("tcp_default",
             name="tcpout",
             disabled=False,
             default_group="test-indexers",
             drop_events_on_queue_full=60,
             index_and_forward=True,
             send_cooked_data=True,
             max_queue_size="100KB")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param OutputsTcpDefaultArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_group.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,15 +440,14 @@
         """
         ## # Resource: OutputsTcpGroup
 
         Access to the configuration of a group of one or more data forwarding destinations.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_group = splunk.OutputsTcpGroup("tcp_group",
             name="tcp-group",
             disabled=False,
@@ -456,15 +455,14 @@
             send_cooked_data=True,
             max_queue_size="100KB",
             servers=[
                 "1.1.1.1:1234",
                 "2.2.2.2:1234",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['OutputsTcpGroupAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[bool] compressed: If true, forwarder sends compressed data. If set to true, the receiver port must also have compression turned on.
         :param pulumi.Input[bool] disabled: If true, disables the group.
         :param pulumi.Input[int] drop_events_on_queue_full: If set to a positive number, wait the specified number of seconds before throwing out all new events until the output queue has space. Defaults to -1 (do not drop events).
@@ -495,15 +493,14 @@
         """
         ## # Resource: OutputsTcpGroup
 
         Access to the configuration of a group of one or more data forwarding destinations.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_group = splunk.OutputsTcpGroup("tcp_group",
             name="tcp-group",
             disabled=False,
@@ -511,15 +508,14 @@
             send_cooked_data=True,
             max_queue_size="100KB",
             servers=[
                 "1.1.1.1:1234",
                 "2.2.2.2:1234",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param OutputsTcpGroupArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_server.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,24 +413,22 @@
         """
         ## # Resource: OutputsTcpServer
 
         Access data forwarding configurations.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_server = splunk.OutputsTcpServer("tcp_server",
             name="new-host:1234",
             ssl_alt_name_to_check="old-host")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['OutputsTcpServerAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[bool] disabled: If true, disables the group.
         :param pulumi.Input[str] method: Valid values: (clone | balance | autobalance)
                The data distribution method used when two or more servers exist in the same forwarder group.
@@ -454,24 +452,22 @@
         """
         ## # Resource: OutputsTcpServer
 
         Access data forwarding configurations.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_server = splunk.OutputsTcpServer("tcp_server",
             name="new-host:1234",
             ssl_alt_name_to_check="old-host")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param OutputsTcpServerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/outputs_tcp_syslog.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/outputs_tcp_syslog.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,25 +326,23 @@
         """
         ## # Resource: OutputsTcpSyslog
 
         Access the configuration of a forwarded server configured to provide data in standard syslog format.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_syslog = splunk.OutputsTcpSyslog("tcp_syslog",
             name="new-syslog",
             server="new-host-1:1234",
             priority=5)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['OutputsTcpSyslogAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[bool] disabled: If true, disables global syslog settings.
         :param pulumi.Input[str] name: Name of the syslog output group. This is name used when creating syslog configuration in outputs.conf.
         :param pulumi.Input[int] priority: Sets syslog priority value. The priority value should specified as an integer. See $SPLUNK_HOME/etc/system/README/outputs.conf.spec for details.
@@ -368,25 +366,23 @@
         """
         ## # Resource: OutputsTcpSyslog
 
         Access the configuration of a forwarded server configured to provide data in standard syslog format.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tcp_syslog = splunk.OutputsTcpSyslog("tcp_syslog",
             name="new-syslog",
             server="new-host-1:1234",
             priority=5)
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param OutputsTcpSyslogArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/provider.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/saved_searches.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/saved_searches.py`

 * *Files 0% similar despite different names*

```diff
@@ -5503,15 +5503,14 @@
         """
         ## # Resource: SavedSearches
 
         Create and manage saved searches.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         saved_search = splunk.SavedSearches("saved_search",
             name="Test New Alert",
             search="index=main",
@@ -5528,15 +5527,14 @@
             cron_schedule="*/5 * * * *",
             acl=splunk.SavedSearchesAclArgs(
                 owner="admin",
                 sharing="app",
                 app="launcher",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['SavedSearchesAclArgs']] acl: The app/user context that is the namespace for the resource
         :param pulumi.Input[str] action_create_xsoar_incident: Enable XSOAR alerting (Should by 1 (Enabled) or 0 (Disabled))
         :param pulumi.Input[str] action_create_xsoar_incident_param_custom_fields: XSOAR custom incident fields (should be a comma separated list)
         :param pulumi.Input[str] action_create_xsoar_incident_param_details: XSOAR incident description
@@ -5718,15 +5716,14 @@
         """
         ## # Resource: SavedSearches
 
         Create and manage saved searches.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         saved_search = splunk.SavedSearches("saved_search",
             name="Test New Alert",
             search="index=main",
@@ -5743,15 +5740,14 @@
             cron_schedule="*/5 * * * *",
             acl=splunk.SavedSearchesAclArgs(
                 owner="admin",
                 sharing="app",
                 app="launcher",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param SavedSearchesArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk/sh_indexes_manager.py` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk/sh_indexes_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -207,26 +207,24 @@
 
         ## Authorization and authentication
 
         As of now there is no support to create indexes in user-specified workspaces on Splunk Cloud.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tf_index = splunk.ShIndexesManager("tf-index",
             name="tf-test-index-0",
             datatype="event",
             frozen_time_period_in_secs="94608000",
             max_global_raw_data_size_mb="100")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] datatype: Valid values: (event | metric). Specifies the type of index.
         :param pulumi.Input[str] frozen_time_period_in_secs: Number of seconds after which indexed data rolls to frozen.
                Defaults to 94608000 (3 years).Freezing data means it is removed from the index. If you need to archive your data, refer to coldToFrozenDir and coldToFrozenScript parameter documentation.
         :param pulumi.Input[str] max_global_raw_data_size_mb: The maximum size of an index (in MB). If an index grows larger than the maximum size, the oldest data is frozen.
@@ -246,26 +244,24 @@
 
         ## Authorization and authentication
 
         As of now there is no support to create indexes in user-specified workspaces on Splunk Cloud.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_splunk as splunk
 
         tf_index = splunk.ShIndexesManager("tf-index",
             name="tf-test-index-0",
             datatype="event",
             frozen_time_period_in_secs="94608000",
             max_global_raw_data_size_mb="100")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ShIndexesManagerArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/PKG-INFO` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1713561402
+Version: 1.3.0a1713904842
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi,splunk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_splunk-1.3.0a1713561402/pulumi_splunk.egg-info/SOURCES.txt` & `pulumi_splunk-1.3.0a1713904842/pulumi_splunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1713561402/pyproject.toml` & `pulumi_splunk-1.3.0a1713904842/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_splunk"
   description = "A Pulumi package for creating and managing splunk cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0a1,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "splunk"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.3.0a1713561402"
+  version = "1.3.0a1713904842"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-splunk"
 
 [build-system]
```

