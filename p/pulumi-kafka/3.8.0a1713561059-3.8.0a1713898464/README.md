# Comparing `tmp/pulumi_kafka-3.8.0a1713561059.tar.gz` & `tmp/pulumi_kafka-3.8.0a1713898464.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kafka-3.8.0a1713561059.tar", last modified: Fri Apr 19 21:13:43 2024, max compression
+gzip compressed data, was "pulumi_kafka-3.8.0a1713898464.tar", last modified: Tue Apr 23 19:28:28 2024, max compression
```

## Comparing `pulumi_kafka-3.8.0a1713561059.tar` & `pulumi_kafka-3.8.0a1713898464.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:13:43.917254 pulumi_kafka-3.8.0a1713561059/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-19 21:13:43.917254 pulumi_kafka-3.8.0a1713561059/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:13:43.913254 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23273 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:13:43.913254 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/get_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    31331 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10408 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka/user_scram_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:13:43.913254 pulumi_kafka-3.8.0a1713561059/pulumi_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-19 21:13:43.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-19 21:13:43.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:13:43.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:13:43.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 21:13:43.000000 pulumi_kafka-3.8.0a1713561059/pulumi_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 21:13:37.000000 pulumi_kafka-3.8.0a1713561059/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:13:43.917254 pulumi_kafka-3.8.0a1713561059/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:28:28.679275 pulumi_kafka-3.8.0a1713898464/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-23 19:28:28.679275 pulumi_kafka-3.8.0a1713898464/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:28:28.679275 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:28:28.679275 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/get_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31331 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka/user_scram_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:28:28.679275 pulumi_kafka-3.8.0a1713898464/pulumi_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-23 19:28:28.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-23 19:28:28.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:28:28.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 19:28:28.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 19:28:28.000000 pulumi_kafka-3.8.0a1713898464/pulumi_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-23 19:28:22.000000 pulumi_kafka-3.8.0a1713898464/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:28:28.679275 pulumi_kafka-3.8.0a1713898464/setup.cfg
```

### Comparing `pulumi_kafka-3.8.0a1713561059/PKG-INFO` & `pulumi_kafka-3.8.0a1713898464/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.8.0a1713561059
+Version: 3.8.0a1713898464
 Summary: A Pulumi package for creating and managing Kafka.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi,kafka
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.8.0a1713561059/README.md` & `pulumi_kafka-3.8.0a1713898464/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka/__init__.py` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka/_utilities.py` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka/acl.py` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka/acl.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,28 +283,26 @@
                  resource_pattern_type_filter: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         A resource for managing Kafka ACLs.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kafka as kafka
 
         test = kafka.Acl("test",
             acl_resource_name="syslog",
             acl_resource_type="Topic",
             acl_principal="User:Alice",
             acl_host="*",
             acl_operation="Write",
             acl_permission_type="Deny")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ACLs can be imported using the following pattern
 
         ```sh
         $ pulumi import kafka:index/acl:Acl test "acl_principal|acl_host|acl_operation|acl_permission_type|resource_type|resource_name|resource_pattern_type_filter"
@@ -338,28 +336,26 @@
                  args: AclArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         A resource for managing Kafka ACLs.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kafka as kafka
 
         test = kafka.Acl("test",
             acl_resource_name="syslog",
             acl_resource_type="Topic",
             acl_principal="User:Alice",
             acl_host="*",
             acl_operation="Write",
             acl_permission_type="Deny")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         ACLs can be imported using the following pattern
 
         ```sh
         $ pulumi import kafka:index/acl:Acl test "acl_principal|acl_host|acl_operation|acl_permission_type|resource_type|resource_name|resource_pattern_type_filter"
```

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka/config/__init__.pyi` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka/config/vars.py` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka/get_topic.py` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka/get_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka/provider.py` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka/quota.py` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka/quota.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,28 +131,26 @@
                  entity_type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         A resource for managing Kafka quotas.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kafka as kafka
 
         quota = kafka.Quota("quota",
             entity_name="app_consumer",
             entity_type="client-id",
             config={
                 "consumer_byte_rate": "5000000",
                 "producer_byte_rate": "2500000",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Mapping[str, Any]] config: A map of string k/v attributes.
         :param pulumi.Input[str] entity_name: The name of the entity to target.
         :param pulumi.Input[str] entity_type: The type of entity. Valid values are `client-id`, `user`, `ip`.
         """
@@ -163,28 +161,26 @@
                  args: QuotaArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         A resource for managing Kafka quotas.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kafka as kafka
 
         quota = kafka.Quota("quota",
             entity_name="app_consumer",
             entity_type="client-id",
             config={
                 "consumer_byte_rate": "5000000",
                 "producer_byte_rate": "2500000",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param QuotaArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka/topic.py` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka/topic.py`

 * *Files 8% similar despite different names*

```diff
@@ -164,29 +164,27 @@
                  replication_factor: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
         A resource for managing Kafka topics. Increases partition count without destroying the topic.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kafka as kafka
 
         logs = kafka.Topic("logs",
             name="systemd_logs",
             replication_factor=2,
             partitions=100,
             config={
                 "segment.ms": "20000",
                 "cleanup.policy": "compact",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Topics can be imported using their ARN, e.g.
 
         ```sh
         $ pulumi import kafka:index/topic:Topic logs systemd_logs
@@ -206,29 +204,27 @@
                  args: TopicArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         A resource for managing Kafka topics. Increases partition count without destroying the topic.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_kafka as kafka
 
         logs = kafka.Topic("logs",
             name="systemd_logs",
             replication_factor=2,
             partitions=100,
             config={
                 "segment.ms": "20000",
                 "cleanup.policy": "compact",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Topics can be imported using their ARN, e.g.
 
         ```sh
         $ pulumi import kafka:index/topic:Topic logs systemd_logs
```

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka/user_scram_credential.py` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka/user_scram_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka.egg-info/PKG-INFO` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.8.0a1713561059
+Version: 3.8.0a1713898464
 Summary: A Pulumi package for creating and managing Kafka.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi,kafka
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.8.0a1713561059/pulumi_kafka.egg-info/SOURCES.txt` & `pulumi_kafka-3.8.0a1713898464/pulumi_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1713561059/pyproject.toml` & `pulumi_kafka-3.8.0a1713898464/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kafka"
   description = "A Pulumi package for creating and managing Kafka."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "kafka"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.8.0a1713561059"
+  version = "3.8.0a1713898464"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-kafka"
 
 [build-system]
```

