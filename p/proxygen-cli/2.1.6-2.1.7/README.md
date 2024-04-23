# Comparing `tmp/proxygen_cli-2.1.6.tar.gz` & `tmp/proxygen_cli-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxygen_cli-2.1.6.tar", max compression
+gzip compressed data, was "proxygen_cli-2.1.7.tar", max compression
```

## Comparing `proxygen_cli-2.1.6.tar` & `proxygen_cli-2.1.7.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     2976 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/README.md
--rw-r--r--   0        0        0      248 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/__init__.py
--rw-r--r--   0        0        0     3268 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/cli/command_credentials.py
--rw-r--r--   0        0        0     1167 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/cli/command_docker.py
--rw-r--r--   0        0        0     4603 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/cli/command_instance.py
--rw-r--r--   0        0        0      850 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/cli/command_main.py
--rw-r--r--   0        0        0     6548 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/cli/command_secret.py
--rw-r--r--   0        0        0     1781 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/cli/command_settings.py
--rw-r--r--   0        0        0     3697 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/cli/command_spec.py
--rw-r--r--   0        0        0     5722 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/lib/auth.py
--rw-r--r--   0        0        0      268 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/lib/constants.py
--rw-r--r--   0        0        0     4170 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/lib/credentials.py
--rw-r--r--   0        0        0     1018 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/lib/dot_proxygen.py
--rw-r--r--   0        0        0     1562 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/lib/output.py
--rw-r--r--   0        0        0     5743 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/lib/proxygen_api.py
--rw-r--r--   0        0        0      865 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/lib/settings.py
--rw-r--r--   0        0        0     3037 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/lib/spec.py
--rw-r--r--   0        0        0     1042 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/lib/spec_server.py
--rw-r--r--   0        0        0      520 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/lib/version.py
--rw-r--r--   0        0        0        0 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/__init__.py
--rw-r--r--   0        0        0     6555 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/command_credentials_test.py
--rw-r--r--   0        0        0    13013 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/command_instance_test.py
--rw-r--r--   0        0        0      752 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/command_main_test.py
--rw-r--r--   0        0        0     7005 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/command_secret_test.py
--rw-r--r--   0        0        0     3591 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/command_settings_test.py
--rw-r--r--   0        0        0     4263 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/command_spec_test.py
--rw-r--r--   0        0        0     6678 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/conftest.py
--rw-r--r--   0        0        0     3272 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/fixtures/client.key
--rw-r--r--   0        0        0     1952 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/fixtures/client.pem
--rw-r--r--   0        0        0       30 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/fixtures/secret.txt
--rw-r--r--   0        0        0      570 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/mock_private_key.py
--rw-r--r--   0        0        0      786 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/proxygen_cli/test/validate_cli_version_test.py
--rw-r--r--   0        0        0      760 2024-04-17 12:12:02.448507 proxygen_cli-2.1.6/pyproject.toml
--rw-r--r--   0        0        0     3946 1970-01-01 00:00:00.000000 proxygen_cli-2.1.6/PKG-INFO
+-rw-r--r--   0        0        0     3336 2024-04-23 08:08:24.425137 proxygen_cli-2.1.7/README.md
+-rw-r--r--   0        0        0      248 2024-04-23 08:08:24.425137 proxygen_cli-2.1.7/proxygen_cli/__init__.py
+-rw-r--r--   0        0        0     3268 2024-04-23 08:08:24.425137 proxygen_cli-2.1.7/proxygen_cli/cli/command_credentials.py
+-rw-r--r--   0        0        0     1167 2024-04-23 08:08:24.425137 proxygen_cli-2.1.7/proxygen_cli/cli/command_docker.py
+-rw-r--r--   0        0        0     4603 2024-04-23 08:08:24.425137 proxygen_cli-2.1.7/proxygen_cli/cli/command_instance.py
+-rw-r--r--   0        0        0      850 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/cli/command_main.py
+-rw-r--r--   0        0        0      861 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/cli/command_pytest_nhsd_apim_token.py
+-rw-r--r--   0        0        0     6548 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/cli/command_secret.py
+-rw-r--r--   0        0        0     1781 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/cli/command_settings.py
+-rw-r--r--   0        0        0     3697 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/cli/command_spec.py
+-rw-r--r--   0        0        0     5722 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/lib/auth.py
+-rw-r--r--   0        0        0      268 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/lib/constants.py
+-rw-r--r--   0        0        0     4170 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/lib/credentials.py
+-rw-r--r--   0        0        0     1018 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/lib/dot_proxygen.py
+-rw-r--r--   0        0        0     1562 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/lib/output.py
+-rw-r--r--   0        0        0     5880 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/lib/proxygen_api.py
+-rw-r--r--   0        0        0      865 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/lib/settings.py
+-rw-r--r--   0        0        0     3037 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/lib/spec.py
+-rw-r--r--   0        0        0     1042 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/lib/spec_server.py
+-rw-r--r--   0        0        0      520 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/lib/version.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/__init__.py
+-rw-r--r--   0        0        0     6555 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/command_credentials_test.py
+-rw-r--r--   0        0        0    13013 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/command_instance_test.py
+-rw-r--r--   0        0        0      752 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/command_main_test.py
+-rw-r--r--   0        0        0      688 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/command_pytest_nhsd_apim_token_test.py
+-rw-r--r--   0        0        0     7005 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/command_secret_test.py
+-rw-r--r--   0        0        0     3591 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/command_settings_test.py
+-rw-r--r--   0        0        0     4263 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/command_spec_test.py
+-rw-r--r--   0        0        0     6678 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/conftest.py
+-rw-r--r--   0        0        0     3272 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/fixtures/client.key
+-rw-r--r--   0        0        0     1952 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/fixtures/client.pem
+-rw-r--r--   0        0        0       30 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/fixtures/secret.txt
+-rw-r--r--   0        0        0      570 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/mock_private_key.py
+-rw-r--r--   0        0        0      786 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/proxygen_cli/test/validate_cli_version_test.py
+-rw-r--r--   0        0        0      760 2024-04-23 08:08:24.429137 proxygen_cli-2.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4306 1970-01-01 00:00:00.000000 proxygen_cli-2.1.7/PKG-INFO
```

### Comparing `proxygen_cli-2.1.6/README.md` & `proxygen_cli-2.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -72,8 +72,15 @@
 
 ### Interacting with your docker repository
 To enable the push and pull of images from the API Management ECR repository, you will need to acquire authentication details.
 
 Use the following command to obtain a docker token:
 ```
 $(proxygen docker get-login)
-```
+```
+### Retrieving a token to use with the pytest-nhsd-apim python testing package
+When testing using the pytest-nhsd-apim python testing package, an apigee management api token is needed. This endpoint provides this token for use in automated tests.
+
+Use the following command to obtain the pytest-nhsd-apim token:
+```
+$(proxygen pytest_nhsd_apim get_token)
+```
```

