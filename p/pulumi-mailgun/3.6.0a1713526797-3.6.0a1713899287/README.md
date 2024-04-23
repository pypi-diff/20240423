# Comparing `tmp/pulumi_mailgun-3.6.0a1713526797.tar.gz` & `tmp/pulumi_mailgun-3.6.0a1713899287.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_mailgun-3.6.0a1713526797.tar", last modified: Fri Apr 19 11:42:39 2024, max compression
+gzip compressed data, was "pulumi_mailgun-3.6.0a1713899287.tar", last modified: Tue Apr 23 19:41:28 2024, max compression
```

## Comparing `pulumi_mailgun-3.6.0a1713526797.tar` & `pulumi_mailgun-3.6.0a1713899287.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:42:39.985923 pulumi_mailgun-3.6.0a1713526797/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-19 11:42:39.985923 pulumi_mailgun-3.6.0a1713526797/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:42:39.985923 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:42:39.985923 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    36508 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    13520 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/domain_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14310 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/route.py
--rw-r--r--   0 runner    (1001) docker     (127)    12401 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 11:42:39.985923 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-19 11:42:39.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 11:42:39.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 11:42:39.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 11:42:39.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 11:42:39.000000 pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 11:42:33.000000 pulumi_mailgun-3.6.0a1713526797/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 11:42:39.985923 pulumi_mailgun-3.6.0a1713526797/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:41:28.092946 pulumi_mailgun-3.6.0a1713899287/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-23 19:41:28.092946 pulumi_mailgun-3.6.0a1713899287/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:41:28.088946 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:41:28.092946 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36352 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13364 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/domain_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:41:28.092946 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-23 19:41:28.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-23 19:41:28.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:41:28.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 19:41:28.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 19:41:28.000000 pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-23 19:41:21.000000 pulumi_mailgun-3.6.0a1713899287/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:41:28.092946 pulumi_mailgun-3.6.0a1713899287/setup.cfg
```

### Comparing `pulumi_mailgun-3.6.0a1713526797/PKG-INFO` & `pulumi_mailgun-3.6.0a1713899287/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mailgun
-Version: 3.6.0a1713526797
+Version: 3.6.0a1713899287
 Summary: A Pulumi package for creating and managing Mailgun resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mailgun
 Keywords: pulumi,mailgun
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mailgun-3.6.0a1713526797/README.md` & `pulumi_mailgun-3.6.0a1713899287/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/__init__.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/_inputs.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/_utilities.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/config/vars.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/domain.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,28 +440,26 @@
         Provides a Mailgun App resource. This can be used to
         create and manage applications on Mailgun.
 
         After DNS records are set, domain verification should be triggered manually using [PUT /domains/\\<domain\\>/verify](https://documentation.mailgun.com/en/latest/api-domains.html#domains)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mailgun as mailgun
 
         # Create a new Mailgun domain
         default = mailgun.Domain("default",
             name="test.example.com",
             region="us",
             spam_action="disabled",
             smtp_password="supersecretpassword1234",
             dkim_key_size=1024)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Domains can be imported using `region:domain_name` via `import` command. Region has to be chosen from `eu` or `us` (when no selection `us` is applied).
 
         hcl
 
@@ -494,28 +492,26 @@
         Provides a Mailgun App resource. This can be used to
         create and manage applications on Mailgun.
 
         After DNS records are set, domain verification should be triggered manually using [PUT /domains/\\<domain\\>/verify](https://documentation.mailgun.com/en/latest/api-domains.html#domains)
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mailgun as mailgun
 
         # Create a new Mailgun domain
         default = mailgun.Domain("default",
             name="test.example.com",
             region="us",
             spam_action="disabled",
             smtp_password="supersecretpassword1234",
             dkim_key_size=1024)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Domains can be imported using `region:domain_name` via `import` command. Region has to be chosen from `eu` or `us` (when no selection `us` is applied).
 
         hcl
```

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/domain_credential.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/domain_credential.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,27 +165,25 @@
         """
         Provides a Mailgun domain credential resource. This can be used to create and manage credential in domain of Mailgun.
 
         > **Note:** Please note that starting of v0.6.1 due to using new Mailgun Client API (v4), there is no possibility to retrieve previously created secrets via API. In order get it worked, it's recommended to mark `password` as ignored under `lifecycle` block. See below.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mailgun as mailgun
 
         # Create a new Mailgun credential
         foobar = mailgun.DomainCredential("foobar",
             domain="toto.com",
             login="test",
             password="supersecretpassword1234",
             region="us")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Domain credential can be imported using `region:email` via `import` command. Region has to be chosen from `eu` or `us` (when no selection `us` is applied).
 
         Password is always exported to `null`.
 
@@ -211,27 +209,25 @@
         """
         Provides a Mailgun domain credential resource. This can be used to create and manage credential in domain of Mailgun.
 
         > **Note:** Please note that starting of v0.6.1 due to using new Mailgun Client API (v4), there is no possibility to retrieve previously created secrets via API. In order get it worked, it's recommended to mark `password` as ignored under `lifecycle` block. See below.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mailgun as mailgun
 
         # Create a new Mailgun credential
         foobar = mailgun.DomainCredential("foobar",
             domain="toto.com",
             login="test",
             password="supersecretpassword1234",
             region="us")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Domain credential can be imported using `region:email` via `import` command. Region has to be chosen from `eu` or `us` (when no selection `us` is applied).
 
         Password is always exported to `null`.
```

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/get_domain.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/get_domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,14 @@
                wildcard: Optional[bool] = None,
                opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetDomainResult:
     """
     `Domain` provides details about a Mailgun domain.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_aws as aws
     import pulumi_mailgun as mailgun
 
     domain = mailgun.get_domain(name="test.example.com")
     mailgun_mx = aws.index.Route53Record("mailgun-mx",
@@ -226,15 +225,14 @@
         type=MX,
         ttl=3600,
         records=[
             f{domain.receiving_records[0].priority} {domain.receiving_records[0].value}.,
             f{domain.receiving_records[1].priority} {domain.receiving_records[1].value}.,
         ])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the domain.
     :param str region: The region where domain will be created. Default value is `us`.
     :param str smtp_password: The password to the SMTP server.
     :param str spam_action: The spam filtering setting.
     :param bool wildcard: Whether or not the domain will accept email for sub-domains.
@@ -282,15 +280,14 @@
                       wildcard: Optional[pulumi.Input[Optional[bool]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainResult]:
     """
     `Domain` provides details about a Mailgun domain.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_aws as aws
     import pulumi_mailgun as mailgun
 
     domain = mailgun.get_domain(name="test.example.com")
     mailgun_mx = aws.index.Route53Record("mailgun-mx",
@@ -299,15 +296,14 @@
         type=MX,
         ttl=3600,
         records=[
             f{domain.receiving_records[0].priority} {domain.receiving_records[0].value}.,
             f{domain.receiving_records[1].priority} {domain.receiving_records[1].value}.,
         ])
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the domain.
     :param str region: The region where domain will be created. Default value is `us`.
     :param str smtp_password: The password to the SMTP server.
     :param str spam_action: The spam filtering setting.
     :param bool wildcard: Whether or not the domain will accept email for sub-domains.
```

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/outputs.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/provider.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/route.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/route.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,30 +180,28 @@
                  region: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Mailgun Route resource. This can be used to create and manage routes on Mailgun.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mailgun as mailgun
 
         # Create a new Mailgun route
         default = mailgun.Route("default",
             priority=0,
             description="inbound",
             expression="match_recipient('.*@foo.example.com')",
             actions=[
                 "forward('http://example.com/api/v1/foos/')",
                 "stop()",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Routes can be imported using `ROUTE_ID` and `region` via `import` command. Route ID can be found on Mailgun portal in section `Receiving/Routes`. Region has to be chosen from `eu` or `us` (when no selection `us` is applied).
 
         hcl
 
@@ -224,30 +222,28 @@
                  args: RouteArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Mailgun Route resource. This can be used to create and manage routes on Mailgun.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mailgun as mailgun
 
         # Create a new Mailgun route
         default = mailgun.Route("default",
             priority=0,
             description="inbound",
             expression="match_recipient('.*@foo.example.com')",
             actions=[
                 "forward('http://example.com/api/v1/foos/')",
                 "stop()",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Routes can be imported using `ROUTE_ID` and `region` via `import` command. Route ID can be found on Mailgun portal in section `Receiving/Routes`. Region has to be chosen from `eu` or `us` (when no selection `us` is applied).
 
         hcl
```

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun/webhook.py` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun/webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,27 +164,25 @@
                  __props__=None):
         """
         Provides a Mailgun App resource. This can be used to
         create and manage applications on Mailgun.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mailgun as mailgun
 
         # Create a new Mailgun webhook
         default = mailgun.Webhook("default",
             domain="test.example.com",
             region="us",
             kind="delivered",
             urls=["https://example.com"])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] domain: The domain to add to Mailgun
         :param pulumi.Input[str] kind: The kind of webhook. Supported values (`clicked` `complained` `delivered` `opened` `permanent_fail`, `temporary_fail` `unsubscribed`)
         :param pulumi.Input[str] region: The region where domain will be created. Default value is `us`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] urls: The urls of webhook
@@ -197,27 +195,25 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a Mailgun App resource. This can be used to
         create and manage applications on Mailgun.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mailgun as mailgun
 
         # Create a new Mailgun webhook
         default = mailgun.Webhook("default",
             domain="test.example.com",
             region="us",
             kind="delivered",
             urls=["https://example.com"])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param WebhookArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun.egg-info/PKG-INFO` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mailgun
-Version: 3.6.0a1713526797
+Version: 3.6.0a1713899287
 Summary: A Pulumi package for creating and managing Mailgun resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mailgun
 Keywords: pulumi,mailgun
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mailgun-3.6.0a1713526797/pulumi_mailgun.egg-info/SOURCES.txt` & `pulumi_mailgun-3.6.0a1713899287/pulumi_mailgun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_mailgun-3.6.0a1713526797/pyproject.toml` & `pulumi_mailgun-3.6.0a1713899287/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_mailgun"
   description = "A Pulumi package for creating and managing Mailgun resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "mailgun"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.6.0a1713526797"
+  version = "3.6.0a1713899287"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-mailgun"
 
 [build-system]
```

