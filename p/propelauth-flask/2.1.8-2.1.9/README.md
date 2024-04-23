# Comparing `tmp/propelauth-flask-2.1.8.tar.gz` & `tmp/propelauth-flask-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-flask-2.1.8.tar", last modified: Sun Oct 15 04:25:34 2023, max compression
+gzip compressed data, was "propelauth-flask-2.1.9.tar", last modified: Thu Jan 18 23:05:22 2024, max compression
```

## Comparing `propelauth-flask-2.1.8.tar` & `propelauth-flask-2.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 04:25:34.846648 propelauth-flask-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-15 04:25:18.000000 propelauth-flask-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-10-15 04:25:34.846648 propelauth-flask-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-10-15 04:25:18.000000 propelauth-flask-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 04:25:34.846648 propelauth-flask-2.1.8/propelauth_flask/
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2023-10-15 04:25:18.000000 propelauth-flask-2.1.8/propelauth_flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7602 2023-10-15 04:25:18.000000 propelauth-flask-2.1.8/propelauth_flask/auth_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-10-15 04:25:18.000000 propelauth-flask-2.1.8/propelauth_flask/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 04:25:34.846648 propelauth-flask-2.1.8/propelauth_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-10-15 04:25:34.000000 propelauth-flask-2.1.8/propelauth_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      314 2023-10-15 04:25:34.000000 propelauth-flask-2.1.8/propelauth_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 04:25:34.000000 propelauth-flask-2.1.8/propelauth_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-15 04:25:34.000000 propelauth-flask-2.1.8/propelauth_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-15 04:25:34.000000 propelauth-flask-2.1.8/propelauth_flask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-15 04:25:34.846648 propelauth-flask-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-10-15 04:25:18.000000 propelauth-flask-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 23:05:22.108378 propelauth-flask-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-18 23:05:10.000000 propelauth-flask-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-01-18 23:05:22.108378 propelauth-flask-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-01-18 23:05:10.000000 propelauth-flask-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 23:05:22.108378 propelauth-flask-2.1.9/propelauth_flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-01-18 23:05:10.000000 propelauth-flask-2.1.9/propelauth_flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7602 2024-01-18 23:05:10.000000 propelauth-flask-2.1.9/propelauth_flask/auth_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-01-18 23:05:10.000000 propelauth-flask-2.1.9/propelauth_flask/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 23:05:22.108378 propelauth-flask-2.1.9/propelauth_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-01-18 23:05:22.000000 propelauth-flask-2.1.9/propelauth_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-18 23:05:22.000000 propelauth-flask-2.1.9/propelauth_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 23:05:22.000000 propelauth-flask-2.1.9/propelauth_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-18 23:05:22.000000 propelauth-flask-2.1.9/propelauth_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-18 23:05:22.000000 propelauth-flask-2.1.9/propelauth_flask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 23:05:22.108378 propelauth-flask-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-18 23:05:10.000000 propelauth-flask-2.1.9/setup.py
```

### Comparing `propelauth-flask-2.1.8/LICENSE` & `propelauth-flask-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.8/PKG-INFO` & `propelauth-flask-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-flask
-Version: 2.1.8
+Version: 2.1.9
 Summary: A library for managing authentication in Flask
 Home-page: https://github.com/propelauth/propelauth-flask
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.8 Summary: A library
+Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.9 Summary: A library
 for managing authentication in Flask Home-page: https://github.com/propelauth/
 propelauth-flask Author: PropelAuth Author-email: support@propelauth.com
 License: MIT Platform: UNKNOWN Description-Content-Type: text/markdown License-
 File: LICENSE # PropelAuth Flask SDK
       _[_h_t_t_p_s_:_/_/_p_r_o_p_e_l_a_u_t_h_-_l_o_g_o_s_._s_3_._u_s_-_w_e_s_t_-_2_._a_m_a_z_o_n_a_w_s_._c_o_m_/_l_o_g_o_-_o_n_l_y_._p_n_g_]
 A Flask library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-flask). [PropelAuth](https://
```

### Comparing `propelauth-flask-2.1.8/README.md` & `propelauth-flask-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.8/propelauth_flask/__init__.py` & `propelauth-flask-2.1.9/propelauth_flask/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         "fetch_batch_user_metadata_by_user_ids",
         "fetch_batch_user_metadata_by_emails",
         "fetch_batch_user_metadata_by_usernames",
         "fetch_org",
         "fetch_org_by_query",
         "fetch_users_by_query",
         "fetch_users_in_org",
+        "fetch_user_signup_query_params_by_user_id",
         "create_user",
         "update_user_email",
         "update_user_metadata",
         "update_user_password",
         "create_magic_link",
         "create_access_token",
         "migrate_user_from_external_source",
@@ -115,14 +116,15 @@
         fetch_user_metadata_by_email=auth.fetch_user_metadata_by_email,
         fetch_user_metadata_by_username=auth.fetch_user_metadata_by_username,
         fetch_batch_user_metadata_by_user_ids=auth.fetch_batch_user_metadata_by_user_ids,
         fetch_batch_user_metadata_by_emails=auth.fetch_batch_user_metadata_by_emails,
         fetch_batch_user_metadata_by_usernames=auth.fetch_batch_user_metadata_by_usernames,
         fetch_org=auth.fetch_org,
         fetch_org_by_query=auth.fetch_org_by_query,
+        fetch_user_signup_query_params_by_user_id=auth.fetch_user_signup_query_params_by_user_id,
         fetch_users_by_query=auth.fetch_users_by_query,
         fetch_users_in_org=auth.fetch_users_in_org,
         create_user=auth.create_user,
         update_user_email=auth.update_user_email,
         update_user_metadata=auth.update_user_metadata,
         update_user_password=auth.update_user_password,
         create_magic_link=auth.create_magic_link,
```

### Comparing `propelauth-flask-2.1.8/propelauth_flask/auth_decorator.py` & `propelauth-flask-2.1.9/propelauth_flask/auth_decorator.py`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.8/propelauth_flask/user.py` & `propelauth-flask-2.1.9/propelauth_flask/user.py`

 * *Files identical despite different names*

### Comparing `propelauth-flask-2.1.8/propelauth_flask.egg-info/PKG-INFO` & `propelauth-flask-2.1.9/propelauth_flask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-flask
-Version: 2.1.8
+Version: 2.1.9
 Summary: A library for managing authentication in Flask
 Home-page: https://github.com/propelauth/propelauth-flask
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.8 Summary: A library
+Metadata-Version: 2.1 Name: propelauth-flask Version: 2.1.9 Summary: A library
 for managing authentication in Flask Home-page: https://github.com/propelauth/
 propelauth-flask Author: PropelAuth Author-email: support@propelauth.com
 License: MIT Platform: UNKNOWN Description-Content-Type: text/markdown License-
 File: LICENSE # PropelAuth Flask SDK
       _[_h_t_t_p_s_:_/_/_p_r_o_p_e_l_a_u_t_h_-_l_o_g_o_s_._s_3_._u_s_-_w_e_s_t_-_2_._a_m_a_z_o_n_a_w_s_._c_o_m_/_l_o_g_o_-_o_n_l_y_._p_n_g_]
 A Flask library for managing authentication, backed by [PropelAuth](https://
 www.propelauth.com/?utm_campaign=github-flask). [PropelAuth](https://
```

### Comparing `propelauth-flask-2.1.8/setup.py` & `propelauth-flask-2.1.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {"pytest", "test", "ptr"}.intersection(sys.argv)
 pytest_runner = ["pytest-runner"] if needs_pytest else []
 
 setup(
     name="propelauth-flask",
-    version="2.1.8",
+    version="2.1.9",
     description="A library for managing authentication in Flask",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-flask",
     packages=find_packages(include=["propelauth_flask"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
-    install_requires=["flask<3", "propelauth-py==3.1.9", "requests"],
+    install_requires=["flask<3", "propelauth-py==3.1.11", "requests"],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

