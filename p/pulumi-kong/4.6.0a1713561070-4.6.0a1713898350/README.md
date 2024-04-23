# Comparing `tmp/pulumi_kong-4.6.0a1713561070.tar.gz` & `tmp/pulumi_kong-4.6.0a1713898350.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kong-4.6.0a1713561070.tar", last modified: Fri Apr 19 21:14:23 2024, max compression
+gzip compressed data, was "pulumi_kong-4.6.0a1713898350.tar", last modified: Tue Apr 23 19:27:29 2024, max compression
```

## Comparing `pulumi_kong-4.6.0a1713561070.tar` & `pulumi_kong-4.6.0a1713898350.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:23.109725 pulumi_kong-4.6.0a1713561070/
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-19 21:14:23.109725 pulumi_kong-4.6.0a1713561070/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:23.105724 pulumi_kong-4.6.0a1713561070/pulumi_kong/
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16572 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:23.105724 pulumi_kong-4.6.0a1713561070/pulumi_kong/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11411 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    18900 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_key_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    22656 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25984 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54868 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/route.py
--rw-r--r--   0 runner    (1001) docker     (127)    36457 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13150 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/target.py
--rw-r--r--   0 runner    (1001) docker     (127)    73268 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong/upstream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:23.109725 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-19 21:14:23.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-19 21:14:23.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:14:23.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:14:23.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 21:14:23.000000 pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-19 21:14:16.000000 pulumi_kong-4.6.0a1713561070/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:14:23.109725 pulumi_kong-4.6.0a1713561070/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:29.882389 pulumi_kong-4.6.0a1713898350/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-23 19:27:29.878389 pulumi_kong-4.6.0a1713898350/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:29.878389 pulumi_kong-4.6.0a1713898350/pulumi_kong/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16572 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13605 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:29.878389 pulumi_kong-4.6.0a1713898350/pulumi_kong/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18776 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer_jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer_key_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22596 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14574 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25552 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54556 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36145 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12994 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73112 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong/upstream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:27:29.878389 pulumi_kong-4.6.0a1713898350/pulumi_kong.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-04-23 19:27:29.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-23 19:27:29.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:27:29.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 19:27:29.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:27:29.000000 pulumi_kong-4.6.0a1713898350/pulumi_kong.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 19:27:23.000000 pulumi_kong-4.6.0a1713898350/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:27:29.882389 pulumi_kong-4.6.0a1713898350/setup.cfg
```

### Comparing `pulumi_kong-4.6.0a1713561070/PKG-INFO` & `pulumi_kong-4.6.0a1713898350/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kong
-Version: 4.6.0a1713561070
+Version: 4.6.0a1713898350
 Summary: A Pulumi package for creating and managing Kong resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kong
 Keywords: pulumi,kong
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kong-4.6.0a1713561070/README.md` & `pulumi_kong-4.6.0a1713898350/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/__init__.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/_inputs.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/_utilities.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/certificate.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,29 +159,27 @@
         """
         ## # Certificate
 
         For more information on creating certificates in Kong [see their documentation](https://docs.konghq.com/gateway-oss/2.5.x/admin-api/#certificate-object)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         certificate = kong.Certificate("certificate",
             certificate="public key --- 123 ----",
             private_key="private key --- 456 ----",
             snis=[
                 "foo.com",
                 "bar.com",
             ],
             tags=["myTag"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a certificate:
 
         ```sh
         $ pulumi import kong:index/certificate:Certificate <certifcate_identifier> <certificate_id>
@@ -202,29 +200,27 @@
         """
         ## # Certificate
 
         For more information on creating certificates in Kong [see their documentation](https://docs.konghq.com/gateway-oss/2.5.x/admin-api/#certificate-object)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         certificate = kong.Certificate("certificate",
             certificate="public key --- 123 ----",
             private_key="private key --- 456 ----",
             snis=[
                 "foo.com",
                 "bar.com",
             ],
             tags=["myTag"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a certificate:
 
         ```sh
         $ pulumi import kong:index/certificate:Certificate <certifcate_identifier> <certificate_id>
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/config/__init__.pyi` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/config/vars.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,25 +135,23 @@
         """
         ## # Consumer
 
         The consumer resource maps directly onto the json for creating a Consumer in Kong.  For more information on the parameters [see the Kong Consumer create documentation](https://docs.konghq.com/gateway-oss/2.5.x/admin-api/#consumer-object).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         consumer = kong.Consumer("consumer",
             username="User1",
             custom_id="123",
             tags=["mySuperTag"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a consumer:
 
         ```sh
         $ pulumi import kong:index/consumer:Consumer <consumer_identifier> <consumer_id>
@@ -174,25 +172,23 @@
         """
         ## # Consumer
 
         The consumer resource maps directly onto the json for creating a Consumer in Kong.  For more information on the parameters [see the Kong Consumer create documentation](https://docs.konghq.com/gateway-oss/2.5.x/admin-api/#consumer-object).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         consumer = kong.Consumer("consumer",
             username="User1",
             custom_id="123",
             tags=["mySuperTag"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a consumer:
 
         ```sh
         $ pulumi import kong:index/consumer:Consumer <consumer_identifier> <consumer_id>
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_acl.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer_acl.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,37 +133,35 @@
         """
         ## # ConsumerAcl
 
         Consumer ACL is a resource that allows you to configure the acl plugin for a consumer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
         acl_plugin = kong.Plugin("acl_plugin",
             name="acl",
-            config_json=\"\"\"	{
-        		"allow": ["group1", "group2"]
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"allow": ["group1", "group2"]
+        \\x09}
         \"\"\")
         consumer_acl = kong.ConsumerAcl("consumer_acl",
             consumer_id=my_consumer.id,
             group="group2",
             tags=[
                 "myTag",
                 "otherTag",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] consumer_id: the id of the consumer to be configured
         :param pulumi.Input[str] group: the acl group
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of strings associated with the consumer acl for grouping and filtering
         """
@@ -176,37 +174,35 @@
         """
         ## # ConsumerAcl
 
         Consumer ACL is a resource that allows you to configure the acl plugin for a consumer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
         acl_plugin = kong.Plugin("acl_plugin",
             name="acl",
-            config_json=\"\"\"	{
-        		"allow": ["group1", "group2"]
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"allow": ["group1", "group2"]
+        \\x09}
         \"\"\")
         consumer_acl = kong.ConsumerAcl("consumer_acl",
             consumer_id=my_consumer.id,
             group="group2",
             tags=[
                 "myTag",
                 "otherTag",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ConsumerAclArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_basic_auth.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer_basic_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,14 @@
         """
         ## # ConsumerBasicAuth
 
         Consumer basic auth is a resource that allows you to configure the basic auth plugin for a consumer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
@@ -183,15 +182,14 @@
             username="foo_updated",
             password="bar_updated",
             tags=[
                 "myTag",
                 "anotherTag",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] consumer_id: the id of the consumer to be configured with basic auth
         :param pulumi.Input[str] password: password to be used for basic auth
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of strings associated with the consumer basic auth for grouping and filtering
         :param pulumi.Input[str] username: username to be used for basic auth
@@ -205,15 +203,14 @@
         """
         ## # ConsumerBasicAuth
 
         Consumer basic auth is a resource that allows you to configure the basic auth plugin for a consumer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
@@ -223,15 +220,14 @@
             username="foo_updated",
             password="bar_updated",
             tags=[
                 "myTag",
                 "anotherTag",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ConsumerBasicAuthArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_jwt_auth.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer_jwt_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,36 +232,34 @@
         """
         ## # ConsumerJwtAuth
 
         Consumer jwt auth is a resource that allows you to configure the jwt auth plugin for a consumer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
         jwt_plugin = kong.Plugin("jwt_plugin",
             name="jwt",
-            config_json=\"\"\"	{
-        		"claims_to_verify": ["exp"]
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"claims_to_verify": ["exp"]
+        \\x09}
         \"\"\")
         consumer_jwt_config = kong.ConsumerJwtAuth("consumer_jwt_config",
             consumer_id=my_consumer.id,
             algorithm="HS256",
             key="my_key",
             rsa_public_key="foo",
             secret="my_secret")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] algorithm: The algorithm used to verify the token’s signature. Can be HS256, HS384, HS512, RS256, or ES256, Default is `HS256`
         :param pulumi.Input[str] consumer_id: the id of the consumer to be configured with jwt auth
         :param pulumi.Input[str] key: A unique string identifying the credential. If left out, it will be auto-generated.
         :param pulumi.Input[str] rsa_public_key: If algorithm is `RS256` or `ES256`, the public key (in PEM format) to use to verify the token’s signature
@@ -277,36 +275,34 @@
         """
         ## # ConsumerJwtAuth
 
         Consumer jwt auth is a resource that allows you to configure the jwt auth plugin for a consumer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
         jwt_plugin = kong.Plugin("jwt_plugin",
             name="jwt",
-            config_json=\"\"\"	{
-        		"claims_to_verify": ["exp"]
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"claims_to_verify": ["exp"]
+        \\x09}
         \"\"\")
         consumer_jwt_config = kong.ConsumerJwtAuth("consumer_jwt_config",
             consumer_id=my_consumer.id,
             algorithm="HS256",
             key="my_key",
             rsa_public_key="foo",
             secret="my_secret")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ConsumerJwtAuthArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_key_auth.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer_key_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,14 @@
         """
         ## # ConsumerKeyAuth
 
         Resource that allows you to configure the [Key Authentication](https://docs.konghq.com/hub/kong-inc/key-auth/) plugin for a consumer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
@@ -151,15 +150,14 @@
             consumer_id=my_consumer.id,
             key="secret",
             tags=[
                 "myTag",
                 "anotherTag",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] consumer_id: the id of the consumer to associate the credentials to
         :param pulumi.Input[str] key: Unique key to authenticate the client; if omitted the plugin will generate one
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: A list of strings associated with the consumer key auth for grouping and filtering
         """
@@ -172,15 +170,14 @@
         """
         ## # ConsumerKeyAuth
 
         Resource that allows you to configure the [Key Authentication](https://docs.konghq.com/hub/kong-inc/key-auth/) plugin for a consumer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
@@ -189,15 +186,14 @@
             consumer_id=my_consumer.id,
             key="secret",
             tags=[
                 "myTag",
                 "anotherTag",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ConsumerKeyAuthArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/consumer_oauth2.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/consumer_oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,44 +265,42 @@
         """
         ## # ConsumerOauth2
 
         Resource that allows you to configure the OAuth2 plugin credentials for a consumer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
         oauth2_plugin = kong.Plugin("oauth2_plugin",
             name="oauth2",
-            config_json=\"\"\"	{
-        		"global_credentials": true,
-        		"enable_password_grant": true,
-        		"token_expiration": 180,
-        		"refresh_token_ttl": 180,
-        		"provision_key": "testprovisionkey"
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"global_credentials": true,
+        \\x09\\x09"enable_password_grant": true,
+        \\x09\\x09"token_expiration": 180,
+        \\x09\\x09"refresh_token_ttl": 180,
+        \\x09\\x09"provision_key": "testprovisionkey"
+        \\x09}
         \"\"\")
         consumer_oauth2 = kong.ConsumerOauth2("consumer_oauth2",
             name="test_application",
             consumer_id=my_consumer.id,
             client_id="client_id",
             client_secret="client_secret",
             redirect_uris=[
                 "https://asdf.com/callback",
                 "https://test.cl/callback",
             ],
             tags=["myTag"])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] client_id: Unique oauth2 client id. If not set, the oauth2 plugin will generate one
         :param pulumi.Input[str] client_secret: Unique oauth2 client secret. If not set, the oauth2 plugin will generate one
         :param pulumi.Input[str] consumer_id: The id of the consumer to be configured with oauth2.
         :param pulumi.Input[bool] hash_secret: A boolean flag that indicates whether the client_secret field will be stored in hashed form. If enabled on existing plugin instances, client secrets are hashed on the fly upon first usage. Default: `false`.
@@ -319,44 +317,42 @@
         """
         ## # ConsumerOauth2
 
         Resource that allows you to configure the OAuth2 plugin credentials for a consumer.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         my_consumer = kong.Consumer("my_consumer",
             username="User1",
             custom_id="123")
         oauth2_plugin = kong.Plugin("oauth2_plugin",
             name="oauth2",
-            config_json=\"\"\"	{
-        		"global_credentials": true,
-        		"enable_password_grant": true,
-        		"token_expiration": 180,
-        		"refresh_token_ttl": 180,
-        		"provision_key": "testprovisionkey"
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"global_credentials": true,
+        \\x09\\x09"enable_password_grant": true,
+        \\x09\\x09"token_expiration": 180,
+        \\x09\\x09"refresh_token_ttl": 180,
+        \\x09\\x09"provision_key": "testprovisionkey"
+        \\x09}
         \"\"\")
         consumer_oauth2 = kong.ConsumerOauth2("consumer_oauth2",
             name="test_application",
             consumer_id=my_consumer.id,
             client_id="client_id",
             client_secret="client_secret",
             redirect_uris=[
                 "https://asdf.com/callback",
                 "https://test.cl/callback",
             ],
             tags=["myTag"])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param ConsumerOauth2Args args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/outputs.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/plugin.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -301,93 +301,85 @@
         ## # Plugin
 
         The plugin resource maps directly onto the json for the API endpoint in Kong.  For more information on the parameters [see the Kong Api create documentation](https://docs.konghq.com/gateway-oss/2.5.x/admin-api/#plugin-object).
         The `config_json` is passed through to the plugin to configure it as is.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         rate_limit = kong.Plugin("rate_limit",
             name="rate-limiting",
-            config_json=\"\"\"	{
-        		"second": 5,
-        		"hour" : 1000
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"second": 5,
+        \\x09\\x09"hour" : 1000
+        \\x09}
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
         To apply a plugin to a consumer use the `consumer_id` property, for example:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         plugin_consumer = kong.Consumer("plugin_consumer",
             username="PluginUser",
             custom_id="567")
         rate_limit = kong.Plugin("rate_limit",
             name="rate-limiting",
             consumer_id=plugin_consumer.id,
-            config_json=\"\"\"	{
-        		"second": 5,
-        		"hour" : 1000
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"second": 5,
+        \\x09\\x09"hour" : 1000
+        \\x09}
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         To apply a plugin to a service use the `service_id` property, for example:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
             name="test",
             protocol="http",
             host="test.org")
         rate_limit = kong.Plugin("rate_limit",
             name="rate-limiting",
             service_id=service.id,
-            config_json=\"\"\"	{
-        		"second": 10,
-        		"hour" : 2000
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"second": 10,
+        \\x09\\x09"hour" : 2000
+        \\x09}
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         To apply a plugin to a route use the `route_id` property, for example:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
             name="test",
             protocol="http",
             host="test.org")
         rate_limit = kong.Plugin("rate_limit",
             name="rate-limiting",
             enabled=True,
             service_id=service.id,
-            config_json=\"\"\"	{
-        		"second": 11,
-        		"hour" : 4000
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"second": 11,
+        \\x09\\x09"hour" : 4000
+        \\x09}
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a plugin:
 
         ```sh
         $ pulumi import kong:index/plugin:Plugin <plugin_identifier> <plugin_id>
@@ -413,93 +405,85 @@
         ## # Plugin
 
         The plugin resource maps directly onto the json for the API endpoint in Kong.  For more information on the parameters [see the Kong Api create documentation](https://docs.konghq.com/gateway-oss/2.5.x/admin-api/#plugin-object).
         The `config_json` is passed through to the plugin to configure it as is.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         rate_limit = kong.Plugin("rate_limit",
             name="rate-limiting",
-            config_json=\"\"\"	{
-        		"second": 5,
-        		"hour" : 1000
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"second": 5,
+        \\x09\\x09"hour" : 1000
+        \\x09}
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
         To apply a plugin to a consumer use the `consumer_id` property, for example:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         plugin_consumer = kong.Consumer("plugin_consumer",
             username="PluginUser",
             custom_id="567")
         rate_limit = kong.Plugin("rate_limit",
             name="rate-limiting",
             consumer_id=plugin_consumer.id,
-            config_json=\"\"\"	{
-        		"second": 5,
-        		"hour" : 1000
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"second": 5,
+        \\x09\\x09"hour" : 1000
+        \\x09}
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         To apply a plugin to a service use the `service_id` property, for example:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
             name="test",
             protocol="http",
             host="test.org")
         rate_limit = kong.Plugin("rate_limit",
             name="rate-limiting",
             service_id=service.id,
-            config_json=\"\"\"	{
-        		"second": 10,
-        		"hour" : 2000
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"second": 10,
+        \\x09\\x09"hour" : 2000
+        \\x09}
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         To apply a plugin to a route use the `route_id` property, for example:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
             name="test",
             protocol="http",
             host="test.org")
         rate_limit = kong.Plugin("rate_limit",
             name="rate-limiting",
             enabled=True,
             service_id=service.id,
-            config_json=\"\"\"	{
-        		"second": 11,
-        		"hour" : 4000
-        	}
+            config_json=\"\"\"\\x09{
+        \\x09\\x09"second": 11,
+        \\x09\\x09"hour" : 4000
+        \\x09}
         \"\"\")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a plugin:
 
         ```sh
         $ pulumi import kong:index/plugin:Plugin <plugin_identifier> <plugin_id>
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/provider.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/route.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,15 +632,14 @@
 
         The route resource maps directly onto the json for the route endpoint in Kong. For more information on the parameters [see the Kong Route create documentation](https://docs.konghq.com/gateway-oss/2.5.x/admin-api/#route-object).
 
         To create a tcp/tls route you set `sources` and `destinations` by repeating the corresponding element (`source` or `destination`) for each source or destination you want.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         route = kong.Route("route",
             name="MyRoute",
             protocols=[
@@ -661,19 +660,17 @@
                 name="x-test-1",
                 values=[
                     "a",
                     "b",
                 ],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         To create a tcp/tls route you set `sources` and `destinations` by repeating the corresponding element (`source` or `destination`) for each source or destination you want, for example:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         route = kong.Route("route",
             protocols=["tcp"],
             strip_path=True,
@@ -690,15 +687,14 @@
             destinations=[kong.RouteDestinationArgs(
                 ip="172.10.1.1",
                 port=81,
             )],
             snis=["foo.com"],
             service_id=service["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a route:
 
         ```sh
         $ pulumi import kong:index/route:Route <route_identifier> <route_id>
@@ -736,15 +732,14 @@
 
         The route resource maps directly onto the json for the route endpoint in Kong. For more information on the parameters [see the Kong Route create documentation](https://docs.konghq.com/gateway-oss/2.5.x/admin-api/#route-object).
 
         To create a tcp/tls route you set `sources` and `destinations` by repeating the corresponding element (`source` or `destination`) for each source or destination you want.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         route = kong.Route("route",
             name="MyRoute",
             protocols=[
@@ -765,19 +760,17 @@
                 name="x-test-1",
                 values=[
                     "a",
                     "b",
                 ],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         To create a tcp/tls route you set `sources` and `destinations` by repeating the corresponding element (`source` or `destination`) for each source or destination you want, for example:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         route = kong.Route("route",
             protocols=["tcp"],
             strip_path=True,
@@ -794,15 +787,14 @@
             destinations=[kong.RouteDestinationArgs(
                 ip="172.10.1.1",
                 port=81,
             )],
             snis=["foo.com"],
             service_id=service["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a route:
 
         ```sh
         $ pulumi import kong:index/route:Route <route_identifier> <route_id>
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/service.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -497,15 +497,14 @@
         """
         ## # Service
 
         The service resource maps directly onto the json for the service endpoint in Kong.  For more information on the parameters [see the Kong Service create documentation](https://docs.konghq.com/gateway-oss/2.5.x/admin-api/#service-object).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
             name="test",
             protocol="http",
@@ -513,19 +512,17 @@
             port=8080,
             path="/mypath",
             retries=5,
             connect_timeout=1000,
             write_timeout=2000,
             read_timeout=3000)
         ```
-        <!--End PulumiCodeChooser -->
 
         To use a client certificate and ca certificates combine with certificate resource (note protocol must be `https`):
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         certificate = kong.Certificate("certificate",
             certificate=\"\"\"    -----BEGIN CERTIFICATE-----
             ......
@@ -551,15 +548,14 @@
             protocol="https",
             host="test.org",
             tls_verify=True,
             tls_verify_depth=2,
             client_certificate_id=certificate.id,
             ca_certificate_ids=[ca.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a service:
 
         ```sh
         $ pulumi import kong:index/service:Service <service_identifier> <service_id>
@@ -591,15 +587,14 @@
         """
         ## # Service
 
         The service resource maps directly onto the json for the service endpoint in Kong.  For more information on the parameters [see the Kong Service create documentation](https://docs.konghq.com/gateway-oss/2.5.x/admin-api/#service-object).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         service = kong.Service("service",
             name="test",
             protocol="http",
@@ -607,19 +602,17 @@
             port=8080,
             path="/mypath",
             retries=5,
             connect_timeout=1000,
             write_timeout=2000,
             read_timeout=3000)
         ```
-        <!--End PulumiCodeChooser -->
 
         To use a client certificate and ca certificates combine with certificate resource (note protocol must be `https`):
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         certificate = kong.Certificate("certificate",
             certificate=\"\"\"    -----BEGIN CERTIFICATE-----
             ......
@@ -645,15 +638,14 @@
             protocol="https",
             host="test.org",
             tls_verify=True,
             tls_verify_depth=2,
             client_certificate_id=certificate.id,
             ca_certificate_ids=[ca.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a service:
 
         ```sh
         $ pulumi import kong:index/service:Service <service_identifier> <service_id>
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/target.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,25 +161,23 @@
                  target: Optional[pulumi.Input[str]] = None,
                  upstream_id: Optional[pulumi.Input[str]] = None,
                  weight: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         target = kong.Target("target",
             target="sample_target:80",
             weight=10,
             upstream_id=upstream["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a target use a combination of the upstream id and the target id as follows:
 
         ```sh
         $ pulumi import kong:index/target:Target <target_identifier> <upstream_id>/<target_id>
@@ -197,25 +195,23 @@
     def __init__(__self__,
                  resource_name: str,
                  args: TargetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         target = kong.Target("target",
             target="sample_target:80",
             weight=10,
             upstream_id=upstream["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import a target use a combination of the upstream id and the target id as follows:
 
         ```sh
         $ pulumi import kong:index/target:Target <target_identifier> <upstream_id>/<target_id>
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong/upstream.py` & `pulumi_kong-4.6.0a1713898350/pulumi_kong/upstream.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,15 +506,14 @@
                  name: Optional[pulumi.Input[str]] = None,
                  slots: Optional[pulumi.Input[int]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         certificate = kong.Certificate("certificate",
             certificate=\"\"\"    -----BEGIN CERTIFICATE-----
             ......
@@ -586,15 +585,14 @@
                             501,
                             502,
                         ],
                     ),
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import an upstream:
 
         ```sh
         $ pulumi import kong:index/upstream:Upstream <upstream_identifier> <upstream_id>
@@ -640,15 +638,14 @@
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[UpstreamArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kong as kong
 
         certificate = kong.Certificate("certificate",
             certificate=\"\"\"    -----BEGIN CERTIFICATE-----
             ......
@@ -720,15 +717,14 @@
                             501,
                             502,
                         ],
                     ),
                 ),
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         To import an upstream:
 
         ```sh
         $ pulumi import kong:index/upstream:Upstream <upstream_identifier> <upstream_id>
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/PKG-INFO` & `pulumi_kong-4.6.0a1713898350/pulumi_kong.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kong
-Version: 4.6.0a1713561070
+Version: 4.6.0a1713898350
 Summary: A Pulumi package for creating and managing Kong resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kong
 Keywords: pulumi,kong
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kong-4.6.0a1713561070/pulumi_kong.egg-info/SOURCES.txt` & `pulumi_kong-4.6.0a1713898350/pulumi_kong.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kong-4.6.0a1713561070/pyproject.toml` & `pulumi_kong-4.6.0a1713898350/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kong"
   description = "A Pulumi package for creating and managing Kong resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "kong"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "4.6.0a1713561070"
+  version = "4.6.0a1713898350"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-kong"
 
 [build-system]
```

