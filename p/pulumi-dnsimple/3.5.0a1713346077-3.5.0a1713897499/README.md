# Comparing `tmp/pulumi_dnsimple-3.5.0a1713346077.tar.gz` & `tmp/pulumi_dnsimple-3.5.0a1713897499.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_dnsimple-3.5.0a1713346077.tar", last modified: Wed Apr 17 09:30:31 2024, max compression
+gzip compressed data, was "pulumi_dnsimple-3.5.0a1713897499.tar", last modified: Tue Apr 23 19:04:17 2024, max compression
```

## Comparing `pulumi_dnsimple-3.5.0a1713346077.tar` & `pulumi_dnsimple-3.5.0a1713897499.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:31.292579 pulumi_dnsimple-3.5.0a1713346077/
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-17 09:30:31.292579 pulumi_dnsimple-3.5.0a1713346077/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:31.288579 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:31.292579 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    13282 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/email_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    19920 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/lets_encrypt_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/record.py
--rw-r--r--   0 runner    (1001) docker     (127)    19029 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/zone_record.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:30:31.292579 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-17 09:30:31.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-17 09:30:31.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:30:31.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 09:30:31.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-17 09:30:31.000000 pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-17 09:30:24.000000 pulumi_dnsimple-3.5.0a1713346077/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:30:31.292579 pulumi_dnsimple-3.5.0a1713346077/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:04:17.776919 pulumi_dnsimple-3.5.0a1713897499/
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-23 19:04:17.776919 pulumi_dnsimple-3.5.0a1713897499/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:04:17.772918 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:04:17.776919 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11788 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/email_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/lets_encrypt_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8730 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12552 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18717 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/zone_record.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:04:17.776919 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-23 19:04:17.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-23 19:04:17.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:04:17.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 19:04:17.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 19:04:17.000000 pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-23 19:04:10.000000 pulumi_dnsimple-3.5.0a1713897499/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:04:17.776919 pulumi_dnsimple-3.5.0a1713897499/setup.cfg
```

### Comparing `pulumi_dnsimple-3.5.0a1713346077/PKG-INFO` & `pulumi_dnsimple-3.5.0a1713897499/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dnsimple
-Version: 3.5.0a1713346077
+Version: 3.5.0a1713897499
 Summary: A Pulumi package for creating and managing dnsimple cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-dnsimple
 Keywords: pulumi,dnsimple
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dnsimple-3.5.0a1713346077/README.md` & `pulumi_dnsimple-3.5.0a1713897499/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/__init__.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/_utilities.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/config/__init__.pyi` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/config/vars.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/domain.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,23 +138,21 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a DNSimple domain resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_dnsimple as dnsimple
 
         # Create a domain
         foobar = dnsimple.Domain("foobar", name=dnsimple["domain"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         DNSimple domains can be imported using their numeric record ID.
 
         ```sh
         $ pulumi import dnsimple:index/domain:Domain resource_name 5678
