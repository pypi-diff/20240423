# Comparing `tmp/onekey_client-2.2.0.tar.gz` & `tmp/onekey_client-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onekey_client-2.2.0.tar", max compression
+gzip compressed data, was "onekey_client-2.3.0.tar", max compression
```

## Comparing `onekey_client-2.2.0.tar` & `onekey_client-2.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1073 2023-10-31 21:02:01.724644 onekey_client-2.2.0/LICENSE
--rw-r--r--   0        0        0     3540 2023-10-31 21:02:01.724644 onekey_client-2.2.0/README.md
--rw-r--r--   0        0        0       72 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/__init__.py
--rw-r--r--   0        0        0        0 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/cli/__init__.py
--rw-r--r--   0        0        0    10859 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/cli/ci.py
--rw-r--r--   0        0        0     3285 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/cli/cli.py
--rw-r--r--   0        0        0     2064 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/cli/firmware_upload.py
--rw-r--r--   0        0        0      450 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/cli/misc.py
--rw-r--r--   0        0        0     8320 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/client.py
--rw-r--r--   0        0        0     1037 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/errors.py
--rw-r--r--   0        0        0        0 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/keys/__init__.py
--rw-r--r--   0        0        0    29677 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/keys/ca.pem
--rw-r--r--   0        0        0      434 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/models.py
--rw-r--r--   0        0        0       30 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/queries/__init__.py
--rw-r--r--   0        0        0      501 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/queries/compare_firmware.graphql
--rw-r--r--   0        0        0      613 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/queries/create_firmware_upload.graphql
--rw-r--r--   0        0        0      137 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/queries/get_firmware_latest_analysis_state.graphql
--rw-r--r--   0        0        0      350 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/queries/get_firmware_latest_results.graphql
--rw-r--r--   0        0        0       62 2023-10-31 21:02:01.724644 onekey_client-2.2.0/onekey_client/queries/get_product_groups.graphql
--rw-r--r--   0        0        0      212 2023-10-31 21:02:01.728644 onekey_client-2.2.0/onekey_client/queries/get_same_product_firmwares.graphql
--rw-r--r--   0        0        0       72 2023-10-31 21:02:01.728644 onekey_client-2.2.0/onekey_client/queries/get_self.graphql
--rw-r--r--   0        0        0      357 2023-10-31 21:02:01.728644 onekey_client-2.2.0/onekey_client/queries/utils.py
--rw-r--r--   0        0        0     1026 2023-10-31 21:02:01.728644 onekey_client-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 onekey_client-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-23 09:48:20.504307 onekey_client-2.3.0/LICENSE
+-rw-r--r--   0        0        0     3873 2024-04-23 09:48:20.504307 onekey_client-2.3.0/README.md
+-rw-r--r--   0        0        0       72 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/cli/__init__.py
+-rw-r--r--   0        0        0    10859 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/cli/ci.py
+-rw-r--r--   0        0        0     3285 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/cli/cli.py
+-rw-r--r--   0        0        0     3143 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/cli/firmware_upload.py
+-rw-r--r--   0        0        0      450 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/cli/misc.py
+-rw-r--r--   0        0        0     8726 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/client.py
+-rw-r--r--   0        0        0     1037 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/errors.py
+-rw-r--r--   0        0        0        0 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/keys/__init__.py
+-rw-r--r--   0        0        0    29677 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/keys/ca.pem
+-rw-r--r--   0        0        0      470 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/models.py
+-rw-r--r--   0        0        0       30 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/queries/__init__.py
+-rw-r--r--   0        0        0      501 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/queries/compare_firmware.graphql
+-rw-r--r--   0        0        0      613 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/queries/create_firmware_upload.graphql
+-rw-r--r--   0        0        0       71 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/queries/get_analysis_configurations.graphql
+-rw-r--r--   0        0        0      137 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/queries/get_firmware_latest_analysis_state.graphql
+-rw-r--r--   0        0        0      350 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/queries/get_firmware_latest_results.graphql
+-rw-r--r--   0        0        0       62 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/queries/get_product_groups.graphql
+-rw-r--r--   0        0        0      212 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/queries/get_same_product_firmwares.graphql
+-rw-r--r--   0        0        0       72 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/queries/get_self.graphql
+-rw-r--r--   0        0        0      357 2024-04-23 09:48:20.504307 onekey_client-2.3.0/onekey_client/queries/utils.py
+-rw-r--r--   0        0        0     1026 2024-04-23 09:48:20.504307 onekey_client-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 onekey_client-2.3.0/PKG-INFO
```

### Comparing `onekey_client-2.2.0/LICENSE` & `onekey_client-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onekey_client-2.2.0/README.md` & `onekey_client-2.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -103,24 +103,36 @@
     id
     name
   }
 }
 """
 res = client.query(GET_PRODUCT_GROUPS)
 default_product_group = next(pg for pg in res["allProductGroups"] if pg["name"] == "Default")
+
+GET_ANALYSIS_CONFIGURATIONS = """
+query {
+  allAnalysisConfigurations {
+    id
+    name
+  }
+}
+"""
+res = client.query(GET_ANALYSIS_CONFIGURATIONS)
+default_analysis_configuration = next(conf for conf in res["allAnalysisConfigurations"] if conf["name"] == "Default")
 ```
 
 You can upload firmwares:
 
 ```python
 metadata = FirmwareMetadata(
     name="myFirmware",
     vendor_name="myVendor",
     product_name="myProduct",
     product_group_id=default_product_group["id"],
+    analysis_configuration_id=default_analysis_configuration["id"],
 )
 
 firmware_path = Path("/path/to/firmware.bin")
 res = client.upload_firmware(metadata, firmware_path, enable_monitoring=True)
 print(res)
 ```
```

### Comparing `onekey_client-2.2.0/onekey_client/cli/ci.py` & `onekey_client-2.3.0/onekey_client/cli/ci.py`

 * *Files identical despite different names*

### Comparing `onekey_client-2.2.0/onekey_client/cli/cli.py` & `onekey_client-2.3.0/onekey_client/cli/cli.py`

 * *Files identical despite different names*

### Comparing `onekey_client-2.2.0/onekey_client/cli/firmware_upload.py` & `onekey_client-2.3.0/onekey_client/cli/firmware_upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,56 +19,88 @@
     "--product-group",
     "product_group_name",
     default="Default",
     show_default=True,
     required=True,
     help="Product group name to add the firmware",
 )
+@click.option(
+    "--analysis-configuration",
+    "analysis_configuration_name",
+    default="Default",
+    show_default=True,
+    required=True,
+    help="Analysis configuration name",
+)
 @click.option("--version", help="Firmware version")
 @click.option("--name", help="Firmware name")
 @click.argument("filename", type=click.Path(exists=True, path_type=Path))
 @click.pass_obj
 def upload_firmware(
     client: Client,
     product_name: str,
     vendor_name: str,
     product_group_name: str,
+    analysis_configuration_name: str,
     version: Optional[str],
     name: Optional[str],
     filename: Path,
 ):
     """Uploads a firmware to the ONEKEY platform"""
 
-    product_groups = client.get_product_groups()
-
-    try:
-        product_group_id = product_groups[product_group_name]
-    except KeyError:
-        click.echo(f"Missing product group: {product_group_name}")
-        click.echo("Available product groups:")
-        for pg in product_groups.keys():
-            click.echo(f"- {pg}")
-        sys.exit(10)
+    product_group_id = _get_product_group_id_by_name(client, product_group_name)
+    analysis_configuration_id = _get_analysis_configuration_id_by_name(
+        client, analysis_configuration_name
+    )
 
     if name is None:
         name = (
             f"{vendor_name}-{product_name}-{filename.name}"
             if version is None
             else f"{vendor_name}-{product_name}-{version}"
         )
 
     metadata = FirmwareMetadata(
         name=name,
         vendor_name=vendor_name,
         product_name=product_name,
         product_group_id=product_group_id,
         version=version,
+        analysis_configuration_id=analysis_configuration_id,
     )
 
     try:
         res = client.upload_firmware(metadata, filename, enable_monitoring=False)
         click.echo(res["id"])
     except QueryError as e:
         click.echo("Error during firmware upload:")
         for error in e._errors:
             click.echo(f"- {error['message']}")
         sys.exit(11)
+
+
+def _get_product_group_id_by_name(client: Client, product_group_name: str):
+    product_groups = client.get_product_groups()
+
+    try:
+        return product_groups[product_group_name]
+    except KeyError:
+        click.echo(f"Missing product group: {product_group_name}")
+        click.echo("Available product groups:")
+        for pg in product_groups.keys():
+            click.echo(f"- {pg}")
+        sys.exit(10)
+
+
+def _get_analysis_configuration_id_by_name(
+    client: Client, analysis_configuration_name: str
+):
+    analysis_configurations = client.get_analysis_configurations()
+
+    try:
+        return analysis_configurations[analysis_configuration_name]
+    except KeyError:
+        click.echo(f"Missing analysis configuration {analysis_configuration_name}")
+        click.echo("Available analysis configurations:")
+        for config in analysis_configurations.keys():
+            click.echo(f"- {config}")
+        sys.exit(12)
```

### Comparing `onekey_client-2.2.0/onekey_client/client.py` & `onekey_client-2.3.0/onekey_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -205,14 +205,15 @@
         variables = {
             "firmware": {
                 "name": metadata.name,
                 "version": metadata.version,
                 "releaseDate": metadata.release_date,
                 "notes": metadata.notes,
                 "enableMonitoring": enable_monitoring,
+                "analysisConfigurationId": str(metadata.analysis_configuration_id),
             },
             "vendorName": metadata.vendor_name,
             "productName": metadata.product_name,
             "productCategory": metadata.product_category,
             "productGroupID": str(metadata.product_group_id),
         }
 
@@ -230,14 +231,22 @@
 
     @_tenant_required
     def get_product_groups(self):
         product_groups_query = load_query("get_product_groups.graphql")
         response = self.query(product_groups_query)
         return {pg["name"]: pg["id"] for pg in response["allProductGroups"]}
 
+    @_tenant_required
+    def get_analysis_configurations(self):
+        analysis_configurations_query = load_query(
+            "get_analysis_configurations.graphql"
+        )
+        response = self.query(analysis_configurations_query)
+        return {c["name"]: c["id"] for c in response["allAnalysisConfigurations"]}
+
     def logout(self):
         del self._state
         gc.collect()
         self._state = _LoginState()
 
 
 def _verify_token(
```

### Comparing `onekey_client-2.2.0/onekey_client/errors.py` & `onekey_client-2.3.0/onekey_client/errors.py`

 * *Files identical despite different names*

### Comparing `onekey_client-2.2.0/onekey_client/keys/ca.pem` & `onekey_client-2.3.0/onekey_client/keys/ca.pem`

 * *Files identical despite different names*

### Comparing `onekey_client-2.2.0/onekey_client/queries/create_firmware_upload.graphql` & `onekey_client-2.3.0/onekey_client/queries/create_firmware_upload.graphql`

 * *Files identical despite different names*

### Comparing `onekey_client-2.2.0/pyproject.toml` & `onekey_client-2.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onekey_client"
-version = "2.2.0"
+version = "2.3.0"
 description = "ONEKEY API client"
 homepage = "https://www.onekey.com/"
 authors = ["ONEKEY <support@onekey.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["iot", "security", "firmware", "analysis"]
 classifiers = [
@@ -16,24 +16,24 @@
     "Topic :: Security"]
 
 [tool.poetry.urls]
 "GitHub" = "https://github.com/onekey-sec/python-client"
 "Bug Tracker" = "https://github.com/onekey-sec/python-client/issues"
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = "^3.8.0"
 httpx = "0.23.0"
 pydantic = "1.8.2"
 Authlib = "^0.15.3"
 importlib-resources = "^5.1.2"
 click = "^8.1.3"
 junit-xml = "^1.9"
 
 [tool.poetry.dev-dependencies]
-black = "^22.3.0"
+black = "^24.4.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 onekey = "onekey_client.cli.cli:main"
```

### Comparing `onekey_client-2.2.0/PKG-INFO` & `onekey_client-2.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: onekey_client
-Version: 2.2.0
+Version: 2.3.0
 Summary: ONEKEY API client
 Home-page: https://www.onekey.com/
 License: MIT
 Keywords: iot,security,firmware,analysis
 Author: ONEKEY
 Author-email: support@onekey.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Security
 Requires-Dist: Authlib (>=0.15.3,<0.16.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: httpx (==0.23.0)
 Requires-Dist: importlib-resources (>=5.1.2,<6.0.0)
 Requires-Dist: junit-xml (>=1.9,<2.0)
@@ -135,24 +135,36 @@
     id
     name
   }
 }
 """
 res = client.query(GET_PRODUCT_GROUPS)
 default_product_group = next(pg for pg in res["allProductGroups"] if pg["name"] == "Default")
+
+GET_ANALYSIS_CONFIGURATIONS = """
+query {
+  allAnalysisConfigurations {
+    id
+    name
+  }
+}
+"""
+res = client.query(GET_ANALYSIS_CONFIGURATIONS)
+default_analysis_configuration = next(conf for conf in res["allAnalysisConfigurations"] if conf["name"] == "Default")
 ```
 
 You can upload firmwares:
 
 ```python
 metadata = FirmwareMetadata(
     name="myFirmware",
     vendor_name="myVendor",
     product_name="myProduct",
     product_group_id=default_product_group["id"],
+    analysis_configuration_id=default_analysis_configuration["id"],
 )
 
 firmware_path = Path("/path/to/firmware.bin")
 res = client.upload_firmware(metadata, firmware_path, enable_monitoring=True)
 print(res)
 ```
```