### Comparing `proxygen_cli-2.1.6/proxygen_cli/cli/command_credentials.py` & `proxygen_cli-2.1.7/proxygen_cli/cli/command_credentials.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/cli/command_docker.py` & `proxygen_cli-2.1.7/proxygen_cli/cli/command_docker.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/cli/command_instance.py` & `proxygen_cli-2.1.7/proxygen_cli/cli/command_instance.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/cli/command_main.py` & `proxygen_cli-2.1.7/proxygen_cli/cli/command_main.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/cli/command_secret.py` & `proxygen_cli-2.1.7/proxygen_cli/cli/command_secret.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/cli/command_settings.py` & `proxygen_cli-2.1.7/proxygen_cli/cli/command_settings.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/cli/command_spec.py` & `proxygen_cli-2.1.7/proxygen_cli/cli/command_spec.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/lib/auth.py` & `proxygen_cli-2.1.7/proxygen_cli/lib/auth.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/lib/credentials.py` & `proxygen_cli-2.1.7/proxygen_cli/lib/credentials.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/lib/dot_proxygen.py` & `proxygen_cli-2.1.7/proxygen_cli/lib/dot_proxygen.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/lib/output.py` & `proxygen_cli-2.1.7/proxygen_cli/lib/output.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/lib/proxygen_api.py` & `proxygen_cli-2.1.7/proxygen_cli/lib/proxygen_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
 
 
 def get_docker_login(api: str):
     resp = _session().get(f"/apis/{api}/docker-token")
     return _resp_json(resp)
 
 
