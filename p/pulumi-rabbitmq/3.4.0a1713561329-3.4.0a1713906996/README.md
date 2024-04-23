# Comparing `tmp/pulumi_rabbitmq-3.4.0a1713561329.tar.gz` & `tmp/pulumi_rabbitmq-3.4.0a1713906996.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rabbitmq-3.4.0a1713561329.tar", last modified: Fri Apr 19 21:18:49 2024, max compression
+gzip compressed data, was "pulumi_rabbitmq-3.4.0a1713906996.tar", last modified: Tue Apr 23 21:20:13 2024, max compression
```

## Comparing `pulumi_rabbitmq-3.4.0a1713561329.tar` & `pulumi_rabbitmq-3.4.0a1713906996.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41845 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20753 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11398 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)    15249 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/federation_upstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_v_host.py
--rw-r--r--   0 runner    (1001) docker     (127)    12015 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/operator_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    37993 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11429 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11886 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/shovel.py
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/topic_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/v_host.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-19 21:18:49.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-19 21:18:49.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:18:49.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:18:49.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 21:18:49.000000 pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 21:18:43.000000 pulumi_rabbitmq-3.4.0a1713561329/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:18:49.423209 pulumi_rabbitmq-3.4.0a1713561329/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:20:13.991858 pulumi_rabbitmq-3.4.0a1713906996/
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-23 21:20:13.991858 pulumi_rabbitmq-3.4.0a1713906996/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:20:13.991858 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35649 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20597 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:20:13.991858 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11242 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15093 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/federation_upstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/get_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/get_v_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/operator_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32119 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13046 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/shovel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12035 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/topic_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/v_host.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:20:13.991858 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-23 21:20:13.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-23 21:20:13.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:20:13.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 21:20:13.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 21:20:13.000000 pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-23 21:20:07.000000 pulumi_rabbitmq-3.4.0a1713906996/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:20:13.991858 pulumi_rabbitmq-3.4.0a1713906996/setup.cfg
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1713906996/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rabbitmq
-Version: 3.4.0a1713561329
+Version: 3.4.0a1713906996
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi,rabbitmq
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/README.md` & `pulumi_rabbitmq-3.4.0a1713906996/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/__init__.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/_inputs.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/_inputs.py`

 * *Files 14% similar despite different names*

```diff
@@ -568,49 +568,14 @@
                  source_address: Optional[pulumi.Input[str]] = None,
                  source_delete_after: Optional[pulumi.Input[str]] = None,
                  source_exchange: Optional[pulumi.Input[str]] = None,
                  source_exchange_key: Optional[pulumi.Input[str]] = None,
                  source_prefetch_count: Optional[pulumi.Input[int]] = None,
                  source_protocol: Optional[pulumi.Input[str]] = None,
                  source_queue: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] destination_uri: The amqp uri for the destination .
