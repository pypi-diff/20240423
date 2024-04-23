# Comparing `tmp/osc_sdk_python-0.28.0.tar.gz` & `tmp/osc_sdk_python-0.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osc_sdk_python-0.28.0.tar", last modified: Fri Mar 15 10:11:42 2024, max compression
+gzip compressed data, was "osc_sdk_python-0.29.0.tar", last modified: Tue Apr 23 13:40:32 2024, max compression
```

## Comparing `osc_sdk_python-0.28.0.tar` & `osc_sdk_python-0.29.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:11:42.169593 osc_sdk_python-0.28.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-03-15 10:11:42.169593 osc_sdk_python-0.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:11:42.165593 osc_sdk_python-0.28.0/osc_sdk_python/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/osc_sdk_python/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/osc_sdk_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/osc_sdk_python/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/osc_sdk_python/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/osc_sdk_python/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:11:42.165593 osc_sdk_python-0.28.0/osc_sdk_python/osc-api/
--rw-r--r--   0 runner    (1001) docker     (127)   840450 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/osc_sdk_python/osc-api/outscale.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/osc_sdk_python/outscale_gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/osc_sdk_python/requester.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:11:42.165593 osc_sdk_python-0.28.0/osc_sdk_python/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    24496 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/osc_sdk_python/resources/gateway_errors.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:11:42.165593 osc_sdk_python-0.28.0/osc_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-03-15 10:11:42.000000 osc_sdk_python-0.28.0/osc_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-15 10:11:42.000000 osc_sdk_python-0.28.0/osc_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 10:11:42.000000 osc_sdk_python-0.28.0/osc_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 10:11:42.000000 osc_sdk_python-0.28.0/osc_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-15 10:11:42.000000 osc_sdk_python-0.28.0/osc_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 10:11:42.169593 osc_sdk_python-0.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 10:11:42.165593 osc_sdk_python-0.28.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/tests/test_manual_aksk.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/tests/test_net.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/tests/test_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/tests/test_vm.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-15 10:11:25.000000 osc_sdk_python-0.28.0/tests/test_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:40:32.261904 osc_sdk_python-0.29.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-23 13:40:32.261904 osc_sdk_python-0.29.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:40:32.261904 osc_sdk_python-0.29.0/osc_sdk_python/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/osc_sdk_python/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/osc_sdk_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/osc_sdk_python/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/osc_sdk_python/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/osc_sdk_python/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:40:32.261904 osc_sdk_python-0.29.0/osc_sdk_python/osc-api/
+-rw-r--r--   0 runner    (1001) docker     (127)   891959 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/osc_sdk_python/osc-api/outscale.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/osc_sdk_python/outscale_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/osc_sdk_python/requester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:40:32.261904 osc_sdk_python-0.29.0/osc_sdk_python/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    24496 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/osc_sdk_python/resources/gateway_errors.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:40:32.261904 osc_sdk_python-0.29.0/osc_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-23 13:40:32.000000 osc_sdk_python-0.29.0/osc_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-23 13:40:32.000000 osc_sdk_python-0.29.0/osc_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:40:32.000000 osc_sdk_python-0.29.0/osc_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:40:32.000000 osc_sdk_python-0.29.0/osc_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 13:40:32.000000 osc_sdk_python-0.29.0/osc_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:40:32.261904 osc_sdk_python-0.29.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:40:32.261904 osc_sdk_python-0.29.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/tests/test_manual_aksk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/tests/test_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/tests/test_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/tests/test_vm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-23 13:40:16.000000 osc_sdk_python-0.29.0/tests/test_volume.py
```

### Comparing `osc_sdk_python-0.28.0/LICENSE` & `osc_sdk_python-0.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/PKG-INFO` & `osc_sdk_python-0.29.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc_sdk_python
-Version: 0.28.0
+Version: 0.29.0
 Summary: Outscale Gateway python SDK
 Home-page: https://github.com/outscale/osc_sdk_python
 Author: Outscal SAS
 Author-email: opensource@outscale.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 
 ```bash
 $ make package
 ```
 
 You can then install it with:
 ```bash
-$ pip install dist/osc_sdk_python-0.28.0-py3-none-any.whl
+$ pip install dist/osc_sdk_python-0.29.0-py3-none-any.whl
 ```
 
 # Configuration & Credentials
 
 When you use the cli you can choose a profile. Profiles can be set with environment variables or in a file.
 It checks environment variables before loading the file.
```

### Comparing `osc_sdk_python-0.28.0/README.md` & `osc_sdk_python-0.29.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 ```bash
 $ make package
 ```
 
 You can then install it with:
 ```bash
-$ pip install dist/osc_sdk_python-0.28.0-py3-none-any.whl
+$ pip install dist/osc_sdk_python-0.29.0-py3-none-any.whl
 ```
 
 # Configuration & Credentials
 
 When you use the cli you can choose a profile. Profiles can be set with environment variables or in a file.
 It checks environment variables before loading the file.
```

### Comparing `osc_sdk_python-0.28.0/osc_sdk_python/__init__.py` & `osc_sdk_python-0.29.0/osc_sdk_python/__init__.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/osc_sdk_python/authentication.py` & `osc_sdk_python-0.29.0/osc_sdk_python/authentication.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/osc_sdk_python/call.py` & `osc_sdk_python-0.29.0/osc_sdk_python/call.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/osc_sdk_python/credentials.py` & `osc_sdk_python-0.29.0/osc_sdk_python/credentials.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/osc_sdk_python/osc-api/outscale.yaml` & `osc_sdk_python-0.29.0/osc_sdk_python/osc-api/outscale.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,45 @@
         VatNumber:
           description: The value added tax (VAT) number for the account.
           type: string
         ZipCode:
           description: The ZIP code of the city.
           type: string
       type: object
+    AddUserToUserGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        UserGroupName:
+          description: The name of the group you want to add a user to.
+          type: string
+        UserGroupPath:
+          description: The path to the group. If not specified, it is set to a slash
+            (`/`).
+          type: string
+        UserName:
+          description: The name of the user you want to add to the group.
+          type: string
+        UserPath:
+          description: The path to the user. If not specified, it is set to a slash
+            (`/`).
+          type: string
+      required:
+      - UserGroupName
+      - UserName
+      type: object
+    AddUserToUserGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+      type: object
     ApiAccessPolicy:
       additionalProperties: false
       description: Information about the API access policy.
       properties:
         MaxAccessKeyExpirationSeconds:
           description: The maximum possible lifetime for your access keys, in seconds.
             If `0`, your access keys can have unlimited lifetimes.
@@ -183,15 +214,15 @@
           type: boolean
       type: object
     ApiAccessRule:
       additionalProperties: false
       description: Information about the API access rule.
       properties:
         ApiAccessRuleId:
-          description: " The ID of the API access rule."
+          description: The ID of the API access rule.
           type: string
         CaIds:
           description: One or more IDs of Client Certificate Authorities (CAs) used
             for the API access rule.
           items:
             type: string
           type: array
@@ -220,30 +251,30 @@
         PolicyName:
           description: The mnemonic name for the policy being created. The name must
             be unique within a set of policies for this load balancer.
           type: string
       type: object
     BackendVmHealth:
       additionalProperties: false
-      description: Information about the health of a back-end VM.
+      description: Information about the health of a backend VM.
       properties:
         Description:
-          description: The description of the state of the back-end VM.
+          description: The description of the state of the backend VM.
           type: string
         State:
