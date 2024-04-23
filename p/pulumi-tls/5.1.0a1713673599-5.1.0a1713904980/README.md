# Comparing `tmp/pulumi_tls-5.1.0a1713673599.tar.gz` & `tmp/pulumi_tls-5.1.0a1713904980.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_tls-5.1.0a1713673599.tar", last modified: Sun Apr 21 04:29:05 2024, max compression
+gzip compressed data, was "pulumi_tls-5.1.0a1713904980.tar", last modified: Tue Apr 23 20:49:31 2024, max compression
```

## Comparing `pulumi_tls-5.1.0a1713673599.tar` & `pulumi_tls-5.1.0a1713904980.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:29:05.608087 pulumi_tls-5.1.0a1713673599/
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-21 04:29:05.604087 pulumi_tls-5.1.0a1713673599/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:29:05.604087 pulumi_tls-5.1.0a1713673599/pulumi_tls/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20591 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/cert_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:29:05.604087 pulumi_tls-5.1.0a1713673599/pulumi_tls/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10489 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/get_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    41155 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/locally_signed_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    50239 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls/self_signed_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:29:05.604087 pulumi_tls-5.1.0a1713673599/pulumi_tls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-21 04:29:05.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-21 04:29:05.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 04:29:05.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-21 04:29:05.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 04:29:05.000000 pulumi_tls-5.1.0a1713673599/pulumi_tls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-21 04:28:59.000000 pulumi_tls-5.1.0a1713673599/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 04:29:05.608087 pulumi_tls-5.1.0a1713673599/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:49:31.067421 pulumi_tls-5.1.0a1713904980/
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-23 20:49:31.067421 pulumi_tls-5.1.0a1713904980/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:49:31.063421 pulumi_tls-5.1.0a1713904980/pulumi_tls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/cert_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:49:31.063421 pulumi_tls-5.1.0a1713904980/pulumi_tls/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/get_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41155 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/locally_signed_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    50239 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls/self_signed_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:49:31.063421 pulumi_tls-5.1.0a1713904980/pulumi_tls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-23 20:49:31.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 20:49:31.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:49:31.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 20:49:31.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 20:49:31.000000 pulumi_tls-5.1.0a1713904980/pulumi_tls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-23 20:49:24.000000 pulumi_tls-5.1.0a1713904980/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:49:31.067421 pulumi_tls-5.1.0a1713904980/setup.cfg
```

### Comparing `pulumi_tls-5.1.0a1713673599/PKG-INFO` & `pulumi_tls-5.1.0a1713904980/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_tls
-Version: 5.1.0a1713673599
+Version: 5.1.0a1713904980
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi,tls
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_tls-5.1.0a1713673599/README.md` & `pulumi_tls-5.1.0a1713904980/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/__init__.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/_inputs.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/_utilities.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/cert_request.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/cert_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,28 +230,26 @@
                  private_key_pem: Optional[pulumi.Input[str]] = None,
                  subject: Optional[pulumi.Input[pulumi.InputType['CertRequestSubjectArgs']]] = None,
                  uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_std as std
         import pulumi_tls as tls
 
         example = tls.CertRequest("example",
             private_key_pem=std.file(input="private_key.pem").result,
             subject=tls.CertRequestSubjectArgs(
                 common_name="example.com",
                 organization="ACME Examples, Inc",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[str] private_key_pem: Private key in PEM (RFC 1421) interpolation function.
         :param pulumi.Input[pulumi.InputType['CertRequestSubjectArgs']] subject: The subject for which a certificate is being requested. The acceptable arguments are all optional and their naming is based upon [Issuer Distinguished Names (RFC5280)](https://tools.ietf.org/html/rfc5280#section-4.1.2.4) section.
@@ -262,28 +260,26 @@
     def __init__(__self__,
                  resource_name: str,
                  args: CertRequestArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_std as std
         import pulumi_tls as tls
 
         example = tls.CertRequest("example",
             private_key_pem=std.file(input="private_key.pem").result,
             subject=tls.CertRequestSubjectArgs(
                 common_name="example.com",
                 organization="ACME Examples, Inc",
             ))
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param CertRequestArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/config/outputs.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/config/vars.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/get_certificate.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/get_public_key.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/get_public_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,27 +134,25 @@
     """
     Get a public key from a PEM-encoded private key.
 
     Use this data source to get the public key from a [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) or [OpenSSH PEM (RFC 4716)](https://datatracker.ietf.org/doc/html/rfc4716) formatted private key, for use in other resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_std as std
     import pulumi_tls as tls
 
     ed25519_example = tls.PrivateKey("ed25519-example", algorithm="ED25519")
     # Public key loaded from a terraform-generated private key, using the PEM (RFC 1421) format
     private_key_pem_example = tls.get_public_key_output(private_key_pem=ed25519_example.private_key_pem)
     # Public key loaded from filesystem, using the Open SSH (RFC 4716) format
     private_key_openssh_example = tls.get_public_key(private_key_openssh=std.file(input="~/.ssh/id_rsa_rfc4716").result)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str private_key_openssh: The private key (in  [OpenSSH PEM (RFC 4716)](https://datatracker.ietf.org/doc/html/rfc4716) format) to extract the public key from. This is *mutually exclusive* with `private_key_pem`. Currently-supported algorithms for keys are: `RSA`, `ECDSA`, `ED25519`.
     :param str private_key_pem: The private key (in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format) to extract the public key from. This is *mutually exclusive* with `private_key_openssh`. Currently-supported algorithms for keys are: `RSA`, `ECDSA`, `ED25519`.
     """
     __args__ = dict()
     __args__['privateKeyOpenssh'] = private_key_openssh
@@ -180,26 +178,24 @@
     """
     Get a public key from a PEM-encoded private key.
 
     Use this data source to get the public key from a [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) or [OpenSSH PEM (RFC 4716)](https://datatracker.ietf.org/doc/html/rfc4716) formatted private key, for use in other resources.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_std as std
     import pulumi_tls as tls
 
     ed25519_example = tls.PrivateKey("ed25519-example", algorithm="ED25519")
     # Public key loaded from a terraform-generated private key, using the PEM (RFC 1421) format
     private_key_pem_example = tls.get_public_key_output(private_key_pem=ed25519_example.private_key_pem)
     # Public key loaded from filesystem, using the Open SSH (RFC 4716) format
     private_key_openssh_example = tls.get_public_key(private_key_openssh=std.file(input="~/.ssh/id_rsa_rfc4716").result)
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str private_key_openssh: The private key (in  [OpenSSH PEM (RFC 4716)](https://datatracker.ietf.org/doc/html/rfc4716) format) to extract the public key from. This is *mutually exclusive* with `private_key_pem`. Currently-supported algorithms for keys are: `RSA`, `ECDSA`, `ED25519`.
     :param str private_key_pem: The private key (in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format) to extract the public key from. This is *mutually exclusive* with `private_key_openssh`. Currently-supported algorithms for keys are: `RSA`, `ECDSA`, `ED25519`.
     """
     ...
```

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/locally_signed_cert.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/locally_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/outputs.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/private_key.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/provider.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls/self_signed_cert.py` & `pulumi_tls-5.1.0a1713904980/pulumi_tls/self_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls.egg-info/PKG-INFO` & `pulumi_tls-5.1.0a1713904980/pulumi_tls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_tls
-Version: 5.1.0a1713673599
+Version: 5.1.0a1713904980
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi,tls
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_tls-5.1.0a1713673599/pulumi_tls.egg-info/SOURCES.txt` & `pulumi_tls-5.1.0a1713904980/pulumi_tls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1713673599/pyproject.toml` & `pulumi_tls-5.1.0a1713904980/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_tls"
   description = "A Pulumi package to create TLS resources in Pulumi programs."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "tls"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "5.1.0a1713673599"
+  version = "5.1.0a1713904980"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-tls"
 
 [build-system]
```

