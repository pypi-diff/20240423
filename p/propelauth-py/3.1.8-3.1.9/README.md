# Comparing `tmp/propelauth-py-3.1.8.tar.gz` & `tmp/propelauth-py-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-py-3.1.8.tar", last modified: Thu Oct  5 20:37:39 2023, max compression
+gzip compressed data, was "propelauth-py-3.1.9.tar", last modified: Sun Oct 15 04:16:32 2023, max compression
```

## Comparing `propelauth-py-3.1.8.tar` & `propelauth-py-3.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:37:39.683933 propelauth-py-3.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-10-05 20:37:39.683933 propelauth-py-3.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:37:39.679933 propelauth-py-3.1.8/propelauth_py/
--rw-r--r--   0 runner    (1001) docker     (127)    19735 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:37:39.683933 propelauth-py-3.1.8/propelauth_py/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/api/access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6276 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/api/end_user_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/api/magic_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/api/migrate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     8796 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/api/org.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/api/token_verification_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    15816 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6481 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/auth_fns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/propelauth_py/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 20:37:39.679933 propelauth-py-3.1.8/propelauth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-10-05 20:37:39.000000 propelauth-py-3.1.8/propelauth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-10-05 20:37:39.000000 propelauth-py-3.1.8/propelauth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 20:37:39.000000 propelauth-py-3.1.8/propelauth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-05 20:37:39.000000 propelauth-py-3.1.8/propelauth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-05 20:37:39.000000 propelauth-py-3.1.8/propelauth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 20:37:39.683933 propelauth-py-3.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-10-05 20:37:24.000000 propelauth-py-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 04:16:32.014097 propelauth-py-3.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-10-15 04:16:32.014097 propelauth-py-3.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 04:16:32.010097 propelauth-py-3.1.9/propelauth_py/
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 04:16:32.014097 propelauth-py-3.1.9/propelauth_py/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/api/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6276 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/api/end_user_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/api/magic_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/api/migrate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8796 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/api/org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/api/token_verification_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15816 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/auth_fns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/propelauth_py/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 04:16:32.014097 propelauth-py-3.1.9/propelauth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2023-10-15 04:16:31.000000 propelauth-py-3.1.9/propelauth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2023-10-15 04:16:31.000000 propelauth-py-3.1.9/propelauth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 04:16:31.000000 propelauth-py-3.1.9/propelauth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-15 04:16:31.000000 propelauth-py-3.1.9/propelauth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-15 04:16:31.000000 propelauth-py-3.1.9/propelauth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-15 04:16:32.014097 propelauth-py-3.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2023-10-15 04:16:20.000000 propelauth-py-3.1.9/setup.py
```

### Comparing `propelauth-py-3.1.8/LICENSE` & `propelauth-py-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/PKG-INFO` & `propelauth-py-3.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.1.8
+Version: 3.1.9
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.8 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.9 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       _[_h_t_t_p_s_:_/_/_p_r_o_p_e_l_a_u_t_h_-_l_o_g_o_s_._s_3_._u_s_-_w_e_s_t_-_2_._a_m_a_z_o_n_a_w_s_._c_o_m_/_l_o_g_o_-_o_n_l_y_._p_n_g_]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.1.8/README.md` & `propelauth-py-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/__init__.py` & `propelauth-py-3.1.9/propelauth_py/__init__.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/api/__init__.py` & `propelauth-py-3.1.9/propelauth_py/api/__init__.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/api/access_token.py` & `propelauth-py-3.1.9/propelauth_py/api/access_token.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/api/end_user_api_keys.py` & `propelauth-py-3.1.9/propelauth_py/api/end_user_api_keys.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/api/magic_link.py` & `propelauth-py-3.1.9/propelauth_py/api/magic_link.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/api/migrate_user.py` & `propelauth-py-3.1.9/propelauth_py/api/migrate_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 
 from propelauth_py.api import _ApiKeyAuth
 from propelauth_py.errors import BadRequestException
 
-ENDPOINT_PATH = "/api/backend/v1/migrate_user/"
+ENDPOINT_PATH = "/api/backend/v1/migrate_user"
 
 
 def _migrate_user_from_external_source(
     auth_url,
     integration_api_key,
     email,
     email_confirmed,
@@ -29,16 +29,17 @@
         "existing_password_hash": existing_password_hash,
         "existing_mfa_base32_encoded_secret": existing_mfa_base32_encoded_secret,
         "ask_user_to_update_password_on_login": ask_user_to_update_password_on_login,
         "enabled": enabled,
         "first_name": first_name,
         "last_name": last_name,
         "username": username,
-        "properties": properties,
     }
+    if properties is not None:
+        json["properties"] = properties
 
     response = requests.post(url, json=json, auth=_ApiKeyAuth(integration_api_key))
     if response.status_code == 401:
         raise ValueError("integration_api_key is incorrect")
     elif response.status_code == 400:
         raise BadRequestException(response.json())
     elif not response.ok:
```

### Comparing `propelauth-py-3.1.8/propelauth_py/api/org.py` & `propelauth-py-3.1.9/propelauth_py/api/org.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/api/token_verification_metadata.py` & `propelauth-py-3.1.9/propelauth_py/api/token_verification_metadata.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/api/user.py` & `propelauth-py-3.1.9/propelauth_py/api/user.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/auth_fns.py` & `propelauth-py-3.1.9/propelauth_py/auth_fns.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/errors.py` & `propelauth-py-3.1.9/propelauth_py/errors.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/jwt.py` & `propelauth-py-3.1.9/propelauth_py/jwt.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py/user.py` & `propelauth-py-3.1.9/propelauth_py/user.py`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/propelauth_py.egg-info/PKG-INFO` & `propelauth-py-3.1.9/propelauth_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-py
-Version: 3.1.8
+Version: 3.1.9
 Summary: A python authentication library
 Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.8 Summary: A python
+Metadata-Version: 2.1 Name: propelauth-py Version: 3.1.9 Summary: A python
 authentication library Home-page: https://github.com/propelauth/propelauth-py
 Author: PropelAuth Author-email: support@propelauth.com License: MIT Platform:
 UNKNOWN Description-Content-Type: text/markdown License-File: LICENSE #
 PropelAuth Python SDK
       _[_h_t_t_p_s_:_/_/_p_r_o_p_e_l_a_u_t_h_-_l_o_g_o_s_._s_3_._u_s_-_w_e_s_t_-_2_._a_m_a_z_o_n_a_w_s_._c_o_m_/_l_o_g_o_-_o_n_l_y_._p_n_g_]
 A python library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-python). [PropelAuth](https://
```

### Comparing `propelauth-py-3.1.8/propelauth_py.egg-info/SOURCES.txt` & `propelauth-py-3.1.9/propelauth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `propelauth-py-3.1.8/setup.py` & `propelauth-py-3.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {"pytest", "test", "ptr"}.intersection(sys.argv)
 pytest_runner = ["pytest-runner"] if needs_pytest else []
 
 setup(
     name="propelauth-py",
-    version="3.1.8",
+    version="3.1.9",
     description="A python authentication library",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-py",
     packages=find_packages(include=["propelauth_py", "propelauth_py.*"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
```