@@ -223,23 +221,21 @@
                  args: DomainArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a DNSimple domain resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_dnsimple as dnsimple
 
         # Create a domain
         foobar = dnsimple.Domain("foobar", name=dnsimple["domain"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         DNSimple domains can be imported using their numeric record ID.
 
         ```sh
         $ pulumi import dnsimple:index/domain:Domain resource_name 5678
```

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/email_forward.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/email_forward.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,26 +146,24 @@
                  domain: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a DNSimple email forward resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_dnsimple as dnsimple
 
         # Add an email forwarding rule to the domain
         foobar = dnsimple.EmailForward("foobar",
             domain=dnsimple_domain,
             alias_name="sales",
             destination_email="jane.doe@example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] alias_name: The name part (the part before the @) of the source email address on the domain
         :param pulumi.Input[str] destination_email: The destination email address on another domain
         :param pulumi.Input[str] domain: The domain to add the email forwarding rule to
         """
@@ -176,26 +174,24 @@
                  args: EmailForwardArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a DNSimple email forward resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_dnsimple as dnsimple
 
         # Add an email forwarding rule to the domain
         foobar = dnsimple.EmailForward("foobar",
             domain=dnsimple_domain,
             alias_name="sales",
             destination_email="jane.doe@example.com")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param EmailForwardArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/get_certificate.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/get_certificate.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,23 +114,21 @@
                     domain: Optional[str] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetCertificateResult:
     """
     Provides a DNSimple certificate data source.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_dnsimple as dnsimple
 
     foobar = dnsimple.get_certificate(domain=dnsimple_domain,
         certificate_id=dnsimple_certificate_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str certificate_id: The ID of the SSL Certificate
     :param str domain: The domain of the SSL Certificate
     """
     __args__ = dict()
     __args__['certificateId'] = certificate_id
@@ -153,22 +151,20 @@
                            domain: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetCertificateResult]:
     """
     Provides a DNSimple certificate data source.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_dnsimple as dnsimple
 
     foobar = dnsimple.get_certificate(domain=dnsimple_domain,
         certificate_id=dnsimple_certificate_id)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str certificate_id: The ID of the SSL Certificate
     :param str domain: The domain of the SSL Certificate
     """
     ...
```

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/get_zone.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/get_zone.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,22 +71,20 @@
 def get_zone(name: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetZoneResult:
     """
     Get information about a DNSimple zone.
 
     Get zone:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_dnsimple as dnsimple
 
     foobar = dnsimple.get_zone(name="dnsimple.com")
     ```
-    <!--End PulumiCodeChooser -->
 
     The following arguments are supported:
 
     * `name` - (Required) The name of the zone
 
     The following attributes are exported:
 
@@ -111,22 +109,20 @@
 def get_zone_output(name: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetZoneResult]:
     """
     Get information about a DNSimple zone.
 
     Get zone:
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_dnsimple as dnsimple
 
     foobar = dnsimple.get_zone(name="dnsimple.com")
     ```
-    <!--End PulumiCodeChooser -->
 
     The following arguments are supported:
 
     * `name` - (Required) The name of the zone
 
     The following attributes are exported:
```

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/lets_encrypt_certificate.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/lets_encrypt_certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,25 +276,23 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a DNSimple Let's Encrypt certificate resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_dnsimple as dnsimple
 
         foobar = dnsimple.LetsEncryptCertificate("foobar",
             domain_id=dnsimple["domainId"],
             auto_renew=False,
             name="www")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] auto_renew: Set to true if the certificate will auto-renew
         :param pulumi.Input[int] contact_id: The contact id for the certificate
         :param pulumi.Input[str] domain_id: The domain to be issued the certificate for
         :param pulumi.Input[str] name: The certificate name
@@ -306,25 +304,23 @@
                  args: LetsEncryptCertificateArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Provides a DNSimple Let's Encrypt certificate resource.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_dnsimple as dnsimple
 
         foobar = dnsimple.LetsEncryptCertificate("foobar",
             domain_id=dnsimple["domainId"],
             auto_renew=False,
             name="www")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param LetsEncryptCertificateArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/provider.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/record.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/record.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple/zone_record.py` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple/zone_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,43 +265,39 @@
         ## Deprecation warning
 
         You can still use the _deprecated_ `Record` configuration, but be aware that it will be removed in the
         upcoming 1.0.0 release.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_dnsimple as dnsimple
 
         # Add a record to the root domain
         foobar = dnsimple.ZoneRecord("foobar",
             zone_name=dnsimple_domain,
             name="",
             value="192.168.0.11",
             type="A",
             ttl="3600")
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_dnsimple as dnsimple
 
         # Add a record to a sub-domain
         foobar = dnsimple.ZoneRecord("foobar",
             zone_name=dnsimple_domain,
             name="terraform",
             value="192.168.0.11",
             type="A",
             ttl="3600")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         DNSimple resources can be imported using their parent zone name (domain name) and numeric record ID.
 
         __Importing record example.com with record ID 1234__
 
@@ -336,43 +332,39 @@
         ## Deprecation warning
 
         You can still use the _deprecated_ `Record` configuration, but be aware that it will be removed in the
         upcoming 1.0.0 release.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_dnsimple as dnsimple
 
         # Add a record to the root domain
         foobar = dnsimple.ZoneRecord("foobar",
             zone_name=dnsimple_domain,
             name="",
             value="192.168.0.11",
             type="A",
             ttl="3600")
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_dnsimple as dnsimple
 
         # Add a record to a sub-domain
         foobar = dnsimple.ZoneRecord("foobar",
             zone_name=dnsimple_domain,
             name="terraform",
             value="192.168.0.11",
             type="A",
             ttl="3600")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         DNSimple resources can be imported using their parent zone name (domain name) and numeric record ID.
 
         __Importing record example.com with record ID 1234__
```

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple.egg-info/PKG-INFO` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dnsimple
-Version: 3.5.0a1713346077
+Version: 3.5.0a1713897499
 Summary: A Pulumi package for creating and managing dnsimple cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-dnsimple
 Keywords: pulumi,dnsimple
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pulumi_dnsimple.egg-info/SOURCES.txt` & `pulumi_dnsimple-3.5.0a1713897499/pulumi_dnsimple.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1713346077/pyproject.toml` & `pulumi_dnsimple-3.5.0a1713897499/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_dnsimple"
   description = "A Pulumi package for creating and managing dnsimple cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "dnsimple"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.5.0a1713346077"
+  version = "3.5.0a1713897499"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-dnsimple"
 
 [build-system]
```