+def get_pytest_nhsd_apim_token(api: str):
+    resp = _session().get(f"/apis/{api}/pytest-nhsd-apim-token")
+    return _resp_json(resp)
+
+
 def get_resources(
     api: str,
     _type: Optional[Literal["instance", "secret"]] = None,
 ):
     """
     Get both resource types across all envs.
     Optionally filter with `_type`.
```

### Comparing `proxygen_cli-2.1.6/proxygen_cli/lib/settings.py` & `proxygen_cli-2.1.7/proxygen_cli/lib/settings.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/lib/spec.py` & `proxygen_cli-2.1.7/proxygen_cli/lib/spec.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/lib/spec_server.py` & `proxygen_cli-2.1.7/proxygen_cli/lib/spec_server.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/lib/version.py` & `proxygen_cli-2.1.7/proxygen_cli/lib/version.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/command_credentials_test.py` & `proxygen_cli-2.1.7/proxygen_cli/test/command_credentials_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/command_instance_test.py` & `proxygen_cli-2.1.7/proxygen_cli/test/command_instance_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/command_main_test.py` & `proxygen_cli-2.1.7/proxygen_cli/test/command_main_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/command_secret_test.py` & `proxygen_cli-2.1.7/proxygen_cli/test/command_secret_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/command_settings_test.py` & `proxygen_cli-2.1.7/proxygen_cli/test/command_settings_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/command_spec_test.py` & `proxygen_cli-2.1.7/proxygen_cli/test/command_spec_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/conftest.py` & `proxygen_cli-2.1.7/proxygen_cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/fixtures/client.key` & `proxygen_cli-2.1.7/proxygen_cli/test/fixtures/client.key`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/fixtures/client.pem` & `proxygen_cli-2.1.7/proxygen_cli/test/fixtures/client.pem`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/mock_private_key.py` & `proxygen_cli-2.1.7/proxygen_cli/test/mock_private_key.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/proxygen_cli/test/validate_cli_version_test.py` & `proxygen_cli-2.1.7/proxygen_cli/test/validate_cli_version_test.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.1.6/pyproject.toml` & `proxygen_cli-2.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proxygen-cli"
-version = "2.1.6"
+version = "2.1.7"
 description = "CLI for interacting with NHSD APIM's proxygen service"
 authors = ["Ben Strutt <ben.strutt1@nhs.net>"]
 readme = "README.md"
 packages = [{include = "proxygen_cli"}]
 repository = "https://github.com/NHSDigital/proxygen-cli"
 
 [tool.poetry.scripts]
```

### Comparing `proxygen_cli-2.1.6/PKG-INFO` & `proxygen_cli-2.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxygen-cli
-Version: 2.1.6
+Version: 2.1.7
 Summary: CLI for interacting with NHSD APIM's proxygen service
 Home-page: https://github.com/NHSDigital/proxygen-cli
 Author: Ben Strutt
 Author-email: ben.strutt1@nhs.net
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -98,7 +98,15 @@
 ### Interacting with your docker repository
 To enable the push and pull of images from the API Management ECR repository, you will need to acquire authentication details.
 
 Use the following command to obtain a docker token:
 ```
 $(proxygen docker get-login)
 ```
+### Retrieving a token to use with the pytest-nhsd-apim python testing package
+When testing using the pytest-nhsd-apim python testing package, an apigee management api token is needed. This endpoint provides this token for use in automated tests.
+
+Use the following command to obtain the pytest-nhsd-apim token:
+```
+$(proxygen pytest_nhsd_apim get_token)
+```
+
```