-          description: The state of the back-end VM (`InService` \| `OutOfService`
+          description: The state of the backend VM (`InService` \| `OutOfService`
             \| `Unknown`).
           type: string
         StateReason:
           description: |-
             Information about the cause of `OutOfService` VMs.<br />
             Specifically, whether the cause is Elastic Load Balancing or the VM (`ELB` \| `Instance` \| `N/A`).
           type: string
         VmId:
-          description: The ID of the back-end VM.
+          description: The ID of the backend VM.
           type: string
       type: object
     BlockDeviceMappingCreated:
       additionalProperties: false
       description: Information about the created block device mapping.
       properties:
         Bsu:
@@ -314,16 +345,16 @@
       description: Information about the created BSU volume.
       properties:
         DeleteOnVmDeletion:
           description: If true, the volume is deleted when terminating the VM. If
             false, the volume is not deleted when terminating the VM.
           type: boolean
         LinkDate:
-          description: The date and time of attachment of the volume to the VM, in
-            ISO 8601 date-time format.
+          description: The date and time (UTC) of attachment of the volume to the
+            VM, in ISO 8601 date-time format.
           format: date
           type: string
         State:
           description: The state of the volume.
           type: string
         VolumeId:
           description: The ID of the volume.
@@ -435,25 +466,25 @@
       properties:
         Entries:
           description: One or more catalog entries.
           items:
             "$ref": "#/components/schemas/CatalogEntry"
           type: array
         FromDate:
-          description: The beginning of the time period, in ISO 8601 date-time format.
+          description: The beginning of the time period (UTC).
           format: date-time
           type: string
         State:
           description: The state of the catalog (`CURRENT` \| `OBSOLETE`).
           enum:
           - CURRENT
           - OBSOLETE
           type: string
         ToDate:
-          description: The end of the time period, in ISO 8601 date-time format.
+          description: The end of the time period (UTC).
           format: date-time
           type: string
       type: object
     CheckAuthenticationRequest:
       additionalProperties: false
       properties:
         DryRun:
@@ -513,15 +544,15 @@
         AccountId:
           description: The ID of your TINA account.
           type: string
         Category:
           description: The category of the resource (for example, `network`).
           type: string
         FromDate:
-          description: The beginning of the time period, in ISO 8601 date-time format.
+          description: The beginning of the time period (UTC).
           format: datetime
           type: string
         Operation:
           description: The API call that triggered the resource consumption (for example,
             `RunInstances` or `CreateVolume`).
           type: string
         PayingAccountId:
@@ -540,15 +571,15 @@
         SubregionName:
           description: The name of the Subregion.
           type: string
         Title:
           description: A description of the consumed resource.
           type: string
         ToDate:
-          description: The end of the time period, in ISO 8601 date-time format.
+          description: The end of the time period (UTC).
           format: datetime
           type: string
         Type:
           description: The type of resource, depending on the API call.
           type: string
         UnitPrice:
           description: The unit price of the consumed resource, in the currency of
@@ -663,15 +694,15 @@
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     CreateApiAccessRuleRequest:
       additionalProperties: false
       properties:
         CaIds:
-          description: " One or more IDs of Client Certificate Authorities (CAs)."
+          description: One or more IDs of Client Certificate Authorities (CAs).
           items:
             type: string
           type: array
         Cns:
           description: One or more Client Certificate Common Names (CNs). If this
             parameter is specified, you must also specify the `CaIds` parameter.
           items:
@@ -681,15 +712,15 @@
           description: A description for the API access rule.
           type: string
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         IpRanges:
-          description: One or more IP addresses or CIDR blocks (for example, `192.0.2.0/16`).
+          description: One or more IPs or CIDR blocks (for example, `192.0.2.0/16`).
           items:
             type: string
           type: array
       type: object
     CreateApiAccessRuleResponse:
       additionalProperties: false
       properties:
@@ -1239,14 +1270,17 @@
       properties:
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     CreateNatServiceRequest:
       additionalProperties: false
       properties:
+        ClientToken:
+          description: A unique identifier which enables you to manage the idempotency.
+          type: string
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         PublicIpId:
           description: |-
             The allocation ID of the public IP to associate with the NAT service.<br />
@@ -1425,14 +1459,15 @@
         Document:
           description: The policy document, corresponding to a JSON string that contains
             the policy. For more information, see [EIM Reference Information](https://docs.outscale.com/en/userguide/EIM-Reference-Information.html).
           type: string
         PolicyOrn:
           description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
             see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          pattern: "^orn:ows:(iam|idauth):\\S*:\\d{12}:policy/\\S+$"
           type: string
         SetAsDefault:
           description: If set to true, the new policy version is set as the default
             version and becomes the operative one.
           type: boolean
       required:
       - Document
@@ -1648,21 +1683,21 @@
           "$ref": "#/components/schemas/SecurityGroup"
       type: object
     CreateServerCertificateRequest:
       additionalProperties: false
       properties:
         Body:
           description: 'The PEM-encoded X509 certificate.<br />With OSC CLI, use the
-            following syntax to make sure your CA file is correctly parsed: `--CaPem=&quot;$(cat
-            FILENAME)&quot;`.'
+            following syntax to make sure your certificate file is correctly parsed:
+            `--Body=&quot;$(cat FILENAME)&quot;`.'
           type: string
         Chain:
           description: 'The PEM-encoded intermediate certification authorities.<br
-            />With OSC CLI, use the following syntax to make sure your CA file is
-            correctly parsed: `--CaPem=&quot;$(cat FILENAME)&quot;`.'
+            />With OSC CLI, use the following syntax to make sure your certificate
+            chain file is correctly parsed: `--Chain=&quot;$(cat FILENAME)&quot;`.'
           type: string
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Name:
           description: 'A unique name for the certificate. Constraints: 1-128 alphanumeric
@@ -1671,16 +1706,16 @@
           type: string
         Path:
           description: The path to the server certificate, set to a slash (/) if not
             specified.
           type: string
         PrivateKey:
           description: 'The PEM-encoded private key matching the certificate.<br />With
-            OSC CLI, use the following syntax to make sure your CA file is correctly
-            parsed: `--CaPem=&quot;$(cat FILENAME)&quot;`.'
+            OSC CLI, use the following syntax to make sure your key file is correctly
+            parsed: `--PrivateKey=&quot;$(cat FILENAME)&quot;`.'
           type: string
       required:
       - Body
       - PrivateKey
       - Name
       type: object
     CreateServerCertificateResponse:
@@ -1812,31 +1847,56 @@
       type: object
     CreateTagsResponse:
       additionalProperties: false
       properties:
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
+    CreateUserGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        Path:
+          description: The path to the group. If not specified, it is set to a slash
+            (`/`).
+          type: string
+        UserGroupName:
+          description: The name of the group.
+          type: string
+      required:
+      - UserGroupName
+      type: object
+    CreateUserGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+        UserGroup:
+          "$ref": "#/components/schemas/UserGroup"
+      type: object
     CreateUserRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Path:
           description: The path to the EIM user you want to create (by default, `/`).
-            This path name must begin and end with a slash (/), and contain between
-            1 and 512 alphanumeric characters and/or slashes (/), or underscores (_).
+            This path name must begin and end with a slash (`/`), and contain between
+            1 and 512 alphanumeric characters and/or slashes (`/`), or underscores
+            (_).
           type: string
         UserName:
-          description: The name of the EIM user you want to create. This user name
-            must contain between 1 and 64 alphanumeric characters and/or pluses (+),
-            equals (=), commas (,), periods (.), at signs (@), dashes (-), or underscores
-            (_).
+          description: The name of the EIM user. This user name must contain between
+            1 and 64 alphanumeric characters and/or pluses (+), equals (=), commas
+            (,), periods (.), at signs (@), dashes (-), or underscores (_).
           type: string
       required:
       - UserName
       type: object
     CreateUserResponse:
       additionalProperties: false
       properties:
@@ -1934,15 +1994,15 @@
           description: The number of vCores to use for each VM.
           type: integer
         CpuGeneration:
           description: The processor generation to use for each VM (for example, `v4`).
           type: string
         CpuPerformance:
           default: high
-          description: 'The performance of the VMs (`medium` \| `high` \|  `highest`). '
+          description: The performance of the VMs (`medium` \| `high` \|  `highest`).
           enum:
           - medium
           - high
           - highest
           type: string
         Description:
           description: A description for the VM template.
@@ -2111,17 +2171,17 @@
         Iops:
           description: The number of I/O operations per second (IOPS). This parameter
             must be specified only if you create an `io1` volume. The maximum number
             of IOPS allowed for `io1` volumes is `13000` with a maximum performance
             ratio of 300 IOPS per gibibyte.
           type: integer
         Size:
-          description: 'The size of the volume, in gibibytes (GiB). The maximum allowed
+          description: The size of the volume, in gibibytes (GiB). The maximum allowed
             size for a volume is 14901 GiB. This parameter is required if the volume
-            is not created from a snapshot (`SnapshotId` unspecified). '
+            is not created from a snapshot (`SnapshotId` unspecified).
           type: integer
         SnapshotId:
           description: The ID of the snapshot from which you want to create the volume.
           type: string
         SubregionName:
           description: The Subregion in which you want to create the volume.
           type: string
@@ -2707,14 +2767,15 @@
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         PolicyOrn:
           description: The OUTSCALE Resource Name (ORN) of the policy you want to
             delete. For more information, see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          pattern: "^orn:ows:(iam|idauth):\\S*:\\d{12}:policy/\\S+$"
           type: string
       required:
       - PolicyOrn
       type: object
     DeletePolicyResponse:
       additionalProperties: false
       properties:
@@ -2723,14 +2784,15 @@
       type: object
     DeletePolicyVersionRequest:
       additionalProperties: false
       properties:
         PolicyOrn:
           description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
             see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          pattern: "^orn:ows:(iam|idauth):\\S*:\\d{12}:policy/\\S+$"
           type: string
         VersionId:
           description: The ID of the version of the policy you want to delete.
           type: string
       required:
       - PolicyOrn
       - VersionId
@@ -2963,14 +3025,68 @@
       type: object
     DeleteTagsResponse:
       additionalProperties: false
       properties:
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
+    DeleteUserGroupPolicyRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        PolicyName:
+          description: The name of the policy document you want to delete.
+          type: string
+        UserGroupName:
+          description: The name of the group.
+          type: string
+        UserGroupPath:
+          description: The path to the group. If not specified, it is set to a slash
+            (`/`).
+          type: string
+      required:
+      - UserGroupName
+      - PolicyName
+      type: object
+    DeleteUserGroupPolicyResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+      type: object
+    DeleteUserGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        Force:
+          description: If true, forces the deletion of the user group even if it is
+            not empty.
+          type: boolean
+        Path:
+          description: The path to the group. If not specified, it is set to a slash
+            (`/`).
+          type: string
+        UserGroupName:
+          description: The name of the group you want to delete.
+          type: string
+      required:
+      - UserGroupName
+      type: object
+    DeleteUserGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+      type: object
     DeleteUserRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
@@ -3028,15 +3144,15 @@
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         VmTemplateId:
-          description: 'The ID of the VM template you want to delete. '
+          description: The ID of the VM template you want to delete.
           type: string
       required:
       - VmTemplateId
       type: object
     DeleteVmTemplateResponse:
       additionalProperties: false
       properties:
@@ -3132,15 +3248,15 @@
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     DeregisterVmsInLoadBalancerRequest:
       additionalProperties: false
       properties:
         BackendVmIds:
-          description: One or more IDs of back-end VMs.
+          description: One or more IDs of backend VMs.
           items:
             type: string
           type: array
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
@@ -3320,21 +3436,23 @@
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     Errors:
       additionalProperties: false
       description: Information about the errors.
       properties:
         Code:
-          description: The code of the error.
+          description: The code of the error (for example, `4078`). You can search
+            for this returned code in the [errors page](api-errors.html) to find more
+            details about the error.
           type: string
         Details:
-          description: The details of the error.
+          description: A description providing more details about the error.
           type: string
         Type:
-          description: The type of the error.
+          description: The type of the error (for example, `InvalidParameterValue`).
           type: string
       type: object
     FiltersAccessKeys:
       additionalProperties: false
       description: One or more filters.
       properties:
         AccessKeyIds:
@@ -3369,15 +3487,15 @@
           type: array
         Descriptions:
           description: One or more descriptions of API access rules.
           items:
             type: string
           type: array
         IpRanges:
-          description: One or more IP addresses or CIDR blocks (for example, `192.0.2.0/16`).
+          description: One or more IPs or CIDR blocks (for example, `192.0.2.0/16`).
           items:
             type: string
           type: array
       type: object
     FiltersApiLog:
       additionalProperties: false
       description: One or more filters.
@@ -3882,14 +4000,19 @@
             type: string
           type: array
       type: object
     FiltersNatService:
       additionalProperties: false
       description: One or more filters.
       properties:
+        ClientTokens:
+          description: The idempotency tokens provided when creating the NAT services.
+          items:
+            type: string
+          type: array
         NatServiceIds:
           description: The IDs of the NAT services.
           items:
             type: string
           type: array
         NetIds:
           description: The IDs of the Nets in which the NAT services are.
@@ -4137,14 +4260,19 @@
           type: array
         LinkPublicIpLinkPublicIpIds:
           description: The association IDs returned when the public IPs were associated
             with the NICs.
           items:
             type: string
           type: array
+        LinkPublicIpPublicDnsNames:
+          description: The public DNS names associated with the public IPs.
+          items:
+            type: string
+          type: array
         LinkPublicIpPublicIpIds:
           description: The allocation IDs returned when the public IPs were allocated
             to their accounts.
           items:
             type: string
           type: array
         LinkPublicIpPublicIps:
@@ -4608,15 +4736,16 @@
           type: array
         SnapshotIds:
           description: The IDs of the snapshots.
           items:
             type: string
           type: array
         States:
-          description: The states of the snapshots (`in-queue` \| `completed` \| `error`).
+          description: The states of the snapshots (`in-queue` \| `pending` \| `completed`
+            \| `error` \| `deleting`).
           items:
             type: string
           type: array
         TagKeys:
           description: The keys of the tags associated with the snapshots.
           items:
             type: string
@@ -4751,14 +4880,28 @@
             You can use this filter alongside the `TagKeys` filter. In that case,
             you filter the resources corresponding to each tag, regardless of the
             other filter.
           items:
             type: string
           type: array
       type: object
+    FiltersUserGroup:
+      additionalProperties: false
+      description: One or more filters.
+      properties:
+        PathPrefix:
+          description: The path prefix of the groups. If not specified, it is set
+            to a slash (`/`).
+          type: string
+        UserGroupIds:
+          description: The IDs of the user groups.
+          items:
+            type: string
+          type: array
+      type: object
     FiltersVirtualGateway:
       additionalProperties: false
       description: One or more filters.
       properties:
         ConnectionTypes:
           description: The types of the virtual gateways (only `ipsec.1` is supported).
           items:
@@ -4820,17 +4963,15 @@
             `/dev/sdXX`, `/dev/xvdX`, or `/dev/xvdXX`).
           items:
             type: string
           type: array
         BlockDeviceMappingLinkDates:
           description: The link dates for the BSU volumes mapped to the VMs (for example,
             `2016-01-23T18:45:30.000Z`).
-          items:
-            format: date
-            type: string
+          items: string
           type: array
         BlockDeviceMappingStates:
           description: The states for the BSU volumes (`attaching` \| `attached` \|
             `detaching` \| `detached`).
           items:
             type: string
           type: array
@@ -4842,17 +4983,15 @@
         ClientTokens:
           description: The idempotency tokens provided when launching the VMs.
           items:
             type: string
           type: array
         CreationDates:
           description: The dates when the VMs were launched.
-          items:
-            format: date
-            type: string
+          items: string
           type: array
         ImageIds:
           description: The IDs of the OMIs used to launch the VMs.
           items:
             type: string
           type: array
         IsSourceDestChecked:
@@ -4900,18 +5039,17 @@
           type: boolean
         NicLinkNicDeviceNumbers:
           description: The device numbers the NICs are attached to.
           items:
             type: integer
           type: array
         NicLinkNicLinkNicDates:
-          description: The dates and time when the NICs were attached to the VMs.
-          items:
-            format: date
-            type: string
+          description: The dates and times (UTC) when the NICs were attached to the
+            VMs.
+          items: string
           type: array
         NicLinkNicLinkNicIds:
           description: The IDs of the NIC attachments.
           items:
             type: string
           type: array
         NicLinkNicStates:
@@ -5200,15 +5338,14 @@
           description: The IDs of the VM templates.
           items:
             type: string
           type: array
       type: object
     FiltersVmTemplate:
       additionalProperties: false
-      description: One or more filters.
       properties:
         CpuCores:
           description: The number of vCores.
           items:
             type: integer
           type: array
         CpuGenerations:
@@ -5329,21 +5466,21 @@
           type: array
         MaintenanceEventDescriptions:
           description: The description of the scheduled event.
           items:
             type: string
           type: array
         MaintenanceEventsNotAfter:
-          description: The latest time the event can end.
+          description: The latest date and time (UTC) the event can end.
           items:
             format: date
             type: string
           type: array
         MaintenanceEventsNotBefore:
-          description: The earliest time the event can start.
+          description: The earliest date and time (UTC) the event can start.
           items:
             format: date
             type: string
           type: array
         SubregionNames:
           description: The names of the Subregions of the VMs.
           items:
@@ -5617,16 +5754,15 @@
           type: string
         BlockDeviceMappings:
           description: One or more block device mappings.
           items:
             "$ref": "#/components/schemas/BlockDeviceMappingImage"
           type: array
         CreationDate:
-          description: The date and time of creation of the OMI, in ISO 8601 date-time
-            format.
+          description: The date and time (UTC) of creation of the OMI.
           format: date
           type: string
         Description:
           description: The description of the OMI.
           type: string
         FileLocation:
           description: The location from which the OMI files were created.
@@ -5688,14 +5824,26 @@
           items:
             "$ref": "#/components/schemas/ResourceTag"
           type: array
         TaskId:
           description: The ID of the OMI export task.
           type: string
       type: object
+    InlinePolicy:
+      additionalProperties: false
+      description: Information about an inline policy.
+      properties:
+        Body:
+          description: The policy document, corresponding to a JSON string that contains
+            the policy. For more information, see [EIM Reference Information](https://docs.outscale.com/en/userguide/EIM-Reference-Information.html).
+          type: string
+        Name:
+          description: The name of the policy.
+          type: string
+      type: object
     InternetService:
       additionalProperties: false
       description: Information about the Internet service.
       properties:
         InternetServiceId:
           description: The ID of the Internet service.
           type: string
@@ -5796,39 +5944,63 @@
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     LinkLoadBalancerBackendMachinesRequest:
       additionalProperties: false
       properties:
         BackendIps:
-          description: " One or more public IPs of back-end VMs."
+          description: One or more public IPs of backend VMs.
           items:
             type: string
           type: array
         BackendVmIds:
-          description: " One or more IDs of back-end VMs."
+          description: One or more IDs of backend VMs.
           items:
             type: string
           type: array
         DryRun:
-          description: " If true, checks whether you have the required permissions
-            to perform the action."
+          description: If true, checks whether you have the required permissions to
+            perform the action.
           type: boolean
         LoadBalancerName:
-          description: " The name of the load balancer. "
+          description: The name of the load balancer.
           type: string
       required:
       - LoadBalancerName
       type: object
     LinkLoadBalancerBackendMachinesResponse:
       additionalProperties: false
       properties:
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
+    LinkManagedPolicyToUserGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        PolicyOrn:
+          description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
+            see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          type: string
+        UserGroupName:
+          description: The name of the group you want to link the policy to.
+          type: string
+      required:
+      - PolicyOrn
+      - UserGroupName
+      type: object
+    LinkManagedPolicyToUserGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+      type: object
     LinkNic:
       additionalProperties: false
       description: Information about the NIC attachment.
       properties:
         DeleteOnVmDeletion:
           description: If true, the NIC is deleted when the VM is terminated.
           type: boolean
@@ -5919,14 +6091,15 @@
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         PolicyOrn:
           description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
             see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          pattern: "^orn:ows:(iam|idauth):\\S*:\\d{12}:policy/\\S+$"
           type: string
         UserName:
           description: The name of the user you want to link the policy to (between
             1 and 64 characters).
           type: string
       required:
       - PolicyOrn
@@ -6055,27 +6228,30 @@
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     LinkRouteTable:
       additionalProperties: false
       description: One or more associations between the route table and the Subnets.
       properties:
         LinkRouteTableId:
-          description: The ID of the association between the route table and the Subnet.
+          description: The ID of the association between the route table and the Net
+            or Subnet.
           type: string
         Main:
           description: If true, the route table is the main one.
           type: boolean
         NetId:
-          description: The ID of the Net.
+          description: The ID of the Net, if the route table is not explicitly linked
+            to a Subnet.
           type: string
         RouteTableId:
           description: The ID of the route table.
           type: string
         SubnetId:
-          description: The ID of the Subnet.
+          description: The ID of the Subnet, if the route table is explicitly linked
+            to a Subnet.
           type: string
       type: object
     LinkRouteTableRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
@@ -6153,26 +6329,27 @@
       additionalProperties: false
       properties:
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     LinkedPolicy:
       additionalProperties: false
-      description: Information about the attached policy.
+      description: Information about the linked policy.
       properties:
         CreationDate:
-          description: The date and time of creation of the attached policy.
+          description: The date and time (UTC) of creation of the linked policy.
           format: date-time
           type: string
         LastModificationDate:
-          description: The date and time at which the attached policy was last modified.
+          description: The date and time (UTC) at which the linked policy was last
+            modified.
           format: date-time
           type: string
         Orn:
-          description: The Outscale Resource Name (ORN) of the policy. For more information,
+          description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
             see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
           type: string
         PolicyId:
           description: The ID of the policy.
           type: string
         PolicyName:
           description: The name of the policy.
@@ -6201,19 +6378,19 @@
           type: string
       type: object
     Listener:
       additionalProperties: false
       description: Information about the listener.
       properties:
         BackendPort:
-          description: The port on which the back-end VM is listening (between `1`
+          description: The port on which the backend VM is listening (between `1`
             and `65535`, both included).
           type: integer
         BackendProtocol:
-          description: The protocol for routing traffic to back-end VMs (`HTTP` \|
+          description: The protocol for routing traffic to backend VMs (`HTTP` \|
             `HTTPS` \| `TCP` \| `SSL`).
           type: string
         LoadBalancerPort:
           description: The port on which the load balancer is listening (between `1`
             and `65535`, both included).
           type: integer
         LoadBalancerProtocol:
@@ -6232,19 +6409,19 @@
           type: string
       type: object
     ListenerForCreation:
       additionalProperties: false
       description: Information about the listener to create.
       properties:
         BackendPort:
-          description: The port on which the back-end VM is listening (between `1`
+          description: The port on which the backend VM is listening (between `1`
             and `65535`, both included).
           type: integer
         BackendProtocol:
-          description: The protocol for routing traffic to back-end VMs (`HTTP` \|
+          description: The protocol for routing traffic to backend VMs (`HTTP` \|
             `HTTPS` \| `TCP` \| `SSL`).
           type: string
         LoadBalancerPort:
           description: The port on which the load balancer is listening (between `1`
             and `65535`, both included).
           type: integer
         LoadBalancerProtocol:
@@ -6301,17 +6478,17 @@
       additionalProperties: false
       description: Information about the listener rule.
       properties:
         Action:
           description: The type of action for the rule (always `forward`).
           type: string
         HostNamePattern:
-          description: 'A host-name pattern for the rule, with a maximum length of
+          description: A host-name pattern for the rule, with a maximum length of
             128 characters. This host-name pattern supports maximum three wildcards,
-            and must not contain any special characters except [-.?]. '
+            and must not contain any special characters except [-.?].
           type: string
         ListenerRuleName:
           description: A human-readable name for the listener rule.
           type: string
         PathPattern:
           description: A path pattern for the rule, with a maximum length of 128 characters.
             This path pattern supports maximum three wildcards, and must not contain
@@ -6334,20 +6511,20 @@
           "$ref": "#/components/schemas/AccessLog"
         ApplicationStickyCookiePolicies:
           description: The stickiness policies defined for the load balancer.
           items:
             "$ref": "#/components/schemas/ApplicationStickyCookiePolicy"
           type: array
         BackendIps:
-          description: One or more public IPs of back-end VMs.
+          description: One or more public IPs of backend VMs.
           items:
             type: string
           type: array
         BackendVmIds:
-          description: One or more IDs of back-end VMs for the load balancer.
+          description: One or more IDs of backend VMs for the load balancer.
           items:
             type: string
           type: array
         DnsName:
           description: The DNS name of the load balancer.
           type: string
         HealthCheck:
@@ -6480,16 +6657,15 @@
         QueryApiVersion:
           description: The version of the API used by the logged call.
           type: string
         QueryCallName:
           description: The name of the logged call.
           type: string
         QueryDate:
-          description: The date and time of the logged call, in ISO 8601 date-time
-            format.
+          description: The date and time (UTC) of the logged call.
           format: date
           type: string
         QueryHeaderRaw:
           description: The raw header of the HTTP request of the logged call.
           type: string
         QueryHeaderSize:
           description: The size of the raw header of the HTTP request of the logged
@@ -6525,26 +6701,29 @@
         Code:
           description: The code of the event (`system-reboot` \| `system-maintenance`).
           type: string
         Description:
           description: The description of the event.
           type: string
         NotAfter:
-          description: The latest scheduled end time for the event.
+          description: The latest scheduled end date and time (UTC) for the event.
           format: date
           type: string
         NotBefore:
-          description: The earliest scheduled start time for the event.
+          description: The earliest scheduled start date and time (UTC) for the event.
           format: date
           type: string
       type: object
     NatService:
       additionalProperties: false
       description: Information about the NAT service.
       properties:
+        ClientToken:
+          description: The idempotency token provided when creating the NAT service.
+          type: string
         NatServiceId:
           description: The ID of the NAT service.
           type: string
         NetId:
           description: The ID of the Net in which the NAT service is.
           type: string
         PublicIps:
@@ -6624,15 +6803,15 @@
     NetPeering:
       additionalProperties: false
       description: Information about the Net peering.
       properties:
         AccepterNet:
           "$ref": "#/components/schemas/AccepterNet"
         ExpirationDate:
-          description: The date and time at which the Net peerings expire.
+          description: The date and time (UTC) at which the Net peerings expire.
           format: date-time
           nullable: true
           type: string
         NetPeeringId:
           description: The ID of the Net peering.
           type: string
         SourceNet:
@@ -6921,16 +7100,16 @@
         Additions:
           "$ref": "#/components/schemas/PermissionsOnResource"
         Removals:
           "$ref": "#/components/schemas/PermissionsOnResource"
       type: object
     Phase1Options:
       additionalProperties: false
-      description: 'Information about Phase 1 of the Internet Key Exchange (IKE) negotiation.
-        When Phase 1 finishes successfully, peers proceed to Phase 2 negotiations. '
+      description: Information about Phase 1 of the Internet Key Exchange (IKE) negotiation.
+        When Phase 1 finishes successfully, peers proceed to Phase 2 negotiations.
       properties:
         DpdTimeoutAction:
           description: The action to carry out after a Dead Peer Detection (DPD) timeout
             occurs.
           type: string
         DpdTimeoutSeconds:
           description: The maximum waiting time for a Dead Peer Detection (DPD) response
@@ -6970,15 +7149,15 @@
         StartupAction:
           description: The action to carry out when establishing tunnels for a VPN
             connection.
           type: string
       type: object
     Phase2Options:
       additionalProperties: false
-      description: 'Information about Phase 2 of the Internet Key Exchange (IKE) negotiation. '
+      description: Information about Phase 2 of the Internet Key Exchange (IKE) negotiation.
       properties:
         Phase2DhGroupNumbers:
           description: The Diffie-Hellman (DH) group numbers allowed for the VPN tunnel
             for phase 2.
           items:
             type: integer
           type: array
@@ -7000,24 +7179,14 @@
           type: integer
         PreSharedKey:
           description: The pre-shared key to establish the initial authentication
             between the client gateway and the virtual gateway. This key can contain
             any character except line breaks and double quotes (&quot;).
           type: string
       type: object
-    Phase2OptionsToUpdate:
-      additionalProperties: false
-      description: 'Information about Phase 2 of the Internet Key Exchange (IKE) negotiation. '
-      properties:
-        PreSharedKey:
-          description: The pre-shared key to establish the initial authentication
-            between the client gateway and the virtual gateway. This key can contain
-            any character except line breaks and double quotes (&quot;).
-          type: string
-      type: object
     Placement:
       additionalProperties: false
       description: Information about the placement of the VM.
       properties:
         SubregionName:
           description: The name of the Subregion. If you specify this parameter, you
             must not specify the `Nics` parameter.
@@ -7028,26 +7197,26 @@
           type: string
       type: object
     Policy:
       additionalProperties: false
       description: Information about the policy.
       properties:
         CreationDate:
-          description: The date and time of creation of the policy.
+          description: The date and time (UTC) of creation of the policy.
           format: date-time
           type: string
         Description:
           description: A friendly name for the policy (between 0 and 1000 characters).
           type: string
         IsLinkable:
           description: Indicates whether the policy can be linked to a group or an
             EIM user.
           type: boolean
         LastModificationDate:
-          description: The date and time at which the policy was last modified.
+          description: The date and time (UTC) at which the policy was last modified.
           format: date-time
           type: string
         Orn:
           description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
             see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
           type: string
         Path:
@@ -7067,18 +7236,19 @@
           type: integer
       type: object
     PolicyVersion:
       additionalProperties: false
       description: Information about the policy version.
       properties:
         Body:
-          description: The policy document as a json string.
+          description: The policy document, corresponding to a JSON string that contains
+            the policy. For more information, see [EIM Reference Information](https://docs.outscale.com/en/userguide/EIM-Reference-Information.html).
           type: string
         CreationDate:
-          description: The date and time of creation of the version.
+          description: The date and time (UTC) of creation of the version.
           format: date-time
           type: string
         DefaultVersion:
           description: If true, the version is the default one.
           type: boolean
         VersionId:
           description: The ID of the version.
@@ -7181,14 +7351,46 @@
           description: The public IP associated with the NAT service.
           type: string
         PublicIpId:
           description: The allocation ID of the public IP associated with the NAT
             service.
           type: string
       type: object
+    PutUserGroupPolicyRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        PolicyDocument:
+          description: The policy document, corresponding to a JSON string that contains
+            the policy. For more information, see [EIM Reference Information](https://docs.outscale.com/en/userguide/EIM-Reference-Information.html).
+          type: string
+        PolicyName:
+          description: The name of the policy.
+          type: string
+        UserGroupName:
+          description: The name of the group.
+          type: string
+        UserGroupPath:
+          description: The path to the group. If not specified, it is set to a slash
+            (`/`).
+          type: string
+      required:
+      - PolicyName
+      - PolicyDocument
+      - UserGroupName
+      type: object
+    PutUserGroupPolicyResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+      type: object
     Quota:
       additionalProperties: false
       description: Information about the quota.
       properties:
         AccountId:
           description: The account ID of the owner of the quotas.
           type: string
@@ -7404,26 +7606,24 @@
         Catalog:
           "$ref": "#/components/schemas/Catalog"
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadCatalogsRequest:
       additionalProperties: false
-      description: ReadCatalogsRequest
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersCatalogs"
       type: object
     ReadCatalogsResponse:
       additionalProperties: false
-      description: ReadCatalogsResponse
       properties:
         Catalogs:
           description: Information about one or more catalogs.
           items:
             "$ref": "#/components/schemas/Catalogs"
           type: array
         ResponseContext:
@@ -7434,23 +7634,37 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersClientGateway"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadClientGatewaysResponse:
       additionalProperties: false
       properties:
         ClientGateways:
           description: Information about one or more client gateways.
           items:
             "$ref": "#/components/schemas/ClientGateway"
           type: array
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadConsoleOutputRequest:
       additionalProperties: false
       properties:
         DryRun:
@@ -7483,33 +7697,36 @@
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         FromDate:
           description: The beginning of the time period, in ISO 8601 date format (for
             example, `2020-06-14`). The date-time format is also accepted, but only
             with a time set to midnight (for example, `2020-06-14T00:00:00.000Z`).
+            This value is included in the time period.
           format: datetime
           type: string
         Overall:
           default: false
           description: By default or if false, returns only the consumption of the
             specific account that sends this request. If true, returns either the
             overall consumption of your paying account and all linked accounts (if
             the account that sends this request is a paying account) or returns nothing
             (if the account that sends this request is a linked account).
           type: boolean
         ShowPrice:
           description: If true, the response also includes the unit price of the consumed
             resource (`UnitPrice`) and the total price of the consumed resource during
-            the specified time period (`Price`), in the currency of the Region's catalog.
+            the specified time period (`Price`), in the currency of your account.
           type: boolean
         ToDate:
           description: The end of the time period, in ISO 8601 date format (for example,
             `2020-06-30`). The date-time format is also accepted, but only with a
-            time set to midnight (for example, `2020-06-30T00:00:00.000Z`).
+            time set to midnight (for example, `2020-06-30T00:00:00.000Z`). This value
+            is excluded from the time period, and must be set to a later date than
+            `FromDate`.
           format: datetime
           type: string
       required:
       - FromDate
       - ToDate
       type: object
     ReadConsumptionAccountResponse:
@@ -7517,35 +7734,54 @@
       properties:
         ConsumptionEntries:
           description: Information about the resources consumed during the specified
             time period.
           items:
             "$ref": "#/components/schemas/ConsumptionEntry"
           type: array
+        Currency:
+          description: The currency of your account for the `UnitPrice` and `Price`
+            parameters, in the ISO-4217 format (for example, `EUR`).
+          nullable: true
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadDedicatedGroupsRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersDedicatedGroup"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadDedicatedGroupsResponse:
       additionalProperties: false
       properties:
         DedicatedGroups:
           description: Information about one or more dedicated groups.
           items:
             "$ref": "#/components/schemas/DedicatedGroup"
           type: array
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadDhcpOptionsRequest:
       additionalProperties: false
       properties:
         DryRun:
@@ -7585,44 +7821,72 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersDirectLinkInterface"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadDirectLinkInterfacesResponse:
       additionalProperties: false
       properties:
         DirectLinkInterfaces:
           description: Information about one or more DirectLink interfaces.
           items:
             "$ref": "#/components/schemas/DirectLinkInterfaces"
           type: array
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadDirectLinksRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersDirectLink"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadDirectLinksResponse:
       additionalProperties: false
       properties:
         DirectLinks:
           description: Information about one or more DirectLinks.
           items:
             "$ref": "#/components/schemas/DirectLink"
           type: array
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadFlexibleGpuCatalogRequest:
       additionalProperties: false
       properties:
         DryRun:
@@ -7668,23 +7932,37 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersExportTask"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadImageExportTasksResponse:
       additionalProperties: false
       properties:
         ImageExportTasks:
           description: Information about one or more image export tasks.
           items:
             "$ref": "#/components/schemas/ImageExportTask"
           type: array
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadImagesRequest:
       additionalProperties: false
       properties:
         DryRun:
@@ -7724,52 +8002,82 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersInternetService"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadInternetServicesResponse:
       additionalProperties: false
       properties:
         InternetServices:
           description: Information about one or more Internet services.
           items:
             "$ref": "#/components/schemas/InternetService"
           type: array
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadKeypairsRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersKeypair"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadKeypairsResponse:
       additionalProperties: false
       properties:
         Keypairs:
           description: Information about one or more keypairs.
           items:
             "$ref": "#/components/schemas/Keypair"
           type: array
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
+      type: object
     ReadLinkedPoliciesFilters:
       additionalProperties: false
       description: One or more filters.
       properties:
         PathPrefix:
-          description: The path prefix of the policies, set to a slash (`/`) by default.
+          description: The path prefix of the policies. If not specified, it is set
+            to a slash (`/`).
           type: string
       type: object
     ReadLinkedPoliciesRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
@@ -7778,19 +8086,21 @@
         Filters:
           "$ref": "#/components/schemas/ReadLinkedPoliciesFilters"
         FirstItem:
           description: The item starting the list of policies requested.
           type: integer
         ResultsPerPage:
           description: The maximum number of items that can be returned in a single
-            response (by default, 100).
+            response (by default, `100`).
           type: integer
         UserName:
           description: The name of the user the policies are linked to.
           type: string
+      required:
+      - UserName
       type: object
     ReadLinkedPoliciesResponse:
       additionalProperties: false
       properties:
         HasMoreItems:
           description: If true, there are more items to return using the `FirstItem`
             parameter in a new request.
@@ -7881,23 +8191,81 @@
     ReadLocationsRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadLocationsResponse:
       additionalProperties: false
       properties:
         Locations:
           description: Information about one or more locations.
           items:
             "$ref": "#/components/schemas/Location"
           type: array
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+      type: object
+    ReadManagedPoliciesLinkedToUserGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        Filters:
+          "$ref": "#/components/schemas/FiltersUserGroup"
+        FirstItem:
+          description: The item starting the list of policies requested.
+          type: integer
+        ResultsPerPage:
+          description: The maximum number of items that can be returned in a single
+            response (by default, `100`).
+          type: integer
+        UserGroupName:
+          description: The name of the group.
+          type: string
+      required:
+      - UserGroupName
+      type: object
+    ReadManagedPoliciesLinkedToUserGroupResponse:
+      additionalProperties: false
+      properties:
+        HasMoreItems:
+          description: If true, there are more items to return using the `FirstItem`
+            parameter in a new request.
+          type: boolean
+        MaxResultsLimit:
+          description: Indicates maximum results defined for the operation.
+          type: integer
+        MaxResultsTruncated:
+          description: If true, indicates whether requested page size is more than
+            allowed.
+          type: boolean
+        Policies:
+          description: A list of policies.
+          items:
+            "$ref": "#/components/schemas/LinkedPolicy"
+          type: array
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadNatServicesRequest:
       additionalProperties: false
       properties:
         DryRun:
@@ -7937,18 +8305,32 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersService"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadNetAccessPointServicesResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         Services:
           description: The names of the services you can use for Net access points.
           items:
             "$ref": "#/components/schemas/Service"
           type: array
@@ -8028,23 +8410,37 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersNet"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadNetsResponse:
       additionalProperties: false
       properties:
         Nets:
           description: Information about the described Nets.
           items:
             "$ref": "#/components/schemas/Net"
           type: array
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadNicsRequest:
       additionalProperties: false
       properties:
         DryRun:
@@ -8069,16 +8465,16 @@
       additionalProperties: false
       description: One or more filters.
       properties:
         OnlyLinked:
           description: If set to true, lists only the policies attached to a user.
           type: boolean
         PathPrefix:
-          description: The path prefix you can use to filter the results, set to a
-            slash (`/`) by default.
+          description: The path prefix you can use to filter the results. If not specified,
+            it is set to a slash (`/`).
           type: string
         Scope:
           description: The scope to filter policies (`OWS` \| `LOCAL`).
           enum:
           - LOCAL
           - OWS
           type: string
@@ -8093,15 +8489,15 @@
         Filters:
           "$ref": "#/components/schemas/ReadPoliciesFilters"
         FirstItem:
           description: The item starting the list of policies requested.
           type: integer
         ResultsPerPage:
           description: The maximum number of items that can be returned in a single
-            response (by default, 100).
+            response (by default, `100`).
           type: integer
       type: object
     ReadPoliciesResponse:
       additionalProperties: false
       properties:
         HasMoreItems:
           description: If true, there are more items to return using the `FirstItem`
@@ -8124,14 +8520,15 @@
       type: object
     ReadPolicyRequest:
       additionalProperties: false
       properties:
         PolicyOrn:
           description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
             see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          pattern: "^orn:ows:(iam|idauth):\\S*:\\d{12}:policy/\\S+$"
           type: string
       required:
       - PolicyOrn
       type: object
     ReadPolicyResponse:
       additionalProperties: false
       properties:
@@ -8142,14 +8539,15 @@
       type: object
     ReadPolicyVersionRequest:
       additionalProperties: false
       properties:
         PolicyOrn:
           description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
             see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          pattern: "^orn:ows:(iam|idauth):\\S*:\\d{12}:policy/\\S+$"
           type: string
         VersionId:
           description: The ID of the policy version.
           type: string
       required:
       - PolicyOrn
       - VersionId
@@ -8167,18 +8565,19 @@
       properties:
         FirstItem:
           description: The item starting the list of policies requested.
           type: integer
         PolicyOrn:
           description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
             see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          pattern: "^orn:ows:(iam|idauth):\\S*:\\d{12}:policy/\\S+$"
           type: string
         ResultsPerPage:
           description: The maximum number of items that can be returned in a single
-            response (by default, 100).
+            response (by default, `100`).
           type: integer
       required:
       - PolicyOrn
       type: object
     ReadPolicyVersionsResponse:
       additionalProperties: false
       properties:
@@ -8202,18 +8601,32 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersProductType"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadProductTypesResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ProductTypes:
           description: Information about one or more product types.
           items:
             "$ref": "#/components/schemas/ProductType"
           type: array
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
@@ -8237,18 +8650,32 @@
     ReadPublicIpRangesRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadPublicIpRangesResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         PublicIps:
           description: The list of public IPv4 addresses used in the Region, in CIDR
             notation.
           items:
             type: string
           type: array
         ResponseContext:
@@ -8294,18 +8721,32 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersQuota"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadQuotasResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         QuotaTypes:
           description: Information about one or more quotas.
           items:
             "$ref": "#/components/schemas/QuotaTypes"
           type: array
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
@@ -8390,18 +8831,32 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersSecurityGroup"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadSecurityGroupsResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         SecurityGroups:
           description: Information about one or more security groups.
           items:
             "$ref": "#/components/schemas/SecurityGroup"
           type: array
@@ -8432,18 +8887,32 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersExportTask"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadSnapshotExportTasksResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         SnapshotExportTasks:
           description: Information about one or more snapshot export tasks.
           items:
             "$ref": "#/components/schemas/SnapshotExportTask"
           type: array
@@ -8453,18 +8922,32 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersSnapshot"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadSnapshotsResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         Snapshots:
           description: Information about one or more snapshots and their permissions.
           items:
             "$ref": "#/components/schemas/Snapshot"
           type: array
@@ -8474,18 +8957,32 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersSubnet"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadSubnetsResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         Subnets:
           description: Information about one or more Subnets.
           items:
             "$ref": "#/components/schemas/Subnet"
           type: array
@@ -8495,18 +8992,32 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersSubregion"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadSubregionsResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         Subregions:
           description: Information about one or more Subregions.
           items:
             "$ref": "#/components/schemas/Subregion"
           type: array
@@ -8516,26 +9027,211 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersTag"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadTagsResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         Tags:
           description: Information about one or more tags.
           items:
             "$ref": "#/components/schemas/Tag"
           type: array
       type: object
+    ReadUserGroupPoliciesRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        FirstItem:
+          description: The item starting the list of policies requested.
+          type: integer
+        ResultsPerPage:
+          description: The maximum number of items that can be returned in a single
+            response (by default, `100`).
+          type: integer
+        UserGroupName:
+          description: The name of the group.
+          type: string
+        UserGroupPath:
+          description: The path to the group. If not specified, it is set to a slash
+            (`/`).
+          type: string
+      required:
+      - UserGroupName
+      type: object
+    ReadUserGroupPoliciesResponse:
+      additionalProperties: false
+      properties:
+        HasMoreItems:
+          description: If true, there are more items to return using the `FirstItem`
+            parameter in a new request.
+          type: boolean
+        MaxResultsLimit:
+          description: Indicates maximum results defined for the operation.
+          type: integer
+        MaxResultsTruncated:
+          description: If true, indicates whether requested page size is more than
+            allowed.
+          type: boolean
+        Policies:
+          description: A list of policies.
+          items:
+            "$ref": "#/components/schemas/InlinePolicy"
+          type: array
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+      type: object
+    ReadUserGroupPolicyRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        PolicyName:
+          description: The name of the policy.
+          type: string
+        UserGroupName:
+          description: The name of the group.
+          type: string
+        UserGroupPath:
+          description: The path to the group. If not specified, it is set to a slash
+            (`/`).
+          type: string
+      required:
+      - PolicyName
+      - UserGroupName
+      type: object
+    ReadUserGroupPolicyResponse:
+      additionalProperties: false
+      properties:
+        Policy:
+          "$ref": "#/components/schemas/InlinePolicy"
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+      type: object
+    ReadUserGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        Path:
+          description: The path to the group. If not specified, it is set to a slash
+            (`/`).
+          type: string
+        UserGroupName:
+          description: The name of the group.
+          type: string
+      required:
+      - UserGroupName
+      type: object
+    ReadUserGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+        UserGroup:
+          "$ref": "#/components/schemas/UserGroup"
+        Users:
+          description: A list of EIM users.
+          items:
+            "$ref": "#/components/schemas/User"
+          type: array
+      type: object
+    ReadUserGroupsPerUserRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        UserName:
+          description: The name of the user.
+          type: string
+        UserPath:
+          description: The path to the user (by default, `/`).
+          type: string
+      required:
+      - UserName
+      type: object
+    ReadUserGroupsPerUserResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+        UserGroups:
+          description: A list of user groups.
+          items:
+            "$ref": "#/components/schemas/UserGroup"
+          type: array
+      type: object
+    ReadUserGroupsRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        Filters:
+          "$ref": "#/components/schemas/FiltersUserGroup"
+        FirstItem:
+          description: The item starting the list of groups requested.
+          type: integer
+        ResultsPerPage:
+          description: The maximum number of items that can be returned in a single
+            response (by default, `100`).
+          type: integer
+      type: object
+    ReadUserGroupsResponse:
+      additionalProperties: false
+      properties:
+        HasMoreItems:
+          description: If true, there are more items to return using the `FirstItem`
+            parameter in a new request.
+          type: boolean
+        MaxResultsLimit:
+          description: Indicates maximum results defined for the operation.
+          type: integer
+        MaxResultsTruncated:
+          description: If true, indicates whether requested page size is more than
+            allowed.
+          type: boolean
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+        UserGroups:
+          description: A list of user groups.
+          items:
+            "$ref": "#/components/schemas/UserGroup"
+          type: array
+      type: object
     ReadUsersRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
@@ -8598,15 +9294,14 @@
       type: object
     ReadVmGroupsResponse:
       additionalProperties: false
       properties:
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         VmGroups:
-          description: Information about one or more VM groups.
           items:
             "$ref": "#/components/schemas/VmGroup"
           type: array
       type: object
     ReadVmTemplatesRequest:
       additionalProperties: false
       properties:
@@ -8633,31 +9328,45 @@
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersVmType"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadVmTypesResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         VmTypes:
           description: Information about one or more VM types.
           items:
             "$ref": "#/components/schemas/VmType"
           type: array
       type: object
     ReadVmsHealthRequest:
       additionalProperties: false
       properties:
         BackendVmIds:
-          description: One or more IDs of back-end VMs.
+          description: One or more IDs of backend VMs.
           items:
             type: string
           type: array
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
@@ -8667,15 +9376,15 @@
       required:
       - LoadBalancerName
       type: object
     ReadVmsHealthResponse:
       additionalProperties: false
       properties:
         BackendVmHealth:
-          description: Information about the health of one or more back-end VMs.
+          description: Information about the health of one or more backend VMs.
           items:
             "$ref": "#/components/schemas/BackendVmHealth"
           type: array
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     ReadVmsRequest:
@@ -8723,18 +9432,32 @@
           type: boolean
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         Filters:
           "$ref": "#/components/schemas/FiltersVmsState"
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
+        ResultsPerPage:
+          description: The maximum number of logs returned in a single response (between
+            `1`and `1000`, both included). By default, `100`.
+          type: integer
       type: object
     ReadVmsStateResponse:
       additionalProperties: false
       properties:
+        NextPageToken:
+          description: The token to request the next page of results. Each token refers
+            to a specific page.
+          format: byte
+          type: string
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         VmStates:
           description: Information about one or more VM states.
           items:
             "$ref": "#/components/schemas/VmStates"
           type: array
@@ -8842,16 +9565,16 @@
           type: string
       type: object
     RegisterVmsInLoadBalancerRequest:
       additionalProperties: false
       properties:
         BackendVmIds:
           description: |-
-            One or more IDs of back-end VMs.<br />
-            Specifying the same ID several times has no effect as each back-end VM has equal weight.
+            One or more IDs of backend VMs.<br />
+            Specifying the same ID several times has no effect as each backend VM has equal weight.
           items:
             type: string
           type: array
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
@@ -8883,14 +9606,44 @@
       type: object
     RejectNetPeeringResponse:
       additionalProperties: false
       properties:
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
+    RemoveUserFromUserGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        UserGroupName:
+          description: The name of the group you want to remove the user from.
+          type: string
+        UserGroupPath:
+          description: The path to the group. If not specified, it is set to a slash
+            (`/`).
+          type: string
+        UserName:
+          description: The name of the user you want to remove from the group.
+          type: string
+        UserPath:
+          description: The path to the user (by default, `/`).
+          type: string
+      required:
+      - UserGroupName
+      - UserName
+      type: object
+    RemoveUserFromUserGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+      type: object
     ResourceLoadBalancerTag:
       additionalProperties: false
       description: Information about the tag.
       properties:
         Key:
           description: The key of the tag, with a minimum of 1 character.
           type: string
@@ -8944,15 +9697,15 @@
         NetPeeringId:
           description: The ID of the Net peering.
           type: string
         NicId:
           description: The ID of the NIC.
           type: string
         State:
-          description: 'The state of a route in the route table (always `active`). '
+          description: The state of a route in the route table (always `active`).
           type: string
         VmAccountId:
           description: The account ID of the owner of the VM.
           type: string
         VmId:
           description: The ID of a VM specified in a route in the table.
           type: string
@@ -9168,16 +9921,16 @@
         Id:
           description: The ID of the server certificate.
           type: string
         Name:
           description: The name of the server certificate.
           type: string
         Orn:
-          description: The Outscale Resource Name (ORN) of the server certificate.
-            For more information, see [Resource Identifiers > Outscale Resource Names
+          description: The OUTSCALE Resource Name (ORN) of the server certificate.
+            For more information, see [Resource Identifiers > OUTSCALE Resource Names
             (ORNs)](https://docs.outscale.com/en/userguide/Resource-Identifiers.html#_outscale_resource_names_orns).
           type: string
         Path:
           description: The path to the server certificate.
           type: string
         UploadDate:
           description: The date at which the server certificate has been uploaded.
@@ -9202,14 +9955,15 @@
       type: object
     SetDefaultPolicyVersionRequest:
       additionalProperties: false
       properties:
         PolicyOrn:
           description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
             see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          pattern: "^orn:ows:(iam|idauth):\\S*:\\d{12}:policy/\\S+$"
           type: string
         VersionId:
           description: The ID of the version.
           type: string
       required:
       - PolicyOrn
       - VersionId
@@ -9227,30 +9981,31 @@
         AccountAlias:
           description: The account alias of the owner of the snapshot.
           type: string
         AccountId:
           description: The account ID of the owner of the snapshot.
           type: string
         CreationDate:
-          description: The date and time of creation of the snapshot.
+          description: The date and time (UTC) of creation of the snapshot.
           format: datetime
           type: string
         Description:
           description: The description of the snapshot.
           type: string
         PermissionsToCreateVolume:
           "$ref": "#/components/schemas/PermissionsOnResource"
         Progress:
           description: The progress of the snapshot, as a percentage.
           type: integer
         SnapshotId:
           description: The ID of the snapshot.
           type: string
         State:
-          description: The state of the snapshot (`in-queue` \| `completed` \| `error`).
+          description: The state of the snapshot (`in-queue` \| `pending` \| `completed`
+            \| `error` \| `deleting`)).
           type: string
         Tags:
           description: One or more tags associated with the snapshot.
           items:
             "$ref": "#/components/schemas/ResourceTag"
           type: array
         VolumeId:
@@ -9493,39 +10248,63 @@
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     UnlinkLoadBalancerBackendMachinesRequest:
       additionalProperties: false
       properties:
         BackendIps:
-          description: " One or more public IPs of back-end VMs."
+          description: One or more public IPs of backend VMs.
           items:
             type: string
           type: array
         BackendVmIds:
-          description: " One or more IDs of back-end VMs."
+          description: One or more IDs of backend VMs.
           items:
             type: string
           type: array
         DryRun:
-          description: " If true, checks whether you have the required permissions
-            to perform the action."
+          description: If true, checks whether you have the required permissions to
+            perform the action.
           type: boolean
         LoadBalancerName:
-          description: " The name of the load balancer."
+          description: The name of the load balancer.
           type: string
       required:
       - LoadBalancerName
       type: object
     UnlinkLoadBalancerBackendMachinesResponse:
       additionalProperties: false
       properties:
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
+    UnlinkManagedPolicyFromUserGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        PolicyOrn:
+          description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
+            see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          type: string
+        UserGroupName:
+          description: The name of the group you want to unlink the policy from.
+          type: string
+      required:
+      - PolicyOrn
+      - UserGroupName
+      type: object
+    UnlinkManagedPolicyFromUserGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+      type: object
     UnlinkNicRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
@@ -9547,14 +10326,15 @@
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         PolicyOrn:
           description: The OUTSCALE Resource Name (ORN) of the policy. For more information,
             see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          pattern: "^orn:ows:(iam|idauth):\\S*:\\d{12}:policy/\\S+$"
           type: string
         UserName:
           description: The name of the user you want to detach the policy from.
           type: string
       required:
       - PolicyOrn
       - UserName
@@ -9834,15 +10614,15 @@
           description: A new description for the API access rule.
           type: string
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         IpRanges:
-          description: One or more IP addresses or CIDR blocks (for example, `192.0.2.0/16`).
+          description: One or more IPs or CIDR blocks (for example, `192.0.2.0/16`).
           items:
             type: string
           type: array
       required:
       - ApiAccessRuleId
       type: object
     UpdateApiAccessRuleResponse:
@@ -9953,26 +10733,28 @@
           "$ref": "#/components/schemas/FlexibleGpu"
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
       type: object
     UpdateImageRequest:
       additionalProperties: false
       properties:
+        Description:
+          description: A new description for the image.
+          type: string
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
         ImageId:
           description: The ID of the OMI you want to modify.
           type: string
         PermissionsToLaunch:
           "$ref": "#/components/schemas/PermissionsOnResourceCreation"
       required:
       - ImageId
-      - PermissionsToLaunch
       type: object
     UpdateImageResponse:
       additionalProperties: false
       properties:
         Image:
           "$ref": "#/components/schemas/Image"
         ResponseContext:
@@ -10051,16 +10833,16 @@
             security groups that you want to keep along with the new ones you are
             assigning. If the list is empty, the default security group of the Net
             is assigned to the load balancer."
           items:
             type: string
           type: array
         ServerCertificateId:
-          description: The Outscale Resource Name (ORN) of the server certificate.
-            For more information, see [Resource Identifiers > Outscale Resource Names
+          description: The OUTSCALE Resource Name (ORN) of the server certificate.
+            For more information, see [Resource Identifiers > OUTSCALE Resource Names
             (ORNs)](https://docs.outscale.com/en/userguide/Resource-Identifiers.html#_outscale_resource_names_orns).
             If this parameter is specified, you must also specify the `LoadBalancerPort`
             parameter.
           type: string
       required:
       - LoadBalancerName
       type: object
@@ -10335,14 +11117,51 @@
       additionalProperties: false
       properties:
         ResponseContext:
           "$ref": "#/components/schemas/ResponseContext"
         Subnet:
           "$ref": "#/components/schemas/Subnet"
       type: object
+    UpdateUserGroupRequest:
+      additionalProperties: false
+      properties:
+        DryRun:
+          description: If true, checks whether you have the required permissions to
+            perform the action.
+          type: boolean
+        NewPath:
+          description: A new path for the group. If not specified, it is set to a
+            slash (`/`).
+          type: string
+        NewUserGroupName:
+          description: A new name for the user group.
+          type: string
+        Path:
+          description: The path to the group. If not specified, it is set to a slash
+            (`/`).
+          type: string
+        UserGroupName:
+          description: The name of the group you want to update.
+          type: string
+      required:
+      - UserGroupName
+      type: object
+    UpdateUserGroupResponse:
+      additionalProperties: false
+      properties:
+        ResponseContext:
+          "$ref": "#/components/schemas/ResponseContext"
+        UserGroup:
+          "$ref": "#/components/schemas/UserGroup"
+        Users:
+          description: A list of EIM users.
+          items:
+            "$ref": "#/components/schemas/User"
+          type: array
+      type: object
     UpdateUserRequest:
       additionalProperties: false
       properties:
         DryRun:
           description: If true, checks whether you have the required permissions to
             perform the action.
           type: boolean
@@ -10555,15 +11374,15 @@
         VirtualGatewayId:
           description: The ID of the virtual gateway.
           type: string
         VpnConnectionId:
           description: The ID of the VPN connection you want to modify.
           type: string
         VpnOptions:
-          "$ref": "#/components/schemas/VpnOptionsToUpdate"
+          "$ref": "#/components/schemas/VpnOptions"
       required:
       - VpnConnectionId
       type: object
     UpdateVpnConnectionResponse:
       additionalProperties: false
       properties:
         ResponseContext:
@@ -10571,24 +11390,60 @@
         VpnConnection:
           "$ref": "#/components/schemas/VpnConnection"
       type: object
     User:
       additionalProperties: false
       description: Information about the EIM user.
       properties:
+        CreationDate:
+          description: The date and time (UTC) of creation of the EIM user.
+          format: date-time
+          type: string
+        LastModificationDate:
+          description: The date and time (UTC) of the last modification of the EIM
+            user.
+          format: date-time
+          type: string
         Path:
           description: The path to the EIM user.
           type: string
         UserId:
-          description: " The ID of the EIM user."
+          description: The ID of the EIM user.
           type: string
         UserName:
           description: The name of the EIM user.
           type: string
       type: object
+    UserGroup:
+      additionalProperties: false
+      description: Information about the user group.
+      properties:
+        CreationDate:
+          description: The date and time (UTC) of creation of the user group.
+          format: date-time
+          type: string
+        LastModificationDate:
+          description: The date and time (UTC) of the last modification of the user
+            group.
+          format: date-time
+          type: string
+        Name:
+          description: The name of the user group.
+          type: string
+        Orn:
+          description: The Outscale Resource Name (ORN) of the user group. For more
+            information, see [Resource Identifiers](https://docs.outscale.com/en/userguide/Resource-Identifiers.html).
+          type: string
+        Path:
+          description: The path to the user group.
+          type: string
+        UserGroupId:
+          description: The ID of the user group.
+          type: string
+      type: object
     VgwTelemetry:
       additionalProperties: false
       description: Information about the current state of a VPN tunnel.
       properties:
         AcceptedRouteCount:
           description: The number of routes accepted through BGP (Border Gateway Protocol)
             route exchanges.
@@ -10649,15 +11504,15 @@
           description: This parameter is not available. It is present in our API for
             the sake of historical compatibility with AWS.
           type: boolean
         ClientToken:
           description: The idempotency token provided when launching the VM.
           type: string
         CreationDate:
-          description: The date and time of creation of the VM.
+          description: The date and time (UTC) of creation of the VM.
           format: datetime
           type: string
         DeletionProtection:
           description: If true, you cannot delete the VM unless you change this parameter
             back to false.
           type: boolean
         Hypervisor:
@@ -10762,15 +11617,15 @@
           type: string
       type: object
     VmGroup:
       additionalProperties: false
       description: Information about the VM group.
       properties:
         CreationDate:
-          description: The date and time of creation of the VM group.
+          description: The date and time (UTC) of creation of the VM group.
           format: datetime
           type: string
         Description:
           description: The description of the VM group.
           type: string
         PositioningStrategy:
           description: The positioning strategy of the VMs on hypervisors. By default,
@@ -10785,29 +11640,27 @@
           type: string
         SecurityGroupIds:
           description: One or more IDs of security groups for the VM group.
           items:
             type: string
           type: array
         State:
-          description: The state of the VM group (`pending` \| `available` \| `scaling
-            up` \| `scaling down` \| `deleting` \| `deleted`).
           enum:
           - available
           - deleted
           - deleting
           - pending
           - scaling down
           - scaling up
           type: string
         SubnetId:
           description: The ID of the Subnet for the VM group.
           type: string
         Tags:
-          description: One or more tags associated with the VM group.
+          description: One or more tags associated with the VM.
           items:
             "$ref": "#/components/schemas/ResourceTag"
           type: array
         VmCount:
           description: The number of VMs in the VM group.
           type: integer
         VmGroupId:
@@ -10859,15 +11712,14 @@
         VmState:
           description: The state of the VM (`pending` \| `running` \| `stopping` \|
             `stopped` \| `shutting-down` \| `terminated` \| `quarantine`).
           type: string
       type: object
     VmTemplate:
       additionalProperties: false
-      description: Information about the VM template.
       properties:
         CpuCores:
           description: The number of vCores.
           type: integer
         CpuGeneration:
           description: The processor generation.
           type: string
@@ -10875,15 +11727,15 @@
           description: The performance of the VMs.
           enum:
           - medium
           - high
           - highest
           type: string
         CreationDate:
-          description: The date and time of creation of the VM template.
+          description: The date and time (UTC) of creation of the VM template.
           format: date-time
           type: string
         Description:
           description: The description of the VM template.
           type: string
         ImageId:
           description: The ID of the OMI.
@@ -10952,15 +11804,15 @@
           type: integer
       type: object
     Volume:
       additionalProperties: false
       description: Information about the volume.
       properties:
         CreationDate:
-          description: The date and time of creation of the volume.
+          description: The date and time (UTC) of creation of the volume.
           format: datetime
           type: string
         Iops:
           description: |-
             The number of I/O operations per second (IOPS):<br />
             - For `io1` volumes, the number of provisioned IOPS<br />
             - For `gp2` volumes, the baseline performance of the volume
@@ -11055,25 +11907,14 @@
         Phase2Options:
           "$ref": "#/components/schemas/Phase2Options"
         TunnelInsideIpRange:
           description: The range of inside IPs for the tunnel. This must be a /30
             CIDR block from the 169.254.254.0/24 range.
           type: string
       type: object
-    VpnOptionsToUpdate:
-      additionalProperties: false
-      description: Information about the VPN options.
-      properties:
-        Phase2Options:
-          "$ref": "#/components/schemas/Phase2OptionsToUpdate"
-        TunnelInsideIpRange:
-          description: The range of inside IPs for the tunnel. This must be a /30
-            CIDR block from the 169.254.254.0/24 range.
-          type: string
-      type: object
     With:
       additionalProperties: false
       description: The information to display in each returned log.
       properties:
         AccountId:
           default: true
           description: By default or if set to true, the account ID is displayed.
@@ -11174,17 +12015,16 @@
     email: support@outscale.com
   description: "Welcome to the OUTSCALE API documentation.<br />\nThe OUTSCALE API
     enables you to manage your resources in the OUTSCALE Cloud. This documentation
     describes the different actions available along with code examples.<br /><br />\nThrottling:
     To protect against overloads, the number of identical requests allowed in a given
     time period is limited.<br />\nBrute force: To protect against brute force attacks,
     the number of failed authentication attempts in a given time period is limited.<br
-    /><br />\nYou can learn more about errors returned by the API in the dedicated
-    [errors page](api/errors).<br /><br />\nNote that the OUTSCALE Cloud is compatible
-    with Amazon Web Services (AWS) APIs, but there are [differences in resource names](https://docs.outscale.com/en/userguide/OUTSCALE-APIs-Reference.html)
+    /><br />\nNote that the OUTSCALE Cloud is compatible with Amazon Web Services
+    (AWS) APIs, but there are [differences in resource names](https://docs.outscale.com/en/userguide/OUTSCALE-APIs-Reference.html)
     between AWS and the OUTSCALE API.<br />\nYou can also manage your resources using
     the [Cockpit](https://docs.outscale.com/en/userguide/About-Cockpit.html) web interface.<br
     /><br />\nAn OpenAPI description of the OUTSCALE API is also available in this
     [GitHub repository](https://github.com/outscale/osc-api).<br />\n# Authentication
     Schemes\n### Access Key/Secret Key\nThe main way to authenticate your requests
     to the OUTSCALE API is to use an access key and a secret key.<br />\nThe mechanism
     behind this is based on AWS Signature Version 4, whose technical implementation
@@ -11193,37 +12033,45 @@
     on the tool or SDK you want to use to interact with the API.<br />\n\n> For example,
     if you use OSC CLI:\n> 1. You need to create an **~/.osc/config.json** file to
     specify your access key, secret key, and the Region of your account.\n> 2. You
     then specify the `--profile` option when executing OSC CLI commands.\n> \n> For
     more information, see [Installing and Configuring OSC CLI](https://docs.outscale.com/en/userguide/Installing-and-Configuring-OSC-CLI.html).\n\nSee
     the code samples in each section of this documentation for specific examples in
     different programming languages.<br />\nFor more information about access keys,
-    see [About Access Keys](https://docs.outscale.com/en/userguide/About-Access-Keys.html).\n###
-    Login/Password\nFor certain API actions, you can also use basic authentication
-    with the login (email address) and password of your TINA account.<br />\nThis
-    is useful only in special circumstances, for example if you do not know your access
-    key/secret key and want to retrieve them programmatically.<br />\nIn most cases,
-    however, you can use the Cockpit web interface to retrieve them.<br />\n\n> For
-    example, if you use OSC CLI:\n> 1. You need to create an **~/.osc/config.json**
-    file to specify the Region of your account, but you leave the access key value
-    and secret key value empty (`&quot;&quot;`).\n> 2. You then specify the `--profile`,
-    `--authentication-method`, `--login`, and `--password` options when executing
-    OSC CLI commands.\n\nSee the code samples in each section of this documentation
-    for specific examples in different programming languages.\n### No Authentication\nA
-    few API actions do not require any authentication. They are indicated as such
-    in this documentation.<br />\n### Other Security Mechanisms\nIn parallel with
-    the authentication schemes, you can add other security mechanisms to your OUTSCALE
-    account, for example to restrict API requests by IP or other criteria.<br />\nFor
-    more information, see [Managing Your API Accesses](https://docs.outscale.com/en/userguide/Managing-Your-API-Accesses.html)."
+    see [About Access Keys](https://docs.outscale.com/en/userguide/About-Access-Keys.html).\n\n>
+    If you try to sign requests with an invalid access key four times in a row, further
+    authentication attempts will be prevented for 1 minute. This lockout time increases
+    1 minute every four failed attempts, for up to 10 minutes.\n\n### Login/Password\nFor
+    certain API actions, you can also use basic authentication with the login (email
+    address) and password of your TINA account.<br />\nThis is useful only in special
+    circumstances, for example if you do not know your access key/secret key and want
+    to retrieve them programmatically.<br />\nIn most cases, however, you can use
+    the Cockpit web interface to retrieve them.<br />\n\n> For example, if you use
+    OSC CLI:\n> 1. You need to create an **~/.osc/config.json** file to specify the
+    Region of your account, but you leave the access key value and secret key value
+    empty (`&quot;&quot;`).\n> 2. You then specify the `--profile`, `--authentication-method`,
+    `--login`, and `--password` options when executing OSC CLI commands.\n\nSee the
+    code samples in each section of this documentation for specific examples in different
+    programming languages.\n\n> If you try to sign requests with an invalid password
+    four times in a row, further authentication attempts will be prevented for 1 minute.
+    This lockout time increases 1 minute every four failed attempts, for up to 10
+    minutes.\n\n### No Authentication\nA few API actions do not require any authentication.
+    They are indicated as such in this documentation.<br />\n### Other Security Mechanisms\nIn
+    parallel with the authentication schemes, you can add other security mechanisms
+    to your OUTSCALE account, for example to restrict API requests by IP or other
+    criteria.<br />\nFor more information, see [Managing Your API Accesses](https://docs.outscale.com/en/userguide/Managing-Your-API-Accesses.html).<br
+    />\n# Error Codes Reference\nYou can learn more about errors returned by the API
+    in the dedicated [errors page](api-errors.html)."
   license:
     name: BSD 3 Clause
     url: https://opensource.org/licenses/BSD-3-Clause
   termsOfService: https://en.outscale.com/terms-of-service/
   title: 3DS OUTSCALE API
-  version: 1.28.7
+  version: 1.29.3
+  x-osc-api-type: external
 openapi: 3.0.0
 paths:
   "/AcceptNetPeering":
     description: |-
       Accepts a Net peering request.<br />
       To accept this request, you must be the owner of the peer Net. If you do not accept the request within 7 days, the state of the Net peering becomes `expired`.<br /><br />
 
@@ -11289,14 +12137,44 @@
           content:
             application/json:
               schema:
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - NetPeering
+  "/AddUserToUserGroup":
+    description: Adds a user to a specified group.
+    post:
+      operationId: AddUserToUserGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/AddUserToUserGroupRequest"
+            examples:
+              ex1:
+                value:
+                  UserGroupName: example-usergroup
+                  UserGroupPath: "/example/"
+                  UserName: example-user
+                  UserPath: "/example/"
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/AddUserToUserGroupResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+          description: The HTTP 200 response (OK).
+      tags:
+      - UserGroup
   "/CheckAuthentication":
     description: Validates the authenticity of the account.
     post:
       operationId: CheckAuthentication
       requestBody:
         content:
           application/json:
@@ -12001,15 +12879,15 @@
               schema:
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Image
   "/CreateImageExportTask":
     description: |-
-      Exports an Outscale machine image (OMI) to an OUTSCALE Object Storage (OOS) bucket.<br />
+      Exports an OUTSCALE machine image (OMI) to an OUTSCALE Object Storage (OOS) bucket.<br />
       This action enables you to copy an OMI between accounts in different Regions. To copy an OMI in the same Region, you can also use the [CreateImage](#createimage) method.<br />
       The copy of the OMI belongs to you and is independent from the source OMI.<br /><br />
 
       **[IMPORTANT]**<br />
       You cannot export a shared or public OMI, as they do not belong to you. To do so, you must first copy it to your account. The copy then belongs to you and you can export it.<br /><br />
       For more information, see [About OMIs](https://docs.outscale.com/en/userguide/About-OMIs.html).
     post:
@@ -12515,15 +13393,15 @@
           description: The HTTP 200 response (OK).
       tags:
       - Listener
   "/CreateLoadBalancerPolicy":
     description: |-
       Creates a stickiness policy with sticky session lifetimes defined by the browser lifetime.<br />
       The created policy can be used with HTTP or HTTPS listeners only.<br />
-      If this policy is implemented by a load balancer, this load balancer uses this cookie in all incoming requests to direct them to the specified back-end server virtual machine (VM). If this cookie is not present, the load balancer sends the request to any other server according to its load-balancing algorithm.<br /><br />
+      If this policy is implemented by a load balancer, this load balancer uses this cookie in all incoming requests to direct them to the specified backend server virtual machine (VM). If this cookie is not present, the load balancer sends the request to any other server according to its load-balancing algorithm.<br /><br />
 
       You can also create a stickiness policy with sticky session lifetimes following the lifetime of an application-generated cookie.<br />
       Unlike the other type of stickiness policy, the lifetime of the special Load Balancer Unit (LBU) cookie follows the lifetime of the application-generated cookie specified in the policy configuration. The load balancer inserts a new stickiness cookie only when the application response includes a new application cookie.<br />
       The session stops being sticky if the application cookie is removed or expires, until a new application cookie is issued.<br /><br />
       For more information, see [About Load Balancers](https://docs.outscale.com/en/userguide/About-Load-Balancers.html).
     post:
       operationId: CreateLoadBalancerPolicy
@@ -13506,15 +14384,15 @@
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - SecurityGroupRule
   "/CreateServerCertificate":
     description: |-
       Creates a server certificate and its matching private key.<br /><br />
       These elements can be used with other services (for example, to configure SSL termination on load balancers).<br /><br />
-      You can also specify the chain of intermediate certification authorities if your certificate is not directly signed by a root one. You can specify multiple intermediate certification authorities in the `CertificateChain` parameter. To do so, concatenate all certificates in the correct order (the first certificate must be the authority of your certificate, the second must the the authority of the first one, and so on).<br /><br />
+      You can also specify the chain of intermediate certification authorities if your certificate is not directly signed by a root one. You can specify multiple intermediate certification authorities in the `CertificateChain` parameter. To do so, concatenate all certificates in the correct order (the first certificate must be the authority of your certificate, the second must be the authority of the first one, and so on).<br /><br />
       The private key must be a RSA key in PKCS1 form. To check this, open the PEM file and ensure its header reads as follows: BEGIN RSA PRIVATE KEY.<br /><br />
       [IMPORTANT]<br /><br />
       This private key must not be protected by a password or a passphrase.<br /><br />
       For more information, see [About Server Certificates in EIM](https://docs.outscale.com/en/userguide/About-Server-Certificates-in-EIM.html).
     post:
       operationId: CreateServerCertificate
       requestBody:
@@ -13553,14 +14431,17 @@
     description: |-
       Creates a snapshot. Snapshots are point-in-time images of a volume that you can use to back up your data or to create replicas of this volume.<br />
       You can use this method in three different ways:
       * **Creating from a volume**: You create a snapshot from one of your volumes.<br />
       * **Copying a snapshot**: You copy an existing snapshot. The source snapshot can be one of your own snapshots, or a snapshot owned by another account that has granted you permission via the [UpdateSnapshot](#updatesnapshot) method.<br />
       * **Importing from a bucket**: You import a snapshot located in an OUTSCALE Object Storage (OOS) bucket. First, the owner of the source snapshot must export it to the bucket by using the [CreateSnapshotExportTask](#createsnapshotexporttask) method. Then, they must grant you permission to read the snapshot via a pre-signed URL or Access Control Lists. For more information, see [Managing Access to Your Buckets and Objects](https://docs.outscale.com/en/userguide/Managing-Access-to-Your-Buckets-and-Objects.html).
 
+      **[NOTE]**<br />
+      In case of excessive use of the snapshot creation feature on the same volume over a short period of time, 3DS OUTSCALE reserves the right to temporarily block the feature.
+
       For more information, see [About Snapshots](https://docs.outscale.com/en/userguide/About-Snapshots.html).
     post:
       operationId: CreateSnapshot
       requestBody:
         content:
           application/json:
             schema:
@@ -13880,14 +14761,51 @@
                       UserId: ABCDEFGHIJKLMNOPQRSTUVWXYZ12345
                       Path: "/documentation/"
                     ResponseContext:
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
       tags:
       - User
+  "/CreateUserGroup":
+    description: |-
+      Creates a group to which you can add users.<br />
+      You can also add an inline policy or link a managed policy to the group, which is applied to all its users.
+    post:
+      operationId: CreateUserGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/CreateUserGroupRequest"
+            examples:
+              ex1:
+                value:
+                  Path: "/example/"
+                  UserGroupName: example-usergroup
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/CreateUserGroupResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+                    UserGroup:
+                      CreationDate: '2010-10-01T12:34:56.789Z'
+                      LastModificationDate: 2010-10-01 12:34:56.789000000 +00:00
+                      Name: example-usergroup
+                      Orn: orn:ows:idauth::012345678910:usergroup/example/usergroup-example
+                      Path: "/example/"
+                      UserGroupId: ug-12345678
+          description: The HTTP 200 response (OK).
+      tags:
+      - UserGroup
   "/CreateVirtualGateway":
     description: |-
       Creates a virtual gateway.<br />
       A virtual gateway is the access point on the Net side of a VPN connection.<br /><br />
       For more information, see [About Virtual Gateways](https://docs.outscale.com/en/userguide/About-Virtual-Gateways.html).
     post:
       operationId: CreateVirtualGateway
@@ -14029,26 +14947,27 @@
           content:
             application/json:
               schema:
                 "$ref": "#/components/schemas/CreateVmTemplateResponse"
               examples:
                 ex1:
                   value:
-                    VmTemplateName: vmtemplate-example
-                    CpuPerformance: high
-                    CreationDate: 2010-10-01 12:34:56.789000000 +00:00
-                    CpuCores: 2
-                    Tags:
-                    - Key: key1
-                      Value: value1
-                    Description: Log collector template
-                    ImageId: ami-12345678
-                    CpuGeneration: v4
-                    VmTemplateId: vmtemplate-98765432109876543210987654321012
-                    Ram: 2
+                    VmTemplate:
+                      VmTemplateName: vmtemplate-example
+                      CpuPerformance: high
+                      CreationDate: 2010-10-01 12:34:56.789000000 +00:00
+                      CpuCores: 2
+                      Tags:
+                      - Key: key1
+                        Value: value1
+                      Description: Log collector template
+                      ImageId: ami-12345678
+                      CpuGeneration: v4
+                      VmTemplateId: vmtemplate-98765432109876543210987654321012
+                      Ram: 2
                     ResponseContext:
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
       tags:
       - VmTemplate
   "/CreateVms":
     description: |-
@@ -16028,15 +16947,15 @@
               schema:
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Tag
   "/DeleteUser":
     description: Deletes a specified EIM user. The EIM user must not belong to any
-      group, nor have any key or attached policy.
+      group, nor have any key or linked policy.
     post:
       operationId: DeleteUser
       requestBody:
         content:
           application/json:
             schema:
               "$ref": "#/components/schemas/DeleteUserRequest"
@@ -16054,14 +16973,77 @@
                 ex1:
                   value:
                     ResponseContext:
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
       tags:
       - User
+  "/DeleteUserGroup":
+    description: |-
+      Deletes a specified user group.<br />
+
+      **[WARNING]**<br />
+      The user group must be empty of any user and must not have any linked policy. Otherwise, you need to force the deletion.<br />
+      If you force the deletion, all inline policies will be deleted with the user group.<br />
+    post:
+      operationId: DeleteUserGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/DeleteUserGroupRequest"
+            examples:
+              ex1:
+                value:
+                  Force: false
+                  Path: "/example/"
+                  UserGroupName: example-usergroup
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/DeleteUserGroupResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+          description: The HTTP 200 response (OK).
+      tags:
+      - UserGroup
+  "/DeleteUserGroupPolicy":
+    description: Deletes a specified inline policy from a specific group.
+    post:
+      operationId: DeleteUserGroupPolicy
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/DeleteUserGroupPolicyRequest"
+            examples:
+              ex1:
+                value:
+                  PolicyName: example-usergroup-policy
+                  UserGroupName: example-usergroup
+                  UserGroupPath: "/example/"
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/DeleteUserGroupPolicyResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+          description: The HTTP 200 response (OK).
+      tags:
+      - Policy
   "/DeleteVirtualGateway":
     description: |-
       Deletes a specified virtual gateway.<br />
       Before deleting a virtual gateway, we recommend to detach it from the Net and delete the VPN connection.
     post:
       operationId: DeleteVirtualGateway
       requestBody:
@@ -16354,15 +17336,18 @@
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
       tags:
       - LoadBalancer
   "/LinkFlexibleGpu":
     description: |-
       Attaches one of your allocated flexible GPUs (fGPUs) to one of your virtual machines (VMs).<br />
-      The fGPU is in the `attaching` state until the VM is stopped, after which it becomes `attached`.
+      The fGPU is in the `attaching` state until the VM is stopped, after which it becomes `attached`. <br /><br />
+
+      **[NOTE]**<br />
+      You can attach fGPUs only to VMs with the `highest` (1) performance flag. For more information see [About Flexible GPUs](https://docs.outscale.com/en/userguide/About-Flexible-GPUs.html) and [VM Types](https://docs.outscale.com/en/userguide/VM-Types.html).
     post:
       operationId: LinkFlexibleGpu
       requestBody:
         content:
           application/json:
             schema:
               "$ref": "#/components/schemas/LinkFlexibleGpuRequest"
@@ -16432,15 +17417,15 @@
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - InternetService
   "/LinkLoadBalancerBackendMachines":
     description: |-
       Attaches one or more virtual machines (VMs) to a specified load balancer. You need to specify at least the `BackendIps` or the `BackendVmIds` parameter.<br />
-      The VMs can be in different Subnets and different Subregions than the load balancer, as long as the VMs and load balancers are all in the public Cloud or all in the same Net. It may take a little time for a VM to be registered with the load balancer. Once the VM is registered with a load balancer, it receives traffic and requests from this load balancer and is called a back-end VM.
+      The VMs can be in different Subnets and different Subregions than the load balancer, as long as the VMs and load balancers are all in the public Cloud or all in the same Net. It may take a little time for a VM to be registered with the load balancer. Once the VM is registered with a load balancer, it receives traffic and requests from this load balancer and is called a backend VM.
     post:
       operationId: LinkLoadBalancerBackendMachines
       requestBody:
         content:
           application/json:
             schema:
               "$ref": "#/components/schemas/LinkLoadBalancerBackendMachinesRequest"
@@ -16475,14 +17460,43 @@
                   summary: Linking public IPs to a load balancer
                   value:
                     ResponseContext:
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
       tags:
       - LoadBalancer
+  "/LinkManagedPolicyToUserGroup":
+    description: Links a managed policy to a specific group. This policy applies to
+      all the users contained in this group.
+    post:
+      operationId: LinkManagedPolicyToUserGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/LinkManagedPolicyToUserGroupRequest"
+            examples:
+              ex1:
+                value:
+                  PolicyOrn: orn:ows:idauth::012345678910:policy/example/example-user-policy
+                  UserGroupName: example-usergroup
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/LinkManagedPolicyToUserGroupResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+          description: The HTTP 200 response (OK).
+      tags:
+      - Policy
   "/LinkNic":
     description: |-
       Attaches a network interface card (NIC) to a virtual machine (VM).<br />
       The interface and the VM must be in the same Subregion. The VM can be either `running` or `stopped`. The NIC must be in the `available` state. For more information, see [Attaching a NIC to a VM](https://docs.outscale.com/en/userguide/Attaching-a-NIC-to-a-VM.html).
     post:
       operationId: LinkNic
       requestBody:
@@ -16812,14 +17826,47 @@
           content:
             application/json:
               schema:
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Volume
+  "/PutUserGroupPolicy":
+    description: |-
+      Creates or updates an inline policy included in a specified group.<br />
+      The policy is automatically applied to all the users of the group after its creation.
+    post:
+      operationId: PutUserGroupPolicy
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/PutUserGroupPolicyRequest"
+            examples:
+              ex1:
+                value:
+                  PolicyDocument: '{"Statement": [ {"Effect": "Allow", "Action": ["*"],
+                    "Resource": ["*"]} ]}'
+                  PolicyName: example-usergroup-policy
+                  UserGroupName: example-usergroup
+                  UserGroupPath: "/example/"
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/PutUserGroupPolicyResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+          description: The HTTP 200 response (OK).
+      tags:
+      - Policy
   "/ReadAccessKeys":
     description: Lists the access key IDs of either your root account or an EIM user.
     post:
       operationId: ReadAccessKeys
       requestBody:
         content:
           application/json:
@@ -17043,15 +18090,15 @@
   "/ReadApiLogs":
     description: |-
       Lists the logs of the API calls you have performed with this account.
 
       **[IMPORTANT]**<br />
       Past logs are accessible for up to 32 days.<br />
       By default, the retrieved interval is 48 hours. If neither of the `QueryDateBefore` nor `QueryDateAfter` parameters are specified, logs from the past 48 hours are retrieved. If you only specify one of two, logs are retrieved from a 2-day interval based on the date you provided. To retrieve logs beyond a 2-day interval, specify both parameters.<br /><br />
-      For more information, see [About OUTSCALE Monitoring Services (OMS)](https://docs.outscale.com/en/userguide/About-OUTSCALE-Monitoring-Services-OMS.html).
+      For more information, see [About OMS](https://docs.outscale.com/en/userguide/About-OMS.html).
     post:
       operationId: ReadApiLogs
       requestBody:
         content:
           application/json:
             schema:
               "$ref": "#/components/schemas/ReadApiLogsRequest"
@@ -17334,26 +18381,29 @@
                 "$ref": "#/components/schemas/ReadConsumptionAccountResponse"
               examples:
                 ex1:
                   value:
                     ResponseContext:
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
                     ConsumptionEntries:
-                    - FromDate: 2023-06-01 00:00:00.000000000 +00:00
+                    - UnitPrice: 0.044
+                      Type: BoxUsage:tinav4.c1r1p2
+                      Operation: RunInstances-OD
                       SubregionName: eu-west-2a
-                      Value: 720.0
-                      Title: Instance - On demand - tinav4.c2r4 high performance -
+                      Value: 1392
+                      Title: Instance - On demand - tinav4.c1r1 high performance -
                         par heure
                       Category: compute
                       ToDate: 2023-06-30 00:00:00.000000000 +00:00
                       Service: TinaOS-FCU
                       AccountId: '123456789012'
                       PayingAccountId: '123456789012'
-                      Operation: RunInstances-OD
-                      Type: BoxUsage:tinav4.c2r4p2
+                      FromDate: 2023-06-01 00:00:00.000000000 +00:00
+                      Price: 61.248
+                    Currency: EUR
           description: The HTTP 200 response (OK).
       tags:
       - Account
   "/ReadDedicatedGroups":
     description: |-
       > [WARNING]<br />
       > This feature is currently in beta.<br />
@@ -18132,14 +19182,56 @@
                       Code: PAR1
                     - Name: Equinix Pantin, France
                       Code: PAR4
           description: The HTTP 200 response (OK).
       security: []
       tags:
       - Location
+  "/ReadManagedPoliciesLinkedToUserGroup":
+    description: Lists the managed policies linked to a specified group.
+    post:
+      operationId: ReadManagedPoliciesLinkedToUserGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/ReadManagedPoliciesLinkedToUserGroupRequest"
+            examples:
+              ex1:
+                value:
+                  Filters:
+                    PathPrefix: "/ex"
+                    UserGroupIds:
+                    - ug-12345678
+                  FirstItem: 1
+                  ResultsPerPage: 30
+                  UserGroupName: example-usergroup
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/ReadManagedPoliciesLinkedToUserGroupResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+                    HasMoreItems: true
+                    MaxResultsLimit: 30
+                    MaxResultsTruncated: true
+                    Policies:
+                    - CreationDate: '2010-10-01T12:34:56.789Z'
+                      LastModificationDate: '2010-10-01T12:34:56.789Z'
+                      Orn: orn:ows:idauth::012345678910:policy/example/example-user-policy
+                      PolicyId: ABCDEFGHIJKLMNOPQRSTUVWXYZ01234
+                      PolicyName: example-policy
+          description: The HTTP 200 response (OK).
+      tags:
+      - Policy
   "/ReadNatServices":
     description: Lists one or more network address translation (NAT) services.
     post:
       operationId: ReadNatServices
       requestBody:
         content:
           application/json:
@@ -19468,14 +20560,205 @@
           content:
             application/json:
               schema:
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Tag
+  "/ReadUserGroup":
+    description: Lists information about a specified user group, including its users.
+    post:
+      operationId: ReadUserGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/ReadUserGroupRequest"
+            examples:
+              ex1:
+                value:
+                  Path: "/example/"
+                  UserGroupName: example-usergroup
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/ReadUserGroupResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+                    UserGroup:
+                      CreationDate: '2010-10-01T12:34:56.789Z'
+                      LastModificationDate: '2010-10-01T12:34:56.789Z'
+                      Name: example-usergroup
+                      Orn: orn:ows:idauth::012345678910:usergroup/example/usergroup-example
+                      Path: "/example/"
+                      UserGroupId: ug-12345678
+                    Users:
+                    - CreationDate: '2010-10-01T12:34:56.789Z'
+                      LastModificationDate: '2010-10-01T12:34:56.789Z'
+                      Path: "/example/"
+                      UserId: ABCDEFGHIJKLMNOPQRSTUVWXYZ12345
+                      UserName: example-user
+          description: The HTTP 200 response (OK).
+      tags:
+      - UserGroup
+  "/ReadUserGroupPolicies":
+    description: Lists the names of the inline policies embedded in a specific group.
+    post:
+      operationId: ReadUserGroupPolicies
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/ReadUserGroupPoliciesRequest"
+            examples:
+              ex1:
+                value:
+                  FirstItem: 1
+                  ResultsPerPage: 30
+                  UserGroupName: example-usergroup
+                  UserGroupPath: "/example/"
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/ReadUserGroupPoliciesResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+                    HasMoreItems: true
+                    MaxResultsLimit: 30
+                    MaxResultsTruncated: true
+                    Policies:
+                    - Body: '{"Statement": [ {"Effect": "Allow", "Action": ["*"],
+                        "Resource": ["*"]} ]}'
+                      Name: example-policy
+          description: The HTTP 200 response (OK).
+      tags:
+      - Policy
+  "/ReadUserGroupPolicy":
+    description: Returns information about an inline policy included in a specified
+      group.
+    post:
+      operationId: ReadUserGroupPolicy
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/ReadUserGroupPolicyRequest"
+            examples:
+              ex1:
+                value:
+                  PolicyName: example-policy
+                  UserGroupName: example-usergroup
+                  UserGroupPath: "/example/"
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/ReadUserGroupPolicyResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+                    Policy:
+                      Body: '{"Statement": [ {"Effect": "Allow", "Action": ["*"],
+                        "Resource": ["*"]} ]}'
+                      Name: example-policy
+          description: The HTTP 200 response (OK).
+      tags:
+      - Policy
+  "/ReadUserGroups":
+    description: |-
+      Lists the groups with the specified path prefix.<br />
+      If you do not specify any path prefix, this action returns all the groups (or an empty list if there are none).
+    post:
+      operationId: ReadUserGroups
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/ReadUserGroupsRequest"
+            examples:
+              ex1:
+                value:
+                  Filters:
+                    PathPrefix: "/ex"
+                    UserGroupIds:
+                    - ug-12345678
+                  FirstItem: 1
+                  ResultsPerPage: 30
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/ReadUserGroupsResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+                    HasMoreItems: true
+                    MaxResultsLimit: 30
+                    MaxResultsTruncated: true
+                    UserGroups:
+                    - CreationDate: '2010-10-01T12:34:56.789Z'
+                      LastModificationDate: '2010-10-01T12:34:56.789Z'
+                      Name: example-usergroup
+                      Orn: orn:ows:idauth::012345678910:usergroup/example/usergroup-example
+                      Path: "/example/"
+                      UserGroupId: ug-12345678
+          description: The HTTP 200 response (OK).
+      tags:
+      - UserGroup
+  "/ReadUserGroupsPerUser":
+    description: Lists the groups a specified user belongs to.
+    post:
+      operationId: ReadUserGroupsPerUser
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/ReadUserGroupsPerUserRequest"
+            examples:
+              ex1:
+                value:
+                  UserName: example-user
+                  UserPath: "/example/"
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/ReadUserGroupsPerUserResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+                    UserGroups:
+                    - CreationDate: '2010-10-01T12:34:56.789Z'
+                      LastModificationDate: '2010-10-01T12:34:56.789Z'
+                      Name: example-usergroup
+                      Orn: orn:ows:idauth::012345678910:usergroup/example/usergroup-example
+                      Path: "/example/"
+                      UserGroupId: ug-12345678
+          description: The HTTP 200 response (OK).
+      tags:
+      - UserGroup
   "/ReadUsers":
     description: |-
       Lists all EIM users that have a specified path.<br />
       If you do not specify a path, this action returns a list of all users in the account (or an empty list if there are none).
     post:
       operationId: ReadUsers
       requestBody:
@@ -19586,16 +20869,18 @@
                 "$ref": "#/components/schemas/ReadVmGroupsResponse"
               examples:
                 ex1:
                   value:
                     ResponseContext:
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
                     VmGroups:
-                      SecurityGroupsIds: sg-87654321
-                      VmIds: i-12345678
+                    - SecurityGroupIds:
+                      - sg-87654321
+                      VmIds:
+                      - i-12345678
                       CreationDate: 2010-10-01 12:34:56.789000000 +00:00
                       VmCount: 1
                       VmGroupName: ClusterLog-PPD01
                       SubnetId: subnet-12345678
                       PositioningStrategy: attract
                       State: available
                       VmGroupId: vmgroup-12345678901234567890123456789012
@@ -19643,36 +20928,38 @@
                     VmTemplateNames:
                     - vmtemplate-example
               ex2:
                 value:
                   Filters:
                     CpuCores:
                     - 2
-                    CpuGeneration:
+                    CpuGenerations:
                     - v4
       responses:
         '200':
           content:
             application/json:
               schema:
                 "$ref": "#/components/schemas/ReadVmTemplatesResponse"
               examples:
                 ex1:
                   value:
                     VmTemplates:
-                      VmTemplateName: vmtemplate-example
+                    - VmTemplateName: vmtemplate-example
                       CpuPerformance: high
                       CreationDate: 2010-10-01 12:34:56.789000000 +00:00
                       CpuCores: 2
                       Tags: []
                       Description: ''
                       ImageId: ami-12345678
                       CpuGeneration: v4
                       VmTemplateId: vmtemplate-98765432109876543210987654321012
                       Ram: 2
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
       tags:
       - VmTemplate
   "/ReadVmTypes":
     description: Lists one or more predefined VM types.
     post:
       operationId: ReadVmTypes
@@ -19697,15 +20984,15 @@
                 ex1:
                   value:
                     VmTypes:
                     - VolumeCount: 0
                       VmTypeName: t2.small
                       BsuOptimized: false
                       MaxPrivateIps: 4
-                      MemorySize: 2.0
+                      MemorySize: 2
                       VcoreCount: 1
                     ResponseContext:
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
       security: []
       tags:
       - Vm
@@ -19828,15 +21115,15 @@
             application/json:
               schema:
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Vm
   "/ReadVmsHealth":
-    description: Lists the state of one or more back-end virtual machines (VMs) registered
+    description: Lists the state of one or more backend virtual machines (VMs) registered
       with a specified load balancer.
     post:
       operationId: ReadVmsHealth
       requestBody:
         content:
           application/json:
             schema:
@@ -20106,15 +21393,15 @@
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Vm
   "/RegisterVmsInLoadBalancer":
     description: |-
       Registers one or more virtual machines (VMs) with a specified load balancer.<br />
-      The VMs can be in different Subnets and different Subregions than the load balancer, as long as the VMs and load balancers are all in the public Cloud or all in the same Net. It may take a little time for a VM to be registered with the load balancer. Once the VM is registered with a load balancer, it receives traffic and requests from this load balancer and is called a back-end VM.
+      The VMs can be in different Subnets and different Subregions than the load balancer, as long as the VMs and load balancers are all in the public Cloud or all in the same Net. It may take a little time for a VM to be registered with the load balancer. Once the VM is registered with a load balancer, it receives traffic and requests from this load balancer and is called a backend VM.
     post:
       operationId: RegisterVmsInLoadBalancer
       requestBody:
         content:
           application/json:
             schema:
               "$ref": "#/components/schemas/RegisterVmsInLoadBalancerRequest"
@@ -20188,14 +21475,44 @@
           content:
             application/json:
               schema:
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - NetPeering
+  "/RemoveUserFromUserGroup":
+    description: Removes a specified user from a specified group.
+    post:
+      operationId: RemoveUserFromUserGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/RemoveUserFromUserGroupRequest"
+            examples:
+              ex1:
+                value:
+                  UserGroupName: example-usergroup
+                  UserGroupPath: "/example/"
+                  UserName: example-user
+                  UserPath: "/example/"
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/RemoveUserFromUserGroupResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+          description: The HTTP 200 response (OK).
+      tags:
+      - UserGroup
   "/ScaleDownVmGroup":
     description: |-
       > [WARNING]<br />
       > This feature is currently under development and may not function properly.<br />
 
       Deletes virtual machines (VMs) from a VM group.<br />
       The oldest VMs are the first to be deleted.
@@ -20429,15 +21746,15 @@
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - Vm
   "/UnlinkFlexibleGpu":
     description: |-
       Detaches a flexible GPU (fGPU) from a virtual machine (VM).<br />
-      The fGPU is in the `detaching` state until the VM is stopped, after which it becomes available for allocation again.
+      The fGPU is in the `detaching` state until the VM is stopped, after which it becomes `allocated`. It is then available again for attachment to a VM.
     post:
       operationId: UnlinkFlexibleGpu
       requestBody:
         content:
           application/json:
             schema:
               "$ref": "#/components/schemas/UnlinkFlexibleGpuRequest"
@@ -20504,17 +21821,16 @@
             application/json:
               schema:
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 500 response (Internal Server Error).
       tags:
       - InternetService
   "/UnlinkLoadBalancerBackendMachines":
-    description: Detaches one or more back-end virtual machines (VMs) from a load
-      balancer. You need to specify at least the `BackendIps` or the `BackendVmIds`
-      parameter.
+    description: Detaches one or more backend virtual machines (VMs) from a load balancer.
+      You need to specify at least the `BackendIps` or the `BackendVmIds` parameter.
     post:
       operationId: UnlinkLoadBalancerBackendMachines
       requestBody:
         content:
           application/json:
             schema:
               "$ref": "#/components/schemas/UnlinkLoadBalancerBackendMachinesRequest"
@@ -20549,14 +21865,42 @@
                   summary: Unlinking public IPs from a load balancer
                   value:
                     ResponseContext:
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
       tags:
       - LoadBalancer
+  "/UnlinkManagedPolicyFromUserGroup":
+    description: Unlinks a managed policy from a specific group.
+    post:
+      operationId: UnlinkManagedPolicyFromUserGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/UnlinkManagedPolicyFromUserGroupRequest"
+            examples:
+              ex1:
+                value:
+                  PolicyOrn: orn:ows:idauth::012345678910:policy/example/example-user-policy
+                  UserGroupName: example-usergroup
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/UnlinkManagedPolicyFromUserGroupResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+          description: The HTTP 200 response (OK).
+      tags:
+      - Policy
   "/UnlinkNic":
     description: |-
       Detaches a network interface card (NIC) from a virtual machine (VM).<br />
       The primary NIC cannot be detached.
     post:
       operationId: UnlinkNic
       requestBody:
@@ -21286,14 +22630,15 @@
                   PermissionsToLaunch:
                     Additions:
                       GlobalPermission: true
               ex4:
                 summary: Making an image private to everyone
                 value:
                   ImageId: ami-12345678
+                  Description: Private image
                   PermissionsToLaunch:
                     Removals:
                       GlobalPermission: true
       responses:
         '200':
           content:
             application/json:
@@ -21407,15 +22752,15 @@
                       ProductCodes:
                       - '0001'
                       PermissionsToLaunch:
                         GlobalPermission: false
                         AccountIds: []
                       AccountId: '123456789012'
                       Tags: []
-                      Description: ''
+                      Description: Private image
                       ImageId: ami-12345678
                       BlockDeviceMappings:
                       - DeviceName: "/dev/sda1"
                         Bsu:
                           VolumeType: standard
                           DeleteOnVmDeletion: true
                           VolumeSize: 50
@@ -22409,14 +23754,57 @@
                       UserId: ABCDEFGHIJKLMNOPQRSTUVWXYZ12345
                       Path: "/product/"
                     ResponseContext:
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
       tags:
       - User
+  "/UpdateUserGroup":
+    description: Modifies the name and/or the path of a specified group.
+    post:
+      operationId: UpdateUserGroup
+      requestBody:
+        content:
+          application/json:
+            schema:
+              "$ref": "#/components/schemas/UpdateUserGroupRequest"
+            examples:
+              ex1:
+                value:
+                  NewPath: "/new-path/"
+                  NewUserGroupName: new-usergroup
+                  Path: "/example/"
+                  UserGroupName: example-usergroup
+      responses:
+        '200':
+          content:
+            application/json:
+              schema:
+                "$ref": "#/components/schemas/UpdateUserGroupResponse"
+              examples:
+                ex1:
+                  value:
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+                    UserGroup:
+                      CreationDate: '2010-10-01T12:34:56.789Z'
+                      LastModificationDate: '2010-10-01T12:34:56.789Z'
+                      Name: new-usergroup
+                      Orn: orn:ows:idauth::012345678910:usergroup/example/usergroup-example
+                      Path: "/new-path/"
+                      UserGroupId: ug-12345678
+                    Users:
+                    - CreationDate: '2010-10-01T12:34:56.789Z'
+                      LastModificationDate: '2010-10-01T12:34:56.789Z'
+                      Path: "/example/"
+                      UserId: ABCDEFGHIJKLMNOPQRSTUVWXYZ12345
+                      UserName: example-user
+          description: The HTTP 200 response (OK).
+      tags:
+      - UserGroup
   "/UpdateVm":
     description: |-
       Modifies the specified attributes of a virtual machine (VM).<br />
       You must stop the VM before modifying the following attributes:<br />
       * `NestedVirtualization`<br />
       * `Performance`<br />
       * `UserData`<br />
@@ -22647,16 +24035,16 @@
                       VmGroupName: new-name
                       SubnetId: subnet-12345678
                       PositioningStrategy: attract
                       State: available
                       VmGroupId: vmgroup-12345678901234567890123456789012
                       Description: New description of the VM group
                       Tags: []
-                      ResponseContext:
-                        RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
+                    ResponseContext:
+                      RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
         '400':
           content:
             application/json:
               schema:
                 "$ref": "#/components/schemas/ErrorResponse"
           description: The HTTP 400 response (Bad Request).
@@ -22698,24 +24086,25 @@
           content:
             application/json:
               schema:
                 "$ref": "#/components/schemas/UpdateVmTemplateResponse"
               examples:
                 ex1:
                   value:
-                    VmTemplateName: second-name
-                    CpuPerformance: high
-                    CreationDate: 2010-10-01 12:34:56.789000000 +00:00
-                    CpuCores: 2
-                    Tags: []
-                    Description: The new description of the VM template
-                    ImageId: ami-12345678
-                    CpuGeneration: v4
-                    VmTemplateId: vmtemplate-98765432109876543210987654321012
-                    Ram: 2
+                    VmTemplate:
+                      VmTemplateName: second-name
+                      CpuPerformance: high
+                      CreationDate: 2010-10-01 12:34:56.789000000 +00:00
+                      CpuCores: 2
+                      Tags: []
+                      Description: The new description of the VM template
+                      ImageId: ami-12345678
+                      CpuGeneration: v4
+                      VmTemplateId: vmtemplate-98765432109876543210987654321012
+                      Ram: 2
                     ResponseContext:
                       RequestId: 0475ca1e-d0c5-441d-712a-da55a4175157
           description: The HTTP 200 response (OK).
       tags:
       - VmTemplate
   "/UpdateVolume":
     description: |-
```

### Comparing `osc_sdk_python-0.28.0/osc_sdk_python/outscale_gateway.py` & `osc_sdk_python-0.29.0/osc_sdk_python/outscale_gateway.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/osc_sdk_python/requester.py` & `osc_sdk_python-0.29.0/osc_sdk_python/requester.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/osc_sdk_python/resources/gateway_errors.yaml` & `osc_sdk_python-0.29.0/osc_sdk_python/resources/gateway_errors.yaml`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/osc_sdk_python.egg-info/PKG-INFO` & `osc_sdk_python-0.29.0/osc_sdk_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osc_sdk_python
-Version: 0.28.0
+Version: 0.29.0
 Summary: Outscale Gateway python SDK
 Home-page: https://github.com/outscale/osc_sdk_python
 Author: Outscal SAS
 Author-email: opensource@outscale.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 
 ```bash
 $ make package
 ```
 
 You can then install it with:
 ```bash
-$ pip install dist/osc_sdk_python-0.28.0-py3-none-any.whl
+$ pip install dist/osc_sdk_python-0.29.0-py3-none-any.whl
 ```
 
 # Configuration & Credentials
 
 When you use the cli you can choose a profile. Profiles can be set with environment variables or in a file.
 It checks environment variables before loading the file.
```

### Comparing `osc_sdk_python-0.28.0/osc_sdk_python.egg-info/SOURCES.txt` & `osc_sdk_python-0.29.0/osc_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/setup.py` & `osc_sdk_python-0.29.0/setup.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/tests/test_log.py` & `osc_sdk_python-0.29.0/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/tests/test_manual_aksk.py` & `osc_sdk_python-0.29.0/tests/test_manual_aksk.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/tests/test_net.py` & `osc_sdk_python-0.29.0/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `osc_sdk_python-0.28.0/tests/test_password.py` & `osc_sdk_python-0.29.0/tests/test_password.py`

 * *Files identical despite different names*