-        :param pulumi.Input[str] source_uri: The amqp uri for the source.
-        :param pulumi.Input[str] ack_mode: Determines how the shovel should acknowledge messages. Possible values are: `on-confirm`, `on-publish` and `no-ack`.
-               Defaults to `on-confirm`.
-        :param pulumi.Input[bool] add_forward_headers: Whether to add `x-shovelled` headers to shovelled messages.
-        :param pulumi.Input[str] delete_after: Determines when (if ever) the shovel should delete itself. Possible values are: `never`, `queue-length` or an integer.
-        :param pulumi.Input[bool] destination_add_forward_headers: Whether to add `x-shovelled` headers to shovelled messages.
-        :param pulumi.Input[str] destination_address: The AMQP 1.0 destination link address.
-        :param pulumi.Input[str] destination_application_properties: Application properties to set when shovelling messages.
-        :param pulumi.Input[str] destination_exchange: The exchange to which messages should be published.
-               Either this or `destination_queue` must be specified but not both.
-        :param pulumi.Input[str] destination_exchange_key: The routing key when using `destination_exchange`.
-        :param pulumi.Input[str] destination_properties: Properties to overwrite when shovelling messages.
-               
-               For more details regarding dynamic shovel parameters please have a look at the official reference documentaion at [RabbitMQ: Configuring Dynamic Shovels](https://www.rabbitmq.com/shovel-dynamic.html).
-        :param pulumi.Input[str] destination_protocol: The protocol (`amqp091` or `amqp10`) to use when connecting to the destination.
-               Defaults to `amqp091`.
-        :param pulumi.Input[str] destination_publish_properties: A map of properties to overwrite when shovelling messages.
-        :param pulumi.Input[str] destination_queue: The queue to which messages should be published.
-               Either this or `destination_exchange` must be specified but not both.
-        :param pulumi.Input[int] prefetch_count: The maximum number of unacknowledged messages copied over a shovel at any one time.
-        :param pulumi.Input[int] reconnect_delay: The duration in seconds to reconnect to a broker after disconnected.
-               Defaults to `1`.
-        :param pulumi.Input[str] source_address: The AMQP 1.0 source link address.
-        :param pulumi.Input[str] source_delete_after: Determines when (if ever) the shovel should delete itself. Possible values are: `never`, `queue-length` or an integer.
-        :param pulumi.Input[str] source_exchange: The exchange from which to consume.
-               Either this or `source_queue` must be specified but not both.
-        :param pulumi.Input[str] source_exchange_key: The routing key when using `source_exchange`.
-        :param pulumi.Input[int] source_prefetch_count: The maximum number of unacknowledged messages copied over a shovel at any one time.
-        :param pulumi.Input[str] source_protocol: The protocol (`amqp091` or `amqp10`) to use when connecting to the source.
-               Defaults to `amqp091`.
-        :param pulumi.Input[str] source_queue: The queue from which to consume.
-               Either this or `source_exchange` must be specified but not both.
-        """
         pulumi.set(__self__, "destination_uri", destination_uri)
         pulumi.set(__self__, "source_uri", source_uri)
         if ack_mode is not None:
             pulumi.set(__self__, "ack_mode", ack_mode)
         if add_forward_headers is not None:
             warnings.warn("""use destination_add_forward_headers instead""", DeprecationWarning)
             pulumi.log.warn("""add_forward_headers is deprecated: use destination_add_forward_headers instead""")
@@ -662,84 +627,65 @@
             pulumi.set(__self__, "source_protocol", source_protocol)
         if source_queue is not None:
             pulumi.set(__self__, "source_queue", source_queue)
 
     @property
     @pulumi.getter(name="destinationUri")
     def destination_uri(self) -> pulumi.Input[str]:
-        """
-        The amqp uri for the destination .
-        """
         return pulumi.get(self, "destination_uri")
 
     @destination_uri.setter
     def destination_uri(self, value: pulumi.Input[str]):
         pulumi.set(self, "destination_uri", value)
 
     @property
     @pulumi.getter(name="sourceUri")
     def source_uri(self) -> pulumi.Input[str]:
-        """
-        The amqp uri for the source.
-        """
         return pulumi.get(self, "source_uri")
 
     @source_uri.setter
     def source_uri(self, value: pulumi.Input[str]):
         pulumi.set(self, "source_uri", value)
 
     @property
     @pulumi.getter(name="ackMode")
     def ack_mode(self) -> Optional[pulumi.Input[str]]:
-        """
-        Determines how the shovel should acknowledge messages. Possible values are: `on-confirm`, `on-publish` and `no-ack`.
-        Defaults to `on-confirm`.
-        """
         return pulumi.get(self, "ack_mode")
 
     @ack_mode.setter
     def ack_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ack_mode", value)
 
     @property
     @pulumi.getter(name="addForwardHeaders")
     def add_forward_headers(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether to add `x-shovelled` headers to shovelled messages.
-        """
         warnings.warn("""use destination_add_forward_headers instead""", DeprecationWarning)
         pulumi.log.warn("""add_forward_headers is deprecated: use destination_add_forward_headers instead""")
 
         return pulumi.get(self, "add_forward_headers")
 
     @add_forward_headers.setter
     def add_forward_headers(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "add_forward_headers", value)
 
     @property
     @pulumi.getter(name="deleteAfter")
     def delete_after(self) -> Optional[pulumi.Input[str]]:
-        """
-        Determines when (if ever) the shovel should delete itself. Possible values are: `never`, `queue-length` or an integer.
-        """
         warnings.warn("""use source_delete_after instead""", DeprecationWarning)
         pulumi.log.warn("""delete_after is deprecated: use source_delete_after instead""")
 
         return pulumi.get(self, "delete_after")
 
     @delete_after.setter
     def delete_after(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "delete_after", value)
 
     @property
     @pulumi.getter(name="destinationAddForwardHeaders")
     def destination_add_forward_headers(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether to add `x-shovelled` headers to shovelled messages.
-        """
         return pulumi.get(self, "destination_add_forward_headers")
 
     @destination_add_forward_headers.setter
     def destination_add_forward_headers(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "destination_add_forward_headers", value)
 
     @property
@@ -750,221 +696,161 @@
     @destination_add_timestamp_header.setter
     def destination_add_timestamp_header(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "destination_add_timestamp_header", value)
 
     @property
     @pulumi.getter(name="destinationAddress")
     def destination_address(self) -> Optional[pulumi.Input[str]]:
-        """
-        The AMQP 1.0 destination link address.
-        """
         return pulumi.get(self, "destination_address")
 
     @destination_address.setter
     def destination_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_address", value)
 
     @property
     @pulumi.getter(name="destinationApplicationProperties")
     def destination_application_properties(self) -> Optional[pulumi.Input[str]]:
-        """
-        Application properties to set when shovelling messages.
-        """
         return pulumi.get(self, "destination_application_properties")
 
     @destination_application_properties.setter
     def destination_application_properties(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_application_properties", value)
 
     @property
     @pulumi.getter(name="destinationExchange")
     def destination_exchange(self) -> Optional[pulumi.Input[str]]:
-        """
-        The exchange to which messages should be published.
-        Either this or `destination_queue` must be specified but not both.
-        """
         return pulumi.get(self, "destination_exchange")
 
     @destination_exchange.setter
     def destination_exchange(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_exchange", value)
 
     @property
     @pulumi.getter(name="destinationExchangeKey")
     def destination_exchange_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        The routing key when using `destination_exchange`.
-        """
         return pulumi.get(self, "destination_exchange_key")
 
     @destination_exchange_key.setter
     def destination_exchange_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_exchange_key", value)
 
     @property
     @pulumi.getter(name="destinationProperties")
     def destination_properties(self) -> Optional[pulumi.Input[str]]:
-        """
-        Properties to overwrite when shovelling messages.
-
-        For more details regarding dynamic shovel parameters please have a look at the official reference documentaion at [RabbitMQ: Configuring Dynamic Shovels](https://www.rabbitmq.com/shovel-dynamic.html).
-        """
         return pulumi.get(self, "destination_properties")
 
     @destination_properties.setter
     def destination_properties(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_properties", value)
 
     @property
     @pulumi.getter(name="destinationProtocol")
     def destination_protocol(self) -> Optional[pulumi.Input[str]]:
-        """
-        The protocol (`amqp091` or `amqp10`) to use when connecting to the destination.
-        Defaults to `amqp091`.
-        """
         return pulumi.get(self, "destination_protocol")
 
     @destination_protocol.setter
     def destination_protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_protocol", value)
 
     @property
     @pulumi.getter(name="destinationPublishProperties")
     def destination_publish_properties(self) -> Optional[pulumi.Input[str]]:
-        """
-        A map of properties to overwrite when shovelling messages.
-        """
         return pulumi.get(self, "destination_publish_properties")
 
     @destination_publish_properties.setter
     def destination_publish_properties(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_publish_properties", value)
 
     @property
     @pulumi.getter(name="destinationQueue")
     def destination_queue(self) -> Optional[pulumi.Input[str]]:
-        """
-        The queue to which messages should be published.
-        Either this or `destination_exchange` must be specified but not both.
-        """
         return pulumi.get(self, "destination_queue")
 
     @destination_queue.setter
     def destination_queue(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "destination_queue", value)
 
     @property
     @pulumi.getter(name="prefetchCount")
     def prefetch_count(self) -> Optional[pulumi.Input[int]]:
-        """
-        The maximum number of unacknowledged messages copied over a shovel at any one time.
-        """
         warnings.warn("""use source_prefetch_count instead""", DeprecationWarning)
         pulumi.log.warn("""prefetch_count is deprecated: use source_prefetch_count instead""")
 
         return pulumi.get(self, "prefetch_count")
 
     @prefetch_count.setter
     def prefetch_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "prefetch_count", value)
 
     @property
     @pulumi.getter(name="reconnectDelay")
     def reconnect_delay(self) -> Optional[pulumi.Input[int]]:
-        """
-        The duration in seconds to reconnect to a broker after disconnected.
-        Defaults to `1`.
-        """
         return pulumi.get(self, "reconnect_delay")
 
     @reconnect_delay.setter
     def reconnect_delay(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "reconnect_delay", value)
 
     @property
     @pulumi.getter(name="sourceAddress")
     def source_address(self) -> Optional[pulumi.Input[str]]:
-        """
-        The AMQP 1.0 source link address.
-        """
         return pulumi.get(self, "source_address")
 
     @source_address.setter
     def source_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source_address", value)
 
     @property
     @pulumi.getter(name="sourceDeleteAfter")
     def source_delete_after(self) -> Optional[pulumi.Input[str]]:
-        """
-        Determines when (if ever) the shovel should delete itself. Possible values are: `never`, `queue-length` or an integer.
-        """
         return pulumi.get(self, "source_delete_after")
 
     @source_delete_after.setter
     def source_delete_after(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source_delete_after", value)
 
     @property
     @pulumi.getter(name="sourceExchange")
     def source_exchange(self) -> Optional[pulumi.Input[str]]:
-        """
-        The exchange from which to consume.
-        Either this or `source_queue` must be specified but not both.
-        """
         return pulumi.get(self, "source_exchange")
 
     @source_exchange.setter
     def source_exchange(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source_exchange", value)
 
     @property
     @pulumi.getter(name="sourceExchangeKey")
     def source_exchange_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        The routing key when using `source_exchange`.
-        """
         return pulumi.get(self, "source_exchange_key")
 
     @source_exchange_key.setter
     def source_exchange_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source_exchange_key", value)
 
     @property
     @pulumi.getter(name="sourcePrefetchCount")
     def source_prefetch_count(self) -> Optional[pulumi.Input[int]]:
-        """
-        The maximum number of unacknowledged messages copied over a shovel at any one time.
-        """
         return pulumi.get(self, "source_prefetch_count")
 
     @source_prefetch_count.setter
     def source_prefetch_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "source_prefetch_count", value)
 
     @property
     @pulumi.getter(name="sourceProtocol")
     def source_protocol(self) -> Optional[pulumi.Input[str]]:
-        """
-        The protocol (`amqp091` or `amqp10`) to use when connecting to the source.
-        Defaults to `amqp091`.
-        """
         return pulumi.get(self, "source_protocol")
 
     @source_protocol.setter
     def source_protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source_protocol", value)
 
     @property
     @pulumi.getter(name="sourceQueue")
     def source_queue(self) -> Optional[pulumi.Input[str]]:
-        """
-        The queue from which to consume.
-        Either this or `source_exchange` must be specified but not both.
-        """
         return pulumi.get(self, "source_queue")
 
     @source_queue.setter
     def source_queue(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source_queue", value)
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/_utilities.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/binding.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,14 @@
                  __props__=None):
         """
         The ``Binding`` resource creates and manages a binding relationship
         between a queue an exchange.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -306,15 +305,14 @@
         test_binding = rabbitmq.Binding("test",
             source=test_exchange.name,
             vhost=test.name,
             destination=test_queue.name,
             destination_type="queue",
             routing_key="#")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Bindings can be imported using the `id` which is composed of
           `vhost/source/destination/destination_type/properties_key`. E.g.
 
         ```sh
@@ -338,15 +336,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The ``Binding`` resource creates and manages a binding relationship
         between a queue an exchange.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -374,15 +371,14 @@
         test_binding = rabbitmq.Binding("test",
             source=test_exchange.name,
             vhost=test.name,
             destination=test_queue.name,
             destination_type="queue",
             routing_key="#")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Bindings can be imported using the `id` which is composed of
           `vhost/source/destination/destination_type/properties_key`. E.g.
 
         ```sh
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/__init__.pyi` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/config/vars.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/exchange.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,14 @@
                  vhost: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The ``Exchange`` resource creates and manages an exchange.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -161,15 +160,14 @@
             vhost=guest.vhost,
             settings=rabbitmq.ExchangeSettingsArgs(
                 type="fanout",
                 durable=False,
                 auto_delete=True,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Exchanges can be imported using the `id` which is composed of  `name@vhost`.
 
         E.g.
 
@@ -191,15 +189,14 @@
                  args: ExchangeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The ``Exchange`` resource creates and manages an exchange.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -214,15 +211,14 @@
             vhost=guest.vhost,
             settings=rabbitmq.ExchangeSettingsArgs(
                 type="fanout",
                 durable=False,
                 auto_delete=True,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Exchanges can be imported using the `id` which is composed of  `name@vhost`.
 
         E.g.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/federation_upstream.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/federation_upstream.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,14 @@
                  vhost: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The ``FederationUpstream`` resource creates and manages a federation upstream parameter.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -195,15 +194,14 @@
                 priority=1,
                 apply_to="exchanges",
                 definition={
                     "federation-upstream": foo_federation_upstream.name,
                 },
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Federation upstream can be imported using the resource `id` which is composed of `name@vhost`, e.g.
 
         ```sh
         $ pulumi import rabbitmq:index/federationUpstream:FederationUpstream foo foo@test
@@ -222,15 +220,14 @@
                  args: FederationUpstreamArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The ``FederationUpstream`` resource creates and manages a federation upstream parameter.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -268,15 +265,14 @@
                 priority=1,
                 apply_to="exchanges",
                 definition={
                     "federation-upstream": foo_federation_upstream.name,
                 },
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         A Federation upstream can be imported using the resource `id` which is composed of `name@vhost`, e.g.
 
         ```sh
         $ pulumi import rabbitmq:index/federationUpstream:FederationUpstream foo foo@test
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_exchange.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/get_exchange.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_user.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/get_v_host.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/get_v_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/operator_policy.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/operator_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,14 @@
                  vhost: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The ``OperatorPolicy`` resource creates and manages operator policies for queues.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -164,15 +163,14 @@
                 apply_to="queues",
                 definition={
                     "message-ttl": 3600000,
                     "expires": 1800000,
                 },
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Operator policies can be imported using the `id` which is composed of `name@vhost`.
 
         E.g.
 
@@ -194,15 +192,14 @@
                  args: OperatorPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The ``OperatorPolicy`` resource creates and manages operator policies for queues.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -221,15 +218,14 @@
                 apply_to="queues",
                 definition={
                     "message-ttl": 3600000,
                     "expires": 1800000,
                 },
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Operator policies can be imported using the `id` which is composed of `name@vhost`.
 
         E.g.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/outputs.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/outputs.py`

 * *Files 20% similar despite different names*

```diff
@@ -613,49 +613,14 @@
                  source_address: Optional[str] = None,
                  source_delete_after: Optional[str] = None,
                  source_exchange: Optional[str] = None,
                  source_exchange_key: Optional[str] = None,
                  source_prefetch_count: Optional[int] = None,
                  source_protocol: Optional[str] = None,
                  source_queue: Optional[str] = None):
-        """
-        :param str destination_uri: The amqp uri for the destination .
-        :param str source_uri: The amqp uri for the source.
-        :param str ack_mode: Determines how the shovel should acknowledge messages. Possible values are: `on-confirm`, `on-publish` and `no-ack`.
-               Defaults to `on-confirm`.
-        :param bool add_forward_headers: Whether to add `x-shovelled` headers to shovelled messages.
-        :param str delete_after: Determines when (if ever) the shovel should delete itself. Possible values are: `never`, `queue-length` or an integer.
-        :param bool destination_add_forward_headers: Whether to add `x-shovelled` headers to shovelled messages.
-        :param str destination_address: The AMQP 1.0 destination link address.
-        :param str destination_application_properties: Application properties to set when shovelling messages.
-        :param str destination_exchange: The exchange to which messages should be published.
-               Either this or `destination_queue` must be specified but not both.
-        :param str destination_exchange_key: The routing key when using `destination_exchange`.
-        :param str destination_properties: Properties to overwrite when shovelling messages.
-               
-               For more details regarding dynamic shovel parameters please have a look at the official reference documentaion at [RabbitMQ: Configuring Dynamic Shovels](https://www.rabbitmq.com/shovel-dynamic.html).
-        :param str destination_protocol: The protocol (`amqp091` or `amqp10`) to use when connecting to the destination.
-               Defaults to `amqp091`.
-        :param str destination_publish_properties: A map of properties to overwrite when shovelling messages.
-        :param str destination_queue: The queue to which messages should be published.
-               Either this or `destination_exchange` must be specified but not both.
-        :param int prefetch_count: The maximum number of unacknowledged messages copied over a shovel at any one time.
-        :param int reconnect_delay: The duration in seconds to reconnect to a broker after disconnected.
-               Defaults to `1`.
-        :param str source_address: The AMQP 1.0 source link address.
-        :param str source_delete_after: Determines when (if ever) the shovel should delete itself. Possible values are: `never`, `queue-length` or an integer.
-        :param str source_exchange: The exchange from which to consume.
-               Either this or `source_queue` must be specified but not both.
-        :param str source_exchange_key: The routing key when using `source_exchange`.
-        :param int source_prefetch_count: The maximum number of unacknowledged messages copied over a shovel at any one time.
-        :param str source_protocol: The protocol (`amqp091` or `amqp10`) to use when connecting to the source.
-               Defaults to `amqp091`.
-        :param str source_queue: The queue from which to consume.
-               Either this or `source_exchange` must be specified but not both.
-        """
         pulumi.set(__self__, "destination_uri", destination_uri)
         pulumi.set(__self__, "source_uri", source_uri)
         if ack_mode is not None:
             pulumi.set(__self__, "ack_mode", ack_mode)
         if add_forward_headers is not None:
             pulumi.set(__self__, "add_forward_headers", add_forward_headers)
         if delete_after is not None:
@@ -698,217 +663,138 @@
             pulumi.set(__self__, "source_protocol", source_protocol)
         if source_queue is not None:
             pulumi.set(__self__, "source_queue", source_queue)
 
     @property
     @pulumi.getter(name="destinationUri")
     def destination_uri(self) -> str:
-        """
-        The amqp uri for the destination .
-        """
         return pulumi.get(self, "destination_uri")
 
     @property
     @pulumi.getter(name="sourceUri")
     def source_uri(self) -> str:
-        """
-        The amqp uri for the source.
-        """
         return pulumi.get(self, "source_uri")
 
     @property
     @pulumi.getter(name="ackMode")
     def ack_mode(self) -> Optional[str]:
-        """
-        Determines how the shovel should acknowledge messages. Possible values are: `on-confirm`, `on-publish` and `no-ack`.
-        Defaults to `on-confirm`.
-        """
         return pulumi.get(self, "ack_mode")
 
     @property
     @pulumi.getter(name="addForwardHeaders")
     def add_forward_headers(self) -> Optional[bool]:
-        """
-        Whether to add `x-shovelled` headers to shovelled messages.
-        """
         warnings.warn("""use destination_add_forward_headers instead""", DeprecationWarning)
         pulumi.log.warn("""add_forward_headers is deprecated: use destination_add_forward_headers instead""")
 
         return pulumi.get(self, "add_forward_headers")
 
     @property
     @pulumi.getter(name="deleteAfter")
     def delete_after(self) -> Optional[str]:
-        """
-        Determines when (if ever) the shovel should delete itself. Possible values are: `never`, `queue-length` or an integer.
-        """
         warnings.warn("""use source_delete_after instead""", DeprecationWarning)
         pulumi.log.warn("""delete_after is deprecated: use source_delete_after instead""")
 
         return pulumi.get(self, "delete_after")
 
     @property
     @pulumi.getter(name="destinationAddForwardHeaders")
     def destination_add_forward_headers(self) -> Optional[bool]:
-        """
-        Whether to add `x-shovelled` headers to shovelled messages.
-        """
         return pulumi.get(self, "destination_add_forward_headers")
 
     @property
     @pulumi.getter(name="destinationAddTimestampHeader")
     def destination_add_timestamp_header(self) -> Optional[bool]:
         return pulumi.get(self, "destination_add_timestamp_header")
 
     @property
     @pulumi.getter(name="destinationAddress")
     def destination_address(self) -> Optional[str]:
-        """
-        The AMQP 1.0 destination link address.
-        """
         return pulumi.get(self, "destination_address")
 
     @property
     @pulumi.getter(name="destinationApplicationProperties")
     def destination_application_properties(self) -> Optional[str]:
-        """
-        Application properties to set when shovelling messages.
-        """
         return pulumi.get(self, "destination_application_properties")
 
     @property
     @pulumi.getter(name="destinationExchange")
     def destination_exchange(self) -> Optional[str]:
-        """
-        The exchange to which messages should be published.
-        Either this or `destination_queue` must be specified but not both.
-        """
         return pulumi.get(self, "destination_exchange")
 
     @property
     @pulumi.getter(name="destinationExchangeKey")
     def destination_exchange_key(self) -> Optional[str]:
-        """
-        The routing key when using `destination_exchange`.
-        """
         return pulumi.get(self, "destination_exchange_key")
 
     @property
     @pulumi.getter(name="destinationProperties")
     def destination_properties(self) -> Optional[str]:
-        """
-        Properties to overwrite when shovelling messages.
-
-        For more details regarding dynamic shovel parameters please have a look at the official reference documentaion at [RabbitMQ: Configuring Dynamic Shovels](https://www.rabbitmq.com/shovel-dynamic.html).
-        """
         return pulumi.get(self, "destination_properties")
 
     @property
     @pulumi.getter(name="destinationProtocol")
     def destination_protocol(self) -> Optional[str]:
-        """
-        The protocol (`amqp091` or `amqp10`) to use when connecting to the destination.
-        Defaults to `amqp091`.
-        """
         return pulumi.get(self, "destination_protocol")
 
     @property
     @pulumi.getter(name="destinationPublishProperties")
     def destination_publish_properties(self) -> Optional[str]:
-        """
-        A map of properties to overwrite when shovelling messages.
-        """
         return pulumi.get(self, "destination_publish_properties")
 
     @property
     @pulumi.getter(name="destinationQueue")
     def destination_queue(self) -> Optional[str]:
-        """
-        The queue to which messages should be published.
-        Either this or `destination_exchange` must be specified but not both.
-        """
         return pulumi.get(self, "destination_queue")
 
     @property
     @pulumi.getter(name="prefetchCount")
     def prefetch_count(self) -> Optional[int]:
-        """
-        The maximum number of unacknowledged messages copied over a shovel at any one time.
-        """
         warnings.warn("""use source_prefetch_count instead""", DeprecationWarning)
         pulumi.log.warn("""prefetch_count is deprecated: use source_prefetch_count instead""")
 
         return pulumi.get(self, "prefetch_count")
 
     @property
     @pulumi.getter(name="reconnectDelay")
     def reconnect_delay(self) -> Optional[int]:
-        """
-        The duration in seconds to reconnect to a broker after disconnected.
-        Defaults to `1`.
-        """
         return pulumi.get(self, "reconnect_delay")
 
     @property
     @pulumi.getter(name="sourceAddress")
     def source_address(self) -> Optional[str]:
-        """
-        The AMQP 1.0 source link address.
-        """
         return pulumi.get(self, "source_address")
 
     @property
     @pulumi.getter(name="sourceDeleteAfter")
     def source_delete_after(self) -> Optional[str]:
-        """
-        Determines when (if ever) the shovel should delete itself. Possible values are: `never`, `queue-length` or an integer.
-        """
         return pulumi.get(self, "source_delete_after")
 
     @property
     @pulumi.getter(name="sourceExchange")
     def source_exchange(self) -> Optional[str]:
-        """
-        The exchange from which to consume.
-        Either this or `source_queue` must be specified but not both.
-        """
         return pulumi.get(self, "source_exchange")
 
     @property
     @pulumi.getter(name="sourceExchangeKey")
     def source_exchange_key(self) -> Optional[str]:
-        """
-        The routing key when using `source_exchange`.
-        """
         return pulumi.get(self, "source_exchange_key")
 
     @property
     @pulumi.getter(name="sourcePrefetchCount")
     def source_prefetch_count(self) -> Optional[int]:
-        """
-        The maximum number of unacknowledged messages copied over a shovel at any one time.
-        """
         return pulumi.get(self, "source_prefetch_count")
 
     @property
     @pulumi.getter(name="sourceProtocol")
     def source_protocol(self) -> Optional[str]:
-        """
-        The protocol (`amqp091` or `amqp10`) to use when connecting to the source.
-        Defaults to `amqp091`.
-        """
         return pulumi.get(self, "source_protocol")
 
     @property
     @pulumi.getter(name="sourceQueue")
     def source_queue(self) -> Optional[str]:
-        """
-        The queue from which to consume.
-        Either this or `source_exchange` must be specified but not both.
-        """
         return pulumi.get(self, "source_queue")
 
 
 @pulumi.output_type
 class TopicPermissionsPermission(dict):
     def __init__(__self__, *,
                  exchange: str,
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/permissions.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,14 @@
                  __props__=None):
         """
         The ``Permissions`` resource creates and manages a user's set of
         permissions.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         test_user = rabbitmq.User("test",
             name="mctest",
@@ -157,15 +156,14 @@
             vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
                 write=".*",
                 read=".*",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Permissions can be imported using the `id` which is composed of  `user@vhost`.
 
         E.g.
 
@@ -188,15 +186,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The ``Permissions`` resource creates and manages a user's set of
         permissions.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         test_user = rabbitmq.User("test",
             name="mctest",
@@ -207,15 +204,14 @@
             vhost=test.name,
             permissions=rabbitmq.PermissionsPermissionsArgs(
                 configure=".*",
                 write=".*",
                 read=".*",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Permissions can be imported using the `id` which is composed of  `user@vhost`.
 
         E.g.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/policy.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,14 @@
                  __props__=None):
         """
         The ``Policy`` resource creates and manages policies for exchanges
         and queues.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -164,15 +163,14 @@
                 priority=0,
                 apply_to="all",
                 definition={
                     "ha-mode": "all",
                 },
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Policies can be imported using the `id` which is composed of `name@vhost`.
 
         E.g.
 
@@ -195,15 +193,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The ``Policy`` resource creates and manages policies for exchanges
         and queues.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -221,15 +218,14 @@
                 priority=0,
                 apply_to="all",
                 definition={
                     "ha-mode": "all",
                 },
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Policies can be imported using the `id` which is composed of `name@vhost`.
 
         E.g.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/provider.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/queue.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/queue.py`

 * *Files 12% similar despite different names*

```diff
@@ -140,15 +140,14 @@
         """
         The ``Queue`` resource creates and manages a queue.
 
         ## Example Usage
 
         ### Basic Example
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -165,19 +164,17 @@
                 durable=False,
                 auto_delete=True,
                 arguments={
                     "x-queue-type": "quorum",
                 },
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example With JSON Arguments
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         config = pulumi.Config()
         arguments = config.get("arguments")
         if arguments is None:
@@ -199,15 +196,14 @@
             vhost=guest.vhost,
             settings=rabbitmq.QueueSettingsArgs(
                 durable=False,
                 auto_delete=True,
                 arguments_json=arguments,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Queues can be imported using the `id` which is composed of `name@vhost`. E.g.
 
         ```sh
         $ pulumi import rabbitmq:index/queue:Queue test name@vhost
@@ -229,15 +225,14 @@
         """
         The ``Queue`` resource creates and manages a queue.
 
         ## Example Usage
 
         ### Basic Example
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         guest = rabbitmq.Permissions("guest",
             user="guest",
@@ -254,19 +249,17 @@
                 durable=False,
                 auto_delete=True,
                 arguments={
                     "x-queue-type": "quorum",
                 },
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example With JSON Arguments
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         config = pulumi.Config()
         arguments = config.get("arguments")
         if arguments is None:
@@ -288,15 +281,14 @@
             vhost=guest.vhost,
             settings=rabbitmq.QueueSettingsArgs(
                 durable=False,
                 auto_delete=True,
                 arguments_json=arguments,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Queues can be imported using the `id` which is composed of `name@vhost`. E.g.
 
         ```sh
         $ pulumi import rabbitmq:index/queue:Queue test name@vhost
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/shovel.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/shovel.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,15 +137,14 @@
                  vhost: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The ``Shovel`` resource creates and manages a dynamic shovel.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         test_exchange = rabbitmq.Exchange("test",
             name="test_exchange",
@@ -169,15 +168,14 @@
                 source_uri="amqp:///test",
                 source_exchange=test_exchange.name,
                 source_exchange_key="test",
                 destination_uri="amqp:///test",
                 destination_queue=test_queue.name,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Shovels can be imported using the `name` and `vhost`
 
         E.g.
 
@@ -199,15 +197,14 @@
                  args: ShovelArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The ``Shovel`` resource creates and manages a dynamic shovel.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         test_exchange = rabbitmq.Exchange("test",
             name="test_exchange",
@@ -231,15 +228,14 @@
                 source_uri="amqp:///test",
                 source_exchange=test_exchange.name,
                 source_exchange_key="test",
                 destination_uri="amqp:///test",
                 destination_queue=test_queue.name,
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Shovels can be imported using the `name` and `vhost`
 
         E.g.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/topic_permissions.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/topic_permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,14 @@
                  __props__=None):
         """
         The ``TopicPermissions`` resource creates and manages a user's set of
         topic permissions.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         test_user = rabbitmq.User("test",
             name="mctest",
@@ -157,15 +156,14 @@
             vhost=test.name,
             permissions=[rabbitmq.TopicPermissionsPermissionArgs(
                 exchange="amq.topic",
                 write=".*",
                 read=".*",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Permissions can be imported using the `id` which is composed of  `user@vhost`.
 
         E.g.
 
@@ -188,15 +186,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The ``TopicPermissions`` resource creates and manages a user's set of
         topic permissions.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.VHost("test", name="test")
         test_user = rabbitmq.User("test",
             name="mctest",
@@ -207,15 +204,14 @@
             vhost=test.name,
             permissions=[rabbitmq.TopicPermissionsPermissionArgs(
                 exchange="amq.topic",
                 write=".*",
                 read=".*",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Permissions can be imported using the `id` which is composed of  `user@vhost`.
 
         E.g.
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/user.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/user.py`

 * *Files 7% similar despite different names*

```diff
@@ -143,28 +143,26 @@
         The ``User`` resource creates and manages a user.
 
         > **Note:** All arguments including username and password will be stored in the raw state as plain-text.
         [Read more about sensitive data in state](https://www.terraform.io/docs/state/sensitive-data.html).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.User("test",
             name="mctest",
             password="foobar",
             tags=[
                 "administrator",
                 "management",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported using the `name`, e.g.
 
         ```sh
         $ pulumi import rabbitmq:index/user:User test mctest
@@ -188,28 +186,26 @@
         The ``User`` resource creates and manages a user.
 
         > **Note:** All arguments including username and password will be stored in the raw state as plain-text.
         [Read more about sensitive data in state](https://www.terraform.io/docs/state/sensitive-data.html).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         test = rabbitmq.User("test",
             name="mctest",
             password="foobar",
             tags=[
                 "administrator",
                 "management",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported using the `name`, e.g.
 
         ```sh
         $ pulumi import rabbitmq:index/user:User test mctest
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq/v_host.py` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq/v_host.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,22 +67,20 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The ``VHost`` resource creates and manages a vhost.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         my_vhost = rabbitmq.VHost("my_vhost", name="my_vhost")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Vhosts can be imported using the `name`, e.g.
 
         ```sh
         $ pulumi import rabbitmq:index/vHost:VHost my_vhost my_vhost
@@ -99,22 +97,20 @@
                  args: Optional[VHostArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The ``VHost`` resource creates and manages a vhost.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_rabbitmq as rabbitmq
 
         my_vhost = rabbitmq.VHost("my_vhost", name="my_vhost")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Vhosts can be imported using the `name`, e.g.
 
         ```sh
         $ pulumi import rabbitmq:index/vHost:VHost my_vhost my_vhost
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/PKG-INFO` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rabbitmq
-Version: 3.4.0a1713561329
+Version: 3.4.0a1713906996
 Summary: A Pulumi package for creating and managing RabbitMQ resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rabbitmq
 Keywords: pulumi,rabbitmq
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pulumi_rabbitmq.egg-info/SOURCES.txt` & `pulumi_rabbitmq-3.4.0a1713906996/pulumi_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_rabbitmq-3.4.0a1713561329/pyproject.toml` & `pulumi_rabbitmq-3.4.0a1713906996/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rabbitmq"
   description = "A Pulumi package for creating and managing RabbitMQ resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rabbitmq"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.4.0a1713561329"
+  version = "3.4.0a1713906996"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rabbitmq"
 
 [build-system]
```

