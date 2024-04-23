# Comparing `tmp/arcane_ga4-0.4.3.tar.gz` & `tmp/arcane_ga4-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcane_ga4-0.4.3.tar", max compression
+gzip compressed data, was "arcane_ga4-0.4.4.tar", max compression
```

## Comparing `arcane_ga4-0.4.3.tar` & `arcane_ga4-0.4.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      345 2024-03-08 10:07:48.039090 arcane_ga4-0.4.3/README.md
--rw-r--r--   0        0        0       70 2024-03-08 10:07:48.039090 arcane_ga4-0.4.3/arcane/ga4/__init__.py
--rw-r--r--   0        0        0     4954 2024-03-08 10:07:48.039090 arcane_ga4-0.4.3/arcane/ga4/client.py
--rw-r--r--   0        0        0      250 2024-03-08 10:07:48.039090 arcane_ga4-0.4.3/arcane/ga4/exception.py
--rw-r--r--   0        0        0     7649 2024-03-08 10:07:48.039090 arcane_ga4-0.4.3/arcane/ga4/helpers.py
--rw-r--r--   0        0        0      602 2024-03-08 10:07:48.039090 arcane_ga4-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 arcane_ga4-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      345 2024-04-23 08:46:11.908928 arcane_ga4-0.4.4/README.md
+-rw-r--r--   0        0        0       70 2024-04-23 08:46:11.908928 arcane_ga4-0.4.4/arcane/ga4/__init__.py
+-rw-r--r--   0        0        0     5074 2024-04-23 08:46:11.908928 arcane_ga4-0.4.4/arcane/ga4/client.py
+-rw-r--r--   0        0        0      250 2024-04-23 08:46:11.908928 arcane_ga4-0.4.4/arcane/ga4/exception.py
+-rw-r--r--   0        0        0     7649 2024-04-23 08:46:11.908928 arcane_ga4-0.4.4/arcane/ga4/helpers.py
+-rw-r--r--   0        0        0      602 2024-04-23 08:46:11.908928 arcane_ga4-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1310 1970-01-01 00:00:00.000000 arcane_ga4-0.4.4/PKG-INFO
```

### Comparing `arcane_ga4-0.4.3/arcane/ga4/client.py` & `arcane_ga4-0.4.4/arcane/ga4/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,16 @@
                     datastore_client=datastore_client
                 )
             else:
                 self.credentials = service_account.Credentials.from_service_account_file(gcp_service_account, scopes=scopes)
         elif gcp_service_account:
             ## Used when posting an account using our credential (it is not yet in our database)
             self.credentials = service_account.Credentials.from_service_account_file(gcp_service_account, scopes=scopes)
+            creator_email = self.credentials.service_account_email
+            print(f"creator_email: {creator_email}")
         else:
             raise BadRequestError('one of the following arguments must be specified: gcp_service_account and (google_ads_account or base_account or user_email)')
 
         self.creator_email = creator_email
 
     def check_access(self):
         """Utility function to check if the user has access to the property (call get_property_name)"""
```

### Comparing `arcane_ga4-0.4.3/arcane/ga4/helpers.py` & `arcane_ga4-0.4.4/arcane/ga4/helpers.py`

 * *Files identical despite different names*

### Comparing `arcane_ga4-0.4.3/pyproject.toml` & `arcane_ga4-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcane-ga4"
-version = "0.4.3"
+version = "0.4.4"
 description = "Utility functions for ga4 api call"
 readme = "README.md"
 authors = ["Arcane <product@arcane.run>"]
 packages = [
     { include = "arcane" }
 ]
```

### Comparing `arcane_ga4-0.4.3/PKG-INFO` & `arcane_ga4-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcane-ga4
-Version: 0.4.3
+Version: 0.4.4
 Summary: Utility functions for ga4 api call
 Author: Arcane
 Author-email: product@arcane.run
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

